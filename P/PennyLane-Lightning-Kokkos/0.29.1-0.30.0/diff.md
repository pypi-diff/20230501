# Comparing `tmp/PennyLane-Lightning-Kokkos-0.29.1.tar.gz` & `tmp/PennyLane-Lightning-Kokkos-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane-Lightning-Kokkos-0.29.1.tar", last modified: Fri Mar 10 20:30:11 2023, max compression
+gzip compressed data, was "PennyLane-Lightning-Kokkos-0.30.0.tar", last modified: Mon May  1 20:15:25 2023, max compression
```

## Comparing `PennyLane-Lightning-Kokkos-0.29.1.tar` & `PennyLane-Lightning-Kokkos-0.30.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-03-10 20:30:11.241275 PennyLane-Lightning-Kokkos-0.29.1/.github/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5286 2023-03-10 20:13:39.000000 PennyLane-Lightning-Kokkos-0.29.1/.github/CHANGELOG.md
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/LICENSE
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       53 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/MANIFEST.in
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/PKG-INFO
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      591 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/dependency_links.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       82 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/entry_points.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       16 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/requires.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-03-10 20:30:11.000000 PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/top_level.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4509 2023-03-10 20:13:39.000000 PennyLane-Lightning-Kokkos-0.29.1/README.rst
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      730 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/__init__.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10167 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/_serialize.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      697 2023-03-10 20:14:24.000000 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/_version.py
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)    30520 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/lightning_kokkos.py
-drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/src/
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)      469 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/src/CMakeLists.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       99 2023-03-10 20:02:32.000000 PennyLane-Lightning-Kokkos-0.29.1/requirements.txt
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-03-10 20:30:11.244609 PennyLane-Lightning-Kokkos-0.29.1/setup.cfg
--rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7464 2023-03-10 20:13:39.000000 PennyLane-Lightning-Kokkos-0.29.1/setup.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.937004 PennyLane-Lightning-Kokkos-0.30.0/.github/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6769 2023-05-01 19:56:53.000000 PennyLane-Lightning-Kokkos-0.30.0/.github/CHANGELOG.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/LICENSE
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       53 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/MANIFEST.in
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/PKG-INFO
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.937004 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5598 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      591 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/dependency_links.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       82 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/entry_points.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       16 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/requires.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-05-01 20:15:25.000000 PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/top_level.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4509 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/README.rst
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      730 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/__init__.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10963 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_serialize.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      697 2023-05-01 19:57:30.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_version.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    31177 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/lightning_kokkos.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/src/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      469 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/src/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       99 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/requirements.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-05-01 20:15:25.940338 PennyLane-Lightning-Kokkos-0.30.0/setup.cfg
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7670 2023-05-01 19:56:43.000000 PennyLane-Lightning-Kokkos-0.30.0/setup.py
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/.github/CHANGELOG.md` & `PennyLane-Lightning-Kokkos-0.30.0/.github/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+# Release 0.30.0
+
+### New features since last release
+
+* Add native support for `expval` and `var` of generic observables. Refactor measurements support.
+[(#47)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/47)
+
+### Breaking changes
+
+* Provide support for PennyLane-Lightning-Kokkos to coexist with PennyLane-Lightning.
+[(#49)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/49)
+
+### Improvements
+
+* Remove deprecated `set-output` commands from workflow files.
+[(#56)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/56)
+
+* `setup.py` works on MacOS without `brew` (which is required by Conda-Forge runners).
+[(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
+
+* MacOS::Intel wheels are built for the SERIAL and THREADS Kokkos backends.
+[(#48)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/48)
+
+* Wheels are now checked with `twine check` post-creation for PyPI compatibility.
+[(#50)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/50)
+
+* Template n-qubit gate methods.
+[(#40)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/40)
+
+### Bug fixes
+
+* Updates to use the new call signature for `QuantumScript.get_operation`.
+  [(#52)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/52)
+
+
+### Contributors
+
+This release contains contributions from (in alphabetical order):
+
+Ali Asadi, Lee James O'Riordan, Vincent Michaud-Rioux, Romain Moyard
+
+---
+
 # Release 0.29.1
 
 ### Improvements
 
 * Use CMake `find_package` to bind pre-installed Kokkos libraries.
 [(#43)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/43)
 
@@ -23,21 +66,23 @@
 ### New features since last release
 
  * Add support for building X86-64 Linux wheels with OpenMP and SERIAL backends with Github Actions.
  [(#14)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/14)
 
  * Add the `kokkos_config` class variable, which stores the kokkos build and runtime information such as `Backend`, `Architecture`, `Kokkos Version`, `Compiler`, to LightningKokkos for users' query purpose. Users can also access other information such as `Options`, `Memory`, `Atomics` and `Vectorization` from `kokkos_config`.
  The workflow for build and runtime information query is:
+
  ```python
  >>> import pennylane as qml
  >>> dev = qml.device('lightning.kokkos', wires=3)
  >>> dev.kokkos_config["Backend"]
  {'Parallel': 'OpenMP'}
  ```
- [(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
+[(#17)](https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/17)
+
 
 ### Breaking changes
 
 * Change LightningKokkos to inherit from QubitDevice instead of LightningQubit. Numpy data initialization is decoupled.
 [(#31)] (https://github.com/PennyLaneAI/pennylane-lightning-kokkos/pull/31)
 
 ### Improvements
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/LICENSE` & `PennyLane-Lightning-Kokkos-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/PKG-INFO` & `PennyLane-Lightning-Kokkos-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning-Kokkos
-Version: 0.29.1
+Version: 0.30.0
 Summary: PennyLane-Lightning-Kokkos plugin
 Home-page: https://github.com/PennyLaneAI/pennylane-lightning-kokkos
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO` & `PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning-Kokkos
-Version: 0.29.1
+Version: 0.30.0
 Summary: PennyLane-Lightning-Kokkos plugin
 Home-page: https://github.com/PennyLaneAI/pennylane-lightning-kokkos
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt` & `PennyLane-Lightning-Kokkos-0.30.0/PennyLane_Lightning_Kokkos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/README.rst` & `PennyLane-Lightning-Kokkos-0.30.0/README.rst`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/__init__.py` & `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/_serialize.py` & `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_serialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 """
 from typing import List, Tuple
 
 import numpy as np
 from pennylane import (
     BasisState,
     Hadamard,
-    Projector,
+    PauliX,
+    PauliY,
+    PauliZ,
+    Identity,
     QubitStateVector,
     Rot,
 )
-from pennylane.grouping import is_pauli_word
-from pennylane.operation import Observable, Tensor
-from pennylane.ops.qubit.observables import Hermitian
+from pennylane.operation import Tensor
 from pennylane.ops.op_math import Adjoint
 from pennylane.tape import QuantumTape
 
 # Remove after the next release of PL
 # Add from pennylane import matrix
 import pennylane as qml
 
@@ -48,57 +49,38 @@
         SparseHamiltonianKokkos_C128,
         HermitianObsKokkos_C64,
         HermitianObsKokkos_C128,
     )
 except ImportError as e:
     print(e)
 
-
-def _obs_has_kernel(obs: Observable) -> bool:
-    """Returns True if the input observable has a supported kernel in the C++ backend.
-
-    Args:
-        obs (Observable): the input observable
-
-    Returns:
-        bool: indicating whether ``obs`` has a dedicated kernel in the backend
-    """
-    if is_pauli_word(obs):
-        return True
-    if isinstance(obs, (Hadamard, Projector)):
-        return True
-    if isinstance(obs, Tensor):
-        return all(_obs_has_kernel(o) for o in obs.obs)
-    return False
+pauli_name_map = {
+    "I": "Identity",
+    "X": "PauliX",
+    "Y": "PauliY",
+    "Z": "PauliZ",
+}
 
 
 def _serialize_named_ob(o, wires_map: dict, use_csingle: bool):
     """Serializes an observable (Named)
 
     Args:
         o (Observable): the input observable (Named)
         wire_map (dict): a dictionary mapping input wires to the device's backend wires
         use_csingle (bool): whether to use np.complex64 instead of np.complex128
 
     Returns:
         named_obs (NamedObsKokkos_C64 or NamedObsKokkos_C128): A Named observable object compatible with the C++ backend
     """
-    assert not isinstance(o, Tensor)
-
-    if use_csingle:
-        ctype = np.complex64
-        named_obs = NamedObsKokkos_C64
-    else:
-        ctype = np.complex128
-        named_obs = NamedObsKokkos_C128
-
-    wires_list = o.wires.tolist()
-    wires = [wires_map[w] for w in wires_list]
-    if _obs_has_kernel(o):
-        return named_obs(o.name, wires)
+    named_obs = NamedObsKokkos_C64 if use_csingle else NamedObsKokkos_C128
+    wires = [wires_map[w] for w in o.wires]
+    if o.name == "Identity":
+        wires = wires[:1]
+    return named_obs(o.name, wires)
 
 
 def _serialize_tensor_ob(ob, wires_map: dict, use_csingle: bool):
     """Serialize an observable (Tensor)
 
     Args:
         o (Observable): the input observable (Tensor)
@@ -190,14 +172,47 @@
         rtype = np.float64
         hermitian_obs = HermitianObsKokkos_C128
 
     data = qml.matrix(ob).astype(rtype).ravel(order="C")
     return hermitian_obs(data, ob.wires.tolist())
 
 
+def _serialize_pauli_word(ob, wires_map: dict, use_csingle: bool):
+    """Serialize a :class:`pennylane.pauli.PauliWord` into a Named or Tensor observable."""
+    if use_csingle:
+        named_obs = NamedObsKokkos_C64
+        tensor_obs = TensorProdObsKokkos_C64
+    else:
+        named_obs = NamedObsKokkos_C128
+        tensor_obs = TensorProdObsKokkos_C128
+
+    if len(ob) == 1:
+        wire, pauli = list(ob.items())[0]
+        return named_obs(pauli_name_map[pauli], [wires_map[wire]])
+
+    return tensor_obs(
+        [named_obs(pauli_name_map[pauli], [wires_map[wire]]) for wire, pauli in ob.items()]
+    )
+
+
+def _serialize_pauli_sentence(ob, wires_map: dict, use_csingle: bool):
+    """Serialize a :class:`pennylane.pauli.PauliSentence` into a Hamiltonian."""
+    if use_csingle:
+        rtype = np.float32
+        hamiltonian_obs = HamiltonianKokkos_C64
+    else:
+        rtype = np.float64
+        hamiltonian_obs = HamiltonianKokkos_C128
+
+    pwords, coeffs = zip(*ob.items())
+    terms = [_serialize_pauli_word(pw, wires_map, use_csingle) for pw in pwords]
+    coeffs = np.array(coeffs).astype(rtype)
+    return hamiltonian_obs(coeffs, terms)
+
+
 def _serialize_ob(ob, wires_map, use_csingle):
     """Serialize an observable.
     Args:
         ob (Observable): the input observable
         wires_map (dict): a dictionary mapping input wires to the device's backend wires
         use_csingle (bool): whether to use np.complex64 instead of np.complex128
     Returns:
@@ -205,20 +220,24 @@
     """
     if isinstance(ob, Tensor):
         return _serialize_tensor_ob(ob, wires_map, use_csingle)
     elif ob.name == "Hamiltonian":
         return _serialize_hamiltonian(ob, wires_map, use_csingle)
     elif ob.name == "SparseHamiltonian":
         return _serialize_sparsehamiltonian(ob, wires_map, use_csingle)
+    elif isinstance(ob, (PauliX, PauliY, PauliZ, Identity, Hadamard)):
+        return _serialize_named_ob(ob, wires_map, use_csingle)
+    elif ob._pauli_rep is not None:
+        return _serialize_pauli_sentence(ob._pauli_rep, wires_map, use_csingle)
     elif ob.name == "Hermitian":
         raise TypeError(
-            f"Hermitian observables are not currently supported for adjoint differentiation. Please use Pauli-words only."
+            "Hermitian observables are not currently supported for adjoint differentiation. Please use Pauli-words only."
         )
     else:
-        return _serialize_named_ob(ob, wires_map, use_csingle)
+        raise TypeError(f"Unknown observable found: {ob}. Please use Pauli-words only.")
 
 
 def _serialize_observables(tape: QuantumTape, wires_map: dict, use_csingle: bool = False) -> List:
     """Serialize the observables of an input tape.
     Args:
         tape (QuantumTape): the input quantum tape
         wires_map (dict): a dictionary mapping input wires to the device's backend wires
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/_version.py` & `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.29.1"
+__version__ = "0.30.0"
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/pennylane_lightning_kokkos/lightning_kokkos.py` & `PennyLane-Lightning-Kokkos-0.30.0/pennylane_lightning_kokkos/lightning_kokkos.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import List
 from warnings import warn
 from itertools import product
 
 import re
 import numpy as np
 from pennylane import (
+    active_return,
     math,
     QubitDevice,
     BasisState,
     QubitStateVector,
     DeviceError,
     Projector,
     Hamiltonian,
@@ -174,14 +175,17 @@
             "PauliX",
             "PauliY",
             "PauliZ",
             "Hadamard",
             "SparseHamiltonian",
             "Hamiltonian",
             "Identity",
+            "Sum",
+            "Prod",
+            "SProd",
         }
 
         def __init__(
             self,
             wires,
             *,
             sync=True,
@@ -672,17 +676,16 @@
             trainable_params = sorted(tape.trainable_params)
 
             tp_shift = []
             record_tp_rows = []
             all_params = 0
 
             for op_idx, tp in enumerate(trainable_params):
-                op, _ = tape.get_operation(
-                    op_idx
-                )  # get op_idx-th operator among differentiable operators
+                # get op_idx-th operator among differentiable operators
+                op, _, _ = tape.get_operation(op_idx)
 
                 if isinstance(op, Operation) and not isinstance(op, (BasisState, QubitStateVector)):
                     # We now just ignore non-op or state preps
                     tp_shift.append(tp)
                     record_tp_rows.append(all_params)
                 all_params += 1
 
@@ -692,15 +695,15 @@
                 tp_shift = [i - 1 for i in tp_shift]
 
             jac = adj.adjoint_jacobian(self._kokkos_state, obs_serialized, ops_serialized, tp_shift)
             jac = np.array(jac)  # only for parameters differentiable with the adjoint method
             jac = jac.reshape(-1, len(tp_shift))
             jac_r = np.zeros((jac.shape[0], all_params))
             jac_r[:, record_tp_rows] = jac
-            return jac_r
+            return self._adjoint_jacobian_processing(jac_r) if active_return() else jac_r
 
         def vjp(self, measurements, dy, starting_state=None, use_device_state=False):
             """Generate the processing function required to compute the vector-Jacobian products of a tape."""
             if self.shots is not None:
                 warn(
                     "Requested adjoint differentiation to be computed with finite shots."
                     " The derivative is always exact when using the adjoint differentiation method.",
@@ -731,20 +734,31 @@
 
                     if num_params == 0:
                         return np.array([], dtype=self._state.dtype)
 
                     new_tape = tape.copy()
                     new_tape._measurements = [qml.expval(ham)]
 
-                    return self.adjoint_jacobian(
-                        new_tape, starting_state, use_device_state
-                    ).reshape(-1)
+                    return self.adjoint_jacobian(new_tape, starting_state, use_device_state)
 
                 return processing_fn
 
+        def _get_diagonalizing_gates(self, circuit: qml.tape.QuantumTape) -> List[Operation]:
+            skip_diagonalizing = lambda obs: isinstance(obs, qml.Hamiltonian) or (
+                isinstance(obs, qml.ops.Sum) and obs._pauli_rep is not None
+            )
+            meas_filtered = list(
+                filter(
+                    lambda m: m.obs is None or not skip_diagonalizing(m.obs), circuit.measurements
+                )
+            )
+            return super()._get_diagonalizing_gates(
+                qml.tape.QuantumScript(measurements=meas_filtered)
+            )
+
 else:  # CPP_BINARY_AVAILABLE:
 
     class LightningKokkos(LightningQubit):
         name = "PennyLane plugin for Kokkos-backed Lightning device"
         short_name = "lightning.kokkos"
         pennylane_requires = ">=0.22"
         version = __version__
```

### Comparing `PennyLane-Lightning-Kokkos-0.29.1/setup.py` & `PennyLane-Lightning-Kokkos-0.30.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,17 +104,21 @@
                 if os.getenv("ARCHS") == "arm64":
                     configure_args += [
                         "-DCMAKE_CXX_COMPILER_TARGET=arm64-apple-macos11",
                         "-DCMAKE_SYSTEM_NAME=Darwin",
                         "-DCMAKE_SYSTEM_PROCESSOR=ARM64",
                     ]
                 else:  # X64 arch
-                    llvmpath = (
-                        subprocess.check_output(["brew", "--prefix", "llvm"]).decode().strip()
-                    )
+                    if shutil.which("brew"):
+                        llvmpath = (
+                            subprocess.check_output(["brew", "--prefix", "llvm"]).decode().strip()
+                        )
+                    else:
+                        llvmpath = shutil.which("clang++")
+                        llvmpath = Path(llvmpath).parent.parent
                     configure_args += [
                         f"-DCMAKE_CXX_COMPILER={llvmpath}/bin/clang++",
                         f"-DCMAKE_LINKER={llvmpath}/bin/lld",
                     ]  # Use clang instead of appleclang
                 # Disable OpenMP in M1 Macs
                 configure_args += ["-DKokkos_ENABLE_OPENMP=OFF"]
             elif platform.system() == "Windows":
```

