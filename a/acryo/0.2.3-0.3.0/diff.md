# Comparing `tmp/acryo-0.2.3.tar.gz` & `tmp/acryo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryo-0.2.3.tar", last modified: Tue Apr 18 14:37:25 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `acryo-0.2.3.tar` & `acryo-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.379999 acryo-0.2.3/
--rw-rw-rw-   0        0        0     1547 2022-04-12 12:12:07.000000 acryo-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2301 2023-04-18 14:37:25.378989 acryo-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2011 2023-03-15 04:48:31.000000 acryo-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.230779 acryo-0.2.3/acryo/
--rw-rw-rw-   0        0        0      380 2023-04-18 14:33:31.000000 acryo-0.2.3/acryo/__init__.py
--rw-rw-rw-   0        0        0    11845 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/_correlation.py
--rw-rw-rw-   0        0        0      661 2023-02-19 09:29:23.000000 acryo-0.2.3/acryo/_fft.py
--rw-rw-rw-   0        0        0     2929 2023-02-20 00:46:56.000000 acryo-0.2.3/acryo/_reader.py
--rw-rw-rw-   0        0        0     2784 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/_rotation.py
--rw-rw-rw-   0        0        0      244 2023-02-23 14:34:20.000000 acryo-0.2.3/acryo/_types.py
--rw-rw-rw-   0        0        0    12048 2023-04-09 13:27:24.000000 acryo-0.2.3/acryo/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.280202 acryo-0.2.3/acryo/alignment/
--rw-rw-rw-   0        0        0      384 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/alignment/__init__.py
--rw-rw-rw-   0        0        0    30369 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_base.py
--rw-rw-rw-   0        0        0     1469 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_bound.py
--rw-rw-rw-   0        0        0     2701 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.290294 acryo-0.2.3/acryo/classification/
--rw-rw-rw-   0        0        0       62 2022-04-12 15:56:50.000000 acryo-0.2.3/acryo/classification/__init__.py
--rw-rw-rw-   0        0        0    18578 2023-02-08 03:31:15.000000 acryo-0.2.3/acryo/classification/_dask_pca.py
--rw-rw-rw-   0        0        0     5185 2023-02-21 02:27:31.000000 acryo-0.2.3/acryo/classification/pca.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.314296 acryo-0.2.3/acryo/loader/
--rw-rw-rw-   0        0        0      187 2023-02-19 15:38:13.000000 acryo-0.2.3/acryo/loader/__init__.py
--rw-rw-rw-   0        0        0    36831 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/loader/_base.py
--rw-rw-rw-   0        0        0     7099 2023-02-26 13:13:09.000000 acryo-0.2.3/acryo/loader/_batch.py
--rw-rw-rw-   0        0        0     1696 2023-02-21 08:34:02.000000 acryo-0.2.3/acryo/loader/_cache.py
--rw-rw-rw-   0        0        0    17909 2023-02-27 14:09:35.000000 acryo-0.2.3/acryo/loader/_group.py
--rw-rw-rw-   0        0        0     9034 2023-02-25 12:12:36.000000 acryo-0.2.3/acryo/loader/_loader.py
--rw-rw-rw-   0        0        0     2222 2023-02-24 06:22:10.000000 acryo-0.2.3/acryo/loader/_misc.py
--rw-rw-rw-   0        0        0     9986 2023-03-15 04:51:58.000000 acryo-0.2.3/acryo/loader/_mock.py
--rw-rw-rw-   0        0        0    34451 2023-04-09 13:27:24.000000 acryo-0.2.3/acryo/molecules.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.324302 acryo-0.2.3/acryo/pick/
--rw-rw-rw-   0        0        0      129 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/__init__.py
--rw-rw-rw-   0        0        0     4680 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/_base.py
--rw-rw-rw-   0        0        0     4799 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.342293 acryo-0.2.3/acryo/pipe/
--rw-rw-rw-   0        0        0      647 2023-02-23 14:49:44.000000 acryo-0.2.3/acryo/pipe/__init__.py
--rw-rw-rw-   0        0        0    12167 2023-02-23 11:14:01.000000 acryo-0.2.3/acryo/pipe/_classes.py
--rw-rw-rw-   0        0        0     3843 2023-02-25 03:55:45.000000 acryo-0.2.3/acryo/pipe/_curry.py
--rw-rw-rw-   0        0        0     5436 2023-02-23 15:13:40.000000 acryo-0.2.3/acryo/pipe/_imread.py
--rw-rw-rw-   0        0        0     3459 2023-02-23 11:14:00.000000 acryo-0.2.3/acryo/pipe/_masking.py
--rw-rw-rw-   0        0        0     1215 2023-02-25 03:55:55.000000 acryo-0.2.3/acryo/pipe/_transform.py
--rw-rw-rw-   0        0        0    13577 2023-02-18 15:53:02.000000 acryo-0.2.3/acryo/simulator.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.351293 acryo-0.2.3/acryo/testing/
--rw-rw-rw-   0        0        0      130 2022-04-15 01:53:16.000000 acryo-0.2.3/acryo/testing/__init__.py
--rw-rw-rw-   0        0        0     1145 2022-05-02 14:08:55.000000 acryo-0.2.3/acryo/testing/_templates.py
--rw-rw-rw-   0        0        0     4432 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/testing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.270211 acryo-0.2.3/acryo.egg-info/
--rw-rw-rw-   0        0        0     2301 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1168 2023-04-18 14:37:25.000000 acryo-0.2.3/acryo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 14:37:25.380998 acryo-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      820 2023-04-18 09:04:57.000000 acryo-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.375489 acryo-0.2.3/tests/
--rw-rw-rw-   0        0        0     5448 2023-04-18 09:04:57.000000 acryo-0.2.3/tests/test_alignment.py
--rw-rw-rw-   0        0        0     2602 2023-02-21 08:34:02.000000 acryo-0.2.3/tests/test_batch.py
--rw-rw-rw-   0        0        0     1360 2023-02-21 08:34:02.000000 acryo-0.2.3/tests/test_cache.py
--rw-rw-rw-   0        0        0     1736 2023-02-23 14:27:37.000000 acryo-0.2.3/tests/test_group.py
--rw-rw-rw-   0        0        0     6716 2023-02-24 04:50:51.000000 acryo-0.2.3/tests/test_molecules.py
--rw-rw-rw-   0        0        0      691 2023-02-21 11:08:36.000000 acryo-0.2.3/tests/test_pipe.py
--rw-rw-rw-   0        0        0     1545 2023-01-29 13:16:40.000000 acryo-0.2.3/tests/test_simulator.py
--rw-rw-rw-   0        0        0      542 2023-02-14 03:49:57.000000 acryo-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/__init__.py
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_correlation.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_dask.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_reader.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_rotation.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_typed_scipy.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_types.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/_utils.py
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/simulator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/alignment/__init__.py
+-rw-r--r--   0        0        0    29980 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/alignment/_base.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/alignment/_bound.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/alignment/_concrete.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/classification/__init__.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/classification/_dask_pca.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/classification/pca.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/__init__.py
+-rw-r--r--   0        0        0    37225 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_base.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_batch.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_cache.py
+-rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_group.py
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_loader.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_misc.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/loader/_mock.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/molecules/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/molecules/_cut.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/molecules/_group.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/molecules/_rotation.py
+-rw-r--r--   0        0        0    33815 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/molecules/core.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pick/__init__.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pick/_base.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pick/_concrete.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/__init__.py
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/_classes.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/_curry.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/_imread.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/_masking.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/pipe/_transform.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/testing/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/testing/_templates.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.3.0/acryo/testing/core.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 acryo-0.3.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 acryo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 acryo-0.3.0/PKG-INFO
```

### Comparing `acryo-0.2.3/LICENSE` & `acryo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/PKG-INFO` & `acryo-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,18 @@
-Metadata-Version: 2.1
-Name: acryo
-Version: 0.2.3
-Summary: An extensible cryo-EM/ET toolkit for Python.
-Author: Hanjin Liu
-Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
-License: BSD 3-Clause
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python package index download statistics](https://img.shields.io/pypi/dm/acryo.svg)](https://pypistats.org/packages/acryo)
 [![PyPI version](https://badge.fury.io/py/acryo.svg)](https://badge.fury.io/py/acryo)
 
 # acryo
 
 `acryo` is an extensible cryo-EM/ET toolkit for Python.
 
 The purpose of this library is to make data analysis of cryo-EM/ET more safe, efficient and reproducible.
 Scientists can avoid the error-prone CLI-based data handling, such as writing out the results to the files every time and manage all the result just by the file names.
 
-[祷 Documentation](https://hanjinliu.github.io/acryo/)
+[📘 Documentation](https://hanjinliu.github.io/acryo/)
 
 ### Install
 
 ###### Use pip
 
 ```bash
 pip install acryo -U
```

### Comparing `acryo-0.2.3/acryo/_correlation.py` & `acryo-0.3.0/acryo/_correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 from functools import lru_cache
 from typing import Sequence, TypeVar
 import numpy as np
 from numpy.typing import NDArray
 
 from scipy.signal import fftconvolve
-from scipy import ndimage as ndi
 
-from acryo._fft import ifftn
+from acryo._typed_scipy import ifftn, map_coordinates
 from acryo._types import pixel
 
 # cross correlation
 # Modified from skimage/registration/_phase_cross_correlation.py
 
 
 def pcc_landscape(
@@ -83,40 +82,40 @@
         shifts = shifts + maxima / upsample_factor
         pcc = np.sqrt(power[tuple(int(np.round(m)) for m in maxima)])
     else:
         pcc = np.sqrt(power[maxima])
     return shifts, pcc
 
 
+_DType = TypeVar("_DType", bound=np.number)
+
+
 def _upsampled_dft(
-    data: NDArray[np.number],
+    data: NDArray[_DType],
     upsampled_region_size: NDArray[np.integer],
     upsample_factor: int,
     axis_offsets: NDArray[np.float32],
-) -> NDArray[np.number]:
+) -> NDArray[_DType]:
     # if people pass in an integer, expand it to a list of equal-sized sections
     upsampled_region_sizes = [upsampled_region_size] * data.ndim
 
     dim_properties = list(zip(data.shape, upsampled_region_sizes, axis_offsets))
 
-    for (n_items, ups_size, ax_offset) in dim_properties[::-1]:
+    for n_items, ups_size, ax_offset in dim_properties[::-1]:
         kernel = (np.arange(ups_size) - ax_offset)[  # type: ignore
             :, np.newaxis
         ] * np.fft.fftfreq(  # type: ignore
             n_items, upsample_factor
         )
         kernel = np.exp(-2j * np.pi * kernel)
 
         data = np.tensordot(kernel, data, axes=(1, -1))  # type: ignore
     return data
 
 
-_DType = TypeVar("_DType", bound=np.number)
-
-
 def _abs2(a: NDArray[np.complex64]) -> NDArray[np.float32]:
     return a.real**2 + a.imag**2
 
 
 def crop_by_max_shifts(power: NDArray[_DType], left, right) -> NDArray[_DType]:
     shifted_power = np.fft.fftshift(power)
     centers = tuple(s // 2 for s in power.shape)
@@ -238,15 +237,15 @@
         coords = _create_mesh(
             upsample_factor,
             maxima,
             max_shifts,
             midpoints.astype(np.float32),
             pad_width_eff,
         )
-        local_response: np.ndarray = ndi.map_coordinates(
+        local_response: np.ndarray = map_coordinates(
             response, coords, order=3, mode="constant", cval=-1.0, prefilter=True
         )
         local_maxima = np.unravel_index(np.argmax(local_response), local_response.shape)
         zncc = local_response[local_maxima]
         shifts = (
             np.array(maxima) - midpoints + np.array(local_maxima) / upsample_factor - 1
         )
```

### Comparing `acryo-0.2.3/acryo/_reader.py` & `acryo-0.3.0/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/_rotation.py` & `acryo-0.3.0/acryo/_rotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 import itertools
 from typing import Callable, Sequence
 import numpy as np
 from scipy.spatial.transform import Rotation
-from scipy import ndimage as ndi
 
 from acryo._types import Ranges, RangeLike
 from acryo.molecules import from_euler_xyz_coords
+from acryo._typed_scipy import affine_transform
 
 
 def _normalize_a_range(rng: RangeLike) -> RangeLike:
     if len(rng) != 2:
         raise TypeError(f"Range must be defined by (float, float), got {rng!r}")
     max_rot, drot = rng
     return float(max_rot), float(drot)
@@ -35,31 +35,31 @@
 
     Returns
     -------
     np.ndarray
         Corresponding quaternions in shape (N, 4).
     """
     if isinstance(rotations, Rotation):
-        quat = rotations.as_quat()
+        quats = rotations.as_quat()
     elif rotations is not None:
         _rotations = _normalize_ranges(rotations)
         angles = []
         for max_rot, step in _rotations:
             if step == 0:
                 angles.append(np.zeros(1))
             else:
                 n = int(max_rot / step)
                 angles.append(np.linspace(-n * step, n * step, 2 * n + 1))
 
-        quat: list[np.ndarray] = []
+        _quat: list[np.ndarray] = []
         for angs in itertools.product(*angles):
-            quat.append(
+            _quat.append(
                 from_euler_xyz_coords(np.array(angs), "zyx", degrees=True).as_quat()
             )
-        quats = np.stack(quat, axis=0)
+        quats = np.stack(_quat, axis=0)
     else:
         quats = np.array([[0.0, 0.0, 0.0, 1.0]])
 
     return quats
 
 
 def rotate(
@@ -77,15 +77,15 @@
         np.array(image.shape[-image.ndim :]) / 2 - 0.5, [rotator]
     )[0]
     if callable(cval):
         _cval = cval(image)
     else:
         _cval = cval
 
-    return ndi.affine_transform(
+    return affine_transform(
         image,
         matrix=matrix,
         order=order,
         mode=mode,
         cval=_cval,
         prefilter=order > 1,
     )
```

### Comparing `acryo-0.2.3/acryo/_utils.py` & `acryo-0.3.0/acryo/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 from numpy.typing import NDArray
 from dask import array as da
 from dask.delayed import delayed
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
-from acryo._fft import fftn, rfftn, irfftn
+from acryo._typed_scipy import fftn, rfftn, irfftn
 
 if TYPE_CHECKING:
     from acryo._types import degree
 
 
 def make_slice_and_pad(
     z0: int, z1: int, size: int
@@ -42,15 +42,15 @@
 
     out_of_bound = z0_pad != 0 or z1_pad != 0
     return slice(z0, z1), (z0_pad, z1_pad), out_of_bound
 
 
 def compose_matrices(
     center: Sequence[float] | np.ndarray,
-    rotators: list[Rotation],
+    rotators: Rotation | list[Rotation],
     output_center: Sequence[float] | np.ndarray | None = None,
 ) -> list[NDArray[np.float32]]:
     """Compose Affine matrices from an array shape and a Rotation object."""
 
     dz, dy, dx = center
     if output_center is None:
         output_center = center
@@ -152,15 +152,15 @@
 
 def prepare_affine(
     img: da.Array,
     center: Sequence[float],
     output_shape: Sequence[int],
     rot: Rotation,
     order: int = 1,
-):
+) -> tuple[da.Array, NDArray[np.float32]]:
     output_center = np.array(output_shape) / 2 - 0.5
     slices: list[slice] = []
     pads: list[tuple[int, ...]] = []
     new_center: list[float] = []
     need_pad = False
     for c, s, s0 in zip(center, output_shape, img.shape):
         x0 = int(c - s / 2 - order)
@@ -182,15 +182,15 @@
 
 def prepare_affine_cornersafe(
     img: da.Array,
     center: Sequence[float],
     output_shape: Sequence[int],
     rot: Rotation,
     order: int = 1,
-):
+) -> tuple[da.Array, NDArray[np.float32]]:
     max_len = np.sqrt(np.sum(np.asarray(output_shape, dtype=np.float32) ** 2))
     output_center = np.array(output_shape) / 2 - 0.5
     half_len = max_len / 2
     slices: list[slice] = []
     pads: list[tuple[int, ...]] = []
     new_center: list[float] = []
     need_pad = False
@@ -208,31 +208,14 @@
         input = da.pad(img0, pads, mode="mean")
     else:
         input = img0
     mtx = compose_matrices(new_center, [rot], output_center=output_center)[0]
     return input, mtx
 
 
-@delayed
-def rotated_crop(subimg: np.ndarray, mtx: np.ndarray, shape, order, mode, cval):
-    if callable(cval):
-        cval = cval(subimg)
-
-    out = ndi.affine_transform(
-        subimg,
-        matrix=mtx,
-        output_shape=shape,
-        order=order,
-        prefilter=order > 1,
-        mode=mode,
-        cval=cval,
-    )
-    return out
-
-
 _delayed_affine_transform = delayed(ndi.affine_transform)
 
 
 def delayed_affine(
     input: np.ndarray,
     matrix: np.ndarray,
     order: int = 3,
@@ -403,8 +386,8 @@
                     DeprecationWarning,
                 )
                 kwargs[new] = kwargs.pop(old)
             return f(*args, **kwargs)
 
         return _func
 
-    return _inner
+    return _inner  # type: ignore
```

### Comparing `acryo-0.2.3/acryo/alignment/_base.py` & `acryo-0.3.0/acryo/alignment/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,36 @@
 from functools import lru_cache
 from typing import (
     Callable,
     Iterable,
     NamedTuple,
     Sequence,
     TYPE_CHECKING,
-    TypeVar,
     Union,
 )
 from typing_extensions import Self
-import inspect
 import warnings
 
 import numpy as np
 from numpy.typing import NDArray
-from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
-from dask import array as da, delayed
 
 from acryo._rotation import normalize_rotations
 from acryo._types import Ranges, subpixel, degree
 from acryo._utils import (
     compose_matrices,
     missing_wedge_mask,
     lowpass_filter_ft,
-    delayed_affine,
 )
-from acryo._fft import ifftn
+from acryo._typed_scipy import ifftn, spline_filter, affine_transform, map_coordinates
+from acryo._dask import DaskTaskPool
 from ._bound import ParametrizedModel
 
 if TYPE_CHECKING:
-    from dask.delayed import Delayed
+    pass
 
 
 TemplateType = Union[NDArray[np.float32], Sequence[NDArray[np.float32]]]
 MaskType = Union[
     NDArray[np.float32],
     Callable[[NDArray[np.float32]], NDArray[np.float32]],
     None,
@@ -313,15 +309,15 @@
         -------
         np.ndarray, AlignmentResult
             Transformed input image and the alignment result.
         """
         result = self.align(img, max_shifts=max_shifts, quaternion=None, pos=None)
         mtx = result.affine_matrix(img.shape)
         _cval = _normalize_cval(cval, img)
-        img_trans: NDArray[np.float32] = ndi.affine_transform(img, mtx, cval=_cval)  # type: ignore
+        img_trans = affine_transform(img, mtx, cval=_cval)
         return img_trans, result
 
     def landscape(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32] | None = None,
@@ -362,26 +358,26 @@
             img,
             self._template_input,
             self._mask_input,
             max_shifts,
             _quat,
             _pos,
         )
-        
+
         if upsample > 1:
             if not self._is_multiple():
                 coords = _create_mesh_for_landscape(lds.shape, max_shifts, upsample)
-                lds_upsampled = ndi.map_coordinates(
-                    lds, coords, order=3, mode="constant", cval=0., prefilter=True
+                lds_upsampled = map_coordinates(
+                    lds, coords, order=3, mode="constant", cval=0.0, prefilter=True
                 )
             else:
                 coords = _create_mesh_for_landscape(lds.shape[1:], max_shifts, upsample)
                 all_lds = [
-                    ndi.map_coordinates(
-                        l, coords, order=3, mode="constant", cval=0., prefilter=True
+                    map_coordinates(
+                        l, coords, order=3, mode="constant", cval=0.0, prefilter=True
                     )
                     for l in lds
                 ]
                 lds_upsampled = np.stack(all_lds, axis=0)
             return lds_upsampled
         return lds
 
@@ -480,14 +476,15 @@
         return self._is_multiple()
 
     @property
     def niter(self) -> int:
         """Number of templates."""
         return self._n_templates
 
+
 # deprecated
 def optimize(self: BaseAlignmentModel, *args, **kwargs):
     warnings.warn(
         "`optimize` is deprecated. It is now a private method.", DeprecationWarning
     )
     return self._optimize(*args, **kwargs)
 
@@ -573,70 +570,58 @@
             Constant value for padding.
 
         Returns
         -------
         np.ndarray, AlignmentResult
             Transformed input image and the alignment result.
         """
-        delayed_optimize = delayed(self._optimize)
-        tasks: list[Delayed] = []
+        pool = DaskTaskPool.from_func(self._optimize)
+        pos = np.zeros(3, dtype=np.float32)
         for quat, tmp, mask in zip(
             self.quaternions, self._template_input, self._mask_input
         ):
-            task = delayed_optimize(
+            pool.add_task(
                 self.pre_transform(img * mask),
                 tmp,
                 max_shifts,
                 quat,
-                pos=None,
+                pos=pos,
             )
-            tasks.append(task)
-        results: list[tuple] = da.compute(tasks)[0]
+        results = pool.compute()
         scores = [x[2] for x in results]
         iopt = np.argmax(scores)
         opt_result = results[iopt]
         result = AlignmentResult(
             label=0,
             shift=opt_result[0],
             quat=self.quaternions[iopt],
             score=opt_result[2],
         )
 
         mtx = result.affine_matrix(img.shape)
         _img_cval = _normalize_cval(cval, img)
-        img_trans: NDArray[np.float32] = ndi.affine_transform(img, mtx, cval=_img_cval)  # type: ignore
+        img_trans = affine_transform(img, mtx, cval=_img_cval)
         return img_trans, result
 
     def _transform_template(
         self,
         temp: NDArray[np.float32],
         matrix: NDArray[np.float32],
         cval: float | None = None,
         order: int = 3,
         prefilter: bool = True,
     ) -> NDArray[np.complex64]:
         _cval = _normalize_cval(cval, temp)
 
         return self.pre_transform(
-            ndi.affine_transform(
+            affine_transform(
                 temp, matrix=matrix, cval=_cval, order=order, prefilter=prefilter
-            )  # type: ignore
+            )
         )
 
-    @delayed
-    def _transform_template_delayed(
-        self,
-        temp: NDArray[np.float32],
-        matrix: NDArray[np.float32],
-        cval: float | None = None,
-        order: int = 3,
-        prefilter: bool = True,
-    ):
-        return self._transform_template(temp, matrix, cval, order, prefilter)
-
     def _get_template_and_mask_input(
         self,
     ) -> tuple[NDArray[np.complex64], NDArray[np.float32]]:
         """
         Returns proper template image for alignment.
 
         Template dimensionality will be dispatched according to the input
@@ -658,112 +643,106 @@
         if self._n_rotations > 1:
             rotators = [Rotation.from_quat(r).inv() for r in self.quaternions]
             matrices = compose_matrices(
                 np.array(self._template.shape[-3:]) / 2 - 0.5, rotators
             )
             cval = float(np.percentile(self._template, 1))
             if self._n_templates > 1:
-                all_templates: list[da.Array] = []
-                all_masks: list[da.Array] = []
+                # all_templates: list[da.Array] = []
+                # all_masks: list[da.Array] = []
                 inputs_templates: list[NDArray[np.float32]] = [
-                    ndi.spline_filter(
+                    spline_filter(
                         tmp * self._mask,
                         order=3,
                         mode="constant",
-                        output=np.float32,  # type: ignore
+                        output=np.float32,
                     )
                     for tmp in self._template
                 ]
+                pool_template = DaskTaskPool.from_func(self._transform_template)
+                pool_mask = DaskTaskPool.from_func(affine_transform)
+                ntmp = len(inputs_templates)
                 for mat in matrices:
                     for tmp in inputs_templates:
-                        all_templates.append(
-                            da.from_delayed(
-                                self._transform_template_delayed(
-                                    tmp, mat, order=3, cval=cval, prefilter=False
-                                ),
-                                shape=tmp.shape,
-                                dtype=tmp.dtype,
-                            )
+                        pool_template.add_task(
+                            tmp, mat, order=3, cval=cval, prefilter=False
                         )
-                    all_masks.extend(
-                        [
-                            delayed_affine(
-                                self._mask,
-                                mat,
-                                order=3,
-                                mode="nearest",
-                                prefilter=False,
-                            )
-                        ]
-                        * len(inputs_templates)
+                        # all_templates.append(
+                        #     da.from_delayed(
+                        #         self._transform_template_delayed(
+                        #             tmp, mat, order=3, cval=cval, prefilter=False
+                        #         ),
+                        #         shape=tmp.shape,
+                        #         dtype=tmp.dtype,
+                        #     )
+                        # )
+                    pool_mask.add_tasks(
+                        ntmp, self._mask, mat, order=3, mode="nearest", prefilter=False
                     )
 
-                template_input, mask_input = da.compute(
-                    da.stack(all_templates, axis=0), da.stack(all_masks, axis=0)
-                )
+                    # all_masks.extend(
+                    #     [
+                    #         delayed_affine(
+                    #             self._mask,
+                    #             mat,
+                    #             order=3,
+                    #             mode="nearest",
+                    #             prefilter=False,
+                    #         )
+                    #     ]
+                    #     * len(inputs_templates)
+                    # )
+                template_input = np.stack(pool_template.compute(), axis=0)
+                mask_input = np.stack(pool_mask.compute(), axis=0)
+                # template_input, mask_input = da.compute(
+                #     da.stack(all_templates, axis=0), da.stack(all_masks, axis=0)
+                # )
 
             else:
-                template_masked: NDArray[np.float32] = ndi.spline_filter(
+                template_masked = spline_filter(
                     self._template * self._mask,
                     order=3,
-                    output=np.float32,  # type: ignore
+                    output=np.float32,
                     mode="constant",
                 )
-                all_templates = [
-                    da.from_delayed(
-                        self._transform_template_delayed(
-                            template_masked, mat, order=3, cval=cval, prefilter=False
-                        ),
-                        shape=template_masked.shape,
-                        dtype=template_masked.dtype,
+                pool_template = DaskTaskPool.from_func(self._transform_template)
+                pool_mask = DaskTaskPool.from_func(affine_transform)
+                for mat in matrices:
+                    pool_template.add_task(
+                        template_masked, mat, order=3, cval=cval, prefilter=False
                     )
-                    for mat in matrices
-                ]
-                all_masks = [
-                    delayed_affine(
-                        self._mask, matrix=mat, order=3, mode="nearest", prefilter=False
+                    pool_mask.add_task(
+                        self._mask, mat, order=3, mode="nearest", prefilter=False
                     )
-                    for mat in matrices
-                ]
-                template_input, mask_input = da.compute(
-                    da.stack(all_templates, axis=0), da.stack(all_masks, axis=0)
-                )
+                template_input = np.stack(pool_template.compute(), axis=0)
+                mask_input = np.stack(pool_mask.compute(), axis=0)
         else:
-            delayed_transform = delayed(self.pre_transform)
+            pool = DaskTaskPool.from_func(self.pre_transform)
             if self._n_templates > 1:
-                template_input = da.stack(
-                    [
-                        da.from_delayed(
-                            delayed_transform(tmp * self._mask),
-                            shape=tmp.shape,
-                            dtype=np.complex64,
-                        )
-                        for tmp in self._template
-                    ],
-                    axis=0,
-                ).compute()
+                for tmp in self._template:
+                    pool.add_task(tmp * self._mask)
+                template_input = np.stack(pool.compute(), axis=0)
                 mask_input = np.stack([self._mask] * len(self._template), axis=0)
 
             else:
                 # NOTE: dask.compute is always called once inside this method.
-                template_input = delayed_transform(
-                    self._template * self._mask
-                ).compute()
+                template_input = pool.add_task(self._template * self._mask).compute()[0]
                 mask_input = self._mask
 
         return template_input, mask_input
 
     def _is_multiple(self) -> bool:
         return self._n_templates * self._n_rotations > 1
 
     @property
     def niter(self) -> int:
         """Number of iteration per sub-volume."""
         return self._n_templates * self._n_rotations
 
+
 class TomographyInput(RotationImplemented):
     """
     An alignment model that implements missing-wedge masking and low-pass filter.
 
     This alignment model is useful for subtomogram averaging of real experimental
     data with limited tilt ranges. Template image will be masked with synthetic
     missing-wedge mask in the frequency domain.
@@ -875,19 +854,21 @@
     else:
         _cval = cval
     return _cval
 
 
 @lru_cache(maxsize=2)
 def _create_mesh_for_landscape(
-    shape: tuple[int, int, int], 
-    max_shifts: tuple[float, float, float], 
+    shape: tuple[int, int, int],
+    max_shifts: tuple[float, float, float],
     upsample: int,
 ) -> NDArray[np.float32]:
     upsampled_max_shifts = (np.asarray(max_shifts) * upsample).astype(np.int32)
     center = np.array(shape) / 2 - 0.5
     mesh = np.meshgrid(
-        *[np.arange(-width, width + 1) / upsample + c
-        for c, width in zip(center, upsampled_max_shifts)], 
+        *[
+            np.arange(-width, width + 1) / upsample + c
+            for c, width in zip(center, upsampled_max_shifts)
+        ],
         indexing="ij",
     )
     return np.stack(mesh, axis=0)
```

### Comparing `acryo-0.2.3/acryo/alignment/_bound.py` & `acryo-0.3.0/acryo/alignment/_bound.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/alignment/_concrete.py` & `acryo-0.3.0/acryo/alignment/_concrete.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from ._base import TomographyInput
 from acryo._correlation import (
     subpixel_pcc,
     subpixel_zncc,
     zncc_landscape_with_crop,
     pcc_landscape,
 )
-from acryo._fft import ifftn
+from acryo._typed_scipy import ifftn
+from acryo._types import pixel
 
 
 class PCCAlignment(TomographyInput):
     """Alignment model using phase cross correlation."""
 
     def _optimize(
         self,
         subvolume: NDArray[np.complex64],
         template: NDArray[np.complex64],
-        max_shifts: tuple[float, float, float],
+        max_shifts: tuple[pixel, pixel, pixel],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
     ) -> tuple[NDArray[np.float32], NDArray[np.float32], float]:
         """Optimize."""
         shift, pcc = subpixel_pcc(
             subvolume,
             self.mask_missing_wedge(template, quaternion),
@@ -52,15 +53,15 @@
 class ZNCCAlignment(TomographyInput):
     """Alignment model using zero-mean normalized cross correlation."""
 
     def _optimize(
         self,
         subvolume: NDArray[np.complex64],
         template: NDArray[np.complex64],
-        max_shifts: tuple[float, float, float],
+        max_shifts: tuple[pixel, pixel, pixel],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
     ) -> tuple[NDArray[np.float32], NDArray[np.float32], float]:
         """Optimize."""
         shift, zncc = subpixel_zncc(
             np.real(ifftn(subvolume)),
             np.real(ifftn(self.mask_missing_wedge(template, quaternion))),
```

### Comparing `acryo-0.2.3/acryo/classification/_dask_pca.py` & `acryo-0.3.0/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/classification/pca.py` & `acryo-0.3.0/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/loader/_base.py` & `acryo-0.3.0/acryo/loader/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     TYPE_CHECKING,
     Iterable,
     Iterator,
     NamedTuple,
     Any,
     Sequence,
     SupportsIndex,
+    TypeVar,
     Union,
     overload,
 )
 from typing_extensions import TypeGuard
 import numpy as np
 from numpy.typing import NDArray
 from dask import array as da
@@ -28,32 +29,34 @@
     ZNCCAlignment,
     RotationImplemented,
     AlignmentFactory,
     AlignmentResult,
 )
 from acryo import _utils
 from acryo._types import nm, pixel
+from acryo._dask import DaskArrayList, DaskTaskList, DaskTaskIterator
 from acryo.molecules import Molecules
 from acryo.loader import _misc
 from acryo.loader._group import LoaderGroup
 from acryo.loader._cache import SubtomogramCache
 from acryo.pipe._classes import ImageProvider, ImageConverter
 
 if TYPE_CHECKING:
     from typing_extensions import Self
     from dask.delayed import Delayed
     from acryo.classification import PcaClassifier
     from acryo.alignment._base import MaskType
 
-    _ShapeType = Union[pixel, tuple[pixel, ...], None]
-
+_ShapeType = Union[pixel, tuple[pixel, ...], None]
 TemplateInputType = Union[NDArray[np.float32], ImageProvider]
 MaskInputType = Union[NDArray[np.float32], ImageProvider, ImageConverter, None]
 AggFunction = Callable[[NDArray[np.float32]], Any]
 
+_R = TypeVar("_R")
+
 
 class Unset:
     def __bool__(self) -> bool:
         return False
 
     def __repr__(self) -> str:
         return "Unset"
@@ -106,17 +109,15 @@
 
     @property
     def corner_safe(self) -> bool:
         """Whether rotation is corner-safe."""
         return self._corner_safe
 
     @abstractmethod
-    def construct_loading_tasks(
-        self, output_shape: _ShapeType = None
-    ) -> list[da.Array]:
+    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
         ...
 
     def _get_cached_array(self, shape: tuple[int, int, int] | None) -> da.Array | None:
         return CACHE.get_cache(id(self), shape)
 
     def construct_dask(
         self,
@@ -159,20 +160,20 @@
 
     def count(self) -> int:
         """Return the number of subtomograms."""
         return len(self.molecules)
 
     def iter_mapping_tasks(
         self,
-        func: Callable,
+        func: Callable[..., _R],
         *const_args,
         output_shape: _ShapeType = None,
         var_kwarg: dict[str, Iterable[Any]] | None = None,
         **const_kwargs,
-    ) -> Iterator[Delayed]:
+    ) -> DaskTaskIterator[_R]:
         """
         Iterate over delayed mapping tasks using subtomograms.
 
         Parameters
         ----------
         func : Callable
             Mapping function. The first argument of the function is the subtomogram.
@@ -193,24 +194,24 @@
         if var_kwarg is None:
             it = (delayed_f(ar, *const_args, **const_kwargs) for ar in dask_array)
         else:
             it = (
                 delayed_f(ar, *const_args, **const_kwargs, **kw)
                 for ar, kw in zip(dask_array, _misc.dict_iterrows(var_kwarg))
             )
-        return it
+        return DaskTaskIterator(it)
 
     def construct_mapping_tasks(
         self,
-        func: Callable,
+        func: Callable[..., _R],
         *const_args,
         output_shape: _ShapeType = None,
         var_kwarg: dict[str, Iterable[Any]] | None = None,
         **const_kwargs,
-    ) -> list[Delayed]:
+    ) -> DaskTaskList[_R]:
         """
         Construct delayed mapping tasks using subtomograms.
 
         Parameters
         ----------
         func : Callable
             Mapping function. The first argument of the function is the subtomogram.
@@ -218,26 +219,24 @@
             Shape of subtomograms.
         var_kwarg : dict, optional
             Variable keyword arguments. The length of each argument must be the same
             as the number of subtomograms.
 
         Returns
         -------
-        list of da.delayed.Delayed object
-            List of delayed tasks that are ready for ``da.compute``.
+        DaskTaskList
+            List of delayed tasks that are ready for computation.
         """
-        return list(
-            self.iter_mapping_tasks(
-                func,
-                *const_args,
-                output_shape=output_shape,
-                var_kwarg=var_kwarg,
-                **const_kwargs,
-            )
-        )
+        return self.iter_mapping_tasks(
+            func,
+            *const_args,
+            output_shape=output_shape,
+            var_kwarg=var_kwarg,
+            **const_kwargs,
+        ).tolist()
 
     def _create_cache(self, output_shape: _ShapeType = None) -> da.Array:
         """
         Create cached stack of subtomograms.
 
         Parameters
         ----------
@@ -424,16 +423,15 @@
             Additional keyword arguments passed to the input alignment model.
 
         Returns
         -------
         subtomogram loader object
             A loader instance of the same type with updated molecules.
         """
-        if np.isscalar(max_shifts):
-            max_shifts = (max_shifts,) * 3
+        max_shifts = _normalize_max_shifts(max_shifts)
         _max_shifts_px = np.asarray(max_shifts) / self.scale
 
         model = alignment_model(
             template=self.normalize_template(template),
             mask=self.normalize_mask(mask),
             **align_kwargs,
         )
@@ -442,15 +440,15 @@
             max_shifts=_max_shifts_px,
             output_shape=model.input_shape,
             var_kwarg=dict(
                 quaternion=self.molecules.quaternion(),
                 pos=self.molecules.pos / self.scale,
             ),
         )
-        all_results = da.compute(tasks)[0]
+        all_results = tasks.compute()
         return self._post_align(all_results, model.input_shape)
 
     def _post_align(
         self,
         results: list[AlignmentResult],
         shape: tuple[int, int, int],
     ) -> Self:
@@ -502,20 +500,19 @@
         Returns
         -------
         subtomogram loader object
             A loader instance of the same type with updated molecules.
         """
         if output_shape is None and isinstance(mask, np.ndarray):
             output_shape = mask.shape
-
         with self.cached(output_shape=output_shape):
             template = self.average(output_shape=output_shape)
             out = self.align(
                 template,
-                mask=self.normalize_mask(mask),
+                mask=mask,
                 max_shifts=max_shifts,
                 alignment_model=alignment_model,
                 **align_kwargs,
             )
         return out
 
     def align_multi_templates(
@@ -568,15 +565,15 @@
             max_shifts=_max_shifts_px,
             output_shape=model.input_shape,
             var_kwarg=dict(
                 quaternion=self.molecules.quaternion(),
                 pos=self.molecules.pos / self.scale,
             ),
         )
-        all_results = da.compute(tasks)[0]
+        all_results = tasks.compute()
         if isinstance(model, RotationImplemented) and model._n_rotations > 1:
             remainder = len(templates)
         else:
             remainder = -1
         return self._post_align_multi_templates(
             all_results, model.input_shape, remainder, label_name
         )
@@ -584,15 +581,14 @@
     def _post_align_multi_templates(
         self,
         results: list[AlignmentResult],
         shape: tuple[int, int, int],
         remainder: int = -1,
         label_name: str = "labels",
     ):
-
         local_shifts, local_rot, scores = _misc.allocate(len(results))
         labels = np.zeros(len(results), dtype=np.uint32)
         for i, result in enumerate(results):
             labels[i], local_shifts[i], local_rot[i], scores[i] = result
 
         rotator = Rotation.from_quat(local_rot)
         mole_aligned = self.molecules.linear_transform(
@@ -623,40 +619,42 @@
     ) -> da.Array:
         """
         Construct a dask array of correlation landscape.
 
         This method internally calls the ``landscape`` method of the input alignment
         model.
         """
-        if np.isscalar(max_shifts):
-            max_shifts = (max_shifts,) * 3
+        max_shifts = _normalize_max_shifts(max_shifts)
         _max_shifts_px = tuple(np.asarray(max_shifts) / self.scale)
 
         model = alignment_model(
             template=self.normalize_template(template),
             mask=self.normalize_mask(mask),
             **align_kwargs,
         )
 
         if model.is_multi_templates:
-            task_shape = (model.niter,) + tuple(2 * np.ceil(_max_shifts_px).astype(np.int32) + 1)
+            task_shape = (model.niter,) + tuple(
+                2 * np.ceil(_max_shifts_px).astype(np.int32) + 1
+            )
         else:
             task_shape = tuple(2 * np.ceil(_max_shifts_px).astype(np.int32) + 1)
-        task_arrays: list[da.Array] = [
-            da.from_delayed(task, shape=task_shape, dtype=np.float32)
-            for task in self.iter_mapping_tasks(
+        task_arrays = (
+            self.iter_mapping_tasks(
                 model.landscape,
                 max_shifts=_max_shifts_px,
                 upsample=upsample,
                 var_kwarg=dict(
                     quaternion=self.molecules.quaternion(),
                     pos=self.molecules.pos / self.scale,
-                )
+                ),
             )
-        ]
+            .tolist()
+            .asarrays(shape=task_shape, dtype=np.float32)
+        )
         return da.stack(task_arrays, axis=0)
 
     def apply(
         self,
         func: AggFunction | Iterable[AggFunction],
         schema: list[str] | None = None,
     ) -> pl.DataFrame:
@@ -671,28 +669,28 @@
             DataFrame schema.
 
         Returns
         -------
         pl.DataFrame
             Result table.
         """
-        all_tasks: list[list[Delayed]] = []
+        all_tasks: list[list[da.Array | Delayed]] = []
         if _is_iterable_of_funcs(func):
             funcs = func
         else:
             funcs: Iterable[AggFunction] = [func]  # type: ignore
         if schema is None:
             schema = [fn.__name__ for fn in funcs]
         if len(set(schema)) != len(schema):
             raise ValueError("Schema names must be unique.")
         if isinstance(self.output_shape, Unset):
             raise ValueError("Output shape is unknown.")
         for fn in funcs:
             tasks = self.construct_mapping_tasks(fn, output_shape=self.output_shape)
-            all_tasks.append(tasks)
+            all_tasks.append(list(tasks))
         all_results = np.array(da.compute(all_tasks)[0])
         return pl.DataFrame(all_results, schema=schema)
 
     def fsc(
         self,
         mask: TemplateInputType | None = None,
         seed: int | None = 0,
@@ -966,15 +964,15 @@
         elif isinstance(template, ImageProvider):
             out = template(self.scale)
             return np.asarray(out, dtype=np.float32)
         raise TypeError(f"Invalid template type: {type(template)}")
 
     def normalize_mask(self, mask: MaskInputType) -> MaskType:
         """Resolve any mask input type to a 3D array."""
-        if isinstance(mask, (np.ndarray, type(None))):
+        if isinstance(mask, np.ndarray) or mask is None:
             return mask
         elif isinstance(mask, ImageProvider):
             out = mask(self.scale)
             return np.asarray(out, dtype=np.float32)
         elif isinstance(mask, ImageConverter):
             return mask.with_scale(self.scale)
         raise TypeError(f"Invalid mask type: {type(mask)}")
@@ -1047,7 +1045,18 @@
     return order, _output_shape, _scale, _corner_safe
 
 
 def _is_iterable_of_funcs(x: Any) -> TypeGuard[Iterable[AggFunction]]:
     if not hasattr(x, "__iter__"):
         return False
     return all(callable(f) for f in x)
+
+
+def _normalize_max_shifts(x: nm | tuple[nm, nm, nm]) -> tuple[nm, nm, nm]:
+    if hasattr(x, "__iter__"):
+        tup = tuple(float(x0) for x0 in x)  # type: ignore
+        if len(tup) != 3:
+            raise ValueError(
+                "max_shifts must be a 3-tuple if multiple values are given."
+            )
+        return tup
+    return (float(x),) * 3  # type: ignore
```

### Comparing `acryo-0.2.3/acryo/loader/_batch.py` & `acryo-0.3.0/acryo/loader/_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import polars as pl
 
 from dask import array as da
 
 from acryo import _utils
 from acryo.molecules import Molecules
 from acryo._types import nm, pixel
+from acryo._dask import DaskArrayList
 from acryo.loader._base import LoaderBase
 from acryo.loader._loader import SubtomogramLoader, Unset
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from typing_extensions import Self
     from acryo.loader._base import _ShapeType
@@ -37,15 +38,14 @@
     def __init__(
         self,
         order: int = 3,
         scale: nm = 1.0,
         output_shape: pixel | tuple[pixel, pixel, pixel] | Unset = Unset(),
         corner_safe: bool = False,
     ) -> None:
-
         super().__init__(order, scale, output_shape, corner_safe)
         self._images: dict[Hashable, NDArray[np.float32] | da.Array] = {}
         self._molecules: Molecules = Molecules.empty([IMAGE_ID_LABEL])
 
     @property
     def loaders(self) -> LoaderAccessor:
         """Interface to access the subtomogram loaders."""
@@ -161,58 +161,58 @@
         out = self.replace(
             molecules=molecules,
             scale=self.scale * binsize,
         )
         out._images = _images
         return out
 
-    def construct_loading_tasks(
-        self, output_shape: _ShapeType = None
-    ) -> list[da.Array]:
-        return sum(
-            (
-                loader.construct_loading_tasks(output_shape=output_shape)
-                for loader in self.loaders
-            ),
-            start=[],
+    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
+        return DaskArrayList.concat(
+            loader.construct_loading_tasks(output_shape=output_shape)
+            for loader in self.loaders
         )
 
 
 class LoaderAccessor:
     def __init__(self, collection: BatchLoader):
-        self._collection = weakref.ref(collection)
+        self._loader = weakref.ref(collection)
 
     def __getitem__(self, idx: int) -> SubtomogramLoader:
-        col = self._collection()
-        mole = col.filter(pl.col(IMAGE_ID_LABEL) == idx).molecules
+        ldr = self._get_loader()
+        mole = ldr.filter(pl.col(IMAGE_ID_LABEL) == idx).molecules
         if mole.features.shape[0] == 0:
             raise KeyError(idx)
-        image = col._images[idx]
+        image = ldr._images[idx]
         loader = SubtomogramLoader(
             image,
             mole,
-            col.order,
-            col.scale,
-            col.output_shape,
-            col.corner_safe,
+            ldr.order,
+            ldr.scale,
+            ldr.output_shape,
+            ldr.corner_safe,
         )
         return loader
 
     def __iter__(self) -> Iterator[SubtomogramLoader]:
-        col = self._collection()
-
-        for key, group in col.molecules.groupby(IMAGE_ID_LABEL):
-            image = col._images[key]
+        ldr = self._get_loader()
+        for key, group in ldr.molecules.groupby(IMAGE_ID_LABEL):
+            image = ldr._images[key]
             loader = SubtomogramLoader(
                 image,
                 group,
-                col.order,
-                col.scale,
-                col.output_shape,
-                col.corner_safe,
+                ldr.order,
+                ldr.scale,
+                ldr.output_shape,
+                ldr.corner_safe,
             )
             yield loader
 
     def __len__(self) -> int:
         """Number of loaders."""
-        col = self._collection()
-        return len(col._images)
+        ldr = self._get_loader()
+        return len(ldr._images)
+
+    def _get_loader(self) -> BatchLoader:
+        loader = self._loader()
+        if loader is None:
+            raise RuntimeError("Loader is no longer available.")
+        return loader
```

### Comparing `acryo-0.2.3/acryo/loader/_cache.py` & `acryo-0.3.0/acryo/loader/_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pyright: reportPrivateImportUsage=false
 from __future__ import annotations
 
 from typing import NamedTuple, Mapping
 import tempfile
 from contextlib import contextmanager
 import numpy as np
 from dask import array as da
```

### Comparing `acryo-0.2.3/acryo/loader/_group.py` & `acryo-0.3.0/acryo/loader/_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 )
 
 from acryo._types import nm
 from acryo import _utils
 from acryo.loader import _misc
 
 if TYPE_CHECKING:
-    from typing_extensions import Self
     from dask.delayed import Delayed
     from numpy.typing import NDArray
     from acryo.loader._base import (
         LoaderBase,
         _ShapeType,
         TemplateInputType,
         MaskInputType,
@@ -155,15 +154,15 @@
         self,
         template: TemplateInputType | Mapping[_K, TemplateInputType],
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         alignment_model: type[BaseAlignmentModel] | AlignmentFactory = ZNCCAlignment,
         **align_kwargs,
-    ) -> Self[_K, _L]:
+    ) -> LoaderGroup[_K, _L]:
         """
         Align subtomograms to the template image.
 
         This method conduct so called "subtomogram alignment". Only shifts and rotations
         are calculated in this method. To get averaged image, you'll have to run "average"
         method using the resulting LoaderGroup instance.
 
@@ -182,33 +181,33 @@
             Additional keyword arguments passed to the input alignment model.
 
         Returns
         -------
         LoaderGroup
             A loader group instance with updated molecules.
         """
-        all_tasks: list[list[Delayed]] = []
+        all_tasks: list[list[da.Array | Delayed]] = []
         template_map = _normalize_template(template)
         for key, loader in self:
             model = alignment_model(
                 template=loader.normalize_template(template_map[key]),
-                mask=mask,
+                mask=loader.normalize_mask(mask),
                 **align_kwargs,
             )
             _max_shifts_px = np.asarray(max_shifts) / loader.scale
             tasks = loader.construct_mapping_tasks(
                 model.align,
                 max_shifts=_max_shifts_px,
                 output_shape=model.input_shape,
                 var_kwarg=dict(
                     quaternion=loader.molecules.quaternion(),
                     pos=loader.molecules.pos / loader.scale,
                 ),
             )
-            all_tasks.append(tasks)
+            all_tasks.append(list(tasks))
         all_results = da.compute(all_tasks)[0]
         out: list[tuple[_K, _L]] = []
         for (key, loader), results in zip(self, all_results):
             new = loader._post_align(results, model.input_shape)
             out.append((key, new))
         return self.__class__(out)
 
@@ -216,15 +215,15 @@
         self,
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         output_shape: _ShapeType = None,
         alignment_model: type[BaseAlignmentModel] = ZNCCAlignment,
         **align_kwargs,
-    ) -> Self[_K, _L]:
+    ) -> LoaderGroup[_K, _L]:
         """
         Align subtomograms without template image.
 
         A template-free version of :func:`align`. This method first
         calculates averaged image and uses it for the alignment template. To
         avoid loading same subtomograms twice, a memory-mapped array is created
         internally (so the second subtomogram loading is faster).
@@ -260,15 +259,15 @@
         templates: list[TemplateInputType] | Mapping[_K, list[TemplateInputType]],
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         alignment_model: type[BaseAlignmentModel] = ZNCCAlignment,
         label_name: str = "labels",
         **align_kwargs,
-    ) -> Self[_K, _L]:
+    ) -> LoaderGroup[_K, _L]:
         """
         Align subtomograms with multiple template images.
 
         A multi-template version of :func:`align`. This method calculate cross
         correlation for every template and uses the best local shift, rotation and
         template.
 
@@ -307,15 +306,15 @@
                 max_shifts=_max_shifts_px,
                 output_shape=model.input_shape,
                 var_kwarg=dict(
                     quaternion=loader.molecules.quaternion(),
                     pos=loader.molecules.pos / loader.scale,
                 ),
             )
-            all_tasks.append(tasks)
+            all_tasks.append(list(tasks))
         all_results = da.compute(all_tasks)[0]
         if isinstance(model, RotationImplemented) and model._n_rotations > 1:
             remainder = len(templates)
         else:
             remainder = -1
         out: list[tuple[_K, _L]] = []
         for (key, loader), results in zip(self, all_results):
@@ -346,27 +345,29 @@
         Returns
         -------
         dict of pl.DataFrame
             Result tables for each group.
         """
         all_tasks: list[list[Delayed]] = []
         if not hasattr(funcs, "__iter__"):
-            funcs = [funcs]
+            _funcs = [funcs]
+        else:
+            _funcs = funcs
         if schema is None:
-            schema = [fn.__name__ for fn in funcs]
+            schema = [fn.__name__ for fn in _funcs]
         if len(set(schema)) != len(schema):
             raise ValueError("Schema names must be unique.")
         keys: list[str] = []
         for key, loader in self:
             taskset = []
-            for fn in funcs:
+            for fn in _funcs:
                 tasks = loader.construct_mapping_tasks(
                     fn, output_shape=loader.output_shape
                 )
-                taskset.append(tasks)
+                taskset.append(list(tasks))
             all_tasks.append(taskset)
             keys.append(key)
         all_results = da.compute(all_tasks)[0]
         out: dict[_K, pl.DataFrame] = {}
         for key, result in zip(keys, all_results):
             out[key] = pl.DataFrame(np.array(result), schema=schema)
         return out
@@ -435,41 +436,41 @@
     def count(self) -> dict[_K, int]:
         """Dictionary of the molecule count in each group."""
         return {key: loader.count() for key, loader in self}
 
     def filter(
         self,
         predicate: pl.Expr | str | pl.Series | list[bool] | np.ndarray,
-    ) -> Self[_K, _L]:
+    ) -> LoaderGroup[_K, _L]:
         """Filter the molecules in each group."""
         return self.__class__((key, loader.filter(predicate)) for key, loader in self)
 
-    def head(self, n: int = 10) -> Self[_K, _L]:
+    def head(self, n: int = 10) -> LoaderGroup[_K, _L]:
         """Get the first n molecules in each group."""
         return self.__class__((key, loader.head(n)) for key, loader in self)
 
-    def tail(self, n: int = 10) -> Self[_K, _L]:
+    def tail(self, n: int = 10) -> LoaderGroup[_K, _L]:
         """Get the last n molecules in each group."""
         return self.__class__((key, loader.tail(n)) for key, loader in self)
 
-    def sample(self, n: int = 10, seed: int | None = None) -> Self[_K, _L]:
+    def sample(self, n: int = 10, seed: int | None = None) -> LoaderGroup[_K, _L]:
         """Get n random molecules in each group."""
         return self.__class__((key, loader.sample(n, seed)) for key, loader in self)
 
 
 class LoaderGroupByIterator(Iterable[tuple[_K, _L]]):
     """Iterator for the loader groupby."""
 
     def __init__(
         self,
         loader: _L,
         by: _K,
         order: int,
         scale: float,
-        output_shape: tuple[int, ...],
+        output_shape: tuple[int, int, int] | None,
         corner_safe: bool,
     ):
         self._loader = loader
         self._by = by
         self._order = order
         self._scale = scale
         self._output_shape = output_shape
```

### Comparing `acryo-0.2.3/acryo/loader/_loader.py` & `acryo-0.3.0/acryo/loader/_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # pyright: reportPrivateImportUsage=false
 
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
+    Callable,
     NamedTuple,
     Any,
 )
 import numpy as np
+from scipy import ndimage as ndi
 from dask import array as da
 
 from acryo._types import nm, pixel
 from acryo._reader import imread
 from acryo.molecules import Molecules
 from acryo import _utils
-from acryo.loader._base import LoaderBase, Unset
+from acryo.loader import _misc
+from acryo.loader._base import LoaderBase, Unset, _ShapeType
+from acryo._dask import DaskTaskPool, DaskArrayList
 
 if TYPE_CHECKING:
     from typing_extensions import Self
     from numpy.typing import NDArray
     from acryo.classification import PcaClassifier
-    from dask.delayed import Delayed
 
 
 class SubtomogramLoader(LoaderBase):
     """
     A class for efficient loading of subtomograms.
 
     A ``SubtomogramLoader`` instance is basically composed of two elements,
@@ -193,58 +196,55 @@
         )
 
         out._image = binned_image
         return out
 
     def construct_loading_tasks(
         self,
-        output_shape: tuple[pixel, ...] = None,
-    ) -> list[da.Array]:
+        output_shape: _ShapeType = None,
+    ) -> DaskArrayList:
         """
         Construct a list of subtomogram lazy loader.
 
         Returns
         -------
         list of Delayed object
             Each object returns a subtomogram on execution by ``da.compute``.
         """
+        output_shape = self._get_output_shape(output_shape)
         if (cached := self._get_cached_array(output_shape)) is not None:
-            return [cached[i] for i in range(len(self))]
+            return DaskArrayList(cached[i] for i in range(len(self)))
+
         image = self.image
         scale = self.scale
         if isinstance(image, np.ndarray):
             image = da.from_array(image)
 
         if self.corner_safe:
             _prep = _utils.prepare_affine_cornersafe
         else:
             _prep = _utils.prepare_affine
-        tasks: list[Delayed] = []
+        pool = DaskTaskPool.from_func(_rotated_crop)
         for i in range(len(self)):
             subvol, mtx = _prep(
                 image,
                 center=self.molecules.pos[i] / scale,
                 output_shape=output_shape,
                 rot=self.molecules.rotator[i],
             )
-            task = da.from_delayed(
-                _utils.rotated_crop(
-                    subvol,
-                    mtx,
-                    shape=output_shape,
-                    order=self.order,
-                    mode="constant",
-                    cval=np.mean,
-                ),
+            pool.add_task(
+                subvol,
+                mtx,
                 shape=output_shape,
-                dtype=np.float32,
+                order=self.order,
+                mode="constant",
+                cval=np.mean,
             )
-            tasks.append(task)
 
-        return tasks
+        return pool.asarrays(shape=output_shape, dtype=np.float32)
 
 
 class ClassificationResult(NamedTuple):
     """Tuple of classification results."""
 
     loader: SubtomogramLoader
     classifier: PcaClassifier
@@ -263,16 +263,39 @@
             f"The third argument 'order' must be 0, 1 or 3, got {order!r}."
         )
 
     # check output_shape
     if isinstance(output_shape, Unset):
         _output_shape = output_shape
     else:
-        _output_shape = _utils.normalize_shape(output_shape, ndim=ndim)
+        _output_shape = _misc.normalize_shape(output_shape, ndim=ndim)
 
     # check scale
     _scale = float(scale)
     if _scale <= 0:
         raise ValueError("Negative scale is not allowed.")
 
     _corner_safe = bool(corner_safe)
     return order, _output_shape, _scale, _corner_safe
+
+
+def _rotated_crop(
+    subimg,
+    mtx: NDArray[np.float32],
+    shape: tuple[int, int, int],
+    order: int,
+    mode: str,
+    cval: float | Callable[[NDArray[np.float32]], float],
+) -> NDArray[np.float32]:
+    if callable(cval):
+        cval = cval(subimg)
+
+    out = ndi.affine_transform(
+        subimg,
+        matrix=mtx,
+        output_shape=shape,
+        order=order,
+        prefilter=order > 1,
+        mode=mode,
+        cval=cval,
+    )
+    return out  # type: ignore
```

### Comparing `acryo-0.2.3/acryo/loader/_misc.py` & `acryo-0.3.0/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/loader/_mock.py` & `acryo-0.3.0/acryo/loader/_mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+# pyright: reportPrivateImportUsage=false
 from __future__ import annotations
 
-from ._base import LoaderBase, Unset
+from ._base import LoaderBase
 from typing import TYPE_CHECKING, Iterable, Sequence
 import numpy as np
 from numpy.typing import NDArray
 from dask import array as da, delayed
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 
 from acryo import _utils
-from acryo._types import nm, pixel
-from acryo._fft import fftn, ifftn
+from acryo._types import nm
+from acryo._typed_scipy import fftn, ifftn, spline_filter, affine_transform
+from acryo._dask import DaskArrayList, DaskTaskPool
 from acryo.molecules import Molecules
 from acryo.pipe._classes import ImageProvider
 
 if TYPE_CHECKING:
     from typing_extensions import Self
-    from dask.delayed import Delayed
     from ._base import _ShapeType
 
 
 class MockLoader(LoaderBase):
     """
     A subtomogram loader from a virtual tomogram.
 
@@ -48,125 +49,128 @@
     """
 
     def __init__(
         self,
         template: NDArray[np.float32] | ImageProvider,
         molecules: Molecules,
         noise: float = 0.0,
-        degrees: Sequence[float] | None = None,
+        degrees: Sequence[float] | NDArray[np.float32] | None = None,
         central_axis: tuple[float, float, float] = (0.0, 1.0, 0.0),
         order: int = 3,
         scale: nm = 1.0,
-        output_shape: pixel | tuple[pixel, pixel, pixel] | Unset = Unset(),
         corner_safe: bool = False,
     ) -> None:
         if noise < 0:
             raise ValueError("Noise must be non-negative.")
-        super().__init__(order, scale, output_shape, corner_safe)
+        super().__init__(order, scale, corner_safe)
         self._template = template
         self._noise = noise
         if degrees is None:
             if noise > 0:
                 # TODO: implement this
                 raise NotImplementedError(
                     "Noise simulation without degrees is not implemented yet."
                 )
             self._degrees = None
         else:
             self._degrees = np.asarray(degrees, dtype=np.float32)
         self._molecules = molecules
         self._central_axis = np.array(central_axis, dtype=np.float32)
+        if isinstance(template, ImageProvider):
+            self._output_shape = template(self.scale).shape
+        else:
+            self._output_shape = template.shape
+        if len(self._output_shape) != 3:
+            raise ValueError("Template must be 3D.")
 
     @property
     def molecules(self) -> Molecules:
         """All the molecules"""
         return self._molecules
 
-    def construct_loading_tasks(
-        self, output_shape: _ShapeType = None
-    ) -> list[da.Array]:
+    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
         # TODO: this implementation is not efficent. Radon transformation is not
         # actually needed. Apply missing wedge mask directly to the template, and
         # apply inverse-Radon only to the noise. The linearity of Radon
         # transformation guarantees that the result is correct.
-        tasks: list[Delayed] = []
         if isinstance(self._template, ImageProvider):
             template = self._template(self.scale)
         else:
             template = self._template
         if output_shape is None:
             output_shape = template.shape
         elif output_shape != template.shape:
-            raise ValueError("Mismatched output shape and template shape.")
+            raise ValueError(
+                f"Mismatched output shape {output_shape!r} and template shape "
+                f"{template.shape}."
+            )
 
         # spline prefilter in advance
         if self.order > 1:
-            template = ndi.spline_filter(
+            template = spline_filter(
                 template, order=self.order, mode="constant", output=np.float32
             )
         center = np.array(template.shape) / 2 - 0.5
         matrices = self.molecules.affine_matrix(
             center, center + self.molecules.pos / self.scale
         )
-        for i, mtx in enumerate(matrices):
-            img = _utils.delayed_affine(
-                template, mtx, order=self.order, prefilter=False
-            )
-            if self._degrees is None:
-                tasks.append(img)
-            else:
-                task = simulate_noise(
-                    img,
+        pool = DaskTaskPool.from_func(affine_transform)
+        for mtx in matrices:
+            pool.add_task(template, mtx, order=self.order, prefilter=False)
+        task_list = pool.asarrays(shape=template.shape, dtype=np.float32)
+        if self._degrees is not None:
+            task_list = DaskArrayList(
+                simulate_noise(
+                    task,
                     self._central_axis,
                     self._degrees,
                     self._noise,
                     seed=i,
                 )
-                tasks.append(task)
-        return tasks
+                for i, task in task_list.enumerate()
+            )
+
+        return task_list
 
     def replace(
         self,
         molecules: Molecules | None = None,
-        output_shape: pixel | tuple[pixel, pixel, pixel] | Unset | None = None,
+        output_shape: None = None,  # just for compatibility
         order: int | None = None,
         scale: float | None = None,
         corner_safe: bool | None = None,
     ) -> Self:
         if molecules is None:
             molecules = self.molecules
-        if output_shape is None:
-            output_shape = self.output_shape
         if order is None:
             order = self.order
         if scale is None:
             scale = self.scale
         if corner_safe is None:
             corner_safe = self.corner_safe
         return self.__class__(
             self._template,
             molecules=molecules,
             noise=self._noise,
             degrees=self._degrees,
-            output_shape=output_shape,
             order=order,
             scale=scale,
             corner_safe=corner_safe,
         )
 
 
 def simulate_noise(
-    img: NDArray[np.float32],
+    img: NDArray[np.float32] | da.Array,
     central_axis,
     degrees: NDArray[np.float32],
     noise: float,
     seed: int,
-):
+) -> da.Array:
     # img: spline filtered
-    matrices, output_shape = normalize_radon_input(img, central_axis, degrees)
+    matrices, output_shape = normalize_radon_input(img.shape, central_axis, degrees)
     sino: da.Array = da.stack(
         [
             da.from_delayed(
                 radon_single(img, mtx, order=3, output_shape=output_shape),
                 shape=output_shape[1:],
                 dtype=np.float32,
             )
@@ -190,31 +194,31 @@
     return out
 
 
 # Radon transform
 
 
 def normalize_radon_input(
-    self: NDArray[np.float32],
+    shape: tuple[int, int, int],
     central_axis: NDArray[np.float32],
-    degrees: NDArray[np.float32] | float,
+    degrees: NDArray[np.float32],
 ):
     radians = np.deg2rad(list(degrees))
 
     # normalize central axis to a 3D vector
     central_axis = np.asarray(central_axis)
     central_axis /= np.sqrt(np.sum(central_axis**2))  # normalize
     if central_axis.shape != (3,):
         raise ValueError("Central axis must be a 3D vector")
 
     # construct Affine transform matrices
-    height = int(np.ceil(np.linalg.norm(self.shape)))
-    output_shape = (height, self.shape[1], self.shape[2])
+    height = int(np.ceil(np.linalg.norm(shape)))
+    output_shape = (height, shape[1], shape[2])
     params = _get_rotation_matrices_for_radon_3d(
-        radians, central_axis, self.shape, output_shape
+        radians, central_axis, shape, output_shape
     )
 
     return params, output_shape
 
 
 @delayed
 def radon_single(img: np.ndarray, mtx: np.ndarray, order: int = 3, output_shape=None):
```

### Comparing `acryo-0.2.3/acryo/molecules.py` & `acryo-0.3.0/acryo/molecules/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 from pathlib import Path
 from typing import (
     Any,
-    Hashable,
     Iterable,
     TYPE_CHECKING,
-    Iterator,
     Sequence,
-    TypeVar,
     Union,
-    Generic,
     overload,
 )
+import warnings
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 import polars as pl
 from scipy.spatial.transform import Rotation
 from acryo._types import nm
 from acryo._utils import deprecated_kwarg
+from acryo.molecules._group import MoleculeGroup
+from acryo.molecules._cut import MoleculeCutGroup
+from acryo.molecules._rotation import (
+    axes_to_rotator,
+    from_euler_xyz_coords,
+    translate_euler,
+)
 
 if TYPE_CHECKING:
     from typing_extensions import Self, TypeGuard
-    from polars.type_aliases import IntoExpr
-    from polars.dataframe.groupby import GroupBy
+    from polars.type_aliases import IntoExpr, ParquetCompression
 
 _CSV_COLUMNS = ["z", "y", "x", "zvec", "yvec", "xvec"]
 PathLike = Union[str, Path, bytes]
 
 
 class Molecules:
     """
@@ -280,53 +283,62 @@
             Float precision, by default 4.
         """
         return self.to_dataframe().write_csv(
             str(save_path),
             float_precision=float_precision,
         )
 
-    def to_parquet(self, save_path: PathLike, *, compression="zstd") -> None:
+    def to_parquet(
+        self,
+        save_path: PathLike,
+        *,
+        compression: ParquetCompression = "zstd",
+    ) -> None:
         """
         Save molecules as a parquet file.
 
         Parameters
         ----------
         save_path : PathLike
             Save path.
         compression : str, default is "zstd"
             Compression method, by default "zstd".
         """
         return self.to_dataframe().write_parquet(
             str(save_path), compression=compression
         )
 
-    def __len__(self) -> int:
+    def count(self) -> int:
         """Return the number of molecules."""
         return self._pos.shape[0]
 
-    def __getitem__(self, key: int | slice | list[int] | np.ndarray) -> Self:
+    def __len__(self) -> int:
+        """Return the number of molecules."""
+        return self.count()
+
+    def __getitem__(self, key: int | slice | list[int] | NDArray[np.integer]) -> Self:
         return self.subset(key)
 
     @property
     def pos(self) -> NDArray[np.float32]:
         """Positions of molecules."""
         return self._pos
 
     @property
-    def x(self) -> NDArray[np.float32]:
+    def x(self) -> NDArray[np.float64]:
         """Vectors of x-axis."""
         return self._rotator.apply([0.0, 0.0, 1.0])
 
     @property
-    def y(self) -> NDArray[np.float32]:
+    def y(self) -> NDArray[np.float64]:
         """Vectors of y-axis."""
         return self._rotator.apply([0.0, 1.0, 0.0])
 
     @property
-    def z(self) -> NDArray[np.float32]:
+    def z(self) -> NDArray[np.float64]:
         """Vectors of z-axis."""
         return self._rotator.apply([1.0, 0.0, 0.0])
 
     @property
     def rotator(self) -> Rotation:
         """Return ``scipy.spatial.transform.Rotation`` object"""
         return self._rotator
@@ -444,70 +456,96 @@
         translation_0[:, :3, 3] = dst
         translation_1[:, :3, 3] = -src
 
         return np.einsum("nij,njk,nkl->nil", translation_0, rot_mat, translation_1)
 
     def cartesian_at(
         self,
-        index: int | slice | Iterable[int],
+        index,
         shape: tuple[int, int, int],
         scale: nm,
+    ):
+        warnings.warn(
+            "`cartesian_at` is deprecated and will be removed in the future. "
+            "Please use `local_coordinates` instead.",
+            DeprecationWarning,
+        )
+        return self.subset(index).local_coordinates(shape, scale, squeeze=True)
+
+    def local_coordinates(
+        self,
+        shape: tuple[int, int, int],
+        scale: nm = 1.0,
+        *,
+        squeeze: bool = True,
     ) -> NDArray[np.float32]:
-        if isinstance(index, int):
-            center = np.array(shape) / 2 - 0.5
-            vec_x = self._rotator[index].apply([0.0, 0.0, 1.0])
-            vec_y = self._rotator[index].apply([0.0, 1.0, 0.0])
+        """
+        Generate local coordinates at the neighborhood of each molecule.
+
+        Parameters
+        ----------
+        shape : (int, int, int)
+            Shape of the local coordinates.
+        scale : float, default is 1.0
+            Scale of the local coordinates.
+        squeeze : bool, default is True
+            If ture and the number of molecules is 1, the first axis will be removed.
+
+        Returns
+        -------
+        (N, D, Z, Y, X) array
+            World coordinates. ``array[i]`` can be directly used as the coordinates
+            for ``ndi.map_coordinates``.
+        """
+        coords_list: list[NDArray[np.float32]] = []
+        all_vec_x = self.x.astype(np.float32)
+        all_vec_y = self.y.astype(np.float32)
+        for index in range(self.count()):
+            center = [s / 2 - 0.5 for s in shape]
+            vec_x = all_vec_x[index]
+            vec_y = all_vec_y[index]
             vec_z = cross(vec_x, vec_y)
-            ind_z, ind_y, ind_x = [np.arange(s) - c for s, c in zip(shape, center)]  # type: ignore
-            x_ax: np.ndarray = vec_x[:, np.newaxis] * ind_x
-            y_ax: np.ndarray = vec_y[:, np.newaxis] * ind_y
-            z_ax: np.ndarray = vec_z[:, np.newaxis] * ind_z
-
-            # There will be many points so data type should be converted into 32-bit
-            x_ax = x_ax.astype(np.float32)
-            y_ax = y_ax.astype(np.float32)
-            z_ax = z_ax.astype(np.float32)
+            ind_z, ind_y, ind_x = (
+                (np.arange(s, dtype=np.float32) - c) for s, c in zip(shape, center)
+            )  # type: ignore
+            x_ax: NDArray[np.float32] = vec_x[:, np.newaxis] * ind_x
+            y_ax: NDArray[np.float32] = vec_y[:, np.newaxis] * ind_y
+            z_ax: NDArray[np.float32] = vec_z[:, np.newaxis] * ind_z
 
             coords = (
                 z_ax[:, :, np.newaxis, np.newaxis]
                 + y_ax[:, np.newaxis, :, np.newaxis]
                 + x_ax[:, np.newaxis, np.newaxis, :]
             )
             shifts = self.pos[index] / scale
             coords += shifts[:, np.newaxis, np.newaxis, np.newaxis]  # unit: pixel
-        elif isinstance(index, slice):
-            start, stop, step = index.indices(len(self))
-            coords = np.stack(
-                [self.cartesian_at(i, shape, scale) for i in range(start, stop, step)],
-                axis=0,
-            )
-        else:
-            coords = np.stack(
-                [self.cartesian_at(i, shape, scale) for i in index],
-                axis=0,
-            )
 
-        return coords
+            coords_list.append(coords)
+
+        if len(coords_list) == 1 and squeeze:
+            return coords_list[0]
+        else:
+            return np.stack(coords_list, axis=0)
 
-    def matrix(self) -> NDArray[np.float32]:
+    def matrix(self) -> NDArray[np.float64]:
         """
         Calculate rotation matrices that align molecules in such orientations
         that ``vec`` belong to the object.
 
         Returns
         -------
         (N, 3, 3) ndarray
             Rotation matrices. Rotations represented by these matrices transform
             molecules to the same orientations, i.e., align all the molecules.
         """
         return self._rotator.as_matrix()
 
     def euler_angle(
         self, seq: str = "ZXZ", degrees: bool = False
-    ) -> NDArray[np.float32]:
+    ) -> NDArray[np.float64]:
         """
         Calculate Euler angles that transforms a source vector to vectors that
         belong to the object.
 
         Parameters
         ----------
         seq : str, default is "ZXZ"
@@ -521,30 +559,30 @@
             angles are in degrees if this flag is True, else they are in radians.
 
         Returns
         -------
         (N, 3) ndarray
             Euler angles.
         """
-        seq = _translate_euler(seq)
+        seq = translate_euler(seq)
         return self._rotator.as_euler(seq, degrees=degrees)[..., ::-1]
 
-    def quaternion(self) -> NDArray[np.float32]:
+    def quaternion(self) -> NDArray[np.float64]:
         """
         Calculate quaternions that transforms a source vector to vectors that
         belong to the object.
 
         Returns
         -------
         (N, 4) ndarray
             Quaternions.
         """
         return self._rotator.as_quat()
 
-    def rotvec(self) -> NDArray[np.float32]:
+    def rotvec(self) -> NDArray[np.float64]:
         """
         Calculate rotation vectors that transforms a source vector to vectors
         that belong to the object.
 
         Returns
         -------
         (N, 3) ndarray
@@ -883,14 +921,26 @@
         ...
 
     def groupby(self, by: IntoExpr | Iterable[IntoExpr], *more_by: IntoExpr):
         """Group molecules into sub-groups."""
         df = self.to_dataframe()
         return MoleculeGroup(df.groupby(by, *more_by, maintain_order=True))
 
+    def cutby(self, by: str, bins: list[float]):
+        cat_label = "__category"
+        if cat_label in self.features.columns:
+            raise ValueError(f"Feature name {cat_label!r} should not be used.")
+        feature = self.features[by]
+        result = feature.cut(bins=bins, category_label=cat_label)
+        cat = result[cat_label]
+        df = self.to_dataframe().with_columns(cat)
+        return MoleculeCutGroup(
+            df.groupby(cat_label, maintain_order=True), label=cat_label
+        )
+
     def filter(
         self,
         predicate: pl.Expr | str | pl.Series | list[bool] | np.ndarray,
     ) -> Self:
         """Filter molecules by its features."""
         df = self.to_dataframe()
         df_filt = df.filter(predicate)
@@ -951,95 +1001,17 @@
         return self.__class__(
             self.pos,
             self.rotator,
             features=self.features.drop(columns, *more_columns),
         )
 
 
-_K = TypeVar("_K", bound=Hashable)
-
-
-class MoleculeGroup(Generic[_K]):
-    """A groupby-like object for molecules."""
-
-    def __init__(self, group: GroupBy[pl.DataFrame]):
-        self._group = group
-
-    def __iter__(self) -> Iterator[tuple[_K, Molecules]]:
-        for key, df in self._group:
-            mole = Molecules.from_dataframe(df)
-            yield key, mole  # type: ignore
-
-    @property
-    def features(self) -> GroupBy:
-        """Return the groupby object."""
-        return self._group
-
-
 def _is_boolean_array(a: Any) -> TypeGuard[NDArray[np.bool_]]:
     if isinstance(a, pl.Series):
         return a.dtype is pl.Boolean
     else:
         return getattr(a, "dtype", None) == "bool"
 
 
-def _translate_euler(seq: str) -> str:
-    table = str.maketrans({"x": "z", "z": "x", "X": "Z", "Z": "X"})
-    return seq[::-1].translate(table)
-
-
-def from_euler_xyz_coords(
-    angles: ArrayLike, seq: str = "ZXZ", degrees: bool = False
-) -> Rotation:
-    """Create a rotator using zyx-coordinate system, from Euler angles."""
-    seq = _translate_euler(seq)
-    angles = np.asarray(angles)
-    return Rotation.from_euler(seq, angles[..., ::-1], degrees)
-
-
-def _normalize(a: np.ndarray) -> np.ndarray:
-    """Normalize vectors to length 1. Input must be (N, 3)."""
-    return a / np.sqrt(np.sum(a**2, axis=1))[:, np.newaxis]
-
-
-def _extract_orthogonal(a: np.ndarray, b: np.ndarray) -> np.ndarray:
-    """Extract component of b orthogonal to a."""
-    a_norm = _normalize(a)
-    return b - np.sum(a_norm * b, axis=1)[:, np.newaxis] * a_norm
-
-
-def axes_to_rotator(z, y) -> Rotation:
-    ref = _normalize(np.atleast_2d(y))
-
-    n = ref.shape[0]
-    yx = np.arctan2(ref[:, 2], ref[:, 1])
-    zy = np.arctan(-ref[:, 0] / np.abs(ref[:, 1]))
-
-    rot_vec_yx = np.zeros((n, 3))
-    rot_vec_yx[:, 0] = yx
-    rot_yx = Rotation.from_rotvec(rot_vec_yx)
-
-    rot_vec_zy = np.zeros((n, 3))
-    rot_vec_zy[:, 2] = zy
-    rot_zy = Rotation.from_rotvec(rot_vec_zy)
-
-    rot1 = rot_yx * rot_zy
-
-    if z is None:
-        return rot1
-
-    vec = _normalize(np.atleast_2d(_extract_orthogonal(ref, z)))
-
-    vec_trans = rot1.apply(vec, inverse=True)  # in zx-plane
-
-    thetas = np.arctan2(vec_trans[..., 0], vec_trans[..., 2]) - np.pi / 2
-
-    rot_vec_zx = np.zeros((n, 3))
-    rot_vec_zx[:, 1] = thetas
-    rot2 = Rotation.from_rotvec(rot_vec_zx)
-
-    return rot1 * rot2
-
-
 def cross(x: ArrayLike, y: ArrayLike, axis=None) -> np.ndarray:
     """Vector outer product in zyx coordinate."""
     return -np.cross(x, y, axis=axis)  # type: ignore
```

### Comparing `acryo-0.2.3/acryo/pick/_base.py` & `acryo-0.3.0/acryo/pick/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from __future__ import annotations
 
 from typing import Any, Sequence, SupportsIndex
 from abc import ABC, abstractmethod
 
 import numpy as np
 from numpy.typing import NDArray
-from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 from dask import array as da
 
 from acryo.pipe._classes import ImageProvider
 from acryo.molecules import Molecules
 from acryo._rotation import normalize_rotations
-from acryo._utils import compose_matrices, missing_wedge_mask, delayed_affine
+from acryo._utils import compose_matrices, missing_wedge_mask
 from acryo._types import nm, Ranges
+from acryo._typed_scipy import spline_filter, affine_transform
+from acryo._dask import DaskTaskPool
 
 
 class BasePickerModel(ABC):
     def pick_molecules(
         self,
         image: da.Array,
         scale: nm = 1.0,
@@ -97,28 +98,28 @@
             template = self._template
 
         rotators = [Rotation.from_quat(r).inv() for r in self._quaternions]
         _center = np.array(template.shape) / 2 - 0.5
         matrices = compose_matrices(_center, rotators)
 
         if self.order > 2:
-            template = ndi.spline_filter(
+            template = spline_filter(
                 template,
                 order=self.order,
-                output=np.float32,  # type: ignore
+                output=np.float32,
                 mode="constant",
             )
-        tasks = [
-            delayed_affine(template, mtx, order=self.order, prefilter=False)
-            for mtx in matrices
-        ]
+
+        pool = DaskTaskPool.from_func(affine_transform)
+        for mtx in matrices:
+            pool.add_task(template, mtx, order=self.order, prefilter=False)
         mask = missing_wedge_mask(
             Rotation.from_quat([0, 0, 0, 1]), self._tilt_range, template.shape
         )
-        out: list[NDArray[np.float32]] = da.compute(tasks)[0]  # rotated templates
+        out = pool.compute()  # rotated templates
         templates = [o * mask for o in out]
         depth = tuple(np.ceil(np.array(templates[0].shape) / 2).astype(np.uint16))
         return {"templates": templates}, depth
 
     def _index_to_quaternions(self, argmax_indices):
         return np.take_along_axis(
             self._quaternions, argmax_indices[:, np.newaxis], axis=0
```

### Comparing `acryo-0.2.3/acryo/pick/_concrete.py` & `acryo-0.3.0/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/pipe/__init__.py` & `acryo-0.3.0/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/pipe/_classes.py` & `acryo-0.3.0/acryo/pipe/_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-from typing import Callable, overload
+from typing import Callable, overload, Union
 from typing_extensions import Self
 
 import numpy as np
 from numpy.typing import NDArray
 from acryo._types import nm
 
+_Quatity = Union[int, float, NDArray[np.float32]]
+
 
 class _Pipeline:
     def __init__(self, fn: Callable):
         self._func = fn
         self.__name__ = getattr(fn, "__name__", repr(fn))
 
     def with_name(self, name: str) -> Self:
@@ -35,19 +37,23 @@
 
 class ImageProvider(_Pipeline):
     """Function that provides an image at a given scale."""
 
     def __init__(self, provider: Callable[[nm], NDArray[np.float32]]):
         super().__init__(provider)
 
-    def __call__(self, scale: nm) -> NDArray[np.float32]:
+    def provide(self, scale: nm) -> NDArray[np.float32]:
+        """Provide an image at a given scale."""
         out = self._func(scale)
         _assert_3d_array(out, self._func)
         return out
 
+    def __call__(self, scale: nm) -> NDArray[np.float32]:
+        return self.provide(scale)
+
     def __add__(self, other) -> ImageProvider:
         if isinstance(other, ImageProvider):
             return self.__class__(lambda scale: self(scale) + other(scale)).with_name(
                 f"({self.__name__} + {other.__name__})"
             )
         return self.__class__(lambda scale: self(scale) + other)
 
@@ -86,38 +92,38 @@
             return self.__class__(lambda scale: self(scale) != other(scale)).with_name(
                 f"{self.__name__} != {other.__name__}"
             )
         return self.__class__(lambda scale: self(scale) != other)
 
     def __lt__(self, other) -> ImageProvider:
         if isinstance(other, ImageProvider):
-            return self.__class__(lambda scale: self(scale) < other(scale)).with_name(
-                f"{self.__name__} < {other.__name__}"
-            )
+            return self.__class__(
+                lambda scale: _lt(self(scale), other(scale))
+            ).with_name(f"{self.__name__} < {other.__name__}")
         return self.__class__(lambda scale: self(scale) < other)
 
     def __le__(self, other) -> ImageProvider:
         if isinstance(other, ImageProvider):
-            return self.__class__(lambda scale: self(scale) <= other(scale)).with_name(
-                f"{self.__name__} <= {other.__name__}"
-            )
+            return self.__class__(
+                lambda scale: _le(self(scale), other(scale))
+            ).with_name(f"{self.__name__} <= {other.__name__}")
         return self.__class__(lambda scale: self(scale) <= other)
 
     def __gt__(self, other) -> ImageProvider:
         if isinstance(other, ImageProvider):
-            return self.__class__(lambda scale: self(scale) > other(scale)).with_name(
-                f"{self.__name__} > {other.__name__}"
-            )
+            return self.__class__(
+                lambda scale: _gt(self(scale), other(scale))
+            ).with_name(f"{self.__name__} > {other.__name__}")
         return self.__class__(lambda scale: self(scale) > other)
 
     def __ge__(self, other) -> ImageProvider:
         if isinstance(other, ImageProvider):
-            return self.__class__(lambda scale: self(scale) >= other(scale)).with_name(
-                f"{self.__name__} >= {other.__name__}"
-            )
+            return self.__class__(
+                lambda scale: _ge(self(scale), other(scale))
+            ).with_name(f"{self.__name__} >= {other.__name__}")
         return self.__class__(lambda scale: self(scale) >= other)
 
     def __neg__(self) -> ImageProvider:
         return self.__class__(lambda scale: -self(scale)).with_name(
             f"(-{self.__name__})"
         )
 
@@ -126,19 +132,22 @@
     """Functionthat convert an image."""
 
     def __init__(
         self, converter: Callable[[NDArray[np.float32], nm], NDArray[np.float32]]
     ):
         super().__init__(converter)
 
-    def __call__(self, image: NDArray[np.float32], scale: nm) -> NDArray[np.float32]:
+    def convert(self, image: NDArray[np.float32], scale: nm) -> NDArray[np.float32]:
         out = self._func(image, scale)
         _assert_3d_array(out, self._func)
         return out
 
+    def __call__(self, image: NDArray[np.float32], scale: nm) -> NDArray[np.float32]:
+        return self.convert(image, scale)
+
     @overload
     def compose(self, other: ImageProvider) -> ImageProvider:
         ...
 
     @overload
     def compose(self, other: ImageConverter) -> ImageConverter:
         ...
@@ -233,59 +242,75 @@
                 lambda x, scale: self(x, scale) != other(scale)
             ).with_name(f"({self.__name__} != {other.__name__})")
         return self.__class__(lambda x, scale: self(x, scale) != other)
 
     def __gt__(self, other) -> ImageConverter:
         if isinstance(other, ImageConverter):
             return self.__class__(
-                lambda x, scale: self(x, scale) > other(x, scale)
+                lambda x, scale: _gt(self(x, scale), other(x, scale))
             ).with_name(f"({self.__name__} > {other.__name__})")
         elif isinstance(other, ImageProvider):
             return self.__class__(
-                lambda x, scale: self(x, scale) > other(scale)
+                lambda x, scale: _gt(self(x, scale), other(scale))
             ).with_name(f"({self.__name__} > {other.__name__})")
         return self.__class__(lambda x, scale: self(x, scale) > other)
 
     def __ge__(self, other) -> ImageConverter:
         if isinstance(other, ImageConverter):
             return self.__class__(
-                lambda x, scale: self(x, scale) >= other(x, scale)
+                lambda x, scale: _ge(self(x, scale), other(x, scale))
             ).with_name(f"({self.__name__} >= {other.__name__})")
         elif isinstance(other, ImageProvider):
             return self.__class__(
-                lambda x, scale: self(x, scale) >= other(scale)
+                lambda x, scale: _ge(self(x, scale), other(scale))
             ).with_name(f"({self.__name__} >= {other.__name__})")
         return self.__class__(lambda x, scale: self(x, scale) >= other)
 
     def __lt__(self, other) -> ImageConverter:
         if isinstance(other, ImageConverter):
             return self.__class__(
-                lambda x, scale: self(x, scale) < other(x, scale)
+                lambda x, scale: _lt(self(x, scale), other(x, scale))
             ).with_name(f"({self.__name__} < {other.__name__})")
         elif isinstance(other, ImageProvider):
             return self.__class__(
-                lambda x, scale: self(x, scale) < other(scale)
+                lambda x, scale: _lt(self(x, scale), other(scale))
             ).with_name(f"({self.__name__} < {other.__name__})")
         return self.__class__(lambda x, scale: self(x, scale) < other)
 
     def __le__(self, other) -> ImageConverter:
         if isinstance(other, ImageConverter):
             return self.__class__(
-                lambda x, scale: self(x, scale) <= other(x, scale)
+                lambda x, scale: _le(self(x, scale), other(x, scale))
             ).with_name(f"({self.__name__} <= {other.__name__})")
         elif isinstance(other, ImageProvider):
             return self.__class__(
-                lambda x, scale: self(x, scale) <= other(scale)
+                lambda x, scale: _le(self(x, scale), other(scale))
             ).with_name(f"({self.__name__} <= {other.__name__})")
         return self.__class__(lambda x, scale: self(x, scale) <= other)
 
     def __neg__(self) -> ImageConverter:
         return self.__class__(lambda x, scale: -self(x, scale))
 
 
 def _assert_3d_array(out, func):
     if not isinstance(out, np.ndarray):
         raise TypeError(
             f"Function {func!r} did not return a numpy.ndarray (got {type(out)})"
         )
     if out.ndim != 3:
         raise ValueError(f"Wrong image dimensionality: {out.shape}")
+
+
+def _ge(a, b) -> NDArray[np.float32]:
+    return np.greater_equal(a, b, dtype=np.float32)
+
+
+def _le(a, b) -> NDArray[np.float32]:
+    return np.less_equal(a, b, dtype=np.float32)
+
+
+def _gt(a, b) -> NDArray[np.float32]:
+    return np.greater(a, b, dtype=np.float32)
+
+
+def _lt(a, b) -> NDArray[np.float32]:
+    return np.less(a, b, dtype=np.float32)
```

### Comparing `acryo-0.2.3/acryo/pipe/_curry.py` & `acryo-0.3.0/acryo/pipe/_curry.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/pipe/_imread.py` & `acryo-0.3.0/acryo/pipe/_imread.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scipy import ndimage as ndi
 from acryo.pipe._curry import provider_function
 from acryo._reader import REG
 from acryo._types import nm
 
 
 @provider_function
-def from_file(scale: nm, path: str, original_scale: float = None, tol=0.01):
+def from_file(scale: nm, path: str, original_scale: float | None = None, tol=0.01):
     """
     An image provider function with rescaling.
 
     This function will provide a subtomogram loader with a resized image from a file.
     Will be used for the template images or the mask images.
 
     >>> loader.align(
```

### Comparing `acryo-0.2.3/acryo/pipe/_masking.py` & `acryo-0.3.0/acryo/pipe/_masking.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/pipe/_transform.py` & `acryo-0.3.0/acryo/pipe/_transform.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 @converter_function
 def center_by_mass(
     img: NDArray[np.float32], scale: nm, *, order: int = 3
 ) -> NDArray[np.float32]:
     """Centering an image by its center of mass."""
     shift = np.array(ndi.center_of_mass(img)) - np.array(img.shape) / 2
-    return ndi.shift(img, -shift, order=order, prefilter=order > 1, mode="nearest")
+    return ndi.shift(img, -shift, order=order, prefilter=order > 1, mode="nearest")  # type: ignore
 
 
 @converter_function
 def gaussian_filter(
     img: NDArray[np.float32], scale: nm, *, sigma: nm, mode="reflect", cval: float = 0.0
 ) -> NDArray[np.float32]:
     """Gaussian filtering an image."""
-    return ndi.gaussian_filter(img, sigma / scale, mode=mode, cval=cval)
+    return ndi.gaussian_filter(img, sigma / scale, mode=mode, cval=cval)  # type: ignore
 
 
 @converter_function
 def lowpass_filter(img: NDArray[np.float32], scale: nm, cutoff: float, order: int = 2):
     return _utils.lowpass_filter(img, cutoff=cutoff, order=order)
```

### Comparing `acryo-0.2.3/acryo/simulator.py` & `acryo-0.3.0/acryo/simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,30 @@
+# pyright: reportPrivateImportUsage=false
 from __future__ import annotations
 
 from types import MappingProxyType
-from typing import Callable, NamedTuple, Sequence, TYPE_CHECKING, Tuple
+from typing import (
+    Callable,
+    Iterable,
+    NamedTuple,
+    Sequence,
+    TYPE_CHECKING,
+    Tuple,
+    TypeVar,
+)
 import numpy as np
 from numpy.typing import NDArray
-from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 
 from acryo import _utils
-from acryo._types import nm, pixel
-from acryo.molecules import Molecules
+from acryo.molecules import Molecules, axes_to_rotator
 from acryo.pipe._classes import ImageProvider
+from acryo._types import nm, pixel
+from acryo._dask import DaskTaskPool
+from acryo._typed_scipy import spline_filter, affine_transform
 
 if TYPE_CHECKING:
     from typing_extensions import Self, Literal
     from scipy.spatial.transform import Rotation
     import polars as pl
 
 ColorType = Tuple[float, float, float]
@@ -78,15 +88,15 @@
     def __repr__(self) -> str:
         clsname = type(self).__name__
         return f"<{clsname} object with {len(self._components)} components>"
 
     @property
     def components(self) -> MappingProxyType[str, Component]:
         """Return all the components in the tomogram."""
-        return MappingProxyType(self._components)
+        return MappingProxyType(self._components)  # type: ignore
 
     @property
     def order(self) -> Literal[0, 1, 3]:
         """Return the interpolation order."""
         return self._order
 
     @property
@@ -196,154 +206,231 @@
 
     def simulate(
         self,
         shape: tuple[pixel, pixel, pixel],
         colormap: Callable[[pl.DataFrame], ColorType] | None = None,
     ) -> NDArray[np.float32]:
         """
-        Simulate tomogram.
+        Simulate a tomogram.
 
         Parameters
         ----------
         shape : tuple of int
             Shape of the tomogram.
         colormap: callable, optional
             Colormap used to generate the colored tomogram. The input is a polars
             row vector of features of each molecule.
+
         Returns
         -------
         np.ndarray
             Simulated tomogram image.
         """
         if len(self._components) == 0:
             import warnings
 
             warnings.warn("No molecules are added to the simulator.", UserWarning)
 
         if colormap is not None:
             return self._simulate_with_color(shape, colormap)
+        if len(shape) != 3:
+            raise ValueError("The shape must be a 3-tuple.")
         return self._simulate(shape)
 
     def _simulate(self, shape: tuple[pixel, pixel, pixel]):
         """Simulate a grayscale tomogram."""
         tomogram = np.zeros(shape, dtype=np.float32)
+        pool = DaskTaskPool.from_func(_simulate_one)
         for mol, image in self._components.values():
-            if isinstance(image, ImageProvider):
-                img = image(self.scale)
-            else:
-                img = image
-            starts, stops, mtxs = _prep_iterators(mol, img, self._scale)
-
-            # prefilter here to avoid repeated computation
-            if self.order > 1:
-                img = ndi.spline_filter(img, order=self.order, mode="constant")
-
+            img = self._get_image(image)
+            starts, stops, mtxs = _prep_iterators(mol, img.shape, self._scale)
             for start, stop, mtx in zip(starts, stops, mtxs):
-                sl_src, sl_dst = _prep_slices(start, stop, shape, img.shape)
+                pool.add_task(img, start, stop, mtx, shape, self.order)
 
-                transformed = ndi.affine_transform(
-                    img,
-                    mtx,
-                    mode="constant",
-                    cval=0.0,
-                    order=self.order,
-                    prefilter=False,
-                )
-                tomogram[sl_dst] += transformed[sl_src]  # type: ignore
+        results = pool.compute()
+        for sl, img_fragment in results:
+            if img_fragment is not None:
+                tomogram[sl] += img_fragment
 
         return tomogram
 
     def _simulate_with_color(
         self,
         shape: tuple[pixel, pixel, pixel],
         colormap: Callable[[pl.DataFrame], ColorType],
     ):
         """Simulate a colored tomogram."""
         tomogram = np.zeros((3,) + shape, dtype=np.float32)
+        pool = DaskTaskPool.from_func(_simulate_color_one)
         for mol, image in self._components.values():
-            if isinstance(image, ImageProvider):
-                img = image(self.scale)
-            else:
-                img = image
-            # image slice must be integer so split it into two parts
-            img_min = img.min()
-            img_max = img.max()
-            starts, stops, mtxs = _prep_iterators(mol, img, self._scale)
-
-            # prefilter here to avoid repeated computation
-            if self.order > 1:
-                img = ndi.spline_filter(img, order=self.order, mode="constant")
-
+            img = self._get_image(image)
+            starts, stops, mtxs = _prep_iterators(mol, img.shape, self._scale)
             feat = mol.features
             for i, (start, stop, mtx) in enumerate(zip(starts, stops, mtxs)):
-                _cr, _cg, _cb = colormap(feat[i])
-                sl_src, sl_dst = _prep_slices(start, stop, shape, img.shape)
-                sl_dst = (slice(None),) + sl_dst
-
-                transformed = ndi.affine_transform(
-                    img,
-                    mtx,
-                    mode="constant",
-                    cval=0.0,
-                    order=self.order,
-                    prefilter=False,
-                )
-                _a = (transformed[sl_src] - img_min) / (img_max - img_min)
-                color_array = np.stack([_cr * _a, _cg * _a, _cb * _a], axis=0)
+                f0 = colormap(feat[i])
+                pool.add_task(img, start, stop, mtx, shape, self.order, f0)
 
-                tomogram[sl_dst] += color_array
+        results = pool.compute()
+        for sl, img_fragment in results:
+            if img_fragment is not None:
+                tomogram[sl] += img_fragment
 
         return tomogram
 
-    def simulate_2d(self, shape: tuple[pixel, pixel]):
+    def simulate_2d(self, shape: tuple[pixel, pixel]) -> NDArray[np.float32]:
         """Simulate a grayscale tomogram."""
-        tomogram = np.zeros(shape, dtype=np.float32)
+        projection = np.zeros(shape, dtype=np.float32)
+        pool = DaskTaskPool.from_func(_simulate_2d_one)
         for mol, image in self._components.values():
-            if isinstance(image, ImageProvider):
-                img = image(self.scale)
-            else:
-                img = image
-            starts, stops, mtxs = _prep_iterators(mol, img, self._scale)
+            img = self._get_image(image)
+            starts, stops, mtxs = _prep_iterators(mol, img.shape, self._scale)
             zsize = mol.pos[:, 0].max() / self.scale + np.sum(img.shape)
             shape3d = (int(np.ceil(zsize)),) + shape
 
             # reduce z axis
             starts, stops, mtxs = starts[1:], stops[1:], mtxs[1:]
 
-            # prefilter here to avoid repeated computation
-            if self.order > 1:
-                img = ndi.spline_filter(img, order=self.order, mode="constant")
-
             for start, stop, mtx in zip(starts, stops, mtxs):
-                sl_src, sl_dst = _prep_slices(start, stop, shape3d, img.shape)
-                transformed = ndi.affine_transform(
-                    img,
-                    mtx,
-                    mode="constant",
-                    cval=0.0,
-                    order=self.order,
-                    prefilter=False,
-                )
-                projected = transformed[sl_src].sum(axis=0)
-                tomogram[sl_dst[1:]] += projected  # type: ignore
+                pool.add_task(img, start, stop, mtx, shape3d, self.order)
 
-        return tomogram
+        results = pool.compute()
+        for sl, img_fragment in results:
+            if img_fragment is not None:
+                projection[sl] += img_fragment
+
+        return projection
+
+    def simulate_projection(
+        self,
+        shape: tuple[int, int],
+        center: tuple[float, float, float],
+        xaxis: tuple[float, float, float],
+        yaxis: tuple[float, float, float],
+    ) -> NDArray[np.float32]:
+        """
+        Simulate a projection of the tomogram in any direction.
+
+        Projection plane and the projection range are defined by the given parameters.
+        ``shape`` and ``center`` define the range of the projection plane. Technically,
+        ``center`` will be the scale-considered center of the assumed 3D tomogram image.
+        ``xaxis`` and ``yaxis`` define the coordinate system of the projection plane.
+
+        Parameters
+        ----------
+        shape : (int, int)
+            Output shape of the projection.
+        center : (float, float, float)
+            Center of the projection plane in world coordinate system.
+        xaxis : (float, float, float)
+            X-axis of the projection plane in world coordinate system.
+        yaxis : (float, float, float)
+            Y-axis of the projection plane in world coordinate system.
+
+        Returns
+        -------
+        2D array
+            Simulated projection image.
+        """
+        projection = np.zeros(shape, dtype=np.float32)
+        ex = np.asarray(xaxis, dtype=np.float32) / np.linalg.norm(xaxis)
+        ey = np.asarray(yaxis, dtype=np.float32) / np.linalg.norm(yaxis)
+        if np.abs(np.dot(ex, ey)) > 1e-6:
+            raise ValueError(f"xaxis {xaxis!r} and yaxis {yaxis!r} are not orthogonal.")
+        rc = np.asarray(center, dtype=np.float32)
+        pool = DaskTaskPool.from_func(_simulate_projection_one)
+        for mol, image in self._components.values():
+            img = self._get_image(image)
+            pos_scaled = (mol.pos - rc) / self.scale
+            xcoords = pos_scaled.dot(ex) + (shape[1] - 1) / 2
+            ycoords = pos_scaled.dot(ey) + (shape[0] - 1) / 2
+            coords = np.stack((ycoords, xcoords), axis=1)
+            glob_rotator = axes_to_rotator(cross(ex, ey), ey)
+            for i, yx in enumerate(coords):
+                pool.add_task(yx, shape, img, mol.rotator[i], glob_rotator)
+
+        results = pool.compute()
+        for sl, img_fragment in results:
+            if img_fragment is not None:
+                projection[sl] += img_fragment
+
+        return projection
+
+    def simulate_tilt_series(
+        self,
+        degrees: Iterable[float],
+        shape: tuple[int, int, int],
+    ) -> NDArray[np.float32]:
+        """
+        Simulate a tilt series of the tomogram.
+
+        This method is a simplified version of :meth:`simulate_projection`. Projection
+        angles are restricted to the rotation around the y-axis of the world coordinate
+        and the tomogram will be projected parallel to the z-axis.
+
+        Parameters
+        ----------
+        degrees : iterable of float
+            Rotation angles.
+        shape : (int, int, int)
+            Tomogram shape.
+
+        Returns
+        -------
+        (N, Y, X) array
+            Tilting series image.
+        """
+        rads = np.deg2rad(list(degrees))
+        ntilt = len(rads)
+        ey = np.array([0, 1, 0], dtype=np.float32)
+        rc = (np.array(shape, dtype=np.float32) / 2 - 0.5) * self.scale
+        tilt_series = np.zeros((ntilt, shape[1], shape[2]), dtype=np.float32)
+        pool = DaskTaskPool.from_func(_simulate_projection_one_labeled)
+        for i, rad in enumerate(rads):
+            ex = np.array([np.sin(rad), 0, np.cos(rad)], dtype=np.float32)
+            for mol, image in self._components.values():
+                img = self._get_image(image)
+                pos_scaled = (mol.pos - rc) / self.scale
+                xcoords = pos_scaled.dot(ex) + (shape[2] - 1) / 2
+                ycoords = pos_scaled.dot(ey) + (shape[1] - 1) / 2
+                coords = np.stack((ycoords, xcoords), axis=1)
+                glob_rotator = axes_to_rotator(cross(ex, ey), ey)
+                for ci, yx in enumerate(coords):
+                    pool.add_task(yx, shape[1:], img, mol.rotator[ci], glob_rotator, i)
+
+        results = pool.compute()
+        for sl, img_fragment in results:
+            if img_fragment is not None:
+                tilt_series[sl] += img_fragment
+
+        return tilt_series
+
+    def _get_image(
+        self, image: NDArray[np.float32] | ImageProvider
+    ) -> NDArray[np.float32]:
+        if isinstance(image, ImageProvider):
+            img = image.provide(self.scale)
+        else:
+            img = image
+
+        if self.order > 1:
+            img = spline_filter(img, order=self.order, mode="constant")
+        return img
 
 
 def _compose_affine_matrices(
     center: np.ndarray,
     rotator: Rotation,
     output_center: np.ndarray | None = None,
-):
+) -> NDArray[np.float32]:
     """Compose Affine matrices from an array shape and a Rotation object."""
-
-    dz, dy, dx = center
     if output_center is None:
         raise NotImplementedError
 
+    dz, dy, dx = center
+
     # center to corner
     translation_0 = np.array(
         [
             [1.0, 0.0, 0.0, dz],
             [0.0, 1.0, 0.0, dy],
             [0.0, 0.0, 1.0, dx],
             [0.0, 0.0, 0.0, 1.0],
@@ -353,52 +440,182 @@
     # corner to center
     translation_1 = _eyes(len(rotator))
     translation_1[:, :3, 3] = -output_center
 
     rot_mtx = _eyes(len(rotator))
     rot_mtx[:, :3, :3] = rotator.as_matrix()
 
-    return np.einsum("ij,njk,nkl->nil", translation_0, rot_mtx, translation_1)
+    return np.einsum("ij,njk,nkl->nil", translation_0, rot_mtx, translation_1)  # type: ignore
 
 
 def _eyes(n: int) -> np.ndarray:
     return np.stack([np.eye(4, dtype=np.float32)] * n, axis=0)
 
 
-def _prep_iterators(mol: Molecules, image: np.ndarray, scale: float):
-
+def _prep_iterators(mol: Molecules, shape: tuple[int, int, int], scale: float):
     # image slice must be integer so split it into two parts
     pos = mol.pos / scale
     intpos = pos.astype(np.int32)
     residue = pos - intpos.astype(np.float32)
-    template_shape = image.shape
 
     # construct matrices
-    center = (np.array(template_shape) - 1.0) / 2.0
+    center = (np.array(shape) - 1.0) / 2.0
     starts = intpos - center.astype(np.int32)
-    stops = starts + template_shape
+    stops = starts + shape
     mtxs = _compose_affine_matrices(
         center, mol.rotator.inv(), output_center=center + residue
     )
 
     return starts, stops, mtxs
 
 
-def _prep_slices(start, stop, tomogram_shape, template_shape):
+_T = TypeVar("_T", bound=Iterable[int])
+
+
+def _prep_slices(
+    start: _T,
+    stop: _T,
+    tomogram_shape: _T,
+    template_shape: _T,
+) -> tuple[tuple[slice, ...], tuple[slice, ...] | None]:
     sl_src_list: list[slice] = []
     sl_dst_list: list[slice] = []
     for s, e, size, tsize in zip(start, stop, tomogram_shape, template_shape):
         try:
             _sl, _pads, _out_of_bound = _utils.make_slice_and_pad(s, e, size)
         except ValueError:
             # out-of-bound is not a problem while simulation
-            continue
+            return (slice(None),), None
         else:
             sl_dst_list.append(_sl)
             if _out_of_bound:
                 s0, s1 = _pads
                 sl_src_list.append(slice(s0, tsize - s1))
             else:
                 sl_src_list.append(slice(None))
     sl_src = tuple(sl_src_list)
     sl_dst = tuple(sl_dst_list)
     return sl_src, sl_dst
+
+
+def _simulate_one(
+    img: NDArray[np.float32],
+    start: tuple[int, int, int],
+    stop: tuple[int, int, int],
+    mtx: NDArray[np.float32],
+    shape: tuple[int, int, int],
+    order: int,
+) -> tuple[tuple[slice, ...], NDArray[np.float32] | None]:
+    sl_src, sl_dst = _prep_slices(start, stop, shape, img.shape)
+    if sl_dst is None:
+        return (slice(None),), None
+    transformed = affine_transform(
+        img,
+        mtx,
+        mode="constant",
+        cval=0.0,
+        order=order,
+        prefilter=False,
+    )
+    return sl_dst, transformed[sl_src]
+
+
+def _simulate_color_one(
+    img: NDArray[np.float32],
+    start: tuple[int, int, int],
+    stop: tuple[int, int, int],
+    mtx: NDArray[np.float32],
+    shape: tuple[int, int, int],
+    order: int,
+    color: tuple[float, float, float],
+) -> tuple[tuple[slice, ...], NDArray[np.float32] | None]:
+    _cr, _cg, _cb = color
+    sl_src, sl_dst = _prep_slices(start, stop, shape, img.shape)
+    if sl_dst is None:
+        return (slice(None),), None
+
+    sl_dst = (slice(None),) + sl_dst
+
+    transformed = affine_transform(
+        img,
+        mtx,
+        mode="constant",
+        cval=0.0,
+        order=order,
+        prefilter=False,
+    )
+    img_min = img.min()
+    img_max = img.max()
+    _a = (transformed[sl_src] - img_min) / (img_max - img_min)
+    color_array = np.stack([_cr * _a, _cg * _a, _cb * _a], axis=0)
+
+    return sl_dst, color_array
+
+
+def _simulate_2d_one(
+    img: NDArray[np.float32],
+    start: tuple[int, int, int],
+    stop: tuple[int, int, int],
+    mtx: NDArray[np.float32],
+    shape: tuple[int, int, int],
+    order: int,
+):
+    sl_src, sl_dst = _prep_slices(start, stop, shape, img.shape)
+    if sl_dst is None:
+        return (slice(None),), None
+    transformed = affine_transform(
+        img,
+        mtx,
+        mode="constant",
+        cval=0.0,
+        order=order,
+        prefilter=False,
+    )
+    projected = np.sum(transformed[sl_src], axis=0)
+    return sl_dst[1:], projected
+
+
+def _simulate_projection_one(
+    yx: NDArray[np.float32],
+    shape: tuple[int, int],
+    image: NDArray[np.float32],
+    rotator: Rotation,
+    glob_rotator: Rotation,
+) -> tuple[tuple[slice, slice], NDArray[np.float32] | None]:
+    proj_shape = np.array(image.shape[1:], dtype=np.int32)
+    min_ = yx - proj_shape.astype(np.float32) / 2 + 0.5
+    int_min_ = min_.astype(np.int32)
+    int_max_ = int_min_ + proj_shape
+
+    sl_src, sl_dst = _prep_slices(int_min_, int_max_, shape, proj_shape)
+
+    if sl_dst is None:
+        return (slice(None), slice(None)), None
+
+    center = np.array(image.shape) / 2 - 0.5
+    residue = np.array([0, *(min_ - int_min_)])
+    mtx = _compose_affine_matrices(
+        center, rotator.inv() * glob_rotator, center + residue
+    )[0]
+
+    transformed = affine_transform(
+        image, mtx, mode="constant", cval=0.0, order=3, prefilter=False
+    )
+    projection: NDArray[np.float32] = np.sum(transformed, axis=0)
+    return sl_dst, projection[sl_src]
+
+
+def _simulate_projection_one_labeled(
+    yx: NDArray[np.float32],
+    shape: tuple[int, int],
+    image: NDArray[np.float32],
+    rotator: Rotation,
+    glob_rotator: Rotation,
+    idx: int,
+) -> tuple[tuple[int, slice, slice], NDArray[np.float32] | None]:
+    sl, img = _simulate_projection_one(yx, shape, image, rotator, glob_rotator)
+    return (idx,) + sl, img
+
+
+def cross(x: np.ndarray, y: np.ndarray, axis=None) -> np.ndarray:
+    """Vector outer product in zyx coordinate."""
+    return -np.cross(x, y, axis=axis)  # type: ignore
```

### Comparing `acryo-0.2.3/acryo/testing/_templates.py` & `acryo-0.3.0/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.3/acryo/testing/core.py` & `acryo-0.3.0/acryo/testing/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import numpy as np
-from scipy import ndimage as ndi
 
-from acryo._fft import fftn, ifftn
+from acryo._typed_scipy import fftn, ifftn, affine_transform
 from acryo.molecules import Molecules
 from acryo._utils import compose_matrices
 from acryo._rotation import normalize_rotations
 from acryo._types import nm, degree
 
 
 class TomogramGenerator:
@@ -72,15 +71,15 @@
             [template.copy() for _ in range(gy)] for _ in range(gx)
         ]
         if self.quaternions.shape[0] > 0:
             matrices = self._get_matrices(rng)
             mtx_iterator = iter(matrices)
             for i, j in wrange(gy, gx):
                 mtx = next(mtx_iterator)
-                mols[i][j] = ndi.affine_transform(mols[i][j], mtx)
+                mols[i][j] = affine_transform(mols[i][j], mtx)
 
         for i, j in wrange(gy, gx):
             mols[i][j] += rng.normal(scale=self.noise_sigma, size=template.shape)
 
         if tilt_range != (-90, 90):
             mw = _missing_wedge_mask(template.shape, tilt_range=tilt_range)
             for i, j in wrange(gy, gx):
```

