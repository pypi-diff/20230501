# Comparing `tmp/which_plates-0.7.0.tar.gz` & `tmp/which_plates-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "which_plates-0.7.0.tar", max compression
+gzip compressed data, was "which_plates-0.8.0.tar", max compression
```

## Comparing `which_plates-0.7.0.tar` & `which_plates-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    18047 2023-04-30 22:20:01.823939 which_plates-0.7.0/LICENSE
--rw-r--r--   0        0        0     1112 2023-04-30 22:20:01.823939 which_plates-0.7.0/README.md
--rw-r--r--   0        0        0     2087 2023-04-30 22:20:01.823939 which_plates-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-30 22:20:01.823939 which_plates-0.7.0/src/which_plates/__init__.py
--rw-r--r--   0        0        0     1634 2023-04-30 22:20:01.823939 which_plates-0.7.0/src/which_plates/functions.py
--rw-r--r--   0        0        0     1759 2023-04-30 22:20:01.823939 which_plates-0.7.0/src/which_plates/main.py
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 which_plates-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    18047 2023-05-01 00:56:11.773947 which_plates-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1112 2023-05-01 00:56:11.773947 which_plates-0.8.0/README.md
+-rw-r--r--   0        0        0     2087 2023-05-01 00:56:11.773947 which_plates-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-05-01 00:56:11.773947 which_plates-0.8.0/src/which_plates/__init__.py
+-rw-r--r--   0        0        0     1637 2023-05-01 00:56:11.773947 which_plates-0.8.0/src/which_plates/functions.py
+-rw-r--r--   0        0        0     1759 2023-05-01 00:56:11.773947 which_plates-0.8.0/src/which_plates/main.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 which_plates-0.8.0/PKG-INFO
```

### Comparing `which_plates-0.7.0/LICENSE` & `which_plates-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `which_plates-0.7.0/README.md` & `which_plates-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `which_plates-0.7.0/pyproject.toml` & `which_plates-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "which_plates"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["Ian Day <ian@ianday.me>"]
 readme = "README.md"
 #packages = [{include = "which_plates"}]
 homepage = "https://github.com/iandday/whichPlates"
 repository = "https://github.com/iandday/whichPlates"
 license = "GNUv2"
```

### Comparing `which_plates-0.7.0/src/which_plates/functions.py` & `which_plates-0.8.0/src/which_plates/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     remaining_weight = Decimal(round_num(weight))
     available_plates.sort(reverse=True)
 
     for plate in available_plates:
         # at least two plates left in remaining weight
         if remaining_weight / Decimal(plate) >= Decimal(2):
             # can only use even number of plates
-            if ((remaining_weight / Decimal(plate)) % 2) == 0:
+            if (int(remaining_weight / Decimal(plate)) % 2) == 0:
                 plate_count = int(Decimal(remaining_weight) // Decimal(plate))
             else:
                 plate_count = int(Decimal(remaining_weight) // Decimal(plate)) - 1
             plates[plate] = plate_count
 
             remaining_weight -= Decimal(plate) * Decimal(plates[plate])
```

### Comparing `which_plates-0.7.0/src/which_plates/main.py` & `which_plates-0.8.0/src/which_plates/main.py`

 * *Files identical despite different names*

### Comparing `which_plates-0.7.0/PKG-INFO` & `which_plates-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: which-plates
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Home-page: https://github.com/iandday/whichPlates
 License: GNUv2
 Author: Ian Day
 Author-email: ian@ianday.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

