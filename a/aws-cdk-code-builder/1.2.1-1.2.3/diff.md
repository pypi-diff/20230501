# Comparing `tmp/aws-cdk-code-builder-1.2.1.tar.gz` & `tmp/aws-cdk-code-builder-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-code-builder-1.2.1.tar", last modified: Sat Nov 26 15:37:04 2022, max compression
+gzip compressed data, was "aws-cdk-code-builder-1.2.3.tar", last modified: Mon May  1 19:30:06 2023, max compression
```

## Comparing `aws-cdk-code-builder-1.2.1.tar` & `aws-cdk-code-builder-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 15:37:04.035536 aws-cdk-code-builder-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2022-11-26 15:37:04.035536 aws-cdk-code-builder-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 15:37:04.031536 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     4509 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 15:37:04.035536 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2022-11-26 15:37:04.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      316 2022-11-26 15:37:04.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-26 15:37:04.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-26 15:37:04.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-26 15:37:04.000000 aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-26 15:37:04.035536 aws-cdk-code-builder-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-26 15:37:04.035536 aws-cdk-code-builder-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4523 2022-11-26 15:36:52.000000 aws-cdk-code-builder-1.2.1/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.180984 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/tests/test_build.py
```

### Comparing `aws-cdk-code-builder-1.2.1/LICENSE` & `aws-cdk-code-builder-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-code-builder-1.2.1/PKG-INFO` & `aws-cdk-code-builder-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-code-builder
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Library that extends the aws_lambda.Code.from_asset and allows for auto packaging of the project
 Home-page: https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 Keywords: aws_cdk,aws_cdk_build,aws_cdk_packaging
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aws-cdk-code-builder-1.2.1/README.md` & `aws-cdk-code-builder-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk-code-builder-1.2.1/aws_cdk_code_builder/__init__.py` & `aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-code-builder-1.2.1/aws_cdk_code_builder.egg-info/PKG-INFO` & `aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-code-builder
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Library that extends the aws_lambda.Code.from_asset and allows for auto packaging of the project
 Home-page: https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 Keywords: aws_cdk,aws_cdk_build,aws_cdk_packaging
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aws-cdk-code-builder-1.2.1/setup.py` & `aws-cdk-code-builder-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # Local Imports
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text(encoding='utf8')
 
 setup(
     name='aws-cdk-code-builder',
     packages=find_packages(),
-    version='1.2.1',
+    version='1.2.3',
     description='A Library that extends the aws_lambda.Code.from_asset and allows for auto '
                 'packaging of the project',
     long_description=README,
     long_description_content_type='text/markdown',
     author='DeadSec-Security',
     author_email='amng835@gmail.com',
     url='https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder',
     install_requires=[
-        'aws-cdk-lib==2.50.0',
+        'aws-cdk-lib>=2.50.0',
     ],
     keywords=[
         'aws_cdk',
         'aws_cdk_build',
         'aws_cdk_packaging'
     ],
     python_requires='>=3.7'
```

### Comparing `aws-cdk-code-builder-1.2.1/tests/test_build.py` & `aws-cdk-code-builder-1.2.3/tests/test_build.py`

 * *Files identical despite different names*

