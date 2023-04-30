# Comparing `tmp/phable-0.1.5.tar.gz` & `tmp/phable-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phable-0.1.5.tar", max compression
+gzip compressed data, was "phable-0.1.6.tar", max compression
```

## Comparing `phable-0.1.5.tar` & `phable-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.5/LICENSE
--rw-r--r--   0        0        0     2645 2023-04-25 15:37:14.606164 phable-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.5/phable/__init__.py
--rw-r--r--   0        0        0     3111 2023-04-25 15:37:14.606725 phable-0.1.5/phable/http.py
--rw-r--r--   0        0        0     5203 2023-04-25 15:37:14.607113 phable-0.1.5/phable/json_parser.py
--rw-r--r--   0        0        0     3266 2023-04-25 15:37:14.607396 phable-0.1.5/phable/kinds.py
--rw-r--r--   0        0        0     3251 2023-04-25 15:37:14.607665 phable-0.1.5/phable/phable.py
--rw-r--r--   0        0        0    16671 2023-04-25 15:37:14.607992 phable-0.1.5/phable/scram.py
--rw-r--r--   0        0        0      721 2023-04-25 15:48:21.586998 phable-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 phable-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2685 2023-04-26 19:55:25.085338 phable-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.6/phable/__init__.py
+-rw-r--r--   0        0        0     3113 2023-04-26 19:54:55.255634 phable-0.1.6/phable/http.py
+-rw-r--r--   0        0        0     5896 2023-04-30 19:19:25.687621 phable-0.1.6/phable/json_parser.py
+-rw-r--r--   0        0        0     3266 2023-04-25 15:37:14.607396 phable-0.1.6/phable/kinds.py
+-rw-r--r--   0        0        0     3251 2023-04-30 19:48:57.508637 phable-0.1.6/phable/phable.py
+-rw-r--r--   0        0        0    16673 2023-04-30 17:57:04.940932 phable-0.1.6/phable/scram.py
+-rw-r--r--   0        0        0      721 2023-04-30 22:19:16.782060 phable-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 phable-0.1.6/PKG-INFO
```

### Comparing `phable-0.1.5/LICENSE` & `phable-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phable-0.1.5/README.md` & `phable-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,13 @@
 - Add more tests
 - Factory for serializers
 - Explain in the docs that zoneinfo module is used for tz data and may require other dependencies
 - Validate the Haystack timezones
 - Only provide tests for what is exposed on the API
 - Test Coord, XStr, and other kinds over API
 - Improve parsing of singletons Marker, Remove, and NA
+- Setup some prod and test log settings
 
 Questions
 ---------
  - What version Haystack should I put in the Grid meta?
  - How do we validate the responses meet the Haystack requirements?
```

### Comparing `phable-0.1.5/phable/http.py` & `phable-0.1.6/phable/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     if params:
         url += "?" + urllib.parse.urlencode(params, doseq=True, safe="/")
 
     if data:
         if data_as_json:
             request_data = json.dumps(data).encode()
             headers["Content-Type"] = "application/json; charset=UTF-8"
-            logger.critical(f"Here is the request data:\n{request_data}")
+            # logger.critical(f"Here is the request data:\n{request_data}")
         else:
             request_data = urllib.parse.urlencode(data).encode()
 
     httprequest = urllib.request.Request(
         url, data=request_data, headers=headers, method=method
     )
```

### Comparing `phable-0.1.5/phable/json_parser.py` & `phable-0.1.6/phable/json_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,40 @@
         if isinstance(new_d[x], dict):
             if "_kind" in new_d[x].keys():
                 new_d[x] = to_kind(new_d[x])
 
 
 # TODO :  Support pandas without requiring pandas dependency
 def grid_to_pandas(g: kinds.Grid) -> pd.DataFrame:
-    # rows = list(map(lambda row: row.cells, g.rows))
-    # return pd.DataFrame(data=rows, columns=g.col_names)
+    # initialize the pandas df
     col_names = [col_grid["name"] for col_grid in g.cols]
-    return pd.DataFrame(data=g.rows, columns=col_names)
+    df = pd.DataFrame(data=g.rows, columns=col_names)
+
+    # find a map for column names - we want something more readable
+    name_map = {}
+    for col in g.cols:
+        if col["name"] == "ts":
+            name_map["ts"] = "Timestamp"
+
+        if "meta" in col.keys():
+            if "id" in col["meta"].keys():
+                name_map[col["name"]] = col["meta"]["id"].dis
+
+    # rename the columns in the df to be easier to read
+    df = df.rename(columns=name_map)
+
+    # convert kind dataclass objects to types supported by Pandas
+    for col in df.columns:
+        x = df[col].iloc[0]
+        if isinstance(x, kinds.DateTime):
+            df[col] = df[col].apply(lambda x: x.val)  # .astype(datetime)
+        if isinstance(x, kinds.Number):
+            df[col] = df[col].apply(lambda x: x.val).astype(float)
+
+    return df
 
 
 def to_kind(d: dict[str, str]):
     # test to make sure d is a Dict
 
     parse_map = {
         "number": _parse_number,
```

### Comparing `phable-0.1.5/phable/kinds.py` & `phable-0.1.6/phable/kinds.py`

 * *Files identical despite different names*

### Comparing `phable-0.1.5/phable/phable.py` & `phable-0.1.6/phable/phable.py`

 * *Files identical despite different names*

### Comparing `phable-0.1.5/phable/scram.py` & `phable-0.1.6/phable/scram.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def get_auth_token(host_url: str, username: str, password: str):
     sc = ScramClient(username, password)
 
     # send hello msg & set the response
     hello_resp = request(host_url, headers=sc.get_hello_req())
-    logger.critical(f"Here are the headers from the hello resp:\n{hello_resp.headers}")
+    # logger.critical(f"Here are the headers from the hello resp:\n{hello_resp.headers}")
     sc.set_hello_resp(hello_resp)
 
     # send first msg & set the response
     first_resp = request(host_url, headers=sc.get_first_req())
     sc.set_first_resp(first_resp)
 
     # send last msg & set the response
```

### Comparing `phable-0.1.5/pyproject.toml` & `phable-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phable"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Rick Jennings <rjennings055@gmail.com>"]
 readme = "README.md"
 packages = [{include = "phable"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `phable-0.1.5/PKG-INFO` & `phable-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phable
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: Rick Jennings
 Author-email: rjennings055@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -69,12 +69,13 @@
 - Add more tests
 - Factory for serializers
 - Explain in the docs that zoneinfo module is used for tz data and may require other dependencies
 - Validate the Haystack timezones
 - Only provide tests for what is exposed on the API
 - Test Coord, XStr, and other kinds over API
 - Improve parsing of singletons Marker, Remove, and NA
+- Setup some prod and test log settings
 
 Questions
 ---------
  - What version Haystack should I put in the Grid meta?
  - How do we validate the responses meet the Haystack requirements?
```

