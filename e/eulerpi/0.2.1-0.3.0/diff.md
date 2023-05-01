# Comparing `tmp/eulerpi-0.2.1.tar.gz` & `tmp/eulerpi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.2.1.tar", max compression
+gzip compressed data, was "eulerpi-0.3.0.tar", max compression
```

## Comparing `eulerpi-0.2.1.tar` & `eulerpi-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1117 2023-04-21 01:14:59.791617 eulerpi-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     4704 2023-04-21 01:14:59.791617 eulerpi-0.2.1/README.md
--rw-r--r--   0        0        0      564 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/__init__.py
--rw-r--r--   0        0        0    10754 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      355 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0     4609 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/inference.py
--rw-r--r--   0        0        0      514 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     3684 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/kde.py
--rw-r--r--   0        0        0    15208 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/model.py
--rw-r--r--   0        0        0    17486 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    17240 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    20637 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     6393 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2767 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0     1811 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1133 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1793 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2316 2023-04-21 01:14:59.803617 eulerpi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6128 1970-01-01 00:00:00.000000 eulerpi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-01 17:45:45.703946 eulerpi-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     4704 2023-05-01 17:45:45.707946 eulerpi-0.3.0/README.md
+-rw-r--r--   0        0        0      564 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0     7531 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/data_transformation.py
+-rw-r--r--   0        0        0      362 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/data_transformation_types.py
+-rw-r--r--   0        0        0    11433 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     6790 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    15896 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/model.py
+-rw-r--r--   0        0        0    17922 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    15769 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    21145 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     7006 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0     1811 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1133 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1859 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2340 2023-05-01 17:45:45.715946 eulerpi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6173 1970-01-01 00:00:00.000000 eulerpi-0.3.0/PKG-INFO
```

### Comparing `eulerpi-0.2.1/LICENSE.md` & `eulerpi-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/README.md` & `eulerpi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/__init__.py` & `eulerpi-0.3.0/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/core/dense_grid.py` & `eulerpi-0.3.0/eulerpi/core/dense_grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import repeat
 from multiprocessing import get_context
 from typing import Dict, Tuple, Union
 
 import numpy as np
 from numpy.polynomial.chebyshev import chebpts1
 
+from eulerpi.core.data_transformation import DataTransformation
 from eulerpi.core.dense_grid_types import DenseGridType
 from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.sampling import calc_kernel_width
 from eulerpi.core.transformations import evaluate_density
 
@@ -64,58 +65,68 @@
     if flatten:
         return np.array(mesh).reshape(ndim, -1).T
     else:
         return mesh
 
 
 def evaluate_on_grid_chunk(
-    args: typing.Tuple[np.ndarray, Model, np.ndarray, np.ndarray, np.ndarray]
+    args: typing.Tuple[
+        np.ndarray,
+        Model,
+        np.ndarray,
+        DataTransformation,
+        np.ndarray,
+        np.ndarray,
+    ]
 ) -> np.ndarray:
     """Define a function which evaluates the density for a given grid chunk. The input args contains the grid chunk, the model, the data, the data_stdevs and the slice.
 
     Args:
         grid_chunk(np.ndarray): The grid chunk contains the grid points (parameter vectors) for which the density should be evaluated.
         model(Model): The model used for the inference.
         data(np.ndarray): The data points used for the inference.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs(np.ndarray): The standard deviations of the data points. (Currently the kernel width, #TODO!)
         slice(np.ndarray): The slice defines for which dimensions of the grid points / paramater vectors the marginal density should be evaluated.
 
     Returns:
         np.ndarray: The evaluation results for the given grid chunk. It is a vector, containing the parameters in the first columns, the simulation results in the second columns and the density evaluations in the last columns.
     """
-    grid_chunk, model, data, data_stdevs, slice = args
+    grid_chunk, model, data, data_transformation, data_stdevs, slice = args
 
     # Init the result array
     evaluation_results = np.zeros(
-        (grid_chunk.shape[0], data.shape[1] + slice.shape[0] + 1)
+        (grid_chunk.shape[0], model.data_dim + slice.shape[0] + 1)
     )
     # Evaluate the grid points
     for i, gridPoint in enumerate(grid_chunk):
         density, param_sim_res_density = evaluate_density(
-            gridPoint, model, data, data_stdevs, slice
+            gridPoint, model, data, data_transformation, data_stdevs, slice
         )
         evaluation_results[i] = param_sim_res_density
     return evaluation_results
 
 
 def run_dense_grid_evaluation(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     slice: np.ndarray,
     result_manager: ResultManager,
     num_grid_points: np.ndarray,
     dense_grid_type: DenseGridType,
     num_processes: int,
     load_balancing_safety_faktor: int,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """This function runs a dense grid evaluation for the given model and data.
 
     Args:
         model(Model): The model for which the evaluation should be performed.
         data(np.ndarray): The data for which the evaluation should be performed.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         slice(np.ndarray): The slice for which the evaluation should be performed.
         result_manager(ResultManager): The result manager that should be used to save the results.
         num_grid_points(np.ndarray): The number of grid points for each dimension.
         dense_grid_type(DenseGridType): The type of grid that should be used. (Default value = DenseGridType.EQUIDISTANT)
         num_processes(int): The number of processes that should be used for the evaluation. (Default value = NUM_PROCESSES)
         load_balancing_safety_faktor(int): Split the grid into num_processes * load_balancing_safety_faktor chunks.
             This will ensure that each process can be loaded with a similar amount of work if the run time difference between the evaluations
@@ -151,38 +162,42 @@
     )
 
     pool = get_context("spawn").Pool(processes=num_processes)
     tasks = zip(
         grid_chunks,
         repeat(model),
         repeat(data),
+        repeat(data_transformation),
         repeat(data_stdevs),
         repeat(slice),
     )
     results = pool.map(evaluate_on_grid_chunk, tasks)
     pool.close()
     pool.join()
     results = np.concatenate(results)
 
+    data_dim = model.data_dim
+
     result_manager.save_overall(
         slice,
         results[:, 0 : slice.shape[0]],
-        results[:, slice.shape[0] : slice.shape[0] + data.shape[1]],
-        results[:, slice.shape[0] + data.shape[1] :],
+        results[:, slice.shape[0] : slice.shape[0] + data_dim],
+        results[:, slice.shape[0] + data_dim :],
     )
     return (
         results[:, 0 : slice.shape[0]],
-        results[:, slice.shape[0] : slice.shape[0] + data.shape[1]],
-        results[:, slice.shape[0] + data.shape[1] :],
+        results[:, slice.shape[0] : slice.shape[0] + data_dim],
+        results[:, slice.shape[0] + data_dim :],
     )
 
 
 def inference_dense_grid(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     result_manager: ResultManager,
     slices: list[np.ndarray],
     num_processes: int,
     num_grid_points: Union[int, list[np.ndarray]] = 10,
     dense_grid_type: DenseGridType = DenseGridType.EQUIDISTANT,
     load_balancing_safety_faktor: int = 4,
 ) -> Tuple[
@@ -192,14 +207,15 @@
     ResultManager,
 ]:
     """This function runs a dense grid evaluation for the given model and data. The grid points are distributed evenly over the parameter space.
 
     Args:
         model (Model): The model describing the mapping from parameters to data.
         data (np.ndarray): The data to be used for the inference.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         result_manager (ResultManager): The result manager to be used for the inference.
         slices (np.ndarray): A list of slices to be used for the inference.
         num_processes (int): The number of processes to be used for the inference.
         num_grid_points (Union[int, list[np.ndarray]], optional): The number of grid points to be used for each parameter. If an int is given, it is assumed to be the same for all parameters. Defaults to 10.
         load_balancing_safety_faktor (int, optional): Split the grid into num_processes * load_balancing_safety_faktor chunks. Defaults to 4.
 
     Returns:
@@ -229,14 +245,15 @@
         (
             overall_params[slice_name],
             overall_sim_results[slice_name],
             overall_density_evals[slice_name],
         ) = run_dense_grid_evaluation(
             model=model,
             data=data,
+            data_transformation=data_transformation,
             slice=slice,
             result_manager=result_manager,
             num_grid_points=n_points,
             dense_grid_type=dense_grid_type,
             num_processes=num_processes,
             load_balancing_safety_faktor=load_balancing_safety_faktor,
         )
```

### Comparing `eulerpi-0.2.1/eulerpi/core/inference_types.py` & `eulerpi-0.3.0/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/core/kde.py` & `eulerpi-0.3.0/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/core/model.py` & `eulerpi-0.3.0/eulerpi/core/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 from jax import jacrev, jit, vmap
 
 import amici
+from eulerpi import logger
 from eulerpi.jax_extension import value_and_jacrev
 
 
 class Model(ABC):
     """The base class for all models using the EPI algorithm.
 
     Args:
@@ -303,30 +304,44 @@
         # Generate python code
         if not skip_creation:
             sbml_importer = amici.SbmlImporter(sbml_file)
             sbml_importer.sbml2amici(
                 self.amici_model_name, self.amici_model_dir
             )
 
+        self.param_names = param_names
+
         # Load the generated model
         self.load_amici_model_and_solver()
 
-        self.param_names = param_names or self.amici_model.getParameterNames()
-
     def load_amici_model_and_solver(self):
         """Loads the AMICI model from the previously generated model."""
         amici_model_module = amici.import_model_module(
             self.amici_model_name, self.amici_model_dir
         )
         self.amici_model = amici_model_module.getModel()
         self.amici_solver = self.amici_model.getSolver()
 
         # TODO: Maybe this is redundant when using settings to hdf5
         self.amici_model.setTimepoints([self.tEnd])
-        self.amici_model.requireSensitivitiesForAllParameters()
+
+        if self.param_names is not None:
+            # We need the indices for setParameterList, not the ids or names
+            amici_param_indices = []
+            for i, param_id in enumerate(self.amici_model.getParameterIds()):
+                if param_id in self.param_names:
+                    amici_param_indices.append(i)
+                else:
+                    logger.warning(
+                        f"Parameter {param_id} is specified in the sbml file, but not in the passed parameter list. It will be ignored."
+                    )
+            self.amici_model.setParameterList(amici_param_indices)
+        else:
+            self.param_names = self.amici_model.getParameterIds()
+            self.amici_model.requireSensitivitiesForAllParameters()
         self.amici_solver.setSensitivityMethod(amici.SensitivityMethod.forward)
         self.amici_solver.setSensitivityOrder(amici.SensitivityOrder.first)
 
     def forward(self, params):
         for i, param in enumerate(params):
             self.amici_model.setParameterByName(self.param_names[i], param)
         rdata = amici.runAmiciSimulation(self.amici_model, self.amici_solver)
```

### Comparing `eulerpi-0.2.1/eulerpi/core/result_manager.py` & `eulerpi-0.3.0/eulerpi/core/result_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,15 +277,15 @@
             model(Model): The model for which the results will be saved.
             inference_type(InferenceType): The type of inference that was performed.
             num_processes(int): The number of processes that were used for the inference.
             **kwargs: Additional information about the inference run.
                 num_runs(int): The number of runs that were performed. Only for mcmc inference.
                 num_walkers(int): The number of walkers that were used. Only for mcmc inference.
                 num_steps(int): The number of steps that were performed. Only for mcmc inference.
-                num_burn_in_samples(int): The number of samples that were ignored. Only for mcmc inference.
+                num_burn_in_samples(int): Number of samples that will be ignored per chain (i.e. walker). Only for mcmc inference.
                 thinning_factor(int): The thinning factor that was used to thin the Markov chain. Only for mcmc inference.
                 load_balancing_safety_faktor(int): The safety factor that was used for load balancing. Only for dense grid inference.
                 num_grid_points(np.ndarray): The number of grid points that were used. Only for dense grid inference.
                 dense_grid_type(DenseGridType): The type of dense grid that was used: either equidistant or chebyshev. Only for dense grid inference.
                 num_levels(int): The number of sparse grid levels that were used. Only for sparse grid inference.
 
         Raises:
@@ -323,15 +323,15 @@
     ) -> Tuple[
         Dict[str, np.ndarray], Dict[str, np.ndarray], Dict[str, np.ndarray]
     ]:
         """Load the inference results generated by EPI.
 
         Args:
             slices(list[np.ndarray]): Slices for which the results will be loaded. Default is None and loads all slices.
-            num_burn_in_samples(int): Number of samples that will be ignored. Only for mcmc inference. Default is None and uses the value that was used for the inference stored in each inference_information.json.
+            num_burn_in_samples(int): Number of samples that will be ignored per chain (i.e. walker). Only for mcmc inference. Default is None and uses the value that was used for the inference stored in inference_information.json.
             thinning_factor(int): Thinning factor that will be used to thin the Markov chain. Only for mcmc inference. Default is None and uses the value that was used for the inference stored in each inference_information.json.
 
         Returns:
             typing.Tuple[Dict[str, np.ndarray], Dict[str, np.ndarray], Dict[str, np.ndarray]]: The parameters, the simulation results and the density evaluations.
 
         """
         if slices is None:
@@ -356,15 +356,15 @@
         num_burn_in_samples: Optional[int] = None,
         thinning_factor: Optional[int] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Load the files generated by the EPI algorithm through sampling
 
         Args:
             slice(np.ndarray): Slice for which the results will be loaded
-            num_burn_in_samples(int): Number of samples that will be ignored. Only for mcmc inference. Default is None and uses the value that was used for the inference stored in inference_information.json.
+            num_burn_in_samples(int): Number of samples that will be ignored per chain (i.e. walker). Only for mcmc inference. Default is None and uses the value that was used for the inference stored in inference_information.json.
             thinning_factor(int): Thinning factor that will be used to thin the Markov chain. Only for mcmc inference. Default is None and uses the value that was used for the inference stored in inference_information.json.
 
         Returns:
             typing.Tuple[np.ndarray, np.ndarray, np.ndarray]: The parameters, the simulation results and the density evaluations.
 
         """
         results_path = self.get_slice_path(slice)
@@ -436,13 +436,29 @@
                     (overall_density_evals, density_evals)
                 )
                 overall_sim_results = np.concatenate(
                     (overall_sim_results, sim_results)
                 )
                 overall_params = np.concatenate((overall_params, params))
 
+        num_walkers = inference_information["num_walkers"]
+
         # thin and burn in
         return (
-            overall_params[num_burn_in_samples::thinning_factor, :],
-            overall_sim_results[num_burn_in_samples::thinning_factor, :],
-            overall_density_evals[num_burn_in_samples::thinning_factor],
+            overall_params[
+                num_burn_in_samples
+                * num_walkers :: thinning_factor
+                * num_walkers,
+                :,
+            ],
+            overall_sim_results[
+                num_burn_in_samples
+                * num_walkers :: thinning_factor
+                * num_walkers,
+                :,
+            ],
+            overall_density_evals[
+                num_burn_in_samples
+                * num_walkers :: thinning_factor
+                * num_walkers
+            ],
         )
```

### Comparing `eulerpi-0.2.1/eulerpi/core/sampling.py` & `eulerpi-0.3.0/eulerpi/core/sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from multiprocessing import get_context
 from os import path
 
 import emcee
 import numpy as np
 
 from eulerpi import logger
+from eulerpi.core.data_transformation import DataTransformation
 from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.kde import calc_kernel_width
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.transformations import eval_log_transformed_density
 
 # TODO: This works on the blob
@@ -31,56 +32,59 @@
 # return sampler.get_chain(discard=0, thin=1, flat=True)
 # TODO: This stores the sample as 2d array in the format walker1_step1, walker2_step1, walker3_step1, walker1_step2, walker2_step2, walker3_step2, ...
 # sampler_results = samplerBlob.reshape(
 #     num_walkers * num_steps, sampling_dim + data_dim + 1
 # )
 
 
-# TODO Give transformation object to eval function
 def evaluate_sample(
     param: np.ndarray,
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
 ) -> typing.Tuple[float, np.ndarray]:
     """Evaluate the log transformed density at the given parameter values.
 
     Args:
         param (np.ndarray): parameter values
         model (Model): The model which will be sampled
         data (np.ndarray): data
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs (np.ndarray): kernel width for the data
         slice (np.ndarray): slice of the parameter space which will be sampled
 
     Returns:
         typing.Tuple[float, np.ndarray]: log transformed density and the sampler result
     """
 
     log_samplerresult = eval_log_transformed_density(
-        param, model, data, data_stdevs, slice
+        param, model, data, data_transformation, data_stdevs, slice
     )
     return log_samplerresult
 
 
 def run_emcee_once(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
     initial_walker_positions: np.ndarray,
     num_walkers: int,
     num_steps: int,
     num_processes: int,
 ) -> np.ndarray:
     """Run the emcee particle swarm sampler once.
 
     Args:
         model (Model): The model which will be sampled
         data (np.ndarray): data
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs (np.ndarray): kernel width for the data
         slice (np.ndarray): slice of the parameter space which will be sampled
         initial_walker_positions (np.ndarray): initial parameter values for the walkers
         num_walkers (int): number of particles in the particle swarm sampler
         num_steps (int): number of samples each particle performs before storing the sub run
         num_processes (int): number of parallel threads
 
@@ -96,15 +100,15 @@
     # Call the sampler for all parallel workers (possibly use arg moves = movePolicy)
     try:
         sampler = emcee.EnsembleSampler(
             num_walkers,
             sampling_dim,
             evaluate_sample,
             pool=pool,
-            args=[model, data, data_stdevs, slice],
+            args=[model, data, data_transformation, data_stdevs, slice],
         )
         # Extract the final walker position and close the pool of worker processes.
         final_walker_positions, _, _, _ = sampler.run_mcmc(
             initial_walker_positions, num_steps, tune=True, progress=True
         )
     except ValueError as e:
         # If the message equals "Probability function returned NaN."
@@ -120,15 +124,15 @@
     if pool is not None:
         pool.close()
         pool.join()
 
     # TODO: Keep as 3d array?
     # Should have shape (num_steps, num_walkers, param_dim+data_dim+1)
     sampler_results = sampler.get_blobs()
-    data_dim = data.shape[1]
+    data_dim = model.data_dim
     sampler_results = sampler_results.reshape(
         num_steps * num_walkers, sampling_dim + data_dim + 1
     )
     sampler_results = sampler_results.reshape(
         num_walkers * num_steps, sampling_dim + data_dim + 1
     )
 
@@ -145,14 +149,15 @@
 
     return sampler_results, final_walker_positions
 
 
 def run_emcee_sampling(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     slice: np.ndarray,
     result_manager: ResultManager,
     num_processes: int,
     num_runs: int,
     num_walkers: int,
     num_steps: int,
     num_burn_in_samples: int,
@@ -160,21 +165,22 @@
 ) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Create a representative sample from the transformed parameter density using the emcee particle swarm sampler.
        Inital values are not stored in the chain and each file contains <num_steps> blocks of size num_walkers.
 
     Args:
         model (Model): The model which will be sampled
         data (np.ndarray): data
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         slice (np.ndarray): slice of the parameter space which will be sampled
         result_manager (ResultManager): ResultManager which will store the results
         num_processes (int): number of parallel threads.
         num_runs (int): number of stored sub runs.
         num_walkers (int): number of particles in the particle swarm sampler.
         num_steps (int): number of samples each particle performs before storing the sub run.
-        num_burn_in_samples (int): number of samples to be discarded as burn-in.
+        num_burn_in_samples(int): Number of samples that will be deleted (burned) per chain (i.e. walker). Only for mcmc inference.
         thinning_factor (int): thinning factor for the samples.
 
     Returns:
         typing.Tuple[np.ndarray, np.ndarray, np.ndarray]: Array with all params, array with all data, array with all log probabilities
         TODO check: are those really log probabilities?
 
     """
@@ -211,14 +217,15 @@
                 f"Continue sampling from saved sampler position in {position_path}"
             )
 
         # Run the sampler.
         sampler_results, final_walker_positions = run_emcee_once(
             model,
             data,
+            data_transformation,
             data_stdevs,
             slice,
             initial_walker_positions,
             num_walkers,
             num_steps,
             num_processes,
         )
@@ -227,79 +234,29 @@
             model, slice, run, sampler_results, final_walker_positions
         )
 
     (
         overall_params,
         overall_sim_results,
         overall_density_evals,
-    ) = concatenate_emcee_sampling_results(model, result_manager, slice)
+    ) = result_manager.load_slice_inference_results(
+        slice, num_burn_in_samples, thinning_factor
+    )
     result_manager.save_overall(
         slice,
-        overall_params[num_burn_in_samples::thinning_factor, :],
-        overall_sim_results[num_burn_in_samples::thinning_factor, :],
-        overall_density_evals[num_burn_in_samples::thinning_factor],
+        overall_params,
+        overall_sim_results,
+        overall_density_evals,
     )
     return (
-        overall_params[num_burn_in_samples::thinning_factor, :],
-        overall_sim_results[num_burn_in_samples::thinning_factor, :],
-        overall_density_evals[num_burn_in_samples::thinning_factor],
-    )
-
-
-# TODO: Make this a method of the ResultManager? It uses the ResultManager to load the results and many hard coded paths.
-def concatenate_emcee_sampling_results(
-    model: Model, result_manager: ResultManager, slice: np.ndarray
-) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """Concatenate many sub runs of the emcee sampler to create 3 large files for sampled parameters, corresponding simulation results and density evaluations.
-        These files are later used for result visualization.
-
-    Args:
-        model (Model): The model for which the results should be concatenated
-        result_manager (ResultManager): ResultManager to load the results from
-        slice (np.ndarray): slice for which the results should be concatenated
-
-    Returns:
-        typing.Tuple[np.ndarray, np.ndarray, np.ndarray]: Array with all params, array with all data, array with all log probabilities
-
-    """
-
-    # Count and print how many sub runs are ready to be merged.
-    num_existing_files = result_manager.count_emcee_sub_runs(slice)
-    logger.info(f"{num_existing_files} existing files found for concatenation")
-
-    densityFiles = (
-        result_manager.get_slice_path(slice)
-        + "/DensityEvals/density_evals_{}.csv"
-    )
-    sim_result_files = (
-        result_manager.get_slice_path(slice) + "/SimResults/sim_results_{}.csv"
-    )
-    paramFiles = result_manager.get_slice_path(slice) + "/Params/params_{}.csv"
-
-    overall_params = np.vstack(
-        [
-            np.loadtxt(paramFiles.format(i), delimiter=",", ndmin=2)
-            for i in range(num_existing_files)
-        ]
-    )
-    overall_sim_results = np.vstack(
-        [
-            np.loadtxt(sim_result_files.format(i), delimiter=",", ndmin=2)
-            for i in range(num_existing_files)
-        ]
-    )
-    overall_density_evals = np.hstack(
-        [
-            np.loadtxt(densityFiles.format(i), delimiter=",")
-            for i in range(num_existing_files)
-        ]
+        overall_params,
+        overall_sim_results,
+        overall_density_evals,
     )
 
-    return overall_params, overall_sim_results, overall_density_evals
-
 
 def calc_walker_acceptance(
     model: Model,
     slice: np.ndarray,
     num_walkers: int,
     num_burn_in_samples: int,
     result_manager: ResultManager,
@@ -307,28 +264,30 @@
     """Calculate the acceptance ratio for each individual walker of the emcee chain.
     This is especially important to find "zombie" walkers, that are never moving.
 
     Args:
         model (Model): The model for which the acceptance ratio should be calculated
         slice (np.ndarray): slice for which the acceptance ratio should be calculated
         num_walkers (int): number of walkers in the emcee chain
-        num_burn_in_samples (int): number of samples that were ignored at the beginning of each chain
+        num_burn_in_samples(int): Number of samples that will be deleted (burned) per chain (i.e. walker). Only for mcmc inference.
         result_manager (ResultManager): ResultManager to load the results from
 
     Returns:
         np.ndarray: Array with the acceptance ratio for each walker
 
     """
 
     # load the emcee parameter chain
-    params = np.loadtxt(
-        result_manager.get_slice_path(slice) + "/overall_params.csv",
-        delimiter=",",
-        ndmin=2,
-    )[num_burn_in_samples:, :]
+    (
+        params,
+        sim_res,
+        density_evals,
+    ) = result_manager.load_slice_inference_results(
+        slice, num_burn_in_samples, 1
+    )
 
     # calculate the number of steps each walker walked
     # subtract 1 because we count the steps between the parameters
     num_steps = int(params.shape[0] / num_walkers) - 1
 
     # Unflatten the parameter chain and count the number of accepted steps for each walker
     params = params.reshape(num_steps + 1, num_walkers, model.param_dim)
@@ -346,89 +305,92 @@
 
     return acceptanceRatios
 
 
 def inference_mcmc(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     result_manager: ResultManager,
     slices: list[np.ndarray],
     num_processes: int,
     num_runs: int = 1,
     num_walkers: int = 10,
     num_steps: int = 2500,
     num_burn_in_samples: typing.Optional[int] = None,
     thinning_factor: typing.Optional[int] = None,
-    calc_walker_acceptance_bool: bool = False,
+    get_walker_acceptance: bool = False,
 ) -> typing.Tuple[
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     ResultManager,
 ]:
     """This function runs a MCMC sampling for the given model and data.
 
     Args:
         model (Model): The model describing the mapping from parameters to data.
         data (np.ndarray): The data to be used for the inference.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         result_manager (ResultManager): The result manager to be used for the inference.
         slices (np.ndarray): A list of slices to be used for the inference.
         num_processes (int): The number of processes to be used for the inference.
         num_runs (int, optional): The number of runs to be used for the inference. For each run except the first, all walkers continue with the end position of the previous run - this parameter does not affect the number of Markov chains, but how often results for each chain are saved. Defaults to 1.
         num_walkers (int, optional): The number of walkers to be used for the inference. Corresponds to the number of Markov chains. Defaults to 10.
         num_steps (int, optional): The number of steps to be used for the inference. Defaults to 2500.
         num_burn_in_samples (int, optional): number of samples to be discarded as burn-in. Defaults to None means a burn in of 10% of the total number of samples.
         thinning_factor (int, optional): thinning factor for the samples. Defaults to None means no thinning.
-        calc_walker_acceptance_bool (bool, optional): If True, the acceptance rate of the walkers is calculated and printed. Defaults to False.
+        get_walker_acceptance (bool, optional): If True, the acceptance rate of the walkers is calculated and printed. Defaults to False.
 
     Returns:
         Tuple[typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], ResultManager]: The parameter samples, the corresponding simulation results, the corresponding density
         evaluations for each slice and the result manager used for the inference.
 
     """
     # Set default values for burn in and thinning factor
     if num_burn_in_samples is None:
-        num_burn_in_samples = int(num_runs * num_walkers * num_steps * 0.1)
+        num_burn_in_samples = int(num_runs * num_steps * 0.1)
     if thinning_factor is None:
         thinning_factor = 1
 
     # create the return dictionaries
     overall_params, overall_sim_results, overall_density_evals = {}, {}, {}
 
     for slice in slices:
         slice_name = result_manager.get_slice_name(slice)
+        result_manager.save_inference_information(
+            slice=slice,
+            model=model,
+            inference_type=InferenceType.MCMC,
+            num_processes=num_processes,
+            num_runs=num_runs,
+            num_walkers=num_walkers,
+            num_steps=num_steps,
+            num_burn_in_samples=num_burn_in_samples,
+            thinning_factor=thinning_factor,
+        )
         (
             overall_params[slice_name],
             overall_sim_results[slice_name],
             overall_density_evals[slice_name],
         ) = run_emcee_sampling(
             model=model,
             data=data,
+            data_transformation=data_transformation,
             slice=slice,
             result_manager=result_manager,
             num_runs=num_runs,
             num_walkers=num_walkers,
             num_steps=num_steps,
             num_burn_in_samples=num_burn_in_samples,
             thinning_factor=thinning_factor,
             num_processes=num_processes,
         )
-        result_manager.save_inference_information(
-            slice=slice,
-            model=model,
-            inference_type=InferenceType.MCMC,
-            num_processes=num_processes,
-            num_runs=num_runs,
-            num_walkers=num_walkers,
-            num_steps=num_steps,
-            num_burn_in_samples=num_burn_in_samples,
-            thinning_factor=thinning_factor,
-        )
 
-        if calc_walker_acceptance_bool:
+        if get_walker_acceptance:
             num_burn_in_steps = int(num_steps * num_runs * 0.01)
             acceptance = calc_walker_acceptance(
                 model, slice, num_walkers, num_burn_in_steps, result_manager
             )
             logger.info(f"Acceptance rate for slice {slice}: {acceptance}")
 
     return (
```

### Comparing `eulerpi-0.2.1/eulerpi/core/sparsegrid.py` & `eulerpi-0.3.0/eulerpi/core/sparsegrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import typing
 from itertools import repeat
 from multiprocessing import get_context
 
 import numpy as np
 
 from eulerpi import logger
+from eulerpi.core.data_transformation import DataTransformation
 from eulerpi.core.inference_types import InferenceType
 from eulerpi.core.kde import calc_kernel_width
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.transformations import evaluate_density
 
 
@@ -365,53 +366,65 @@
                             self.levels,
                         )
                         * self.coeffs[p]
                     )
 
 
 def evaluate_on_sparse_grid(
-    args: typing.Tuple[np.ndarray, Model, np.ndarray, np.ndarray, np.ndarray]
+    args: typing.Tuple[
+        np.ndarray,
+        Model,
+        np.ndarray,
+        DataTransformation,
+        np.ndarray,
+        np.ndarray,
+    ]
 ) -> np.ndarray:
     """This function is used to evaluate a function on a sparse grid in parallel. The input args is a tuple containing the function, the sparse grid and the number of processes to be used.
 
     Args:
         params (np.ndarray): The parameters to be evaluated.
         model(Model): The model used for the inference.
         data(np.ndarray): The data points used for the inference.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs(np.ndarray): The standard deviations of the data points. (Currently the kernel width, #TODO!)
         slice(np.ndarray): The slice defines for which dimensions of the grid points / paramater vectors the marginal density should be evaluated.
 
     Returns:
         np.ndarray: The density values for the given params.
     """
 
-    params, model, data, data_stdevs, slice = args
-    return evaluate_density(params, model, data, data_stdevs, slice)[1]
+    params, model, data, data_transformation, data_stdevs, slice = args
+    return evaluate_density(
+        params, model, data, data_transformation, data_stdevs, slice
+    )[1]
 
 
 def inference_sparse_grid(
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     result_manager: ResultManager,
     slices: typing.List[np.ndarray],
     num_processes: int,
     num_levels: int = 5,
 ) -> typing.Tuple[
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     typing.Dict[str, np.ndarray],
     ResultManager,
 ]:
     """Evaluates the transformed parameter density over a set of points resembling a sparse grid, thereby attempting parameter inference. If a data path is given, it is used to load the data for the model. Else, the default data path of the model is used.
 
     Args:
-      model(Model): The model describing the mapping from parameters to data.
-      data(np.ndarray): The data to be used for inference.
-      num_processes(int): number of processes to use for parallel evaluation of the model.
-      num_levels(int, optional): Maximum sparse grid level depth that mainly defines the number of points. Defaults to 5.
+        model(Model): The model describing the mapping from parameters to data.
+        data(np.ndarray): The data to be used for inference.
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
+        num_processes(int): number of processes to use for parallel evaluation of the model.
+        num_levels(int, optional): Maximum sparse grid level depth that mainly defines the number of points. Defaults to 5.
 
     Returns:
         Tuple[typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], typing.Dict[str, np.ndarray], ResultManager]: The parameter samples, the corresponding simulation results, the corresponding density
         evaluations for each slice and the result manager used for the inference.
 
     """
 
@@ -437,14 +450,15 @@
 
         # Create a pool of worker processes
         pool = get_context("spawn").Pool(processes=num_processes)
         tasks = zip(
             scaledSparseGridPoints,
             repeat(model),
             repeat(data),
+            repeat(data_transformation),
             repeat(data_stdevs),
             repeat(slice),
         )
 
         # evaluate the probability density transformation for all sparse grid points in parallel
         results = pool.map(
             evaluate_on_sparse_grid,
@@ -455,28 +469,30 @@
         pool.close()
         pool.join()
 
         # convert the results to a numpy array
         # Take care! The results here are for single points, therefore we cant use np.concatenate
         results = np.vstack(results)
 
+        data_dim = model.data_dim
+
         # save the results
         result_manager.save_overall(
             slice,
             results[:, 0 : slice.shape[0]],
-            results[:, slice.shape[0] : slice.shape[0] + data.shape[1]],
-            results[:, slice.shape[0] + data.shape[1] :],
+            results[:, slice.shape[0] : slice.shape[0] + data_dim],
+            results[:, slice.shape[0] + data_dim :],
         )
         slice_name = result_manager.get_slice_name(slice)
         overall_params[slice_name] = results[:, 0 : slice.shape[0]]
         overall_sim_results[slice_name] = results[
-            :, slice.shape[0] : slice.shape[0] + data.shape[1]
+            :, slice.shape[0] : slice.shape[0] + data_dim
         ]
         overall_density_evals[slice_name] = results[
-            :, slice.shape[0] + data.shape[1] :
+            :, slice.shape[0] + data_dim :
         ]
         result_manager.save_inference_information(
             slice=slice,
             model=model,
             inference_type=InferenceType.SPARSE_GRID,
             num_processes=num_processes,
             num_levels=num_levels,
```

### Comparing `eulerpi-0.2.1/eulerpi/core/transformations.py` & `eulerpi-0.3.0/eulerpi/core/transformations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from typing import Tuple
 
 import jax.numpy as jnp
 import numpy as np
 from jax import jit
 
 from eulerpi import logger
+from eulerpi.core.data_transformation import DataTransformation
 from eulerpi.core.kde import eval_kde_gauss
 from eulerpi.core.model import Model
 
 
 def evaluate_density(
     param: np.ndarray,
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
 ) -> Tuple[np.double, np.ndarray]:
     """Given a simulation model, its derivative and corresponding data, evaluate the parameter density that is the backtransformed data distribution.
 
     Args:
         param (np.ndarray): parameter for which the transformed density shall be evaluated
         model (Model): model to be evaluated
         data (np.ndarray): data for the model. 2D array with shape (#num_data_points, #data_dim)
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs (np.ndarray): array of suitable kernel width for each data dimension
         slice (np.ndarray): slice of the parameter vector that is to be evaluated
 
     Returns:
         Tuple[np.double, np.ndarray]:
             : parameter density at the point param
             : vector containing the parameter, the simulation result and the density
@@ -43,23 +46,32 @@
             "Parameters outside of predefined range"
         )  # Slows down the sampling to much? -> Change logger level to warning or even error
         return 0, np.zeros(slice.shape[0] + model.data_dim + 1)
 
     # If the parameter is within the valid ranges...
     else:
         # Evaluating the model and the jacobian for the specified parameter simultaneously provide a little speedup over calculating it separately in some cases.
-        sim_res, jac = model.forward_and_jacobian(fullParam)
+        sim_res, model_jac = model.forward_and_jacobian(fullParam)
 
-        # TODO transform sim res and use transformed simres below
+        # normalize sim_res
+        transformed_sim_res = data_transformation.transform(sim_res)
 
-        # Evaluate the data density in the simulation result. # TODO scale with determinant transformation matrix
-        densityEvaluation = eval_kde_gauss(data, sim_res, data_stdevs)
+        # Evaluate the data density in the simulation result.
+        densityEvaluation = eval_kde_gauss(
+            data, transformed_sim_res, data_stdevs
+        )
 
         # Calculate the simulation model's pseudo-determinant in the parameter point (also called the correction factor).
-        correction = calc_gram_determinant(jac)
+        # Scale with the determinant of the transformation matrix.
+        transformation_jac = data_transformation.jacobian(sim_res)
+        correction = calc_gram_determinant(
+            jnp.dot(
+                transformation_jac, model_jac
+            )  # We use dot, because matmul does not support scalars
+        )
 
         # Multiply data density and correction factor.
         trafo_density_evaluation = densityEvaluation * correction
 
         # Store the current parameter, its simulation result as well as its density in a large vector that is stored separately by emcee.
         evaluation_results = np.concatenate(
             (param, sim_res, np.array([trafo_density_evaluation]))
@@ -68,36 +80,37 @@
         return trafo_density_evaluation, evaluation_results
 
 
 def eval_log_transformed_density(
     param: np.ndarray,
     model: Model,
     data: np.ndarray,
+    data_transformation: DataTransformation,
     data_stdevs: np.ndarray,
     slice: np.ndarray,
 ) -> Tuple[np.double, np.ndarray]:
     """Given a simulation model, its derivative and corresponding data, evaluate the natural log of the parameter density that is the backtransformed data distribution.
         This function is intended to be used with the emcee sampler and can be implemented more efficiently at some points.
 
     Args:
         param (np.ndarray): parameter for which the transformed density shall be evaluated
         model (Model): model to be evaluated
         data (np.ndarray): data for the model. 2D array with shape (#num_data_points, #data_dim)
+        data_transformation (DataTransformation): The data transformation used to normalize the data.
         data_stdevs (np.ndarray): array of suitable kernel width for each data dimension
         slice (np.ndarray): slice of the parameter vector that is to be evaluated
 
     Returns:
         Tuple[np.double, np.ndarray]:
             : natural log of the parameter density at the point param
             : sampler_results (array concatenation of parameters, simulation results and evaluated density, stored as "blob" by the emcee sampler)
 
     """
-    # TODO give transformation object to evaluation function
     trafo_density_evaluation, evaluation_results = evaluate_density(
-        param, model, data, data_stdevs, slice
+        param, model, data, data_transformation, data_stdevs, slice
     )
     if trafo_density_evaluation == 0:
         return -np.inf, evaluation_results
     return np.log(trafo_density_evaluation), evaluation_results
 
 
 def calc_gram_determinant(jac: jnp.ndarray) -> jnp.double:
```

### Comparing `eulerpi-0.2.1/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.3.0/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/corona/corona.py` & `eulerpi-0.3.0/eulerpi/examples/corona/corona.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.3.0/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.3.0/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.3.0/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.3.0/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.3.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.py` & `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import numpy as np
 
 from eulerpi.core.model import ArtificialModelInterface, SBMLModel
 
 
 class MentenSBMLModel(SBMLModel, ArtificialModelInterface):
     """The MentenModel is a simple model for the Michaelis-Menten enzyme kinetics.
-    It requires a few adaptations to the SBMLModel class to work with the inference, because the first output of the model does not depend on the parameters.
+    It requires a few adaptations to the SBMLModel class to work with the inference, because
+    the first output of the model does not depend on the parameters and the second output is linear dependent on the third output.
     See data_dim, forward, jacobian, forward_and_jacobian.
     """
 
     CENTRAL_PARAM = np.array([50.0, 1.0])
     PARAM_LIMITS = np.array([[0.0, 100.0], [0.0, 2.0]])
 
     def __init__(
@@ -30,25 +31,25 @@
             param_limits,
             param_names,
             **kwargs,
         )
 
     @property
     def data_dim(self) -> int:
-        return 2
+        return 1
 
     def forward(self, params) -> np.ndarray:
-        return super().forward(params)[1:]
+        return super().forward(params)[2:]
 
     def jacobian(self, params) -> np.ndarray:
-        return super().jacobian(params)[1:, :]
+        return super().jacobian(params)[2:, :]
 
     def forward_and_jacobian(self, params) -> np.ndarray:
         val, jac = super().forward_and_jacobian(params)
-        return val[1:], jac[1:, :]
+        return val[2:], jac[2:, :]
 
     def generate_artificial_params(self, num_samples: int) -> np.ndarray:
         diff0 = 5.0
         diff1 = 0.2
         params = np.random.rand(num_samples, self.param_dim)
         params[:, 0] *= diff0
         params[:, 0] += 50.0 - diff0 / 2.0
```

### Comparing `eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/simple_models.py` & `eulerpi-0.3.0/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.3.0/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/stock/stock.py` & `eulerpi-0.3.0/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.3.0/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/eulerpi/jax_extension.py` & `eulerpi-0.3.0/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.1/pyproject.toml` & `eulerpi-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.2.1"
+version = "0.3.0"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -25,14 +25,15 @@
 diffrax = "^0.3.1"
 emcee = "^3.1.4"
 jaxlib = "^0.4.7"
 tqdm = "^4.65.0"
 seedir = "^0.4.2"
 yfinance = "^0.2.14"
 amici = "^0.16.1"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
```

### Comparing `eulerpi-0.2.1/PKG-INFO` & `eulerpi-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.2.1
+Version: 0.3.0
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: amici (>=0.16.1,<0.17.0)
 Requires-Dist: diffrax (>=0.3.1,<0.4.0)
 Requires-Dist: emcee (>=3.1.4,<4.0.0)
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seedir (>=0.4.2,<0.5.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: yfinance (>=0.2.14,<0.3.0)
 Project-URL: Bug Tracker, https://github.com/Systems-Theory-in-Systems-Biology/EPI/issues
 Project-URL: Documentation, https://Systems-Theory-in-Systems-Biology.github.io/EPI/
 Project-URL: Homepage, https://github.com/Systems-Theory-in-Systems-Biology/EPI
 Description-Content-Type: text/markdown
```

