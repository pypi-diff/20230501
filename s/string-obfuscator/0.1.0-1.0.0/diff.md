# Comparing `tmp/string-obfuscator-0.1.0.tar.gz` & `tmp/string-obfuscator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string-obfuscator-0.1.0.tar", last modified: Mon May 16 15:22:20 2022, max compression
+gzip compressed data, was "string-obfuscator-1.0.0.tar", last modified: Sun Apr 30 23:37:40 2023, max compression
```

## Comparing `string-obfuscator-0.1.0.tar` & `string-obfuscator-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-05-16 15:22:20.484443 string-obfuscator-0.1.0/
--rw-rw-rw-   0        0        0     1098 2022-05-13 22:15:26.000000 string-obfuscator-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1384 2022-05-16 15:22:20.484443 string-obfuscator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      793 2022-05-16 13:36:48.000000 string-obfuscator-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2022-05-13 22:13:12.000000 string-obfuscator-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      728 2022-05-16 15:22:20.485452 string-obfuscator-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-16 15:22:20.462443 string-obfuscator-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-05-16 15:22:20.478443 string-obfuscator-0.1.0/src/string_obfuscator/
--rw-rw-rw-   0        0        0        0 2022-05-13 21:44:19.000000 string-obfuscator-0.1.0/src/string_obfuscator/__init__.py
--rw-rw-rw-   0        0        0     1942 2022-05-16 15:21:22.000000 string-obfuscator-0.1.0/src/string_obfuscator/obfuscate.py
-drwxrwxrwx   0        0        0        0 2022-05-16 15:22:20.483443 string-obfuscator-0.1.0/src/string_obfuscator.egg-info/
--rw-rw-rw-   0        0        0     1384 2022-05-16 15:22:20.000000 string-obfuscator-0.1.0/src/string_obfuscator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2022-05-16 15:22:20.000000 string-obfuscator-0.1.0/src/string_obfuscator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-16 15:22:20.000000 string-obfuscator-0.1.0/src/string_obfuscator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-05-16 15:22:20.000000 string-obfuscator-0.1.0/src/string_obfuscator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 23:37:40.137900 string-obfuscator-1.0.0/
+-rw-rw-rw-   0        0        0     1098 2022-05-13 22:15:26.000000 string-obfuscator-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1715 2023-04-30 23:37:40.137900 string-obfuscator-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1124 2023-04-30 23:17:21.000000 string-obfuscator-1.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-05-13 22:13:12.000000 string-obfuscator-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2023-04-30 23:37:40.138866 string-obfuscator-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 23:37:40.121725 string-obfuscator-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 23:37:40.129726 string-obfuscator-1.0.0/src/string_obfuscator/
+-rw-rw-rw-   0        0        0        0 2022-05-13 21:44:19.000000 string-obfuscator-1.0.0/src/string_obfuscator/__init__.py
+-rw-rw-rw-   0        0        0     3442 2023-04-30 23:25:29.000000 string-obfuscator-1.0.0/src/string_obfuscator/obfuscate.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:37:40.133725 string-obfuscator-1.0.0/src/string_obfuscator.egg-info/
+-rw-rw-rw-   0        0        0     1715 2023-04-30 23:37:40.000000 string-obfuscator-1.0.0/src/string_obfuscator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-30 23:37:40.000000 string-obfuscator-1.0.0/src/string_obfuscator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 23:37:40.000000 string-obfuscator-1.0.0/src/string_obfuscator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-30 23:37:40.000000 string-obfuscator-1.0.0/src/string_obfuscator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 23:37:40.136866 string-obfuscator-1.0.0/tests/
+-rw-rw-rw-   0        0        0    10102 2023-04-30 23:23:34.000000 string-obfuscator-1.0.0/tests/test_obfuscate.py
```

### Comparing `string-obfuscator-0.1.0/LICENSE` & `string-obfuscator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `string-obfuscator-0.1.0/README.md` & `string-obfuscator-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,12 +7,17 @@
 This module obfuscates strings, integers, list items.
 
 ## How to use
 This module was developed with easy-of-use in mind, so it's pretty straightforward:
 
 Step-by-step guide:
 + `from string_obfuscator.obfuscate import obfuscate`
-+ Dict can be obfuscated by calling: `obfuscate(dict_to_obfuscate, list_with_keys_to_obfuscate)`
-+ Enum can also be passed as an optional parameter: `obfuscate(dict_to_obfuscate, [], enum_with_keys_to_obfuscate)`
++ Dict can be obfuscated by calling: `obfuscate(dict_to_obfuscate, fields=list_with_keys_to_obfuscate)`
+
+The `fields` argument can be a list, an enum, a string or 0.
+
+If the argument provided is 0 and payload is str (Eg. document number), obfuscate returns obfuscated payload(str).
+If the argument provided is of type string, only the existing dict items with keys matching the string will be obfuscated.
+If the argument provided is of type list or enum, all the fields with corresponding keys in the dict_to_obfuscate will be obfuscated.
 
 ## Python version
 This module was tested in Python 3.7, 3.8.5, 3.9
```

### Comparing `string-obfuscator-0.1.0/setup.cfg` & `string-obfuscator-1.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 696e 672d 6f62 6675 7363   = string-obfusc
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 302e 312e 300d 0a61 7574 686f 7220 3d20  0.1.0..author = 
+00000030: 312e 302e 300d 0a61 7574 686f 7220 3d20  1.0.0..author = 
 00000040: 4564 7561 7264 6f20 4c6f 6469 204d 6172  Eduardo Lodi Mar
 00000050: 7a61 6e6f 0d0a 6175 7468 6f72 5f65 6d61  zano..author_ema
 00000060: 696c 203d 206c 6f64 6930 3031 4075 6f6c  il = lodi001@uol
 00000070: 2e63 6f6d 2e62 720d 0a64 6573 6372 6970  .com.br..descrip
 00000080: 7469 6f6e 203d 2041 2073 696d 706c 6520  tion = A simple 
 00000090: 7374 7269 6e67 206f 6266 7573 6361 746f  string obfuscato
 000000a0: 7220 666f 7220 6f62 6675 7363 6174 696e  r for obfuscatin
```

