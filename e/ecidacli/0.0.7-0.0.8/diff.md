# Comparing `tmp/ecidacli-0.0.7.tar.gz` & `tmp/ecidacli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecidacli-0.0.7.tar", last modified: Mon May  1 08:40:35 2023, max compression
+gzip compressed data, was "ecidacli-0.0.8.tar", last modified: Mon May  1 08:44:27 2023, max compression
```

## Comparing `ecidacli-0.0.7.tar` & `ecidacli-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:40:35.485450 ecidacli-0.0.7/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:40:35.485450 ecidacli-0.0.7/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.7/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:40:35.481450 ecidacli-0.0.7/ecidacli.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/entry_points.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-05-01 08:40:35.000000 ecidacli-0.0.7/ecidacli.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     3583 2023-05-01 08:27:50.000000 ecidacli-0.0.7/ecidacli.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-01 08:40:35.485450 ecidacli-0.0.7/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-05-01 08:40:30.000000 ecidacli-0.0.7/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:44:27.288248 ecidacli-0.0.8/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:44:27.288248 ecidacli-0.0.8/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       66 2023-03-09 16:23:50.000000 ecidacli-0.0.8/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-01 08:44:27.288248 ecidacli-0.0.8/ecidacli.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      455 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      224 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       43 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/entry_points.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       26 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        9 2023-05-01 08:44:27.000000 ecidacli-0.0.8/ecidacli.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     3580 2023-05-01 08:44:16.000000 ecidacli-0.0.8/ecidacli.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-01 08:44:27.288248 ecidacli-0.0.8/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      809 2023-05-01 08:44:24.000000 ecidacli-0.0.8/setup.py
```

### Comparing `ecidacli-0.0.7/ecidacli.py` & `ecidacli-0.0.8/ecidacli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # Define the Dockerfile commands
     dockerfile = []
     dockerfile.append(f"FROM {base_image}")
     dockerfile.append(f"WORKDIR {workdir}")
     dockerfile.append("COPY requirements.txt .")
     dockerfile.append("RUN pip install --no-cache-dir -r requirements.txt")
     dockerfile.append("COPY . .")
-    dockerfile.append(f"CMD [\"python\", \"{mainfile}.py\"]")
+    dockerfile.append(f"CMD [\"python\", \"{mainfile}\"]")
 
     # Write the Dockerfile to disk
     with open("Dockerfile", "w") as f:
         f.write("\n".join(dockerfile))
 
     # Build the Docker image
```

### Comparing `ecidacli-0.0.7/setup.py` & `ecidacli-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecidacli',
-   version='0.0.7',
+   version='0.0.8',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-CLI for python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    classifiers=[
```

