# Comparing `tmp/ezfinpy-0.1.1.tar.gz` & `tmp/ezfinpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfinpy-0.1.1.tar", max compression
+gzip compressed data, was "ezfinpy-0.1.2.tar", max compression
```

## Comparing `ezfinpy-0.1.1.tar` & `ezfinpy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       29 2023-04-26 22:08:04.122488 ezfinpy-0.1.1/ezfinpy/__init__.py
--rw-r--r--   0        0        0     3421 2023-04-27 01:25:54.042405 ezfinpy-0.1.1/ezfinpy/pandas_patcher.py
--rw-r--r--   0        0        0     3885 2023-04-27 01:35:40.047916 ezfinpy-0.1.1/ezfinpy/simulator.py
--rw-r--r--   0        0        0     1128 2023-04-26 23:08:56.557202 ezfinpy-0.1.1/ezfinpy/utils.py
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      508 2023-04-27 01:50:14.135897 ezfinpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.1/README.md
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 ezfinpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-04-26 22:08:04.122488 ezfinpy-0.1.2/ezfinpy/__init__.py
+-rw-r--r--   0        0        0     3431 2023-05-01 00:00:11.815291 ezfinpy-0.1.2/ezfinpy/pandas_patcher.py
+-rw-r--r--   0        0        0     5919 2023-05-01 00:01:35.584345 ezfinpy-0.1.2/ezfinpy/simulator.py
+-rw-r--r--   0        0        0      668 2023-05-01 00:01:27.977646 ezfinpy-0.1.2/ezfinpy/utils.py
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      567 2023-05-01 00:02:12.027231 ezfinpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.2/README.md
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 ezfinpy-0.1.2/PKG-INFO
```

### Comparing `ezfinpy-0.1.1/ezfinpy/pandas_patcher.py` & `ezfinpy-0.1.2/ezfinpy/pandas_patcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """
     if rebalance:
         return simulate_with_rebalance(
             prices=prices, rebal_weights=weights, rebal_freq=rebal_freq
         )
     else:
         return simulate_without_rebalance(
-            prices=prices, start_weights=weights
+            prices=prices, starting_weights=weights
         )
 
 # utils
 
 def base(data, base=1):
     return data.div(data.iloc[0]).mul(base)
 
@@ -56,15 +56,15 @@
                 _self = pd.concat([_self, s], axis=1)
             else:
                 raise ValueError("Invalid types inside list")
 
     elif isinstance(data, (Series, DataFrame)):
         _self = pd.concat([_self, data], axis=1)
     else:
-        raise ValueError(f"Invalid arg type.")
+        raise ValueError("Invalid arg type.")
     return _self
 
 def exclude(_self, names: str | list | Series | DataFrame):
     return _self.drop(columns=names)
 
 def total_return(prices):
     return prices.iloc[-1]/prices.iloc[0] - 1
@@ -96,15 +96,15 @@
 
 def ezprint():
     pass
 
 def ezstats():
     pass
 
-def ezfreq(data, freq):
+def ezresample(data, freq):
     all_dates = data.index
     dates = pd.DataFrame(index=all_dates)
     dates['correct_date'] = dates.index
     dates = dates.resample(freq).last()
     resampled_data = data.loc[dates['correct_date'].values].copy()
     return resampled_data
 
@@ -118,13 +118,13 @@
     drawdown,
     volatility,
     rolling_volatility,
     cagr,
     sharpe,
     ezplot,
     ezprint,
-    ezfreq,
+    ezresample,
 ]
 for pandas_type in [Series, DataFrame]:
     for func in funcs:
         setattr(pandas_type, func.__name__, func)
```

### Comparing `ezfinpy-0.1.1/LICENSE.txt` & `ezfinpy-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.1/PKG-INFO` & `ezfinpy-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ezfinpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/renanmoretto/ezfinpy
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datetime (>=4.9)
 Requires-Dist: matplotlib (>=3.6.0)
-Requires-Dist: numpy (>=1.23.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.0)
+Requires-Dist: ruff (>=0.0.263,<0.0.264)
 Project-URL: Repository, https://github.com/renanmoretto/ezfinpy
 Description-Content-Type: text/markdown
```

