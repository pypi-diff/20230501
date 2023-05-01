# Comparing `tmp/flake8_linenumber-0.1.7.tar.gz` & `tmp/flake8_linenumber-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_linenumber-0.1.7.tar", last modified: Mon Feb 10 16:26:41 2020, max compression
+gzip compressed data, was "dist/flake8_linenumber-0.1.8.tar", last modified: Wed Feb 12 10:04:41 2020, max compression
```

## Comparing `flake8_linenumber-0.1.7.tar` & `flake8_linenumber-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 brabadu    (501) staff       (20)        0 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/
--rw-r--r--   0 brabadu    (501) staff       (20)     1330 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/PKG-INFO
--rw-r--r--   0 brabadu    (501) staff       (20)      412 2020-02-10 09:12:11.000000 flake8_linenumber-0.1.7/README.md
-drwxr-xr-x   0 brabadu    (501) staff       (20)        0 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/
--rw-r--r--   0 brabadu    (501) staff       (20)     1330 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/PKG-INFO
--rw-r--r--   0 brabadu    (501) staff       (20)      287 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/SOURCES.txt
--rw-r--r--   0 brabadu    (501) staff       (20)        1 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/dependency_links.txt
--rw-r--r--   0 brabadu    (501) staff       (20)       62 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/entry_points.txt
--rw-r--r--   0 brabadu    (501) staff       (20)       13 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/requires.txt
--rw-r--r--   0 brabadu    (501) staff       (20)       18 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/flake8_linenumber.egg-info/top_level.txt
--rw-r--r--   0 brabadu    (501) staff       (20)     1872 2020-02-10 16:25:20.000000 flake8_linenumber-0.1.7/flake8_linenumber.py
--rw-r--r--   0 brabadu    (501) staff       (20)       38 2020-02-10 16:26:41.000000 flake8_linenumber-0.1.7/setup.cfg
--rw-r--r--   0 brabadu    (501) staff       (20)     1093 2020-02-10 16:20:36.000000 flake8_linenumber-0.1.7/setup.py
+drwxr-xr-x   0 brabadu    (501) staff       (20)        0 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/
+-rw-r--r--   0 brabadu    (501) staff       (20)     1330 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/PKG-INFO
+-rw-r--r--   0 brabadu    (501) staff       (20)      412 2020-02-10 09:12:11.000000 flake8_linenumber-0.1.8/README.md
+drwxr-xr-x   0 brabadu    (501) staff       (20)        0 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/
+-rw-r--r--   0 brabadu    (501) staff       (20)     1330 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/PKG-INFO
+-rw-r--r--   0 brabadu    (501) staff       (20)      287 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/SOURCES.txt
+-rw-r--r--   0 brabadu    (501) staff       (20)        1 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/dependency_links.txt
+-rw-r--r--   0 brabadu    (501) staff       (20)       62 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/entry_points.txt
+-rw-r--r--   0 brabadu    (501) staff       (20)       13 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/requires.txt
+-rw-r--r--   0 brabadu    (501) staff       (20)       18 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/flake8_linenumber.egg-info/top_level.txt
+-rw-r--r--   0 brabadu    (501) staff       (20)     2169 2020-02-12 10:03:21.000000 flake8_linenumber-0.1.8/flake8_linenumber.py
+-rw-r--r--   0 brabadu    (501) staff       (20)       38 2020-02-12 10:04:41.000000 flake8_linenumber-0.1.8/setup.cfg
+-rw-r--r--   0 brabadu    (501) staff       (20)     1093 2020-02-12 10:03:27.000000 flake8_linenumber-0.1.8/setup.py
```

### Comparing `flake8_linenumber-0.1.7/PKG-INFO` & `flake8_linenumber-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_linenumber
-Version: 0.1.7
+Version: 0.1.8
 Summary: flake8 plugin to limit line number in a module
 Home-page: https://github.com/brabadu/flake8-linenumber
 Author: Boryslav Larin
 Author-email: brabadu@gmail.com
 License: MIT
 Description: flake8-linenumber
         =================
```

### Comparing `flake8_linenumber-0.1.7/flake8_linenumber.egg-info/PKG-INFO` & `flake8_linenumber-0.1.8/flake8_linenumber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-linenumber
-Version: 0.1.7
+Version: 0.1.8
 Summary: flake8 plugin to limit line number in a module
 Home-page: https://github.com/brabadu/flake8-linenumber
 Author: Boryslav Larin
 Author-email: brabadu@gmail.com
 License: MIT
 Description: flake8-linenumber
         =================
```

### Comparing `flake8_linenumber-0.1.7/flake8_linenumber.py` & `flake8_linenumber-0.1.8/flake8_linenumber.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,43 +9,51 @@
 def config_parser(linenumber_config):
     size_pairs = map(lambda s: s.split('='), linenumber_config)
     return {Path(filename): int(size) for filename, size in size_pairs}
 
 
 class LineNumberPlugin:
     name = __name__
-    version = '0.1.7'
+    version = '0.1.8'
 
     def __init__(self, tree, total_lines, filename):
         self.total_lines = total_lines
         self.filename = Path(filename)
         self.last_changed_lines = {
             Path(f): max(changed_lines)
             for f, changed_lines in parse_unified_diff().items()
             if changed_lines
         }
 
     @classmethod
     def add_options(cls, options_manager):
         options_manager.add_option(
+            '--max-linenumber',
+            type='int',
+            default=None,
+            parse_from_config=True,
+            help='Default max line limit for a python module'
+        )
+        options_manager.add_option(
             '--linenumber',
             type='str',
             comma_separated_list=True,
             default=[],
             parse_from_config=True,
             help='List of modules and their max line nums'
         )
 
     @classmethod
     def parse_options(cls, options):
         cls.filesizes = config_parser(options.linenumber)
         cls.diff = options.diff
+        cls.default_limit = options.max_linenumber
 
     def run(self):
-        filesize_limit = self.filesizes.get(self.filename)
+        filesize_limit = self.filesizes.get(self.filename, self.default_limit)
 
         if filesize_limit and self.total_lines > filesize_limit:
             message = LineNumberErrors.L001.value.format(
                 limit=filesize_limit,
                 total_lines=self.total_lines
             )
```

### Comparing `flake8_linenumber-0.1.7/setup.py` & `flake8_linenumber-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flake8_linenumber",
     license="MIT",
-    version="0.1.7",
+    version="0.1.8",
     description="flake8 plugin to limit line number in a module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Boryslav Larin",
     author_email="brabadu@gmail.com",
     url="https://github.com/brabadu/flake8-linenumber",
     py_modules=['flake8_linenumber'],
```

