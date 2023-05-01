# Comparing `tmp/deepdog-0.6.7.tar.gz` & `tmp/deepdog-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.6.7.tar", max compression
+gzip compressed data, was "deepdog-0.7.0.tar", max compression
```

## Comparing `deepdog-0.6.7.tar` & `deepdog-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0       73 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/meta.py
--rw-r--r--   0        0        0     6873 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     6794 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      895 2023-04-14 01:26:39.666616 deepdog-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      630 2023-04-14 01:27:49.567318 deepdog-0.6.7/setup.py
--rw-r--r--   0        0        0      408 2023-04-14 01:27:49.567639 deepdog-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-05-01 15:27:10.915961 deepdog-0.7.0/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0       73 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/meta.py
+-rw-r--r--   0        0        0     8471 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     6794 2023-05-01 15:27:10.919962 deepdog-0.7.0/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      895 2023-05-01 15:27:10.919962 deepdog-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-05-01 15:29:16.038480 deepdog-0.7.0/setup.py
+-rw-r--r--   0        0        0      408 2023-05-01 15:29:16.038812 deepdog-0.7.0/PKG-INFO
```

### Comparing `deepdog-0.6.7/deepdog/bayes_run.py` & `deepdog-0.7.0/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.7/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.0/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.7/deepdog/real_spectrum_run.py` & `deepdog-0.7.0/deepdog/real_spectrum_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,73 @@
 import pdme.inputs
 import pdme.model
 import pdme.measurement
 import pdme.measurement.input_types
 import pdme.measurement.oscillating_dipole
 import pdme.util.fast_v_calc
 import pdme.util.fast_nonlocal_spectrum
-from typing import Sequence, Tuple, List, Dict, Union
+from typing import Sequence, Tuple, List, Dict, Union, Optional
 import datetime
 import csv
 import multiprocessing
 import logging
 import numpy
 
 
 # TODO: remove hardcode
 CHUNKSIZE = 50
 
 
 _logger = logging.getLogger(__name__)
 
 
-def get_a_result(input) -> int:
-	model, dot_inputs, lows, highs, monte_carlo_count, seed = input
+def get_a_result_fast_filter_pairs(input) -> int:
+	(
+		model,
+		dot_inputs,
+		lows,
+		highs,
+		pair_inputs,
+		pair_lows,
+		pair_highs,
+		monte_carlo_count,
+		seed,
+	) = input
 
 	rng = numpy.random.default_rng(seed)
 	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
 	sample_dipoles = model.get_monte_carlo_dipole_inputs(
 		monte_carlo_count, None, rng_to_use=rng
 	)
-	vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(dot_inputs, sample_dipoles)
-	return numpy.count_nonzero(pdme.util.fast_v_calc.between(vals, lows, highs))
+
+	current_sample = sample_dipoles
+	for di, low, high in zip(dot_inputs, lows, highs):
+
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(
+			numpy.array([di]), current_sample
+		)
+
+		current_sample = current_sample[numpy.all((vals > low) & (vals < high), axis=1)]
+
+	for pi, plow, phigh in zip(pair_inputs, pair_lows, pair_highs):
+		if len(current_sample) < 1:
+			break
+		vals = pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
+			numpy.array([pi]), current_sample
+		)
+
+		current_sample = current_sample[
+			numpy.all(
+				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
+				axis=1,
+			)
+		]
+	return len(current_sample)
 
 
 def get_a_result_fast_filter(input) -> int:
 	model, dot_inputs, lows, highs, monte_carlo_count, seed = input
 
 	rng = numpy.random.default_rng(seed)
 	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
@@ -83,24 +117,41 @@
 		filename_slug: str,
 		monte_carlo_count: int = 10000,
 		monte_carlo_cycles: int = 10,
 		target_success: int = 100,
 		max_monte_carlo_cycles_steps: int = 10,
 		chunksize: int = CHUNKSIZE,
 		initial_seed: int = 12345,
-		use_fast_filter: bool = True,
 		cap_core_count: int = 0,
+		pair_measurements: Optional[
+			Sequence[pdme.measurement.DotPairRangeMeasurement]
+		] = None,
 	) -> None:
 		self.measurements = measurements
 		self.dot_inputs = [(measure.r, measure.f) for measure in self.measurements]
 
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
 			self.dot_inputs
 		)
 
+		if pair_measurements is not None:
+			self.pair_measurements = pair_measurements
+			self.use_pair_measurements = True
+			self.dot_pair_inputs = [
+				(measure.r1, measure.r2, measure.f)
+				for measure in self.pair_measurements
+			]
+			self.dot_pair_inputs_array = (
+				pdme.measurement.input_types.dot_pair_inputs_to_array(
+					self.dot_pair_inputs
+				)
+			)
+		else:
+			self.use_pair_measurements = False
+
 		self.models = [model for (_, model) in models_with_names]
 		self.model_names = [name for (name, _) in models_with_names]
 		self.model_count = len(self.models)
 
 		self.monte_carlo_count = monte_carlo_count
 		self.monte_carlo_cycles = monte_carlo_cycles
 		self.target_success = target_success
@@ -113,18 +164,17 @@
 		for name in self.model_names:
 			self.csv_fields.extend([f"{name}_success", f"{name}_count", f"{name}_prob"])
 
 		# for now initialise priors as uniform.
 		self.probabilities = [1 / self.model_count] * self.model_count
 
 		timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-		self.use_fast_filter = use_fast_filter
-		ff_string = "no_fast_filter"
-		if self.use_fast_filter:
-			ff_string = "fast_filter"
+
+		ff_string = "fast_filter"
+
 		self.filename = f"{timestamp}-{filename_slug}.realdata.{ff_string}.bayesrun.csv"
 		self.initial_seed = initial_seed
 
 		self.cap_core_count = cap_core_count
 
 	def go(self) -> None:
 		with open(self.filename, "a", newline="") as outfile:
@@ -134,14 +184,24 @@
 		(
 			lows,
 			highs,
 		) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
 			self.measurements
 		)
 
+		pair_lows = None
+		pair_highs = None
+		if self.use_pair_measurements:
+			(
+				pair_lows,
+				pair_highs,
+			) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
+				self.pair_measurements
+			)
+
 		# define a new seed sequence for each run
 		seed_sequence = numpy.random.SeedSequence(self.initial_seed)
 
 		results = []
 		_logger.debug("Going to iterate over models now")
 		core_count = multiprocessing.cpu_count() - 1 or 1
 		if (self.cap_core_count >= 1) and (self.cap_core_count < core_count):
@@ -164,35 +224,54 @@
 					cycle_count += self.monte_carlo_count * self.monte_carlo_cycles
 
 					# generate a seed from the sequence for each core.
 					# note this needs to be inside the loop for monte carlo cycle steps!
 					# that way we get more stuff.
 					seeds = seed_sequence.spawn(self.monte_carlo_cycles)
 
-					if self.use_fast_filter:
-						result_func = get_a_result_fast_filter
+					if self.use_pair_measurements:
+						current_success = sum(
+							pool.imap_unordered(
+								get_a_result_fast_filter_pairs,
+								[
+									(
+										model,
+										self.dot_inputs_array,
+										lows,
+										highs,
+										self.dot_pair_inputs_array,
+										pair_lows,
+										pair_highs,
+										self.monte_carlo_count,
+										seed,
+									)
+									for seed in seeds
+								],
+								self.chunksize,
+							)
+						)
 					else:
-						result_func = get_a_result
-					current_success = sum(
-						pool.imap_unordered(
-							result_func,
-							[
-								(
-									model,
-									self.dot_inputs_array,
-									lows,
-									highs,
-									self.monte_carlo_count,
-									seed,
-								)
-								for seed in seeds
-							],
-							self.chunksize,
+
+						current_success = sum(
+							pool.imap_unordered(
+								get_a_result_fast_filter,
+								[
+									(
+										model,
+										self.dot_inputs_array,
+										lows,
+										highs,
+										self.monte_carlo_count,
+										seed,
+									)
+									for seed in seeds
+								],
+								self.chunksize,
+							)
 						)
-					)
 
 					cycle_success += current_success
 					_logger.debug(f"current running successes: {cycle_success}")
 				results.append((cycle_count, cycle_success))
 
 		_logger.debug("Done, constructing output now")
 		row: Dict[str, Union[int, float, str]] = {}
```

### Comparing `deepdog-0.6.7/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.0/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.7/pyproject.toml` & `deepdog-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.6.7"
+version = "0.7.0"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 pdme = "^0.8.6"
 numpy = "1.22.3"
```

### Comparing `deepdog-0.6.7/setup.py` & `deepdog-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.6.7',
+    'version': '0.7.0',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

