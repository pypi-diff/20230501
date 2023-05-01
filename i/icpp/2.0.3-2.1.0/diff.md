# Comparing `tmp/icpp-2.0.3-py3-none-any.whl.zip` & `tmp/icpp-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3088 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      322 b- defN 23-Apr-29 23:12 icpp/__init__.py
--rw-rw-r--  2.0 unx      816 b- defN 23-Apr-29 23:02 icpp/__main__.py
--rw-rw-r--  2.0 unx       98 b- defN 23-Apr-29 23:08 icpp/py.typed
--rw-rw-r--  2.0 unx      322 b- defN 23-Apr-29 23:15 icpp/version.py
--rw-rw-r--  2.0 unx     1116 b- defN 23-Apr-29 23:15 icpp-2.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-29 23:15 icpp-2.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Apr-29 23:15 icpp-2.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Apr-29 23:15 icpp-2.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      660 b- defN 23-Apr-29 23:15 icpp-2.0.3.dist-info/RECORD
-9 files, 3475 bytes uncompressed, 1956 bytes compressed:  43.7%
+Zip file size: 3104 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      322 b- defN 23-Apr-29 23:19 icpp/__init__.py
+-rw-rw-r--  2.0 unx      825 b- defN 23-May-01 20:05 icpp/__main__.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-29 23:19 icpp/py.typed
+-rw-rw-r--  2.0 unx      322 b- defN 23-May-01 19:58 icpp/version.py
+-rw-rw-r--  2.0 unx     1079 b- defN 23-May-01 20:05 icpp-2.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-01 20:05 icpp-2.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-May-01 20:05 icpp-2.1.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-May-01 20:05 icpp-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      660 b- defN 23-May-01 20:05 icpp-2.1.0.dist-info/RECORD
+9 files, 3447 bytes uncompressed, 1972 bytes compressed:  42.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: icpp/py.typed
 Comment: 
 
 Filename: icpp/version.py
 Comment: 
 
-Filename: icpp-2.0.3.dist-info/METADATA
+Filename: icpp-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: icpp-2.0.3.dist-info/WHEEL
+Filename: icpp-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: icpp-2.0.3.dist-info/entry_points.txt
+Filename: icpp-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: icpp-2.0.3.dist-info/top_level.txt
+Filename: icpp-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: icpp-2.0.3.dist-info/RECORD
+Filename: icpp-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## icpp/__main__.py

```diff
@@ -10,16 +10,17 @@
 """
 count = 0
 def main() -> None:
     """Entry point of program"""
     global count
     if count==0:
         print("")
-        print("The package `icpp` has been replaced by `icpp-free` (https://pypi.org/project/icpp-free/)")
-        print("Install it with: pip install icpp-free")
+        print("You installed the package `icpp` from PyPI")
+        print("This has been replaced by icpp-pro.")
+        print("For details, see: htpps://docs.icpp.world")
         print("")
         count = count+1
 
 
 #
 # Always start it up or debug as a module:
 #  python -m icpp.__main__
```

## icpp/version.py

```diff
@@ -5,8 +5,8 @@
 (-) do not add anything but the version number here!
 
 We do it this way, so both __init__.py and setup.py can use it.
 
 see:
 https://packaging.python.org/guides/single-sourcing-package-version/
 """
-__version__ = "2.0.3"
+__version__ = "2.1.0"
```

## Comparing `icpp-2.0.3.dist-info/METADATA` & `icpp-2.1.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp
-Version: 2.0.3
+Version: 2.1.0
 Summary: `icpp` had been replaced by `icpp-free`
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: Freemium
 Keywords: Internet Computer,C++,Smart Contracts,blockchain
 Classifier: Development Status :: 4 - Beta
@@ -22,8 +22,8 @@
 Requires-Dist: pylint (==2.13.9) ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: mkdocs ; extra == 'dev'
 Requires-Dist: types-requests ; extra == 'dev'
 
-# The icpp package has been replaced by [icpp-free](https://pypi.org/project/icpp-free/)
+# Replaced by [icpp-pro](https://docs.icpp.world) !
```

