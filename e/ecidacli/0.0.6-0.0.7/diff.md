# Comparing `tmp/ecidacli-0.0.6.tar.gz` & `tmp/ecidacli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecidacli-0.0.6.tar", last modified: Sat Mar 11 11:57:26 2023, max compression
+gzip compressed data, was "ecidacli-0.0.7.tar", last modified: Mon May  1 08:40:35 2023, max compression
```

## Comparing `ecidacli-0.0.6.tar` & `ecidacli-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-03-11 11:57:26.637649 ecidacli-0.0.6/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-03-11 11:57:26.637649 ecidacli-0.0.6/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.6/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-03-11 11:57:26.637649 ecidacli-0.0.6/ecidacli.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/entry_points.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-03-11 11:57:26.000000 ecidacli-0.0.6/ecidacli.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     3494 2023-03-11 11:55:17.000000 ecidacli-0.0.6/ecidacli.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-03-11 11:57:26.637649 ecidacli-0.0.6/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-03-11 11:55:51.000000 ecidacli-0.0.6/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:40:35.485450 ecidacli-0.0.7/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:40:35.485450 ecidacli-0.0.7/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.7/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:40:35.481450 ecidacli-0.0.7/ecidacli.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/entry_points.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     3583 2023-05-01 08:27:50.000000 ecidacli-0.0.7/ecidacli.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-01 08:40:35.485450 ecidacli-0.0.7/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-05-01 08:40:30.000000 ecidacli-0.0.7/setup.py
```

### Comparing `ecidacli-0.0.6/ecidacli.py` & `ecidacli-0.0.7/ecidacli.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,31 +79,32 @@
     parser.add_argument("-u", "--username", help="Username for Dockerhub authentication")
     parser.add_argument("-f", "--main-file", help="Main file to process (example: main.py)")
 
     # Parse the command line arguments
     args = parser.parse_args()
     mainfilepath = args.main_file
     
-    module_name = mainfilepath[:-3]
-    module_name = module_name.replace("/", ".")
-    module_name = module_name.lstrip('.')
+    python_module_path = mainfilepath[:-3]
+    python_module_path = python_module_path.replace("/", ".")
+    python_module_path = python_module_path.lstrip('.')
     
     username = args.username
     
     # Import the module dynamically
     try:
-        module = importlib.import_module(module_name)
+        module = importlib.import_module(python_module_path)
         M = module.create_module()
         
         imageTag = username + "/" + M.name + ":" + M.version
         apply_yaml(M, imageTag)
         
         dirname = os.path.dirname(mainfilepath)
         os.chdir(dirname)
-        create_deploy_docker_image(imageTag, module_name)
+        mainfile = os.path.basename(mainfilepath)
+        create_deploy_docker_image(imageTag, mainfile)
         
         print(f"{mainfilepath} processed successfully")
         
     except Exception as e:
         print(e)
         # print(f"{mainfile} does not contain an EcidaModule")
```

### Comparing `ecidacli-0.0.6/setup.py` & `ecidacli-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecidacli',
-   version='0.0.6',
+   version='0.0.7',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-CLI for python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    classifiers=[
```

