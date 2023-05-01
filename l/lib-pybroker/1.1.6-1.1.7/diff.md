# Comparing `tmp/lib-pybroker-1.1.6.tar.gz` & `tmp/lib-pybroker-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.6.tar", last modified: Wed Apr 26 06:50:02 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.7.tar", last modified: Mon May  1 20:41:31 2023, max compression
```

## Comparing `lib-pybroker-1.1.6.tar` & `lib-pybroker-1.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-26 06:50:02.964577 lib-pybroker-1.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.952577 lib-pybroker-1.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.956577 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 06:50:02.000000 lib-pybroker-1.1.6/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.960577 lib-pybroker-1.1.6/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43710 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    56921 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:50:02.960577 lib-pybroker-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    71227 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-26 06:49:54.000000 lib-pybroker-1.1.6/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.973930 lib-pybroker-1.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.973930 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 20:41:31.000000 lib-pybroker-1.1.7/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.977930 lib-pybroker-1.1.7/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46093 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:41:31.981930 lib-pybroker-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76914 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-01 20:41:17.000000 lib-pybroker-1.1.7/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.6/LICENSE` & `lib-pybroker-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/PKG-INFO` & `lib-pybroker-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.6
+Version: 1.1.7
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.6/README.md` & `lib-pybroker-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/setup.cfg` & `lib-pybroker-1.1.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lib-pybroker
-version = 1.1.6
+version = attr: pybroker.__version__
 url = http://www.pybroker.com
 author = Edward West
 author_email = edwest@pybroker.com
 description = Algorithmic trading with machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0 with Commons Clause
```

### Comparing `lib-pybroker-1.1.6/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.7/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.6
+Version: 1.1.7
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.6/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.7/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/__init__.py` & `lib-pybroker-1.1.7/src/pybroker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,7 +42,9 @@
     enable_logging,
     param,
     register_columns,
     unregister_columns,
 )
 from .strategy import Strategy, TestResult
 from .vect import cross, highv, lowv, sumv
+
+__version__ = "1.1.7"
```

### Comparing `lib-pybroker-1.1.6/src/pybroker/cache.py` & `lib-pybroker-1.1.7/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/common.py` & `lib-pybroker-1.1.7/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/config.py` & `lib-pybroker-1.1.7/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/context.py` & `lib-pybroker-1.1.7/src/pybroker/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,30 +239,34 @@
         """
         return self.positions(symbol, "short")
 
     def _verify_pos_type(self, pos_type: str):
         if pos_type != "short" and pos_type != "long":
             raise ValueError(f"Unknown pos_type: {pos_type!r}.")
 
-    def calc_target_shares(self, target_size: float, price: float) -> int:
-        r"""Calculates the number of shares given a ``target_size`` equity
-        allocation and share ``price``.
+    def calc_target_shares(
+        self, target_size: float, price: float, cash: Optional[float] = None
+    ) -> int:
+        r"""Calculates the number of shares given a ``target_size`` allocation
+        and share ``price``.
 
         Args:
-            target_size: Amount of :class:`pybroker.portfolio.Portfolio` equity
-                used to calculate the number of shares, where the max
-                ``target_size`` is ``1``. For example, a ``target_size`` of
-                ``0.1`` would represent 10% of equity.
+            target_size: Proportion of cash used to calculate the number of
+                shares, where the max ``target_size`` is ``1``. For example, a
+                ``target_size`` of ``0.1`` would represent 10% of cash.
             price: Share price used to calculate the number of shares.
+            cash: Cash used to calculate the number of number of shares. If
+                ``None``, then the :class:`pybroker.portfolio.Portfolio` equity
+                is used to calculate the number of shares.
 
         Returns:
             Number of shares given ``target_size`` and share ``price``.
         """
         return int(
-            self._portfolio.equity
+            (to_decimal(cash) if cash is not None else self._portfolio.equity)
             * to_decimal(target_size)
             / to_decimal(price)
         )
 
     def model(self, name: str, symbol: str) -> Any:
         r"""Returns a trained model.
 
@@ -348,14 +352,17 @@
         buy_shares: Number of shares to buy of ``symbol``.
         buy_limit_price: Limit price used for a buy (long) order of ``symbol``.
         sell_shares: Number of shares to sell of ``symbol``.
         sell_limit_price: Limit price used for a sell (short) order of
             ``symbol``.
         long_stops: Stops for long :class:`pybroker.portfolio.Entry`\ s.
         short_stops: Stops for short :class:`pybroker.portfolio.Entry`\ s.
+        cover: Whether ``buy_shares`` are used to cover a short position. If
+            ``True``, the resulting buy order will be placed before sell
+            orders.
         pending_order_id: ID of :class:`pybroker.scope.PendingOrder` that was
             created.
     """
 
     symbol: str
     date: np.datetime64
     buy_fill_price: Union[
@@ -378,14 +385,15 @@
     hold_bars: Optional[int]
     buy_shares: Optional[Decimal]
     buy_limit_price: Optional[Decimal]
     sell_shares: Optional[Decimal]
     sell_limit_price: Optional[Decimal]
     long_stops: Optional[frozenset[Stop]]
     short_stops: Optional[frozenset[Stop]]
+    cover: bool = field(default=False)
     pending_order_id: Optional[int] = field(default=None)
 
 
 class ExecSignal(NamedTuple):
     """Holds data of a buy/sell signal.
 
     Attributes:
@@ -648,14 +656,16 @@
         self.stop_profit: Optional[Union[int, float, Decimal]] = None
         self.stop_profit_pct: Optional[Union[int, float, Decimal]] = None
         self.stop_profit_limit: Optional[Union[int, float, Decimal]] = None
         self.stop_trailing: Optional[Union[int, float, Decimal]] = None
         self.stop_trailing_pct: Optional[Union[int, float, Decimal]] = None
         self.stop_trailing_limit: Optional[Union[int, float, Decimal]] = None
 
+        self._cover: bool = False
+
     def _verify_symbol(self):
         if self.symbol is None:
             raise ValueError("symbol is not set.")
 
     @property
     def bars(self) -> int:
         """Number of bars of data that have completed."""
@@ -736,27 +746,84 @@
         self._verify_symbol()
         return self._col_scope.fetch(  # type: ignore[return-value]
             self.symbol,  # type: ignore[arg-type]
             DataCol.VWAP.value,
             self._sym_end_index[self.symbol],
         )
 
+    @property
+    def cover_fill_price(
+        self,
+    ) -> Union[
+        int,
+        float,
+        np.floating,
+        Decimal,
+        PriceType,
+        Callable[[str, BarData], Union[int, float, Decimal]],
+    ]:
+        """Alias for :attr:`.buy_fill_price`. When set, this causes the buy
+        order to be placed before any sell orders.
+        """
+        return self.buy_fill_price
+
+    @cover_fill_price.setter
+    def cover_fill_price(
+        self,
+        fill_price: Union[
+            int,
+            float,
+            np.floating,
+            Decimal,
+            PriceType,
+            Callable[[str, BarData], Union[int, float, Decimal]],
+        ],
+    ):
+        self.buy_fill_price = fill_price
+        self._cover = True
+
+    @property
+    def cover_shares(self) -> Optional[Union[int, float, Decimal]]:
+        """Alias for :attr:`.buy_shares`. When set, this causes the buy
+        order to be placed before any sell orders.
+        """
+        return self.buy_shares
+
+    @cover_shares.setter
+    def cover_shares(self, shares: Optional[Union[int, float, Decimal]]):
+        self.buy_shares = shares
+        self._cover = True
+
+    @property
+    def cover_limit_price(self) -> Optional[Union[int, float, Decimal]]:
+        """Alias for :attr:`.buy_limit_price`. When set, this causes the buy
+        order to be placed before any sell orders.
+        """
+        return self.buy_limit_price
+
+    @cover_limit_price.setter
+    def cover_limit_price(
+        self, limit_price: Optional[Union[int, float, Decimal]]
+    ):
+        self.buy_limit_price = limit_price
+        self._cover = True
+
     def sell_all_shares(self):
         """Sells all long shares of :attr:`.ExecContext.symbol`."""
         pos = self.long_pos()
         if pos is None:
             return
         self.sell_shares = pos.shares
 
     def cover_all_shares(self):
         """Covers all short shares of :attr:`.ExecContext.symbol`."""
         pos = self.short_pos()
         if pos is None:
             return
-        self.buy_shares = pos.shares
+        self.cover_shares = pos.shares
 
     def foreign(
         self, symbol: str, col: Optional[str] = None
     ) -> Union[BarData, Optional[NDArray]]:
         """Retrieves bar data for another ticker symbol.
 
         Args:
@@ -885,32 +952,38 @@
             :class:`pybroker.portfolio.Position` if one exists, otherwise
             ``None``.
         """
         symbol = self._get_symbol(symbol)
         return super().pos(symbol, "short")
 
     def calc_target_shares(
-        self, target_size: float, price: Optional[float] = None
+        self,
+        target_size: float,
+        price: Optional[float] = None,
+        cash: Optional[float] = None,
     ) -> int:
-        r"""Calculates the number of shares given a ``target_size`` equity
-        allocation and share ``price``.
+        r"""Calculates the number of shares given a ``target_size`` allocation
+        and share ``price``.
 
         Args:
-            target_size: Amount of :class:`pybroker.portfolio.Portfolio` equity
-                used to calculate the number of shares, where the max
-                ``target_size`` is ``1``. For example, a ``target_size`` of
-                ``0.1`` would result in 10% of equity.
+            target_size: Proportion of cash used to calculate the number of
+                shares, where the max ``target_size`` is ``1``. For example, a
+                ``target_size`` of ``0.1`` would represent 10% of cash.
             price: Share price used to calculate the number of shares. If
                 ``None``, the share price of the ``ExecContext``\ 's
                 :attr:`.symbol` is used.
+            cash: Cash used to calculate the number of number of shares. If
+                ``None``, then the :class:`pybroker.portfolio.Portfolio` equity
+                is used to calculate the number of shares.
+
         Returns:
             Number of shares given ``target_size`` and share ``price``.
         """
         price = self.close[-1] if price is None else price
-        return super().calc_target_shares(target_size, price)
+        return super().calc_target_shares(target_size, price, cash)
 
     def cancel_pending_order(self, order_id: int) -> bool:
         """Cancels a :class:`pybroker.scope.PendingOrder` with ``order_id``."""
         return self._pending_order_scope.remove(order_id)
 
     def cancel_all_pending_orders(self, symbol: Optional[str] = None):
         r"""Cancels all :class:`pybroker.scope.PendingOrder`\ s for ``symbol``.
@@ -1152,14 +1225,15 @@
             hold_bars=self.hold_bars,
             buy_shares=buy_shares,
             buy_limit_price=buy_limit_price,
             sell_shares=sell_shares,
             sell_limit_price=sell_limit_price,
             long_stops=long_stops,
             short_stops=short_stops,
+            cover=self._cover,
         )
 
     def __getattr__(self, attr):
         if attr in self._scope.custom_data_cols:
             if self.symbol is None:
                 raise ValueError("symbol is not set.")
             return self._col_scope.fetch(
@@ -1174,14 +1248,15 @@
     Args:
         ctx: :class:`.ExecContext`.
         date: Current bar's date.
     """
     ctx._curr_date = date
     ctx._dt = None
     ctx._foreign.clear()
+    ctx._cover = False
     ctx.buy_fill_price = PriceType.MIDDLE
     ctx.buy_shares = None
     ctx.buy_limit_price = None
     ctx.sell_fill_price = PriceType.MIDDLE
     ctx.sell_shares = None
     ctx.sell_limit_price = None
     ctx.hold_bars = None
```

### Comparing `lib-pybroker-1.1.6/src/pybroker/data.py` & `lib-pybroker-1.1.7/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/eval.py` & `lib-pybroker-1.1.7/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/indicator.py` & `lib-pybroker-1.1.7/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/log.py` & `lib-pybroker-1.1.7/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/model.py` & `lib-pybroker-1.1.7/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/portfolio.py` & `lib-pybroker-1.1.7/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/src/pybroker/scope.py` & `lib-pybroker-1.1.7/src/pybroker/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,20 @@
             :class:`numpy.ndarray` of model predictions for every bar until
             ``end_index`` (when specified).
         """
         model_sym = ModelSymbol(name, symbol)
         if model_sym in self._sym_preds:
             return self._sym_preds[model_sym][:end_index]
         input_ = self._input_scope.fetch(symbol, name)
+        if input_.empty:
+            raise ValueError(
+                f"No input data found for model {name!r}. Consider "
+                "passing input_data_fn to pybroker#model() if custom columns "
+                "were registered."
+            )
         if model_sym not in self._models:
             raise ValueError(f"Model {name!r} not found for {symbol}.")
         trained_model = self._models[model_sym]
         if trained_model.predict_fn is not None:
             pred = trained_model.predict_fn(trained_model.instance, input_)
         else:
             predict_fn = getattr(trained_model.instance, "predict", None)
```

### Comparing `lib-pybroker-1.1.6/src/pybroker/strategy.py` & `lib-pybroker-1.1.7/src/pybroker/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
                 )
                 if exec.fn is not None:
                     exec_fns[sym] = exec.fn
         sym_exec_dates = {
             sym: frozenset(test_data.loc[pd.IndexSlice[sym, :]].index.values)
             for sym in exec_ctxs.keys()
         }
+        cover_sched: dict[np.datetime64, list[ExecResult]] = defaultdict(list)
         buy_sched: dict[np.datetime64, list[ExecResult]] = defaultdict(list)
         sell_sched: dict[np.datetime64, list[ExecResult]] = defaultdict(list)
         if pos_size_handler is not None:
             pos_ctx = PosSizeContext(
                 config=config,
                 portfolio=portfolio,
                 col_scope=col_scope,
@@ -205,14 +206,15 @@
                 pending_order_scope=pending_order_scope,
                 models=models,
                 sessions=sessions,
                 sym_end_index=sym_end_index,
             )
         logger = StaticScope.instance().logger
         logger.backtest_executions_start(test_dates)
+        cover_results: deque[ExecResult] = deque()
         buy_results: deque[ExecResult] = deque()
         sell_results: deque[ExecResult] = deque()
         exit_syms: deque[str] = deque()
         active_ctxs: dict[str, ExecContext] = {}
         for i, date in enumerate(test_dates):
             active_ctxs.clear()
             for sym, ctx in exec_ctxs.items():
@@ -223,35 +225,53 @@
                 set_exec_ctx_data(ctx, date)
                 if (
                     exit_dates
                     and sym in exit_dates
                     and date == exit_dates[sym]
                 ):
                     exit_syms.append(sym)
+            is_cover_sched = date in cover_sched
             is_buy_sched = date in buy_sched
             is_sell_sched = date in sell_sched
-            if is_buy_sched and (
+            if (
                 config.max_long_positions is not None
                 or pos_size_handler is not None
             ):
-                buy_sched[date].sort(key=_sort_by_score, reverse=True)
+                if is_cover_sched:
+                    cover_sched[date].sort(key=_sort_by_score, reverse=True)
+                elif is_buy_sched:
+                    buy_sched[date].sort(key=_sort_by_score, reverse=True)
             if is_sell_sched and (
                 config.max_short_positions is not None
                 or pos_size_handler is not None
             ):
                 sell_sched[date].sort(key=_sort_by_score, reverse=True)
             if pos_size_handler is not None and (
-                is_buy_sched or is_sell_sched
+                is_cover_sched or is_buy_sched or is_sell_sched
             ):
+                pos_size_buy_results = None
+                if is_cover_sched:
+                    pos_size_buy_results = cover_sched[date]
+                elif is_buy_sched:
+                    pos_size_buy_results = buy_sched[date]
                 self._set_pos_sizes(
                     pos_size_handler=pos_size_handler,
                     pos_ctx=pos_ctx,
-                    buy_results=buy_sched[date] if is_buy_sched else None,
+                    buy_results=pos_size_buy_results,
                     sell_results=sell_sched[date] if is_sell_sched else None,
                 )
+            if is_cover_sched:
+                self._place_buy_orders(
+                    date=date,
+                    price_scope=price_scope,
+                    pending_order_scope=pending_order_scope,
+                    buy_sched=cover_sched,
+                    portfolio=portfolio,
+                    enable_fractional_shares=enable_fractional_shares,
+                )
             if is_sell_sched:
                 self._place_sell_orders(
                     date=date,
                     price_scope=price_scope,
                     pending_order_scope=pending_order_scope,
                     sell_sched=sell_sched,
                     portfolio=portfolio,
@@ -276,17 +296,30 @@
             if after_exec_fn is not None:
                 after_exec_fn(active_ctxs)
             for ctx in active_ctxs.values():
                 result = self._to_result(ctx)
                 if result is None:
                     continue
                 if result.buy_shares is not None:
-                    buy_results.append(result)
+                    if result.cover:
+                        cover_results.append(result)
+                    else:
+                        buy_results.append(result)
                 if result.sell_shares is not None:
                     sell_results.append(result)
+            while cover_results:
+                self._schedule_order(
+                    result=cover_results.popleft(),
+                    created=date,
+                    sym_end_index=sym_end_index,
+                    delay=config.buy_delay,
+                    sched=cover_sched,
+                    col_scope=col_scope,
+                    pending_order_scope=pending_order_scope,
+                )
             while buy_results:
                 self._schedule_order(
                     result=buy_results.popleft(),
                     created=date,
                     sym_end_index=sym_end_index,
                     delay=config.buy_delay,
                     sched=buy_sched,
```

### Comparing `lib-pybroker-1.1.6/src/pybroker/vect.py` & `lib-pybroker-1.1.7/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_cache.py` & `lib-pybroker-1.1.7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_common.py` & `lib-pybroker-1.1.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_context.py` & `lib-pybroker-1.1.7/tests/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -466,14 +466,18 @@
     assert not len(tuple(ctx.short_positions(symbol)))
 
 
 def test_calc_target_shares(ctx):
     assert ctx.calc_target_shares(0.5, 33.50) == 50_000 // 33.5
 
 
+def test_calc_target_shares_with_cash(ctx):
+    assert ctx.calc_target_shares(1 / 3, 20, 10_000) == 166
+
+
 def test_to_result(ctx, symbol, date):
     ctx.buy_fill_price = PriceType.AVERAGE
     ctx.buy_shares = 20
     ctx.buy_limit_price = 99.99
     ctx.sell_fill_price: PriceType = PriceType.HIGH
     ctx.sell_shares = 20
     ctx.sell_limit_price = 110.11
@@ -595,17 +599,33 @@
     assert tuple(ctx_with_orders.trades()) == trades
 
 
 def test_trades_when_empty(ctx):
     assert not len(list(ctx.trades()))
 
 
-def test_set_exec_ctx_data(ctx, symbols, sym_end_index):
+@pytest.mark.parametrize(
+    "cover_attr, buy_attr",
+    [
+        ("cover_fill_price", "buy_fill_price"),
+        ("cover_shares", "buy_shares"),
+        ("cover_limit_price", "buy_limit_price"),
+    ],
+)
+def test_cover(ctx, cover_attr, buy_attr):
+    setattr(ctx, cover_attr, 99)
+    assert getattr(ctx, cover_attr) == 99
+    assert getattr(ctx, cover_attr) == getattr(ctx, buy_attr)
+    assert ctx._cover is True
+
+
+def test_set_exec_ctx_data(ctx, sym_end_index):
     date = np.datetime64("2020-01-01")
     ctx._foreign = {"SPY": np.random.rand(100)}
+    ctx._cover = True
     ctx.buy_fill_price = PriceType.AVERAGE
     ctx.buy_shares = 100
     ctx.buy_limit_price = 99
     ctx.sell_fill_price = PriceType.CLOSE
     ctx.sell_shares = 200
     ctx.sell_limit_price = 80
     ctx.hold_bars = 5
@@ -619,14 +639,15 @@
     ctx.stop_trailing = 100
     ctx.stop_trailing_pct = 15
     ctx.stop_trailing_limit = 80.8
     set_exec_ctx_data(ctx, date)
     assert ctx.dt == to_datetime(date)
     assert ctx.bars == sym_end_index[ctx.symbol]
     assert not ctx._foreign
+    assert ctx._cover is False
     assert ctx.buy_fill_price == PriceType.MIDDLE
     assert ctx.buy_shares is None
     assert ctx.buy_limit_price is None
     assert ctx.sell_fill_price == PriceType.MIDDLE
     assert ctx.sell_shares is None
     assert ctx.sell_limit_price is None
     assert ctx.hold_bars is None
```

### Comparing `lib-pybroker-1.1.6/tests/test_data.py` & `lib-pybroker-1.1.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_eval.py` & `lib-pybroker-1.1.7/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_indicator.py` & `lib-pybroker-1.1.7/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_log.py` & `lib-pybroker-1.1.7/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_model.py` & `lib-pybroker-1.1.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_portfolio.py` & `lib-pybroker-1.1.7/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.6/tests/test_scope.py` & `lib-pybroker-1.1.7/tests/test_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 You should have received a copy of the GNU Lesser General Public License along
 with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 import pandas as pd
+import pybroker
 import pytest
 import re
 from .fixtures import *
 from decimal import Decimal
 from pybroker.common import PriceType
 from pybroker.indicator import IndicatorSymbol
 from pybroker.model import model
@@ -115,14 +116,21 @@
 
 @pytest.mark.parametrize("value", [42, None])
 def test_param_when_set_and_get(value):
     param("foo", value)
     assert param("foo") == value
 
 
+def test_param_when_set_to_none():
+    param("baz", 11)
+    assert param("baz") == 11
+    param("baz", None)
+    assert param("baz") is None
+
+
 class TestStaticScope:
     def test_set_and_get_indicator(self, scope, hhv_ind):
         scope.set_indicator(hhv_ind)
         assert scope.has_indicator(hhv_ind.name)
         assert scope.get_indicator(hhv_ind.name) == hhv_ind
 
     def test_get_indicator_when_not_found_then_error(self, scope):
@@ -396,14 +404,33 @@
                 f"Model instance trained for {MODEL_NAME!r} does not define a "
                 "predict function. Please pass a predict_fn to "
                 "pybroker.model()."
             ),
         ):
             pred_scope.fetch("SPY", MODEL_NAME)
 
+    def test_fetch_when_input_data_empty_then_error(self, col_scope):
+        ind_scope = IndicatorScope({}, [])
+        input_scope = ModelInputScope(col_scope, ind_scope)
+        pybroker.model(MODEL_NAME, lambda sym, train, test: {})
+        model = TrainedModel(name=MODEL_NAME, instance={}, predict_fn=None)
+        pred_scope = PredictionScope(
+            models={ModelSymbol(MODEL_NAME, "SPY"): model},
+            input_scope=input_scope,
+        )
+        with pytest.raises(
+            ValueError,
+            match=re.escape(
+                f"No input data found for model {MODEL_NAME!r}. Consider "
+                "passing input_data_fn to pybroker#model() if custom columns "
+                "were registered."
+            ),
+        ):
+            pred_scope.fetch("SPY", MODEL_NAME)
+
 
 class TestPriceScope:
     @pytest.mark.parametrize(
         "price, expected_price",
         [
             (50, 50),
             (111.1, Decimal("111.1")),
```

### Comparing `lib-pybroker-1.1.6/tests/test_strategy.py` & `lib-pybroker-1.1.7/tests/test_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,86 @@
             assert kwargs["symbol"] == "AAPL"
             assert kwargs["shares"] == expected_sell_shares
             assert kwargs["fill_price"] == Decimal(
                 str(sell_df[sell_df["date"] == date]["close"].values[0])
             )
             assert kwargs["limit_price"] == 50.5
 
+    def test_backtest_when_pos_size_handler_and_cover(self, data_source_df):
+        def pos_size_handler(ctx):
+            signals = tuple(ctx.signals())
+            ctx.set_shares(signals[0], shares=10)
+            ctx.set_shares(signals[1], shares=20)
+            assert type(ctx.sessions["SPY"]) == dict
+            assert type(ctx.sessions["AAPL"]) == dict
+
+        def buy_exec_fn(ctx):
+            ctx.cover_fill_price = 1
+            ctx.cover_shares = 2
+
+        def sell_exec_fn(ctx):
+            ctx.sell_fill_price = 1
+            ctx.sell_shares = 1
+
+        buy_exec = Execution(
+            id=1,
+            symbols=frozenset(["SPY"]),
+            fn=buy_exec_fn,
+            model_names=frozenset(),
+            indicator_names=frozenset(),
+        )
+        sell_exec = Execution(
+            id=2,
+            symbols=frozenset(["AAPL"]),
+            fn=sell_exec_fn,
+            model_names=frozenset(),
+            indicator_names=frozenset(),
+        )
+        execs = {buy_exec, sell_exec}
+        portfolio = Portfolio(1_000_000)
+        mixin = BacktestMixin()
+        mixin.backtest_executions(
+            config=StrategyConfig(),
+            executions=execs,
+            before_exec_fn=None,
+            after_exec_fn=None,
+            sessions=defaultdict(dict),
+            models={},
+            indicator_data={},
+            test_data=data_source_df,
+            portfolio=portfolio,
+            pos_size_handler=pos_size_handler,
+            exit_dates={},
+        )
+        buy_df = data_source_df[data_source_df["symbol"] == "SPY"]
+        buy_dates = buy_df["date"].unique()[1:]
+        sell_df = data_source_df[data_source_df["symbol"] == "AAPL"]
+        sell_dates = sell_df["date"].unique()[1:]
+        assert len(portfolio.orders) == len(buy_dates) + len(sell_dates)
+        assert len(
+            list(
+                filter(
+                    lambda o: o.type == "buy"
+                    and o.symbol == "SPY"
+                    and o.shares == 10,
+                    portfolio.orders,
+                )
+            )
+        ) == len(buy_dates)
+        assert len(
+            list(
+                filter(
+                    lambda o: o.type == "sell"
+                    and o.symbol == "AAPL"
+                    and o.shares == 20,
+                    portfolio.orders,
+                )
+            )
+        ) == len(sell_dates)
+
     def test_backtest_executions_when_buy_delay(self, data_source_df):
         def buy_exec_fn(ctx):
             ctx.buy_fill_price = PriceType.CLOSE
             ctx.buy_limit_price = 100
             ctx.buy_shares = 200
 
         buy_exec = Execution(
@@ -611,14 +683,114 @@
                     df[(df["date"] == date) & (df["symbol"] == sym)][
                         "close"
                     ].values[0]
                 )
             )
             assert kwargs["limit_price"] is None
 
+    def test_backtest_executions_when_max_short_positions_and_cover(
+        self, data_source_df
+    ):
+        def sell_exec_fn(ctx):
+            if ctx.symbol == "AAPL":
+                if ctx.bars == 1:
+                    ctx.sell_shares = 200
+                elif ctx.bars == 2:
+                    ctx.cover_all_shares()
+            else:
+                if ctx.bars == 2:
+                    ctx.sell_shares = 100
+
+        exec = Execution(
+            id=1,
+            symbols=frozenset(["AAPL", "SPY"]),
+            fn=sell_exec_fn,
+            model_names=frozenset(),
+            indicator_names=frozenset(),
+        )
+        execs = {exec}
+        portfolio = Portfolio(100_000, max_short_positions=1)
+        mixin = BacktestMixin()
+        mixin.backtest_executions(
+            config=StrategyConfig(max_short_positions=1),
+            executions=execs,
+            before_exec_fn=None,
+            after_exec_fn=None,
+            sessions=defaultdict(dict),
+            models={},
+            indicator_data={},
+            test_data=data_source_df,
+            portfolio=portfolio,
+            pos_size_handler=None,
+            exit_dates={},
+        )
+        assert len(portfolio.short_positions) == 1
+        assert not portfolio.long_positions
+        assert len(portfolio.orders) == 3
+        orders = portfolio.orders
+        assert orders[0].symbol == "AAPL"
+        assert orders[0].shares == 200
+        assert orders[0].type == "sell"
+        assert orders[1].symbol == "AAPL"
+        assert orders[1].shares == 200
+        assert orders[1].type == "buy"
+        assert orders[2].symbol == "SPY"
+        assert orders[2].shares == 100
+        assert orders[2].type == "sell"
+        trades = portfolio.trades
+        assert len(trades) == 1
+        assert trades[0].symbol == "AAPL"
+        assert trades[0].type == "short"
+
+    def test_backtest_executions_when_max_long_positions_and_cover(
+        self, data_source_df
+    ):
+        def cover_exec_fn(ctx):
+            if ctx.symbol == "AAPL":
+                ctx.score = 2
+            else:
+                ctx.score = 1
+            ctx.cover_shares = 100
+            ctx.hold_bars = 1
+
+        exec = Execution(
+            id=1,
+            symbols=frozenset(["AAPL", "SPY"]),
+            fn=cover_exec_fn,
+            model_names=frozenset(),
+            indicator_names=frozenset(),
+        )
+        execs = {exec}
+        portfolio = Portfolio(100_000, max_long_positions=1)
+        mixin = BacktestMixin()
+        mixin.backtest_executions(
+            config=StrategyConfig(max_long_positions=1),
+            executions=execs,
+            before_exec_fn=None,
+            after_exec_fn=None,
+            sessions=defaultdict(dict),
+            models={},
+            indicator_data={},
+            test_data=data_source_df,
+            portfolio=portfolio,
+            pos_size_handler=None,
+            exit_dates={},
+        )
+        dates = data_source_df["date"].unique()[1:]
+        orders = portfolio.orders
+        assert (
+            len(list(filter(lambda o: o.symbol == "AAPL", orders)))
+            == len(dates) * 2 - 1
+        )
+        trades = portfolio.trades
+        assert (
+            len(list(filter(lambda t: t.symbol == "AAPL", trades)))
+            == len(dates) - 1
+        )
+
     @pytest.mark.parametrize(
         "price_type, expected_fill_price",
         [
             (50, 50),
             (Decimal(111.1), Decimal(111.1)),
             (lambda _symbol, _bar_data: 60, 60),
             (PriceType.OPEN, 200),
```

### Comparing `lib-pybroker-1.1.6/tests/test_vect.py` & `lib-pybroker-1.1.7/tests/test_vect.py`

 * *Files identical despite different names*

