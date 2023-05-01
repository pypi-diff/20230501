# Comparing `tmp/quera-ahs-utils-0.4.0.tar.gz` & `tmp/quera-ahs-utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.4.0.tar", last modified: Mon Apr 24 04:44:52 2023, max compression
+gzip compressed data, was "quera-ahs-utils-0.4.1.tar", last modified: Mon May  1 15:41:56 2023, max compression
```

## Comparing `quera-ahs-utils-0.4.0.tar` & `quera-ahs-utils-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.186166 quera-ahs-utils-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.576982 quera-ahs-utils-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.4.0/LICENSE` & `quera-ahs-utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/PKG-INFO` & `quera-ahs-utils-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.0/README.md` & `quera-ahs-utils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/pyproject.toml` & `quera-ahs-utils-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/analysis.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/drive.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/ir.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/ir.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,33 +158,33 @@
                 lattice_site_coefficients=field.pattern
             )
         
     @staticmethod
     def get_rabi_frequency_amplitude(driving: braket_ir.DrivingField):
         field = braket_to_quera.get_global_field(driving.amplitude)
         return RabiFrequencyAmplitude(
-            **{"global":braket_to_quera.get_global_field(driving.amplitude)}
+            global_=braket_to_quera.get_global_field(driving.amplitude)
         )
         
     @staticmethod
     def get_rabi_frequency_phase(driving: braket_ir.DrivingField):
         return RabiFrequencyPhase(
-            **{"global":braket_to_quera.get_global_field(driving.phase)}
+            global_=braket_to_quera.get_global_field(driving.phase)
         )
     
     @staticmethod
     def get_detuning(driving: braket_ir.DrivingField, shifting: Optional[braket_ir.ShiftingField]):
         if shifting == None:
             return Detuning(
-                **{"global":braket_to_quera.get_global_field(driving.detuning)}
+                global_=braket_to_quera.get_global_field(driving.detuning)
             )
         else:
             return Detuning(
-                **{"global":braket_to_quera.get_global_field(driving.detuning),
-                "local":braket_to_quera.get_local_field(shifting.magnitude)}
+                global_=braket_to_quera.get_global_field(driving.detuning),
+                local=braket_to_quera.get_local_field(shifting.magnitude)
             )
 
     @staticmethod
     def get_rydberg(driving: braket_ir.DrivingField, shifting: Optional[braket_ir.ShiftingField] = None):
         return RydbergHamiltonian(
             rabi_frequency_amplitude = braket_to_quera.get_rabi_frequency_amplitude(driving),
             rabi_frequency_phase=braket_to_quera.get_rabi_frequency_phase(driving),
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/parallelize.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/plotting.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 class RydbergCapabilities(BaseModel):
     c6_coefficient: float
     global_: RydbergGlobalCapabilities
     local: RydbergLocalCapabilities
 
     class Config:
+        allow_population_by_field_name = True
         fields = {
             'global_': 'global'
         }
 
 class LatticeGeometryCapabilities(BaseModel):
     spacing_radial_min: float
     spacing_vertical_min: float
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_results.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,42 +58,39 @@
             shot_outputs=shot_outputs
         )
 
 class QuEraTaskResults(BaseModel):
     task_status: QuEraTaskStatusCode = QuEraTaskStatusCode.Failed
     shot_outputs: conlist(QuEraShotResult, min_items=0) = []
     
-    def export_as_probabilties(self, post_process=False) -> TaskProbabilities:
+    def export_as_probabilities(self) -> TaskProbabilities:
         """converts from shot results to probabilities
 
         Returns:
             TaskProbabilities: The task results as probabilties
         """
-        probabilities = dict()
-        n = 0
+        counts = dict()
+        nshots = len(self.shot_outputs)
         for shot_result in self.shot_outputs:
-            if any(bit==0 for bit in shot_result.pre_sequence):
-                continue
             
             pre_sequence_str = "".join(
                 str(bit) for bit in shot_result.pre_sequence
             )
             
             post_sequence_str = "".join(
                 str(bit) for bit in shot_result.post_sequence
             )
             
-            configuration = (pre_sequence_str,post_sequence_str)
+            configuration = (pre_sequence_str, post_sequence_str)
             # iterative average
-            probabilities[configuration] = \
-                ((n + 1.0) * probabilities.get(configuration, 0) + 1.0)/n
-                
-            n += 1
-            
-        return TaskProbabilities(list(probabilities.items()))
+            current_count = counts.get(configuration, 0)
+            counts[configuration] = current_count + 1
+
+        probabilities = [(config,count/nshots) for config,count in counts.items()]
+        return TaskProbabilities(probabilities=probabilities)
     
     def post_process(self, keep_shot_result: Optional[Callable] = None, args = ()) -> 'QuEraTaskResults':
         
         if keep_shot_result == None:
             filter_func = \
                 lambda shot_result: \
                     all(bit==1 for bit in shot_result.pre_sequence)
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,76 +32,88 @@
     def __hash__(self):
         return hash((LocalField, tuple(self.times), tuple(self.values), tuple(self.lattice_site_coefficients)))
 
 class RabiFrequencyAmplitude(BaseModel):
     global_: GlobalField
     
     class Config:
+        allow_population_by_field_name = True
         fields = {
             'global_': 'global'
         }
     
     def __hash__(self):
         return hash((RabiFrequencyAmplitude, self.global_))
     
     def discretize(self, task_capabilities: QuEraCapabilities):
         global_time_resolution = task_capabilities.capabilities.rydberg.global_.time_resolution
         global_value_resolution =  task_capabilities.capabilities.rydberg.global_.rabi_frequency_resolution
         
-        return RabiFrequencyAmplitude(**{"global":GlobalField(
+        return RabiFrequencyAmplitude(
+            global_ = GlobalField(
                 times = discretize_list(self.global_.times, global_time_resolution),
-                values = discretize_list(self.global_.values, global_value_resolution))} 
-            )
+                values = discretize_list(self.global_.values, global_value_resolution)
+            ) 
+        )
 
 class RabiFrequencyPhase(BaseModel):
     global_: GlobalField
     
     class Config:
+        allow_population_by_field_name = True
         fields = {
             'global_': 'global'
         }
         
     def __hash__(self):
         return hash((RabiFrequencyPhase, self.global_))
     
     def discretize(self, task_capabilities: QuEraCapabilities):
         global_time_resolution = task_capabilities.capabilities.rydberg.global_.time_resolution
         global_value_resolution =  task_capabilities.capabilities.rydberg.global_.phase_resolution
         
-        return RabiFrequencyPhase(**{"global":GlobalField(
-                times = discretize_list(self.global_.times, global_time_resolution),
-                values = discretize_list(self.global_.values, global_value_resolution))}               
+        return RabiFrequencyPhase(global_=GlobalField(
+                    times = discretize_list(self.global_.times, global_time_resolution),
+                    values = discretize_list(self.global_.values, global_value_resolution)
+                )
             )
     
 class Detuning(BaseModel):
     global_: GlobalField
     local: Optional[LocalField]
     
     class Config:
+        allow_population_by_field_name = True
         fields = {
             'global_': 'global'
         }
 
     def __hash__(self):
         return hash((Detuning, self.global_, self.local))
     
     def discretize(self, task_capabilities: QuEraCapabilities):
         global_time_resolution = task_capabilities.capabilities.rydberg.global_.time_resolution
         global_value_resolution =  task_capabilities.capabilities.rydberg.global_.detuning_resolution
         local_time_resolution = task_capabilities.capabilities.rydberg.local.time_resolution
 
-        return Detuning(**{"global":GlobalField(
-                times = discretize_list(self.global_.times, global_time_resolution),
-                values = discretize_list(self.global_.values, global_value_resolution)
-            ),"local": LocalField(
-                    times = discretize_list(self.local.times, local_time_resolution), values = self.local.values,
+        if self.local != None:
+            self.local = LocalField(
+                    times = discretize_list(self.local.times, local_time_resolution), 
+                    values = self.local.values,
                     lattice_site_coefficients=self.local.lattice_site_coefficients
                 )
-            }
-        )
+
+
+        return Detuning(
+                global_ = GlobalField(
+                    times = discretize_list(self.global_.times, global_time_resolution),
+                    values = discretize_list(self.global_.values, global_value_resolution)
+                ),
+                local = self.local
+            )
     
 class RydbergHamiltonian(BaseModel):
     rabi_frequency_amplitude: RabiFrequencyAmplitude
     rabi_frequency_phase: RabiFrequencyPhase
     detuning: Detuning
     
     def __hash__(self):
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/test/test_drive.py` & `quera-ahs-utils-0.4.1/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/test/test_ir.py` & `quera-ahs-utils-0.4.1/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/test/test_parallelize.py` & `quera-ahs-utils-0.4.1/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.0/test/test_plotting.py` & `quera-ahs-utils-0.4.1/test/test_plotting.py`

 * *Files identical despite different names*

