# Comparing `tmp/cloud_radar-0.6.4.tar.gz` & `tmp/cloud_radar-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.6.4.tar", max compression
+gzip compressed data, was "cloud_radar-0.6.5.tar", max compression
```

## Comparing `cloud_radar-0.6.4.tar` & `cloud_radar-0.6.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0    12792 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/README.md
--rw-r--r--   0        0        0     1431 2023-04-24 00:45:28.601597 cloud_radar-0.6.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0     8886 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24195 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    13992 1970-01-01 00:00:00.000000 cloud_radar-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-01 19:49:52.609153 cloud_radar-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0    12792 2023-05-01 19:49:52.609153 cloud_radar-0.6.5/README.md
+-rw-r--r--   0        0        0     1431 2023-05-01 19:50:07.737241 cloud_radar-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0     8886 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-05-01 19:49:52.613153 cloud_radar-0.6.5/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    13992 1970-01-01 00:00:00.000000 cloud_radar-0.6.5/PKG-INFO
```

### Comparing `cloud_radar-0.6.4/LICENSE.txt` & `cloud_radar-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.4/README.md` & `cloud_radar-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.4/pyproject.toml` & `cloud_radar-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.6.4"
+version = "0.6.5"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.6.4/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.6.5/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.4/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.6.5/src/cloud_radar/cf/unit/_template.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.6.4/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.6.5/src/cloud_radar/cf/unit/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,19 +389,25 @@
     Raises:
         TypeError: If region is not a string.
 
     Returns:
         List[str]: The list of AZs for the provided region.
     """
 
+    if region is None:
+        region = _t.Region
+
     if not isinstance(region, str):
         raise TypeError(
             f"Fn::GetAZs - The region must be a String, not {type(region).__name__}."
         )
 
+    if region == "":
+        region = _t.Region
+
     return get_region_azs(region)
 
 
 def import_value(template: "Template", name: Any) -> str:
     """Solves AWS ImportValue intrinsic function.
 
     Args:
@@ -600,18 +606,30 @@
         value (str): The String containing variables.
 
     Returns:
         str: Input String with variables substituted.
     """
 
     def replace_var(m):
-        var = m.group(2)
-        return ref(template, var)
+        var = m.group(1)
+
+        if "." in var:
+            parts = var.split(".")
+
+            resouce_id = parts[0]
+
+            attributes = ".".join(parts[1:])
+
+            result = get_att(template, [resouce_id, attributes])
+        else:
+            result = ref(template, var)
 
-    reVar = r"(?!\$\{\!)\$(\w+|\{([^}]*)\})"
+        return result
+
+    reVar = r"(?!\$\{\!)\$\{(\w+[^}]*)\}"
 
     if re.search(reVar, value):
         return re.sub(reVar, replace_var, value).replace("${!", "${")
 
     return value.replace("${!", "${")
 
 
@@ -646,22 +664,33 @@
         local_vars = values[1]
     else:
         raise TypeError(
             "Fn::Sub - The first value must be a String and the second a Map."
         )
 
     def replace_var(m):
-        var = m.group(2)
+        var: str = m.group(1)
 
         if var in local_vars:
             return local_vars[var]
 
-        return ref(template, var)
+        if "." in var:
+            parts = var.split(".")
+
+            resouce_id = parts[0]
+
+            attributes = ".".join(parts[1:])
+
+            result = get_att(template, [resouce_id, attributes])
+        else:
+            result = ref(template, var)
+
+        return result
 
-    reVar = r"(?!\$\{\!)\$(\w+|\{([^}]*)\})"
+    reVar = r"(?!\$\{\!)\$\{(\w+[^}]*)\}"
 
     if re.search(reVar, source_string):
         return re.sub(reVar, replace_var, source_string).replace("${!", "${")
 
     return source_string.replace("${!", "${")
```

### Comparing `cloud_radar-0.6.4/PKG-INFO` & `cloud_radar-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.6.4
+Version: 0.6.5
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.6.4 Summary: Run functional
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.6.5 Summary: Run functional
 tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
 cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
 radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
 shadycuz@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

