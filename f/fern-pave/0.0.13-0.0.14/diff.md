# Comparing `tmp/fern_pave-0.0.13.tar.gz` & `tmp/fern_pave-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_pave-0.0.13.tar", max compression
+gzip compressed data, was "fern_pave-0.0.14.tar", max compression
```

## Comparing `fern_pave-0.0.13.tar` & `fern_pave-0.0.14.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      411 2023-05-01 02:10:43.568468 fern_pave-0.0.13/pyproject.toml
--rw-r--r--   0        0        0      745 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/__init__.py
--rw-r--r--   0        0        0      915 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/client.py
--rw-r--r--   0        0        0      348 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      196 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/environment.py
--rw-r--r--   0        0        0        0 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/py.typed
--rw-r--r--   0        0        0      689 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/__init__.py
--rw-r--r--   0        0        0      647 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/client.py
--rw-r--r--   0        0        0      934 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/__init__.py
--rw-r--r--   0        0        0     1900 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/detailed_financial_health_summary.py
--rw-r--r--   0        0        0     5469 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/expenditure_tag.py
--rw-r--r--   0        0        0     2901 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/fee_tag.py
--rw-r--r--   0        0        0     1664 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/get_financial_health_response.py
--rw-r--r--   0        0        0     1292 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py
--rw-r--r--   0        0        0     1020 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/necessity_level.py
--rw-r--r--   0        0        0     1610 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/normalized_frequency.py
--rw-r--r--   0        0        0     3704 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/recurring_expenditure.py
--rw-r--r--   0        0        0     1161 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/top_level_financial_health_summary.py
--rw-r--r--   0        0        0     1397 2023-05-01 02:10:43.568468 fern_pave-0.0.13/src/pave/resources/cashflow/types/transaction.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 fern_pave-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      411 2023-05-01 02:31:21.527135 fern_pave-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/client.py
+-rw-r--r--   0        0        0      348 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      196 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/environment.py
+-rw-r--r--   0        0        0        0 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/py.typed
+-rw-r--r--   0        0        0      689 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/__init__.py
+-rw-r--r--   0        0        0     5156 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/client.py
+-rw-r--r--   0        0        0      934 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/__init__.py
+-rw-r--r--   0        0        0     1900 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/detailed_financial_health_summary.py
+-rw-r--r--   0        0        0     5469 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/expenditure_tag.py
+-rw-r--r--   0        0        0     2901 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/fee_tag.py
+-rw-r--r--   0        0        0     1664 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/get_financial_health_response.py
+-rw-r--r--   0        0        0     1292 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py
+-rw-r--r--   0        0        0     1020 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/necessity_level.py
+-rw-r--r--   0        0        0     1610 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/normalized_frequency.py
+-rw-r--r--   0        0        0     3704 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/recurring_expenditure.py
+-rw-r--r--   0        0        0     1161 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/top_level_financial_health_summary.py
+-rw-r--r--   0        0        0     1397 2023-05-01 02:31:21.527135 fern_pave-0.0.14/src/pave/resources/cashflow/types/transaction.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 fern_pave-0.0.14/PKG-INFO
```

### Comparing `fern_pave-0.0.13/src/pave/__init__.py` & `fern_pave-0.0.14/src/pave/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/client.py` & `fern_pave-0.0.14/src/pave/client.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/core/datetime_utils.py` & `fern_pave-0.0.14/src/pave/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/core/jsonable_encoder.py` & `fern_pave-0.0.14/src/pave/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/__init__.py` & `fern_pave-0.0.14/src/pave/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/__init__.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/client.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
-from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PaveEnvironment
 from .types.get_financial_health_response import GetFinancialHealthResponse
 from .types.get_recurring_expenditures_response import GetRecurringExpendituresResponse
 
 
 class CashflowClient:
@@ -23,19 +22,15 @@
 
     def get_financial_health(
         self, user_id: str, *, start_date: dt.date, end_date: dt.date, with_transactions: typing.Optional[bool] = None
     ) -> GetFinancialHealthResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"v1/users/{user_id}/financial_health"),
-            params={
-                "start_date": str(start_date),
-                "end_date": str(end_date),
-                "with_transactions": jsonable_encoder(with_transactions),
-            },
+            params={"start_date": str(start_date), "end_date": str(end_date), "with_transactions": with_transactions},
             headers=remove_none_from_headers({"X-API-KEY": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFinancialHealthResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -73,15 +68,15 @@
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"v1/users/{user_id}/financial_health"),
                 params={
                     "start_date": str(start_date),
                     "end_date": str(end_date),
-                    "with_transactions": jsonable_encoder(with_transactions),
+                    "with_transactions": with_transactions,
                 },
                 headers=remove_none_from_headers({"X-API-KEY": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFinancialHealthResponse, _response.json())  # type: ignore
         try:
```

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/__init__.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/detailed_financial_health_summary.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/detailed_financial_health_summary.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/expenditure_tag.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/expenditure_tag.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/fee_tag.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/fee_tag.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/get_financial_health_response.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/get_financial_health_response.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/get_recurring_expenditures_response.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/necessity_level.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/necessity_level.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/normalized_frequency.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/normalized_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/recurring_expenditure.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/recurring_expenditure.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/top_level_financial_health_summary.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/top_level_financial_health_summary.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/src/pave/resources/cashflow/types/transaction.py` & `fern_pave-0.0.14/src/pave/resources/cashflow/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_pave-0.0.13/PKG-INFO` & `fern_pave-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-pave
-Version: 0.0.13
+Version: 0.0.14
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

