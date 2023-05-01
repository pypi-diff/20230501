# Comparing `tmp/numerizer-0.2.2.tar.gz` & `tmp/numerizer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerizer-0.2.2.tar", last modified: Tue Jan  3 08:05:37 2023, max compression
+gzip compressed data, was "numerizer-0.2.3.tar", last modified: Mon May  1 07:53:44 2023, max compression
```

## Comparing `numerizer-0.2.2.tar` & `numerizer-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-01-03 08:05:37.030810 numerizer-0.2.2/
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     1203 2021-10-26 09:22:40.000000 numerizer-0.2.2/.gitignore
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)      510 2023-01-03 08:01:52.000000 numerizer-0.2.2/.travis.yml
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     1073 2021-10-26 09:22:40.000000 numerizer-0.2.2/LICENSE
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2992 2023-01-03 08:05:37.030810 numerizer-0.2.2/PKG-INFO
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2640 2023-01-03 08:01:52.000000 numerizer-0.2.2/README.rst
-drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-01-03 08:05:37.030810 numerizer-0.2.2/numerizer/
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)       62 2021-10-26 09:22:40.000000 numerizer-0.2.2/numerizer/__init__.py
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2321 2021-10-26 09:22:40.000000 numerizer-0.2.2/numerizer/consts.py
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)    11459 2023-01-03 08:01:52.000000 numerizer-0.2.2/numerizer/numerizer.py
-drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-01-03 08:05:37.030810 numerizer-0.2.2/numerizer.egg-info/
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2992 2023-01-03 08:05:36.000000 numerizer-0.2.2/numerizer.egg-info/PKG-INFO
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)      274 2023-01-03 08:05:36.000000 numerizer-0.2.2/numerizer.egg-info/SOURCES.txt
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)        1 2023-01-03 08:05:36.000000 numerizer-0.2.2/numerizer.egg-info/dependency_links.txt
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)       10 2023-01-03 08:05:36.000000 numerizer-0.2.2/numerizer.egg-info/top_level.txt
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)      242 2023-01-03 08:05:37.030810 numerizer-0.2.2/setup.cfg
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     1135 2023-01-03 08:01:52.000000 numerizer-0.2.2/setup.py
--rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)    10160 2023-01-03 08:01:52.000000 numerizer-0.2.2/test_numerize.py
+drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-05-01 07:53:44.191919 numerizer-0.2.3/
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     1073 2021-10-26 09:22:40.000000 numerizer-0.2.3/LICENSE
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2992 2023-05-01 07:53:44.191919 numerizer-0.2.3/PKG-INFO
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2640 2023-01-03 08:01:52.000000 numerizer-0.2.3/README.rst
+drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-05-01 07:53:44.191919 numerizer-0.2.3/numerizer/
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)       62 2021-10-26 09:22:40.000000 numerizer-0.2.3/numerizer/__init__.py
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2321 2021-10-26 09:22:40.000000 numerizer-0.2.3/numerizer/consts.py
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)    11915 2023-05-01 07:49:27.000000 numerizer-0.2.3/numerizer/numerizer.py
+drwxrwxr-x   0 jaidevd   (1000) jaidevd   (1000)        0 2023-05-01 07:53:44.191919 numerizer-0.2.3/numerizer.egg-info/
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     2992 2023-05-01 07:53:44.000000 numerizer-0.2.3/numerizer.egg-info/PKG-INFO
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)      234 2023-05-01 07:53:44.000000 numerizer-0.2.3/numerizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)        1 2023-05-01 07:53:44.000000 numerizer-0.2.3/numerizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)       10 2023-05-01 07:53:44.000000 numerizer-0.2.3/numerizer.egg-info/top_level.txt
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)      242 2023-05-01 07:53:44.191919 numerizer-0.2.3/setup.cfg
+-rw-rw-r--   0 jaidevd   (1000) jaidevd   (1000)     1135 2023-05-01 07:49:48.000000 numerizer-0.2.3/setup.py
```

### Comparing `numerizer-0.2.2/LICENSE` & `numerizer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `numerizer-0.2.2/PKG-INFO` & `numerizer-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerizer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python module for converting natural language numbers into ints and floats.
 Home-page: https://github.com/jaidevd/numerizer
 Download-URL: https://pypi.org/project/numerizer/#files
 Maintainer: Jaidev Deshpande
 Maintainer-email: deshpande.jaidev@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `numerizer-0.2.2/README.rst` & `numerizer-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `numerizer-0.2.2/numerizer/consts.py` & `numerizer-0.2.3/numerizer/consts.py`

 * *Files identical despite different names*

### Comparing `numerizer-0.2.2/numerizer/numerizer.py` & `numerizer-0.2.3/numerizer/numerizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -235,23 +235,33 @@
     s = re.sub(r'<num>', '', s)
     return s
 
 
 def andition(s):
     pat = re.compile(r'<num>(\d+)( | and )<num>(\d+)(?=[^\w]|$)', flags=re.IGNORECASE)
     while True:
-        m = re.search(pat, s)
-        if m is not None:
-            if (m.group(2) == 'and') or (len(m.group(1)) > len(m.group(3))):
-                s = re.sub(pat, lambda m: '<num>' + str(int(m.group(1)) + int(m.group(3))),
-                           s, count=1)
-            else:
-                break
+        matches = list(re.finditer(pat, s))
 
-        else:
+        # If there are no matches found, break out of the loop
+        if len(matches) == 0:
+            break
+
+        substitutions = 0
+        # Iterate through matches in reverse order
+        for match in reversed(matches):
+            # Check if the numbers should be unified
+            if (match.group(2) == 'and') or (len(match.group(1)) > len(match.group(3))):
+                # Replace the matched part with the unified number
+                s = s[:match.start()] + '<num>'\
+                    + str(int(match.group(1)) +
+                          int(match.group(3))) + s[match.end():]
+                substitutions += 1
+
+        # If there were no substitutions, break out of the loop
+        if not substitutions:
             break
     return s
 
 
 def cleanup_fractions(s):
     #  evaludate  fractions when preceded by another number
     pat = re.compile(r'(\d+)(?: | and |-)+(<num>|\s)*(\d+)\s*\/\s*(\d+)',
```

### Comparing `numerizer-0.2.2/numerizer.egg-info/PKG-INFO` & `numerizer-0.2.3/numerizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerizer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python module for converting natural language numbers into ints and floats.
 Home-page: https://github.com/jaidevd/numerizer
 Download-URL: https://pypi.org/project/numerizer/#files
 Maintainer: Jaidev Deshpande
 Maintainer-email: deshpande.jaidev@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `numerizer-0.2.2/setup.py` & `numerizer-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 DOWNLOAD_URL = 'https://pypi.org/project/numerizer/#files'
 LICENSE = 'MIT'
 PROJECT_URLS = {
     'Bug Tracker': 'https://github.com/jaidevd/numerizer/issues',
     'Documentation': 'https://github.com/jaidevd/numerizer/tree/master/README.rst',
     'Source Code': 'https://github.com/jaidevd/numerizer'
 }
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # Requirements
 install_requires = []
 
 # Setup
 setup(
     name=NAME,
```

