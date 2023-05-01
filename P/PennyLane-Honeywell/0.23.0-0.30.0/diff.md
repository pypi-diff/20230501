# Comparing `tmp/PennyLane_Honeywell-0.23.0-py3-none-any.whl.zip` & `tmp/PennyLane_Honeywell-0.30.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14810 bytes, number of entries: 9
--rw-r--r--  2.0 unx      770 b- defN 22-Apr-25 22:40 pennylane_honeywell/__init__.py
--rw-r--r--  2.0 unx      692 b- defN 22-Apr-25 22:40 pennylane_honeywell/_version.py
--rw-r--r--  2.0 unx    16409 b- defN 22-Apr-25 22:40 pennylane_honeywell/device.py
--rw-r--r--  2.0 unx    11558 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7884 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      821 b- defN 22-Apr-25 22:40 PennyLane_Honeywell-0.23.0.dist-info/RECORD
-9 files, 38313 bytes uncompressed, 13368 bytes compressed:  65.1%
+Zip file size: 14954 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      770 b- defN 23-May-01 19:02 pennylane_honeywell/__init__.py
+-rw-r--r--  2.0 unx      692 b- defN 23-May-01 19:02 pennylane_honeywell/_version.py
+-rw-r--r--  2.0 unx    16796 b- defN 23-May-01 19:02 pennylane_honeywell/device.py
+-rw-r--r--  2.0 unx    11558 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7843 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      821 b- defN 23-May-01 19:02 PennyLane_Honeywell-0.30.0.dist-info/RECORD
+9 files, 38659 bytes uncompressed, 13512 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pennylane_honeywell/_version.py
 Comment: 
 
 Filename: pennylane_honeywell/device.py
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/LICENSE
+Filename: PennyLane_Honeywell-0.30.0.dist-info/LICENSE
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/METADATA
+Filename: PennyLane_Honeywell-0.30.0.dist-info/METADATA
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/WHEEL
+Filename: PennyLane_Honeywell-0.30.0.dist-info/WHEEL
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/entry_points.txt
+Filename: PennyLane_Honeywell-0.30.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/top_level.txt
+Filename: PennyLane_Honeywell-0.30.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PennyLane_Honeywell-0.23.0.dist-info/RECORD
+Filename: PennyLane_Honeywell-0.30.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pennylane_honeywell/_version.py

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.23.0"
+__version__ = "0.30.0"
```

## pennylane_honeywell/device.py

```diff
@@ -98,15 +98,15 @@
             been saved to the config file automatically by the ``save_tokens`` method.
         retry_delay (float): The time (in seconds) to wait between requests
             to the remote server when checking for completion of circuit
             execution.
     """
     # pylint: disable=too-many-instance-attributes
     name = "Honeywell Quantum Solutions PennyLane plugin"
-    pennylane_requires = ">=0.15.0"
+    pennylane_requires = ">=0.30.0"
     version = __version__
     author = "Xanadu Inc."
     _capabilities = {
         "model": "qubit",
         "tensor_observables": True,
         "inverse_operations": True,
     }
@@ -442,15 +442,14 @@
             response = requests.get(job_endpoint, headers=header)
             response.raise_for_status()
 
             job_data = response.json()
         return job_data
 
     def execute(self, tape, **kwargs):
-
         self.check_validity(tape.operations, tape.observables)
         response = self._submit_circuit(tape)
         response.raise_for_status()
 
         job_data = response.json()
 
         job_data = self._query_results(job_data)
@@ -472,24 +471,33 @@
         # pylint: disable=attribute-defined-outside-init
         self._results = job_data["results"]["c"]  # list of binary strings
 
         # generate computational basis samples
         self._samples = self.generate_samples()
 
         # compute the required statistics
-        results = self.statistics(tape.observables)
+        if not qml.active_return():
+            results = self._statistics_legacy(tape)
+        else:
+            results = self.statistics(tape)
 
         # Ensures that a combination with sample does not put
         # expvals and vars in superfluous arrays
         all_sampled = all(obs.return_type is Sample for obs in tape.observables)
         if tape.is_sampled and not all_sampled:
             return self._asarray(results, dtype="object")  # pragma: no cover
 
         return self._asarray(results)
 
+    def _execute_legacy(self, tape, **kwargs):
+        """Wrapper for ``execute`` to be consistent with ``QubitDevice`` for the old
+        return type."""
+        # This function just runs `execute`, which handles both the new and old return types
+        return self.execute(tape, **kwargs)
+
     def generate_samples(self):
         int_values = [int(x, 2) for x in self._results]
         samples_array = np.stack(np.unravel_index(int_values, [2] * self.num_wires)).T
         return samples_array
 
     def apply(self, operations, **kwargs):  # pragma: no cover
         """This method is not used in the HQSDevice class."""
```

## Comparing `PennyLane_Honeywell-0.23.0.dist-info/LICENSE` & `PennyLane_Honeywell-0.30.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PennyLane_Honeywell-0.23.0.dist-info/METADATA` & `PennyLane_Honeywell-0.30.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Honeywell
-Version: 0.23.0
+Version: 0.30.0
 Summary: PennyLane plugin to access the Honeywell Quantum Solutions cloud service.
 Home-page: http://xanadu.ai
 Maintainer: Xanadu Inc.
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -13,23 +13,22 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pennylane_honeywell
-Requires-Dist: pennylane (>=0.23)
+Requires-Dist: pennylane (>=0.30)
 Requires-Dist: requests
 Requires-Dist: pyjwt
 Requires-Dist: toml
 
 PennyLane-Honeywell Plugin
 ##########################
 
@@ -41,17 +40,17 @@
     :alt: Codecov coverage
     :target: https://codecov.io/gh/PennyLaneAI/pennylane-honeywell
 
 .. image:: https://img.shields.io/codefactor/grade/github/PennyLaneAI/pennylane-honeywell/master?logo=codefactor&style=flat-square
     :alt: CodeFactor Grade
     :target: https://www.codefactor.io/repository/github/pennylaneai/pennylane-honeywell
 
-.. image:: https://img.shields.io/readthedocs/pennylane-honeywell.svg?logo=read-the-docs&style=flat-square
+.. image:: https://readthedocs.com/projects/xanaduai-pennylane-honeywell/badge/?version=latest&style=flat-square
     :alt: Read the Docs
-    :target: https://pennylane-honeywell.readthedocs.io
+    :target: https://docs.pennylane.ai/projects/honeywell
 
 .. image:: https://img.shields.io/pypi/v/PennyLane-honeywell.svg?style=flat-square
     :alt: PyPI
     :target: https://pypi.org/project/PennyLane-honeywell
 
 .. image:: https://img.shields.io/pypi/pyversions/PennyLane-honeywell.svg?style=flat-square
     :alt: PyPI - Python Version
```

## Comparing `PennyLane_Honeywell-0.23.0.dist-info/RECORD` & `PennyLane_Honeywell-0.30.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pennylane_honeywell/__init__.py,sha256=qmjGWYag6PbZuVf4aZmtWE-51JV8W0Jui574XMrAufc,770
-pennylane_honeywell/_version.py,sha256=1eMm85l7y2zBpw-4tLWgPv8aAvoCvUWvbQDNI5Wx2us,692
-pennylane_honeywell/device.py,sha256=PAdKoujfwwX4_XPhDeNNo0zce16a_h8JJlG-MLIdlic,16409
-PennyLane_Honeywell-0.23.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-PennyLane_Honeywell-0.23.0.dist-info/METADATA,sha256=BuMgTCAM6Lik_87rX7WaPi1HJrPTVdaj_ZA9wBIjmZ4,7884
-PennyLane_Honeywell-0.23.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PennyLane_Honeywell-0.23.0.dist-info/entry_points.txt,sha256=7FXaAFNMKGYsVdZIZZOg3LWqWm4XfXJi7it9t8s_8lY,67
-PennyLane_Honeywell-0.23.0.dist-info/top_level.txt,sha256=hN6X_-V8ZqyJ-S-mbRzA1_yERmO_LWwPz-y72KjI1M0,20
-PennyLane_Honeywell-0.23.0.dist-info/RECORD,,
+pennylane_honeywell/_version.py,sha256=BlcXfPBaERzCvbKv1iJpNAns8dL3I4Uy0IxhYXAYJTo,692
+pennylane_honeywell/device.py,sha256=CnCfBodteWG0T6hBAWqxflFu4x18dMFM8TACyaC5Fc4,16796
+PennyLane_Honeywell-0.30.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+PennyLane_Honeywell-0.30.0.dist-info/METADATA,sha256=ErHL5WFMyohRCePwgDDX0PWyMBzd6cX-Bpy-TpaTIlI,7843
+PennyLane_Honeywell-0.30.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PennyLane_Honeywell-0.30.0.dist-info/entry_points.txt,sha256=7FXaAFNMKGYsVdZIZZOg3LWqWm4XfXJi7it9t8s_8lY,67
+PennyLane_Honeywell-0.30.0.dist-info/top_level.txt,sha256=hN6X_-V8ZqyJ-S-mbRzA1_yERmO_LWwPz-y72KjI1M0,20
+PennyLane_Honeywell-0.30.0.dist-info/RECORD,,
```

