# Comparing `tmp/feiticeiro_tec-1.1.3.tar.gz` & `tmp/feiticeiro_tec-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiticeiro_tec-1.1.3.tar", last modified: Mon May  1 03:28:34 2023, max compression
+gzip compressed data, was "feiticeiro_tec-1.1.4.tar", last modified: Mon May  1 03:31:37 2023, max compression
```

## Comparing `feiticeiro_tec-1.1.3.tar` & `feiticeiro_tec-1.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3332 2023-04-29 06:54:41.000000 feiticeiro_tec-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.699964 feiticeiro_tec-1.1.3/feiticeiro_tec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:10:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-29 05:32:12.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/api/
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-01 03:20:40.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 01:50:18.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-05-01 02:41:14.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/forms.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-05-01 03:04:05.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/api/v1/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-01 02:27:59.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/api/v1/usuario/
--rw-r--r--   0 root         (0) root         (0)      788 2023-05-01 03:06:36.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/api/v1/usuario/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/create/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/app.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-29 05:30:31.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/env.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/model.py
--rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/namespace.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-05-01 03:11:51.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/create/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/database/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-01 03:18:28.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-05-01 03:18:46.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/base.py
--rw-r--r--   0 root         (0) root         (0)      612 2023-05-01 03:16:32.000000 feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/usuario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:28:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-01 03:28:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 03:28:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-01 03:28:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-01 03:28:34.000000 feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 03:28:34.703964 feiticeiro_tec-1.1.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1063 2023-05-01 03:27:21.000000 feiticeiro_tec-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-04-29 06:54:41.000000 feiticeiro_tec-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:10:34.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-29 05:32:12.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/api/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-01 03:20:40.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 01:50:18.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-05-01 02:41:14.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-05-01 03:04:05.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/api/v1/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-01 02:27:59.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/api/v1/usuario/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-01 03:06:36.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/api/v1/usuario/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/create/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/app.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-29 05:30:31.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/env.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/model.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/namespace.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-05-01 03:11:51.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/create/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/database/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-01 03:18:28.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-05-01 03:18:46.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/base.py
+-rw-r--r--   0 root         (0) root         (0)      612 2023-05-01 03:16:32.000000 feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/usuario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:31:37.000000 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-01 03:31:37.000000 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 03:31:37.000000 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-01 03:31:37.000000 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2023-05-01 03:31:37.000000 feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 03:31:37.880671 feiticeiro_tec-1.1.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1063 2023-05-01 03:31:07.000000 feiticeiro_tec-1.1.4/setup.py
```

### Comparing `feiticeiro_tec-1.1.3/PKG-INFO` & `feiticeiro_tec-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiticeiro_tec
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
```

### Comparing `feiticeiro_tec-1.1.3/README.md` & `feiticeiro_tec-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/__main__.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/__main__.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/forms.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/forms.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/api/utils/serializers.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/api/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/api/v1/usuario/__init__.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/api/v1/usuario/__init__.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/create/namespace.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/create/namespace.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/create/server.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/create/server.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/base.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/base.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec/database/models/usuario.py` & `feiticeiro_tec-1.1.4/feiticeiro_tec/database/models/usuario.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/PKG-INFO` & `feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiticeiro-tec
-Version: 1.1.3
+Version: 1.1.4
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
```

### Comparing `feiticeiro_tec-1.1.3/feiticeiro_tec.egg-info/SOURCES.txt` & `feiticeiro_tec-1.1.4/feiticeiro_tec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.3/setup.py` & `feiticeiro_tec-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='feiticeiro_tec',
-    version='1.1.3',
+    version='1.1.4',
     url='https://github.com/feiticeiro-tec/feiticeiro-tec',
     license='BSD3',
     author='Silvio Henrique Cruz Da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silviohenriquecruzdasilva@gmail.com',
     keywords='Pacote',
```

