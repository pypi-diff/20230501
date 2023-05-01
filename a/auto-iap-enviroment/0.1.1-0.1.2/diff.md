# Comparing `tmp/auto-iap-enviroment-0.1.1.tar.gz` & `tmp/auto-iap-enviroment-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-iap-enviroment-0.1.1.tar", last modified: Sun Apr 30 22:06:13 2023, max compression
+gzip compressed data, was "auto-iap-enviroment-0.1.2.tar", last modified: Mon May  1 15:05:37 2023, max compression
```

## Comparing `auto-iap-enviroment-0.1.1.tar` & `auto-iap-enviroment-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/
--rw-rw-r--   0 luis      (1000) luis      (1000)      522 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)        5 2023-04-29 20:37:50.000000 auto-iap-enviroment-0.1.1/README.md
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)      522 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      344 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       71 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/entry_points.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        7 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        4 2023-04-30 22:06:13.000000 auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/top_level.txt
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/iap/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1056 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/helpers.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      471 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/iaApi.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      508 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.1/iap/main.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     1168 2023-04-30 22:01:54.000000 auto-iap-enviroment-0.1.1/iap/scrapeMe.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-04-30 22:06:13.880209 auto-iap-enviroment-0.1.1/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      880 2023-04-30 22:05:20.000000 auto-iap-enviroment-0.1.1/setup.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-01 15:05:37.804587 auto-iap-enviroment-0.1.2/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      524 2023-05-01 15:05:37.804587 auto-iap-enviroment-0.1.2/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-05-01 02:50:43.000000 auto-iap-enviroment-0.1.2/README.md
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-01 15:05:37.788587 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      524 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)      344 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)       71 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/entry_points.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        7 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        4 2023-05-01 15:05:37.000000 auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/top_level.txt
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-01 15:05:37.804587 auto-iap-enviroment-0.1.2/iap/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1056 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.2/iap/helpers.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      471 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.2/iap/iaApi.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      508 2023-04-30 22:01:53.000000 auto-iap-enviroment-0.1.2/iap/main.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1233 2023-04-30 23:23:40.000000 auto-iap-enviroment-0.1.2/iap/scrapeMe.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-01 15:05:37.804587 auto-iap-enviroment-0.1.2/setup.cfg
+-rw-rw-r--   0 luis      (1000) luis      (1000)      880 2023-05-01 15:05:09.000000 auto-iap-enviroment-0.1.2/setup.py
```

### Comparing `auto-iap-enviroment-0.1.1/PKG-INFO` & `auto-iap-enviroment-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: auto-iap-enviroment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Um pacote que integra o OpenAI GPT ao seu computados
 Home-page: https://github.com/seu-usuario/meu-pacote
 Author: Luis Arthur Rodrigues da Silva
 Author-email: luisarthurlards03@gmail.com
 License: UNKNOWN
-Description: # IAp
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `auto-iap-enviroment-0.1.1/auto_iap_enviroment.egg-info/PKG-INFO` & `auto-iap-enviroment-0.1.2/auto_iap_enviroment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: auto-iap-enviroment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Um pacote que integra o OpenAI GPT ao seu computados
 Home-page: https://github.com/seu-usuario/meu-pacote
 Author: Luis Arthur Rodrigues da Silva
 Author-email: luisarthurlards03@gmail.com
 License: UNKNOWN
-Description: # IAp
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `auto-iap-enviroment-0.1.1/iap/helpers.py` & `auto-iap-enviroment-0.1.2/iap/helpers.py`

 * *Files identical despite different names*

### Comparing `auto-iap-enviroment-0.1.1/iap/scrapeMe.py` & `auto-iap-enviroment-0.1.2/iap/scrapeMe.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from .helpers import getArg
 
 curr_path = os.getcwd()
 initial_text = "chat gpt, saiba que:\n"
 
 def scrap_sistem():
     extension = getArg(1,'a.py').split('.')[-1]
-
-    print(extension)
     messages = [{"role": "system", "content": initial_text}]
     files_info_text = ""
     for dirpath, dirnames, filenames in os.walk(curr_path):
         for filename in filenames:
-            if filename.endswith(f".{extension}") or filename.endswith(getArg(2,'breakit')):
+            if  filename.endswith(getArg(2,f".{extension}")):
+                path_name= f"{'/'.join(dirpath.split('/')[-2:])}/{filename}"
+                print(path_name, 'lido')
                 file_path = os.path.join(dirpath, filename)
                 try:
                     with open(file_path, "r") as arquivo:
                         conteudo = arquivo.read()
                         curr_text = f"""
 ```python
-O arquivo {file_path} contém:
+O arquivo {path_name} contém:
 
 {conteudo}
 ```
 
 """
                         messages.append(
                             {"role": "user", "content": curr_text},
```

### Comparing `auto-iap-enviroment-0.1.1/setup.py` & `auto-iap-enviroment-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="auto-iap-enviroment",
-    version="0.1.1",
+    version="0.1.2",
     author="Luis Arthur Rodrigues da Silva",
     author_email="luisarthurlards03@gmail.com",
     description="Um pacote que integra o OpenAI GPT ao seu computados",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seu-usuario/meu-pacote",
     packages=['iap'],
```

