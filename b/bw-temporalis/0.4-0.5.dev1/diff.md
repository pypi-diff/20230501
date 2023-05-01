# Comparing `tmp/bw_temporalis-0.4.tar.gz` & `tmp/bw_temporalis-0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-0.4.tar", last modified: Fri Apr 28 08:05:27 2023, max compression
+gzip compressed data, was "bw_temporalis-0.5.dev1.tar", last modified: Mon May  1 08:05:06 2023, max compression
```

## Comparing `bw_temporalis-0.4.tar` & `bw_temporalis-0.5.dev1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.792483 bw_temporalis-0.4/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.4/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.4/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-04-28 08:05:27.792547 bw_temporalis-0.4/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1955 2023-04-23 13:14:37.000000 bw_temporalis-0.4/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.790923 bw_temporalis-0.4/bw_temporalis/
--rw-r--r--   0 chrismutel   (501) staff       (20)        4 2023-04-28 07:40:18.000000 bw_temporalis-0.4/bw_temporalis/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      316 2023-04-27 11:45:54.000000 bw_temporalis-0.4/bw_temporalis/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7987 2023-04-28 07:40:12.000000 bw_temporalis-0.4/bw_temporalis/lca.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.788456 bw_temporalis-0.4/bw_temporalis/lcia/
--rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-27 12:03:34.000000 bw_temporalis-0.4/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4718 2023-04-27 17:46:01.000000 bw_temporalis-0.4/bw_temporalis/lcia/climate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5352 2023-04-27 11:45:54.000000 bw_temporalis-0.4/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6513 2023-04-27 12:06:28.000000 bw_temporalis-0.4/bw_temporalis/timeline.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1197 2023-04-27 11:45:54.000000 bw_temporalis-0.4/bw_temporalis/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.791711 bw_temporalis-0.4/bw_temporalis.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-04-28 08:05:27.000000 bw_temporalis-0.4/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      642 2023-04-28 08:05:27.000000 bw_temporalis-0.4/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-28 08:05:27.000000 bw_temporalis-0.4/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.4/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      175 2023-04-28 08:05:27.000000 bw_temporalis-0.4/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-04-28 08:05:27.000000 bw_temporalis-0.4/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.788847 bw_temporalis-0.4/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.4/docs/conf.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.790690 bw_temporalis-0.4/examples/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.4/examples/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.4/examples/ia.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.4/examples/inv.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.4/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-04-28 08:05:27.792961 bw_temporalis-0.4/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 08:05:27.792310 bw_temporalis-0.4/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.4/tests/test_fixtures.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4585 2023-04-27 11:45:54.000000 bw_temporalis-0.4/tests/test_td.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3620 2023-04-27 11:45:54.000000 bw_temporalis-0.4/tests/test_timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/bw_temporalis/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/bw_temporalis/lcia/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/ia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/inv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_td.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_utils.py
```

### Comparing `bw_temporalis-0.4/LICENSE` & `bw_temporalis-0.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/PKG-INFO` & `bw_temporalis-0.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.4
+Version: 0.5.dev1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.4/README.md` & `bw_temporalis-0.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/bw_temporalis/lca.py` & `bw_temporalis-0.5.dev1/bw_temporalis/lca.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     """
     Calculate an LCA using graph traversal, with edges using temporal distributions.
 
     Edges with temporal distributions should store this information using `"temporal_distributions"`:
 
     ```python
         exchange["temporal_distribution"] = bw_temporalis.TemporalDistribution(
-            times=numpy.array([-2, -1, 0, 1, 2], dtype="timedelta64[D]"),
+            times=numpy.array([-2, -1, 0, 1, 2], dtype="timedelta64[s]"),
             values=numpy.ones(5)
         )
     ```
 
-    Temporal distribution times must always have the data type `timedelta64[D]`. Not all edges need to have temporal distributions.
+    Temporal distribution times must always have the data type `timedelta64[s]`. Not all edges need to have temporal distributions.
 
     Temporal distributions are **not density functions** - their values should sum to the exchange amount.
 
     As graph traversal is much slower than matrix calculations, we can limit which nodes get traversed in several ways:
 
     * All activities in a database marked as `static`
     * Any activity ids passed in `static_activity_indices`
@@ -44,15 +44,15 @@
     The output of a Temporalis LCA calculation is a `bw_temporalis.Timeline`, which can be characterized.
 
     Parameters
     ----------
     lca_object : bw2calc.LCA
         The already instantiated and calculated LCA class (i.e. `.lci()` and `.lcia()` have already been done)
     starting_datetime : datetime.datetime | str
-        When the functional unit happens. Must be a point in time. Can be `"now"` or `"2023-01-01"`.
+        When the functional unit happens. Must be a point in time. Normally something like `"now"` or `"2023-01-01"`.
     cutoff : float
         The fraction of the total score below which graph traversal should stop. In range `(0, 1)`.
     biosphere_cutoff : float
         The fraction of the total score below which we don't include separate biosphere nodes to be characterized in the `Timeline`. In range `(0, 1)`.
     max_calc : int
         Total number of LCA inventory calculations to perform during graph traversal
     static_activity_indices : set[int]
@@ -77,15 +77,15 @@
         skip_coproducts: bool | None = False,
         functional_unit_unique_id: int | None = -1,
         graph_traversal: GraphTraversal | None = GraphTraversal,
     ):
         self.lca_object = lca_object
         self.unique_id = functional_unit_unique_id
         self.t0 = TD(
-            np.array([np.datetime64(starting_datetime)]).astype("datetime64[D]"),
+            np.array([np.datetime64(starting_datetime)]),
             np.array([1]),
         )
         for db in bd.databases:
             if bd.databases[db].get("static"):
                 static_activity_indices.add(
                     {
                         obj[0]
```

### Comparing `bw_temporalis-0.4/bw_temporalis/lcia/climate.py` & `bw_temporalis-0.5.dev1/bw_temporalis/lcia/climate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 
 def characterize_co2(
     series,
     period: int | None = 100,
     cumulative: bool | None = False,
 ) -> pd.DataFrame:
@@ -114,17 +114,20 @@
     tau = 12.4  # Lifetime (years)
 
     date_beginning: np.datetime64 = series["date"].to_numpy()
     date_characterized: np.ndarray = date_beginning + np.arange(
         start=0, stop=period, dtype="timedelta64[Y]"
     ).astype("timedelta64[s]")
 
-    decay_multipliers: list = np.array([
-        (1 + f1 + f2) * alpha * tau * (1 - np.exp(-year / tau)) for year in range(period)
-    ])
+    decay_multipliers: list = np.array(
+        [
+            (1 + f1 + f2) * alpha * tau * (1 - np.exp(-year / tau))
+            for year in range(period)
+        ]
+    )
 
     forcing = pd.Series(data=series.amount * decay_multipliers, dtype="float64")
     if not cumulative:
         forcing = forcing.diff(periods=1).fillna(0)
 
     return pd.DataFrame(
         {
```

### Comparing `bw_temporalis-0.4/bw_temporalis/temporal_distribution.py` & `bw_temporalis-0.5.dev1/bw_temporalis/temporal_distribution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,151 @@
 from numbers import Number
+from typing import Any, SupportsFloat, Union
 
 import numpy as np
-from bw2speedups import consolidate
+import numpy.typing as npt
+
+from .convolution import (
+    consolidate,
+    datetime_type,
+    temporal_convolution_datetime_timedelta,
+    temporal_convolution_timedelta_timedelta,
+    timedelta_type,
+)
 
 
 class TemporalDistribution:
     """A container for a series of amount spread over time.
     Args:
         * *date* (ndarray): 1D array containg temporal info of `amount` with type `timedelta64` or `datetime64` .
         * *amount* (ndarray): 1D array containg amount with type `float`
 
         Times and amount must have same length and element of `amount` must correspond to the element of `date`
         with the same index.
     """
 
-    def __init__(self, date, amount):
+    def __init__(
+        self, date: npt.NDArray[np.datetime64 | np.timedelta64], amount: npt.NDArray
+    ):
         if not isinstance(date, np.ndarray) or not isinstance(amount, np.ndarray):
             raise ValueError("Invalid input types")
-        if not date.shape == amount.shape:
+        elif not date.shape == amount.shape:
             raise ValueError("Shapes of input `date` and `amount` not identical")
-        if not (
+        elif not (
             np.issubdtype(date.dtype, np.datetime64)
             or np.issubdtype(date.dtype, np.timedelta64)
         ):
-            raise ValueError("Incorrect `date` dtype")
+            raise ValueError(f"Incorrect `date` dtype ({date.dtype})")
+        elif not len(date):
+            raise ValueError("Empty array")
 
-        # Conversion needed for bw2speedups.consolidate function
+        # Conversion needed for `temporal_convolution` functions
         self.amount = amount.astype(np.float64)
 
         if np.issubdtype(date.dtype, np.datetime64):
-            self.date = date.astype("datetime64[D]")
-            self.base_time_type = "datetime64[D]"
+            self.date = date.astype(datetime_type)
+            self.base_time_type = datetime_type
         elif np.issubdtype(date.dtype, np.timedelta64):
-            self.date = date.astype("timedelta64[D]")
-            self.base_time_type = "timedelta64[D]"
+            self.date = date.astype(timedelta_type)
+            self.base_time_type = timedelta_type
         else:
             raise ValueError("`date` must be numpy datetime or timedelta array")
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self.amount.shape[0]
 
     @property
-    def total(self):
+    def total(self) -> float:
         return float(self.amount.sum())
 
-    def nonzero(self):
-        mask = self.amount != 0
-        return TemporalDistribution(self.date[mask], self.amount[mask])
-
-    def __getitem__(self, index):
-        return TemporalDistribution(
-            np.array(self.date[index]), np.array(self.amount[index])
-        )
-
-    def __mul__(self, other):
+    def __mul__(
+        self, other: Union["TemporalDistribution", SupportsFloat]
+    ) -> "TemporalDistribution":
         if isinstance(other, TemporalDistribution):
             if (
-                self.base_time_type == "datetime64[D]"
-                and other.base_time_type == "datetime64[D]"
+                self.base_time_type == datetime_type
+                and other.base_time_type == datetime_type
             ):
                 raise ValueError("Can't multiple two datetime arrays")
-
-            date = (self.date.reshape((-1, 1)) + other.date.reshape((1, -1))).ravel()
-            amount = (
-                self.amount.reshape((-1, 1)) * other.amount.reshape((1, -1))
-            ).ravel()
-
-            # Use array view in consolidate
-            # http://stackoverflow.com/a/33528073/4929813
-            t, v = consolidate(date.view("int64"), amount)
-            return TemporalDistribution(t.astype(self.base_time_type), v)
-        else:
-            try:
-                return TemporalDistribution(self.date, self.amount * float(other))
-            except:
-                raise ValueError(
-                    "Can't multiply `TemporalDistribution` and {}".format(type(other))
+            elif self.base_time_type == datetime_type:
+                date, amount = temporal_convolution_datetime_timedelta(
+                    first_date=self.date,
+                    first_amount=self.amount,
+                    second_date=other.date,
+                    second_amount=other.amount,
+                )
+            elif other.base_time_type == datetime_type:
+                date, amount = temporal_convolution_datetime_timedelta(
+                    first_date=other.date,
+                    first_amount=other.amount,
+                    second_date=self.date,
+                    second_amount=self.amount,
+                )
+            else:
+                date, amount = temporal_convolution_timedelta_timedelta(
+                    first_date=self.date,
+                    first_amount=self.amount,
+                    second_date=other.date,
+                    second_amount=other.amount,
                 )
+            return TemporalDistribution(date=date, amount=amount)
+        elif isinstance(other, Number):
+            return TemporalDistribution(
+                date=self.date, amount=self.amount * float(other)
+            )
+        else:
+            raise ValueError(
+                "Can't multiply `TemporalDistribution` and {}".format(type(other))
+            )
 
-    def __truediv__(self, other):
-        if self.base_time_type == "datetime64[D]":
+    def __truediv__(self, other: SupportsFloat) -> "TemporalDistribution":
+        if self.base_time_type == datetime_type:
             raise ValueError("Can't divide a datetime array")
         elif not isinstance(other, Number):
             raise ValueError("Can only divide time deltas by a number")
         return TemporalDistribution(self.date, self.amount / float(other))
 
-    def __lt__(self, other):
+    def __lt__(self, other: Any) -> bool:
         if not isinstance(other, TemporalDistribution):
             return False
         return self.amount.sum() < other.amount.sum()
 
-    def __add__(self, other):
+    def __add__(
+        self, other: Union["TemporalDistribution", SupportsFloat]
+    ) -> "TemporalDistribution":
         if isinstance(other, TemporalDistribution):
-            if self.base_time_type == other.base_time_type == "datetime64[D]":
-                raise ValueError("Can't add two datedate")
-            elif self.base_time_type == other.base_time_type == "timedelta64[D]":
+            if self.base_time_type == other.base_time_type == datetime_type:
+                raise ValueError("Can't add two datetimes")
+            elif self.base_time_type == other.base_time_type == timedelta_type:
                 date = np.hstack((self.date, other.date))
                 amount = np.hstack((self.amount, other.amount))
                 # same as in __mul__
-                t, v = consolidate(date.view("int64"), amount)
-                return TemporalDistribution(t.astype("timedelta64[D]"), v)
+                t, v = consolidate(indices=date.astype("int64"), amounts=amount)
+                return TemporalDistribution(t.astype(timedelta_type), v)
             else:
                 if not len(self) == len(other):
                     raise ValueError("Incompatible dimensions")
-                elif self.base_time_type == "timedelta64[D]":
+                elif self.base_time_type == timedelta_type:
+                    # `self` is timedelta, `other` is datetime
                     return TemporalDistribution(
                         other.date + self.date, self.amount + other.amount
                     )
                 else:
+                    # `self` is datetime, `other` is timedelta
                     return TemporalDistribution(
                         self.date + other.date, self.amount + other.amount
                     )
         elif isinstance(other, Number):
             return TemporalDistribution(self.date, self.amount + float(other))
         else:
             raise ValueError(
                 "Can't add TemporalDistribution and {}".format(type(other))
             )
 
-    def __iter__(self):
-        for index in range(len(self)):
-            yield (self.date[index], float(self.amount[index]))
-
-    def __str__(self):
+    def __str__(self) -> str:
         return "TemporalDistribution instance with %s amount and total: %.4g" % (
             len(self.amount),
             self.total,
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self)
-
-    def cumulative(self):
-        """Return new temporal distribution with cumulative amount"""
-        return TemporalDistribution(self.date, np.cumsum(self.amount))
```

### Comparing `bw_temporalis-0.4/bw_temporalis/timeline.py` & `bw_temporalis-0.5.dev1/bw_temporalis/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 import numpy as np
 import pandas as pd
 
 from .temporal_distribution import TemporalDistribution
 
 
+class EmptyTimeline(Exception):
+    """Operation on empty timeline"""
+
+    pass
+
+
 @dataclass
 class FlowTD:
     """
     Class for storing a temporal distribution associated with a flow and activity.
 
     Attributes
     ----------
@@ -72,15 +78,28 @@
         -------
         None, creates class attribute Pandas DataFrame `df` with the following columns:
         - date: datetime64[s]
         - amount: float64
         - flow: int
         - activity: int
         """
+        if not len(self.data):
+            raise EmptyTimeline("No `FlowTD` elements present")
+
         date = np.hstack([o.distribution.date for o in self.data])
+
+        # Not really testable; `TemporalDistribution` will raise an error with an
+        # empty array. But our users are creative...
+        if not len(date):
+            raise EmptyTimeline(
+                "This timeline is empty; element: {}".format(
+                    [len(x) for x in self.data]
+                )
+            )
+
         amount = np.hstack([o.distribution.amount for o in self.data])
         flow = np.hstack([o.flow * np.ones(len(o.distribution)) for o in self.data])
         activity = np.hstack(
             [o.activity * np.ones(len(o.distribution)) for o in self.data]
         )
 
         self.df = pd.DataFrame(
@@ -136,15 +155,15 @@
             Period in days.
         flow : int
         activity : int
 
         Returns
         -------
         A Pandas DataFrame with the following columns:
-        - date: datetime64[D]
+        - date: datetime64[s]
         - amount: float64
         - flow: int
         - activity: int
 
         """
         df = self.df.copy()
         if activity:
```

### Comparing `bw_temporalis-0.4/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-0.5.dev1/bw_temporalis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-temporalis
-Version: 0.4
+Version: 0.5.dev1
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.4/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-0.5.dev1/bw_temporalis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 ./bw_temporalis/__init__.py
+./bw_temporalis/convolution.py
 ./bw_temporalis/lca.py
 ./bw_temporalis/temporal_distribution.py
 ./bw_temporalis/timeline.py
 ./bw_temporalis/utils.py
 ./bw_temporalis/lcia/__init__.py
 ./bw_temporalis/lcia/climate.py
 ./docs/conf.py
@@ -17,10 +18,12 @@
 bw_temporalis/VERSION
 bw_temporalis.egg-info/PKG-INFO
 bw_temporalis.egg-info/SOURCES.txt
 bw_temporalis.egg-info/dependency_links.txt
 bw_temporalis.egg-info/not-zip-safe
 bw_temporalis.egg-info/requires.txt
 bw_temporalis.egg-info/top_level.txt
+tests/test_convolution.py
 tests/test_fixtures.py
 tests/test_td.py
-tests/test_timeline.py
+tests/test_timeline.py
+tests/test_utils.py
```

### Comparing `bw_temporalis-0.4/docs/conf.py` & `bw_temporalis-0.5.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/examples/__init__.py` & `bw_temporalis-0.5.dev1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/examples/ia.py` & `bw_temporalis-0.5.dev1/examples/ia.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/examples/inv.py` & `bw_temporalis-0.5.dev1/examples/inv.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/setup.cfg` & `bw_temporalis-0.5.dev1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 include_package_data = True
 package_dir = 
 	=.
 python_requires = >=3.8
 install_requires = 
 	bw2calc >=2.0.dev12
 	bw2data >=4.0.dev18
-	bw2speedups
 	bw_graph_tools
 	numpy
 	pandas
+	tqdm
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `bw_temporalis-0.4/tests/test_fixtures.py` & `bw_temporalis-0.5.dev1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.4/tests/test_td.py` & `bw_temporalis-0.5.dev1/tests/test_td.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,24 +143,13 @@
 
 def test_add_td_to_dt_error(simple):
     td2 = TD(np.array((-1, 0, 1), dtype="datetime64[D]"), np.ones(3).astype(float))
     with pytest.raises(ValueError):
         simple + td2
 
 
-def test_iter(simple):
-    td = iter(simple)
-    assert next(td) == (np.timedelta64(0, "D"), 2)
-    assert next(td) == (np.timedelta64(1, "D"), 2)
-    assert next(td) == (np.timedelta64(2, "D"), 2)
-    assert next(td) == (np.timedelta64(3, "D"), 2)
-    assert next(td) == (np.timedelta64(4, "D"), 2)
-    with pytest.raises(StopIteration):
-        next(td)
-
-
 def test_str(simple):
     assert str(simple)
 
 
 def test_repr(simple):
     assert repr(simple)
```

