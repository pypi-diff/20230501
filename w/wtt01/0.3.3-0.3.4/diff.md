# Comparing `tmp/wtt01-0.3.3.tar.gz` & `tmp/wtt01-0.3.4.tar.gz`

## Comparing `wtt01-0.3.3.tar` & `wtt01-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.3/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.3/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/_env.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/cli.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 wtt01-0.3.3/wtt01/main.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.3/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 wtt01-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wtt01-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.4/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.4/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.4/wtt01/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.4/wtt01/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.4/wtt01/_env.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.4/wtt01/cli.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 wtt01-0.3.4/wtt01/main.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.4/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 wtt01-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wtt01-0.3.4/PKG-INFO
```

### Comparing `wtt01-0.3.3/tests/test_load.py` & `wtt01-0.3.4/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.3/wtt01/cli.py` & `wtt01-0.3.4/wtt01/cli.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.3/wtt01/main.py` & `wtt01-0.3.4/wtt01/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,29 +114,30 @@
                 )
 
             filename = f"{name}.duckdb_extension.gz"
             url = f"https://dbe.wheretrue.com/{name}/{version}/v0.7.1/{duckdb_arch}/{filename}"
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir_path = Path(temp_dir)
+
                 temp_file_name = temp_dir_path / filename
 
                 try:
                     urllib.request.urlretrieve(url, temp_file_name)
                 except Exception as retrieve_exp:
                     raise WTTException(
-                        f"Unable to download extension from {full_s3_path}"
+                        f"Unable to download extension from {url}"
                     ) from retrieve_exp
 
                 # ungzip the file
+                output_file = temp_dir_path / filename.rstrip(".gz")
                 with gzip.open(temp_file_name, "rb") as f_in:
-                    with open(temp_file_name, "wb") as f_out:
+                    with open(output_file, "wb") as f_out:
                         shutil.copyfileobj(f_in, f_out)
 
-                output_file = temp_dir_path / f"{name}.duckdb_extension"
                 if not output_file.exists():
                     raise WTTException(
                         f"Unable to find extension file at {output_file}"
                     ) from exp
 
                 con.install_extension(output_file.as_posix(), force_install=True)
                 con.load_extension(EXTENSION_NAME)
```

### Comparing `wtt01-0.3.3/.gitignore` & `wtt01-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.3/LICENSE.txt` & `wtt01-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.3/pyproject.toml` & `wtt01-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.3/PKG-INFO` & `wtt01-0.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt01
-Version: 0.3.3
+Version: 0.3.4
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

