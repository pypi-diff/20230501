# Comparing `tmp/strangeworks_vqe-0.1.2.tar.gz` & `tmp/strangeworks_vqe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_vqe-0.1.2.tar", max compression
+gzip compressed data, was "strangeworks_vqe-0.1.3.tar", max compression
```

## Comparing `strangeworks_vqe-0.1.2.tar` & `strangeworks_vqe-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       19 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/README.md
--rw-r--r--   0        0        0      659 2023-04-18 13:22:04.374911 strangeworks_vqe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    11128 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/sdk.py
--rw-r--r--   0        0        0      691 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/serializer.py
--rw-r--r--   0        0        0     5677 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/utils.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/README.md
+-rw-r--r--   0        0        0      659 2023-05-01 16:14:49.365245 strangeworks_vqe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/__init__.py
+-rw-r--r--   0        0        0    11090 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/sdk.py
+-rw-r--r--   0        0        0      691 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/serializer.py
+-rw-r--r--   0        0        0     5714 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/utils.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.3/PKG-INFO
```

### Comparing `strangeworks_vqe-0.1.2/pyproject.toml` & `strangeworks_vqe-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-vqe"
-version = "0.1.2"
+version = "0.1.3"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_vqe"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_vqe-0.1.2/strangeworks_vqe/sdk.py` & `strangeworks_vqe-0.1.3/strangeworks_vqe/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 from typing import Optional
 
 import strangeworks
 from strangeworks.core.errors.error import StrangeworksError
 
 import strangeworks_vqe.serializer as serializer
 import strangeworks_vqe.utils as utils
@@ -20,16 +19,18 @@
                 if rsc_list[rr].product.slug == "vqe":
                     self.rsc = rsc_list[rr]
 
         self.backend_list = " "
 
     def backends(self):
         """
-        To-Do: Add cross check as to which backends the current user actually has access to.
-                Currently, this just lists all backends that could work with the qaoa service.
+        To-Do: Add cross check as to which backends the current user actually has
+          access to.
+                Currently, this just lists all backends that could work with the qaoa
+                  service.
         """
 
         all_backends = strangeworks.backends(backend_type_slugs=["sw-vqe"])
 
         aws_backends = []
         aws_sim_backends = []
         ibmq_backends = []
@@ -56,15 +57,15 @@
                         backend_temp = {
                             "name": all_backends[bb].name,
                             "provider": "AWS",
                             "remote_status": all_backends[bb].remote_status,
                             "arn": all_backends[bb].remote_backend_id,
                         }
                         aws_backends.append(backend_temp)
-            except:
+            except AttributeError:
                 None
 
             try:
                 ibm_str = all_backends[bb].name[0:3]
                 id_str = all_backends[bb].remote_backend_id[0:3]
                 if ibm_str == "ibm":
                     if id_str == "ibm":
@@ -96,15 +97,15 @@
                     prov = "IBM_Simulator"
                     backend_temp = {
                         "backend_name": all_backends[bb].name,
                         "provider": prov,
                         "remote_status": all_backends[bb].remote_status,
                     }
                     ibm_sim_backends.append(backend_temp)
-            except:
+            except AttributeError:
                 None
 
         self.backend_list = {
             "AWS": aws_backends,
             "AWS_Sim": aws_sim_backends,
             "IBMQ": ibmq_backends,
             "IBM_Cloud": ibm_cloud_backends,
@@ -153,22 +154,16 @@
         string_list = H.primitive.paulis.to_labels()
         coeffs_list = H.primitive.coeffs.tolist()
         Ham = [string_list, coeffs_list]
 
         shotsin = problem_params["shotsin"]
         maxiter = problem_params["maxiter"]
         nqubits = problem_params["nqubits"]
-        try:
-            optimizer = problem_params["optimizer"]
-        except:
-            x = None
-        try:
-            ansatz = problem_params["ansatz"]
-        except:
-            None
+        optimizer = problem_params.get("optimizer", None)
+        ansatz = problem_params.get("ansatz", None)
 
         hyperparams = {
             "H": serializer.pickle_serializer(H, "json"),
             "Ham": serializer.pickle_serializer(Ham, "json"),
             "nqubits": str(nqubits),
             "maxiter": str(maxiter),
             "optimizer": optimizer,
```

### Comparing `strangeworks_vqe-0.1.2/strangeworks_vqe/serializer.py` & `strangeworks_vqe-0.1.3/strangeworks_vqe/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_vqe-0.1.2/strangeworks_vqe/utils.py` & `strangeworks_vqe-0.1.3/strangeworks_vqe/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,17 @@
 
 
 def convert_QUBO_to_Ising(QUBO_mat):
     nodes = np.size(QUBO_mat[0])
     Ising_mat = QUBO_mat / 4
 
     for nn in range(nodes):
-        Ising_mat[nn][nn] = QUBO_mat[nn][nn] / 2 + sum(QUBO_mat[nn][nn + 1:] / 4)
+        Ising_mat[nn][nn] = QUBO_mat[nn][nn] / 2 + sum(
+            QUBO_mat[nn][nn + 1 :] / 4  # noqa: E203
+        )
 
     for nn in range(nodes):
         Ising_mat[nn][nn] += sum(QUBO_mat[:nn, nn] / 4)
 
     return Ising_mat
```

### Comparing `strangeworks_vqe-0.1.2/PKG-INFO` & `strangeworks_vqe-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-vqe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

