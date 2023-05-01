# Comparing `tmp/puffy-0.2.0.tar.gz` & `tmp/puffy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puffy-0.2.0.tar", last modified: Fri Apr 28 06:39:40 2023, max compression
+gzip compressed data, was "puffy-0.3.0.tar", last modified: Mon May  1 04:30:16 2023, max compression
```

## Comparing `puffy-0.2.0.tar` & `puffy-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730876 puffy-0.2.0/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.2.0/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)    13398 2023-04-28 06:39:40.731015 puffy-0.2.0/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)    12905 2023-04-28 06:38:18.000000 puffy-0.2.0/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.2.0/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-04-28 06:39:40.731751 puffy-0.2.0/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.728752 puffy-0.2.0/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.729892 puffy-0.2.0/src/puffy/
--rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.2.0/src/puffy/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730645 puffy-0.2.0/src/puffy/error/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.2.0/src/puffy/error/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730771 puffy-0.2.0/src/puffy/object/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.2.0/src/puffy/object/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730513 puffy-0.2.0/src/puffy.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)    13398 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      285 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427446 puffy-0.3.0/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.3.0/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    18912 2023-05-01 04:30:16.427537 puffy-0.3.0/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    18419 2023-05-01 04:27:50.000000 puffy-0.3.0/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.3.0/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-05-01 04:30:16.427903 puffy-0.3.0/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.425390 puffy-0.3.0/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.426322 puffy-0.3.0/src/puffy/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.3.0/src/puffy/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427068 puffy-0.3.0/src/puffy/error/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.3.0/src/puffy/error/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427191 puffy-0.3.0/src/puffy/log/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     4341 2023-05-01 04:07:48.000000 puffy-0.3.0/src/puffy/log/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427318 puffy-0.3.0/src/puffy/object/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.3.0/src/puffy/object/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.426943 puffy-0.3.0/src/puffy.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    18912 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      311 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/top_level.txt
```

### Comparing `puffy-0.2.0/LICENSE` & `puffy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puffy-0.2.0/PKG-INFO` & `puffy-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: puffy
-Version: 0.2.0
-Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
-Home-page: https://github.com/nicolasdao/pypuffy
-Author: Nicolas Dao
-Author-email: nicolas.dao@gmail.com
-License: BSD-3-Clause
-Keywords: util
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PUFFY
 
 A collection of modules with zero-dependencies to help manage common programming tasks.
 
 ```
 pip install puffy
 ```
@@ -47,17 +31,22 @@
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
+>   - [`log`](#log)
+>       - [Basic `log` APIs](#basic-log-apis)
+>       - [Logging errors](#logging-errors)
+>       - [Environment variables](#environment-variables)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
+>	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
 >		- [Skipping tests](#skipping-tests)
 >		- [Executing a specific test only](#executing-a-specific-test-only)
 >	- [Building and distributing this package](#building-and-distributing-this-package)
@@ -173,14 +162,103 @@
 # error: Failed
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail
 #     raise Exception("Failed")
 ```
 
+## `log`
+### Basic `log` APIs
+
+This method prints a structured log to stdout. That structured log is a standard Python `dict` which is then serialized to `str` using `json.dumps`. This method is designed to never fail. It was originally designed to log messages to AWS CloudWatch.
+
+```python
+from puffy.log import log
+
+log() # '{ "level":"INFO" }'
+
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    metric=23,
+    unit="beers", # Default is "ms" (i.e., milliseconds)
+    data= {
+        "name": "Dave",
+        "age": 45
+    },
+    op_id= 12345,
+    test=True
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "test": true, "metric": 23, "unit": "beers", "op_id": 12345, "data": {"name": "Dave", "age": 45}}'
+
+# Logging time:
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    time=34 # This is converted to the "metric" input with "unit" set to "ms" (cannot be overwritten)
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "metric": 34, "unit": "ms"}'
+```
+
+### Logging errors
+
+The `log` API is designed to support puffy's `StackedException` errors. The advantage of using `StackedException` is that you can have confidence that the stacked errors are properly serialized (i.e., including message and traceback).
+
+```python
+from puffy.log import log
+from puffy.error import catch_errors, StackedException as e
+
+@catch_errors("Should fail")
+def fail():
+    err, resp = fail_again()
+    if err:
+        raise e(err)
+    return "yes"
+
+@catch_errors("Should fail again")
+def fail_again():
+    raise Exception("Failed again")
+    return "yes"
+
+err, *_ = fail()
+
+# Supports `StackedException`
+log(
+    level="ERROR",
+    errors=err) 
+# '{"level": "INFO", "errors": "error: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+
+# Supports standard errors
+log(
+    level="ERROR",
+    errors=Exception("Bim bam boom")) # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports strings
+log(
+    level="ERROR",
+    errors="Bim bam boom") # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports list of errors
+log(
+    level="ERROR",
+    errors=["Bim bam boom", Exception("Booom"), err]) # '{"level": "ERROR", "errors": "Bim bam boom\nBooom\nerror: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+```
+
+### Environment variables
+
+Often, specific common metadata must be added to all logs (e.g., server's details, api name, ...). For this purpose, use the `LOG_META` environment variable. This environment variable expects a stringified JSON object:
+
+```python
+from puffy.log import log
+
+os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
+
+log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -192,36 +270,74 @@
 print(obj.g('address.line1')) # Magic street
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street' } }
 print(obj.g('address.line2')) # Nonce
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street', line2: None } }
 ```
 
 # Dev
+## Dev - Getting started
+
+1. Clone this project:
+```shell
+git clone https://github.com/nicolasdao/pypuffy.git
+```
+2. Browse to the root folder:
+```shell
+cd pypuffy
+```
+3. Create a new virtual environment:
+```shell
+python3 -m venv .venv
+```
+4. Activate this virtual environment:
+```shell
+source .venv/bin/activate
+```
+
+To deactivate that virtual environment:
+```shell
+deactivate
+```
+
 ## CLI commands
 
 `make` commands:
 
 | Command | Description |
 |:--------|:------------|
+| `python3 -m venv .venv` | Create a new virtual environment. |
+| `source .venv/bin/activate` | Activate the virtual environment |
+| `deactivate` | Deactivate the virtual environment |
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
 | `make t` | Formats, lints and then unit tests the project. |
 | `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
+| `easyv` | Returns the version defined in `setup.cfg`. |
+| `easyv bump` | Bumps the patch version defined in `setup.cfg` (1).|
+| `easyv bump minor` | Bumps the minor version defined in `setup.cfg` (1).|
+| `easyv bump major` | Bumps the major version defined in `setup.cfg` (1).|
+| `easyv bump x.x.x` | Sets the version defined in `setup.cfg` to x.x.x (1).|
+
+> __(1):__ Bumping a version using `easyv` can apply up to three updates:
+>1. Updates the version property in the `setup.cfg` file.
+>2. If the project is under source control with git and git is installed:
+>   1. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag. If the `CHANGELOG.md` file does not exist, it is automatically created.
+>   2. git commit and tag (using the version number prefixed with `v`) the project.
 
 ## Install dependencies with `easypipinstall`
 
-`easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
+`easypipinstall` adds three new CLI utilities: `easyi` (install) `easyu` (uninstall) and `easyv` (manages package's version). To learn the full details about `easypipinstall`, please refer to https://github.com/nicolasdao/easypipinstall.
 
 Examples:
 ```
 easyi numpy
 ```
 
 This installs `numpy` (via `pip install`) then automatically updates the following files:
@@ -306,55 +422,48 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
-
-__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
-
-To build your package, run:
-
+1. Make sure the test and lint operations have not produced errors:
+```shell
+make t
 ```
+2. Build this package:
+```shell
 make b
 ```
-
-This command is a wrapper around `python3 -m build`.
-
-To build and publish your package to https://pypi.org, run:
-
-```
+> This command is a wrapper around `python3 -m build`.
+3. Version and tag this package using one of the following command (1):
+    - `easyv bump`: Use this to bump the patch version.
+    - `easyv bump minor`: Use this to bump the minor version.
+    - `easyv bump major`: Use this to bump the major version.
+    - `easyv bump x.x.x`: Use this to bump the version to a specific value.
+4 . Publish this package to https://pypi.org:
+```shell
 make p
 ```
+> This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
-This command is a wrapper around the following commands:
-
-```
-python3 -m build; \
-twine upload dist/*
-```
-
-Those two steps have been bundled in a single command:
-
-```
-make bp
-```
-
-> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
-```
+```shell
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
 
+> (1): This step applies three updates:
+> 1. Updates the version property in the `setup.cfg` file.
+> 2. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag.
+> 3. git commit and tag (using the version number prefixed with `v`) the project.
+
 # FAQ
 
 # References
 
 # License
 
 BSD 3-Clause License
```

### Comparing `puffy-0.2.0/README.md` & `puffy-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: puffy
+Version: 0.3.0
+Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
+Home-page: https://github.com/nicolasdao/pypuffy
+Author: Nicolas Dao
+Author-email: nicolas.dao@gmail.com
+License: BSD-3-Clause
+Keywords: util
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PUFFY
 
 A collection of modules with zero-dependencies to help manage common programming tasks.
 
 ```
 pip install puffy
 ```
@@ -31,17 +47,22 @@
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
+>   - [`log`](#log)
+>       - [Basic `log` APIs](#basic-log-apis)
+>       - [Logging errors](#logging-errors)
+>       - [Environment variables](#environment-variables)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
+>	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
 >		- [Skipping tests](#skipping-tests)
 >		- [Executing a specific test only](#executing-a-specific-test-only)
 >	- [Building and distributing this package](#building-and-distributing-this-package)
@@ -157,14 +178,103 @@
 # error: Failed
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail
 #     raise Exception("Failed")
 ```
 
+## `log`
+### Basic `log` APIs
+
+This method prints a structured log to stdout. That structured log is a standard Python `dict` which is then serialized to `str` using `json.dumps`. This method is designed to never fail. It was originally designed to log messages to AWS CloudWatch.
+
+```python
+from puffy.log import log
+
+log() # '{ "level":"INFO" }'
+
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    metric=23,
+    unit="beers", # Default is "ms" (i.e., milliseconds)
+    data= {
+        "name": "Dave",
+        "age": 45
+    },
+    op_id= 12345,
+    test=True
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "test": true, "metric": 23, "unit": "beers", "op_id": 12345, "data": {"name": "Dave", "age": 45}}'
+
+# Logging time:
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    time=34 # This is converted to the "metric" input with "unit" set to "ms" (cannot be overwritten)
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "metric": 34, "unit": "ms"}'
+```
+
+### Logging errors
+
+The `log` API is designed to support puffy's `StackedException` errors. The advantage of using `StackedException` is that you can have confidence that the stacked errors are properly serialized (i.e., including message and traceback).
+
+```python
+from puffy.log import log
+from puffy.error import catch_errors, StackedException as e
+
+@catch_errors("Should fail")
+def fail():
+    err, resp = fail_again()
+    if err:
+        raise e(err)
+    return "yes"
+
+@catch_errors("Should fail again")
+def fail_again():
+    raise Exception("Failed again")
+    return "yes"
+
+err, *_ = fail()
+
+# Supports `StackedException`
+log(
+    level="ERROR",
+    errors=err) 
+# '{"level": "INFO", "errors": "error: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+
+# Supports standard errors
+log(
+    level="ERROR",
+    errors=Exception("Bim bam boom")) # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports strings
+log(
+    level="ERROR",
+    errors="Bim bam boom") # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports list of errors
+log(
+    level="ERROR",
+    errors=["Bim bam boom", Exception("Booom"), err]) # '{"level": "ERROR", "errors": "Bim bam boom\nBooom\nerror: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+```
+
+### Environment variables
+
+Often, specific common metadata must be added to all logs (e.g., server's details, api name, ...). For this purpose, use the `LOG_META` environment variable. This environment variable expects a stringified JSON object:
+
+```python
+from puffy.log import log
+
+os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
+
+log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -176,36 +286,74 @@
 print(obj.g('address.line1')) # Magic street
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street' } }
 print(obj.g('address.line2')) # Nonce
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street', line2: None } }
 ```
 
 # Dev
+## Dev - Getting started
+
+1. Clone this project:
+```shell
+git clone https://github.com/nicolasdao/pypuffy.git
+```
+2. Browse to the root folder:
+```shell
+cd pypuffy
+```
+3. Create a new virtual environment:
+```shell
+python3 -m venv .venv
+```
+4. Activate this virtual environment:
+```shell
+source .venv/bin/activate
+```
+
+To deactivate that virtual environment:
+```shell
+deactivate
+```
+
 ## CLI commands
 
 `make` commands:
 
 | Command | Description |
 |:--------|:------------|
+| `python3 -m venv .venv` | Create a new virtual environment. |
+| `source .venv/bin/activate` | Activate the virtual environment |
+| `deactivate` | Deactivate the virtual environment |
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
 | `make t` | Formats, lints and then unit tests the project. |
 | `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
+| `easyv` | Returns the version defined in `setup.cfg`. |
+| `easyv bump` | Bumps the patch version defined in `setup.cfg` (1).|
+| `easyv bump minor` | Bumps the minor version defined in `setup.cfg` (1).|
+| `easyv bump major` | Bumps the major version defined in `setup.cfg` (1).|
+| `easyv bump x.x.x` | Sets the version defined in `setup.cfg` to x.x.x (1).|
+
+> __(1):__ Bumping a version using `easyv` can apply up to three updates:
+>1. Updates the version property in the `setup.cfg` file.
+>2. If the project is under source control with git and git is installed:
+>   1. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag. If the `CHANGELOG.md` file does not exist, it is automatically created.
+>   2. git commit and tag (using the version number prefixed with `v`) the project.
 
 ## Install dependencies with `easypipinstall`
 
-`easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
+`easypipinstall` adds three new CLI utilities: `easyi` (install) `easyu` (uninstall) and `easyv` (manages package's version). To learn the full details about `easypipinstall`, please refer to https://github.com/nicolasdao/easypipinstall.
 
 Examples:
 ```
 easyi numpy
 ```
 
 This installs `numpy` (via `pip install`) then automatically updates the following files:
@@ -290,55 +438,48 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
-
-__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
-
-To build your package, run:
-
+1. Make sure the test and lint operations have not produced errors:
+```shell
+make t
 ```
+2. Build this package:
+```shell
 make b
 ```
-
-This command is a wrapper around `python3 -m build`.
-
-To build and publish your package to https://pypi.org, run:
-
-```
+> This command is a wrapper around `python3 -m build`.
+3. Version and tag this package using one of the following command (1):
+    - `easyv bump`: Use this to bump the patch version.
+    - `easyv bump minor`: Use this to bump the minor version.
+    - `easyv bump major`: Use this to bump the major version.
+    - `easyv bump x.x.x`: Use this to bump the version to a specific value.
+4 . Publish this package to https://pypi.org:
+```shell
 make p
 ```
+> This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
-This command is a wrapper around the following commands:
-
-```
-python3 -m build; \
-twine upload dist/*
-```
-
-Those two steps have been bundled in a single command:
-
-```
-make bp
-```
-
-> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
-```
+```shell
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
 
+> (1): This step applies three updates:
+> 1. Updates the version property in the `setup.cfg` file.
+> 2. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag.
+> 3. git commit and tag (using the version number prefixed with `v`) the project.
+
 # FAQ
 
 # References
 
 # License
 
 BSD 3-Clause License
```

### Comparing `puffy-0.2.0/setup.cfg` & `puffy-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = puffy
-version = 0.2.0
+version = 0.3.0
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = A collection of modules with zero-dependencies to help manage common programming tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/pypuffy
 readme = README.md
```

### Comparing `puffy-0.2.0/src/puffy/error/__init__.py` & `puffy-0.3.0/src/puffy/error/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.2.0/src/puffy/object/__init__.py` & `puffy-0.3.0/src/puffy/object/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.2.0/src/puffy.egg-info/PKG-INFO` & `puffy-0.3.0/src/puffy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -47,17 +47,22 @@
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
+>   - [`log`](#log)
+>       - [Basic `log` APIs](#basic-log-apis)
+>       - [Logging errors](#logging-errors)
+>       - [Environment variables](#environment-variables)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
+>	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
 >		- [Skipping tests](#skipping-tests)
 >		- [Executing a specific test only](#executing-a-specific-test-only)
 >	- [Building and distributing this package](#building-and-distributing-this-package)
@@ -173,14 +178,103 @@
 # error: Failed
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail
 #     raise Exception("Failed")
 ```
 
+## `log`
+### Basic `log` APIs
+
+This method prints a structured log to stdout. That structured log is a standard Python `dict` which is then serialized to `str` using `json.dumps`. This method is designed to never fail. It was originally designed to log messages to AWS CloudWatch.
+
+```python
+from puffy.log import log
+
+log() # '{ "level":"INFO" }'
+
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    metric=23,
+    unit="beers", # Default is "ms" (i.e., milliseconds)
+    data= {
+        "name": "Dave",
+        "age": 45
+    },
+    op_id= 12345,
+    test=True
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "test": true, "metric": 23, "unit": "beers", "op_id": 12345, "data": {"name": "Dave", "age": 45}}'
+
+# Logging time:
+log(
+    level="WARN", # Supported values: "INFO" (default), "WARN" (or "WARNING"), "ERROR", "CRITICAL"
+    message="Seems drunk",
+    code="drunky_drunky",
+    time=34 # This is converted to the "metric" input with "unit" set to "ms" (cannot be overwritten)
+) # '{"level": "WARN", "message": "Seems drunk", "code": "drunky_drunky", "metric": 34, "unit": "ms"}'
+```
+
+### Logging errors
+
+The `log` API is designed to support puffy's `StackedException` errors. The advantage of using `StackedException` is that you can have confidence that the stacked errors are properly serialized (i.e., including message and traceback).
+
+```python
+from puffy.log import log
+from puffy.error import catch_errors, StackedException as e
+
+@catch_errors("Should fail")
+def fail():
+    err, resp = fail_again()
+    if err:
+        raise e(err)
+    return "yes"
+
+@catch_errors("Should fail again")
+def fail_again():
+    raise Exception("Failed again")
+    return "yes"
+
+err, *_ = fail()
+
+# Supports `StackedException`
+log(
+    level="ERROR",
+    errors=err) 
+# '{"level": "INFO", "errors": "error: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+
+# Supports standard errors
+log(
+    level="ERROR",
+    errors=Exception("Bim bam boom")) # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports strings
+log(
+    level="ERROR",
+    errors="Bim bam boom") # '{"level": "ERROR", "errors": "Bim bam boom"}'
+
+# Supports list of errors
+log(
+    level="ERROR",
+    errors=["Bim bam boom", Exception("Booom"), err]) # '{"level": "ERROR", "errors": "Bim bam boom\nBooom\nerror: Should fail\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Should fail again\n  File \"/Users/.../ur_code.py\", line 153, in fail\nerror: Failed again\n  File \"/Users/.../ur_code.py\", line 112, in safe_exec\n    data = ffn(*args, **named_args)\n  File \"/Users/.../ur_code.py\", line 162, in fail_again\n    raise Exception(\"Failed again\")\n"}'
+```
+
+### Environment variables
+
+Often, specific common metadata must be added to all logs (e.g., server's details, api name, ...). For this purpose, use the `LOG_META` environment variable. This environment variable expects a stringified JSON object:
+
+```python
+from puffy.log import log
+
+os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
+
+log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -192,36 +286,74 @@
 print(obj.g('address.line1')) # Magic street
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street' } }
 print(obj.g('address.line2')) # Nonce
 print(obj) # { 'hello':'world', 'person': { 'name': None }, 'address': { 'line1': 'Magic street', line2: None } }
 ```
 
 # Dev
+## Dev - Getting started
+
+1. Clone this project:
+```shell
+git clone https://github.com/nicolasdao/pypuffy.git
+```
+2. Browse to the root folder:
+```shell
+cd pypuffy
+```
+3. Create a new virtual environment:
+```shell
+python3 -m venv .venv
+```
+4. Activate this virtual environment:
+```shell
+source .venv/bin/activate
+```
+
+To deactivate that virtual environment:
+```shell
+deactivate
+```
+
 ## CLI commands
 
 `make` commands:
 
 | Command | Description |
 |:--------|:------------|
+| `python3 -m venv .venv` | Create a new virtual environment. |
+| `source .venv/bin/activate` | Activate the virtual environment |
+| `deactivate` | Deactivate the virtual environment |
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
 | `make t` | Formats, lints and then unit tests the project. |
 | `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
+| `easyv` | Returns the version defined in `setup.cfg`. |
+| `easyv bump` | Bumps the patch version defined in `setup.cfg` (1).|
+| `easyv bump minor` | Bumps the minor version defined in `setup.cfg` (1).|
+| `easyv bump major` | Bumps the major version defined in `setup.cfg` (1).|
+| `easyv bump x.x.x` | Sets the version defined in `setup.cfg` to x.x.x (1).|
+
+> __(1):__ Bumping a version using `easyv` can apply up to three updates:
+>1. Updates the version property in the `setup.cfg` file.
+>2. If the project is under source control with git and git is installed:
+>   1. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag. If the `CHANGELOG.md` file does not exist, it is automatically created.
+>   2. git commit and tag (using the version number prefixed with `v`) the project.
 
 ## Install dependencies with `easypipinstall`
 
-`easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
+`easypipinstall` adds three new CLI utilities: `easyi` (install) `easyu` (uninstall) and `easyv` (manages package's version). To learn the full details about `easypipinstall`, please refer to https://github.com/nicolasdao/easypipinstall.
 
 Examples:
 ```
 easyi numpy
 ```
 
 This installs `numpy` (via `pip install`) then automatically updates the following files:
@@ -306,55 +438,48 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
-
-__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
-
-To build your package, run:
-
+1. Make sure the test and lint operations have not produced errors:
+```shell
+make t
 ```
+2. Build this package:
+```shell
 make b
 ```
-
-This command is a wrapper around `python3 -m build`.
-
-To build and publish your package to https://pypi.org, run:
-
-```
+> This command is a wrapper around `python3 -m build`.
+3. Version and tag this package using one of the following command (1):
+    - `easyv bump`: Use this to bump the patch version.
+    - `easyv bump minor`: Use this to bump the minor version.
+    - `easyv bump major`: Use this to bump the major version.
+    - `easyv bump x.x.x`: Use this to bump the version to a specific value.
+4 . Publish this package to https://pypi.org:
+```shell
 make p
 ```
+> This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
-This command is a wrapper around the following commands:
-
-```
-python3 -m build; \
-twine upload dist/*
-```
-
-Those two steps have been bundled in a single command:
-
-```
-make bp
-```
-
-> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
-```
+```shell
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
 
+> (1): This step applies three updates:
+> 1. Updates the version property in the `setup.cfg` file.
+> 2. Updates the `CHANGELOG.md` file using the commit messages between the current branch and the last version tag.
+> 3. git commit and tag (using the version number prefixed with `v`) the project.
+
 # FAQ
 
 # References
 
 # License
 
 BSD 3-Clause License
```

