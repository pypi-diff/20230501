# Comparing `tmp/fern_pave-0.0.14.tar.gz` & `tmp/fern_pave-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_pave-0.0.14.tar", max compression
+gzip compressed data, was "fern_pave-0.0.17.tar", max compression
```

## Comparing `fern_pave-0.0.14.tar` & `fern_pave-0.0.17.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      411 2023-05-01 02:31:21.527135 fern_pave-0.0.14/pyproject.toml
--rw-r--r--   0        0        0      745 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/__init__.py
--rw-r--r--   0        0        0      915 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/client.py
--rw-r--r--   0        0        0      348 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      196 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/environment.py
--rw-r--r--   0        0        0        0 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/py.typed
--rw-r--r--   0        0        0      689 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/__init__.py
--rw-r--r--   0        0        0      647 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/__init__.py
--rw-r--r--   0        0        0     5156 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/client.py
--rw-r--r--   0        0        0      934 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/__init__.py
--rw-r--r--   0        0        0     1900 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/detailed_financial_health_summary.py
--rw-r--r--   0        0        0     5469 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/expenditure_tag.py
--rw-r--r--   0        0        0     2901 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/fee_tag.py
--rw-r--r--   0        0        0     1664 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/get_financial_health_response.py
--rw-r--r--   0        0        0     1292 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py
--rw-r--r--   0        0        0     1020 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/necessity_level.py
--rw-r--r--   0        0        0     1610 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/normalized_frequency.py
--rw-r--r--   0        0        0     3704 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/recurring_expenditure.py
--rw-r--r--   0        0        0     1161 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/top_level_financial_health_summary.py
--rw-r--r--   0        0        0     1397 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/transaction.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 fern_pave-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0      503 2023-05-01 02:43:43.852100 fern_pave-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/client.py
+-rw-r--r--   0        0        0      348 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      196 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/environment.py
+-rw-r--r--   0        0        0        0 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/py.typed
+-rw-r--r--   0        0        0      689 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/__init__.py
+-rw-r--r--   0        0        0     5156 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/client.py
+-rw-r--r--   0        0        0      934 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/__init__.py
+-rw-r--r--   0        0        0     1900 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/detailed_financial_health_summary.py
+-rw-r--r--   0        0        0     5469 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/expenditure_tag.py
+-rw-r--r--   0        0        0     2901 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/fee_tag.py
+-rw-r--r--   0        0        0     1664 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/get_financial_health_response.py
+-rw-r--r--   0        0        0     1292 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py
+-rw-r--r--   0        0        0     1020 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/necessity_level.py
+-rw-r--r--   0        0        0     1610 2023-05-01 02:43:43.852100 fern_pave-0.0.17/src/pave/resources/cashflow/types/normalized_frequency.py
+-rw-r--r--   0        0        0     3704 2023-05-01 02:43:43.856099 fern_pave-0.0.17/src/pave/resources/cashflow/types/recurring_expenditure.py
+-rw-r--r--   0        0        0     1161 2023-05-01 02:43:43.856099 fern_pave-0.0.17/src/pave/resources/cashflow/types/top_level_financial_health_summary.py
+-rw-r--r--   0        0        0     1397 2023-05-01 02:43:43.856099 fern_pave-0.0.17/src/pave/resources/cashflow/types/transaction.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 fern_pave-0.0.17/PKG-INFO
```

### Comparing `fern_pave-0.0.14/src/pave/__init__.py` & `fern_pave-0.0.17/src/pave/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/client.py` & `fern_pave-0.0.17/src/pave/client.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/core/datetime_utils.py` & `fern_pave-0.0.17/src/pave/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/core/jsonable_encoder.py` & `fern_pave-0.0.17/src/pave/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/__init__.py` & `fern_pave-0.0.17/src/pave/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/__init__.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/client.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/client.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/__init__.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/detailed_financial_health_summary.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/detailed_financial_health_summary.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/expenditure_tag.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/expenditure_tag.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/fee_tag.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/fee_tag.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/get_financial_health_response.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/get_financial_health_response.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/necessity_level.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/necessity_level.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/normalized_frequency.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/normalized_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/recurring_expenditure.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/recurring_expenditure.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/top_level_financial_health_summary.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/top_level_financial_health_summary.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/src/pave/resources/cashflow/types/transaction.py` & `fern_pave-0.0.17/src/pave/resources/cashflow/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.14/PKG-INFO` & `fern_pave-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-pave
-Version: 0.0.14
+Version: 0.0.17
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

