# Comparing `tmp/katalytic-images-0.1.3.tar.gz` & `tmp/katalytic-images-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.1.3.tar", last modified: Fri Apr 14 07:46:55 2023, max compression
+gzip compressed data, was "katalytic-images-0.2.0.tar", last modified: Mon May  1 11:06:19 2023, max compression
```

## Comparing `katalytic-images-0.1.3.tar` & `katalytic-images-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.travis.yml
--rw-r--r--   0        0        0      675 2023-04-14 07:46:40.322644 katalytic-images-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2165 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/README.md
--rw-r--r--   0        0        0     1805 2023-04-14 07:46:39.866416 katalytic-images-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/pytest.sh
--rw-r--r--   0        0        0     2867 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/venv.sh
--rw-r--r--   0        0        0     2825 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/src/katalytic/images.py
--rw-r--r--   0        0        0     7796 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/tests/test_images.py
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 katalytic-images-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3324 2023-04-30 14:15:39.110597 katalytic-images-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1198 2023-05-01 11:06:00.384195 katalytic-images-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.2.0/README.md
+-rw-r--r--   0        0        0     1503 2023-05-01 11:06:00.368194 katalytic-images-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-05-01 10:57:08.769254 katalytic-images-0.2.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    11945 2023-05-01 11:00:26.823672 katalytic-images-0.2.0/tests/test_images.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 katalytic-images-0.2.0/PKG-INFO
```

### Comparing `katalytic-images-0.1.3/.gitignore` & `katalytic-images-0.2.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __pycache__/*
 .cache/*
 .*.swp
 */.ipynb_checkpoints/*
 .DS_Store
 data/
 logs/
+sandbox.*
 
 # Project files
 .ropeproject
 .project
 .pydevproject
 .settings
 .idea
```

### Comparing `katalytic-images-0.1.3/LICENSE.txt` & `katalytic-images-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.3/README.md` & `katalytic-images-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-images)](https://pypi.org/project/katalytic-images/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-images.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-images)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-images?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-images)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-images/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-images?branch=main)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-images/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-images/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-images.svg)](https://katalytic-images.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-images
 ```
```

### Comparing `katalytic-images-0.1.3/pyproject.toml` & `katalytic-images-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.1.3"
+version = "0.2.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -45,26 +45,9 @@
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-images.git"
 repository = "https://gitlab.com/katalytic/katalytic-images.git"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-env_list = py36, py37, py38, py39
-isolated_build = True
-
-[testenv]
-extras = dev
-deps = -e .
-
-commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
-"""
-
-[tool.semantic_release]
-version_variable = "pyproject.toml:version"
-branch = "main"
-
 [tool.flit.module]
 name = "katalytic.images"
```

### Comparing `katalytic-images-0.1.3/PKG-INFO` & `katalytic-images-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.1.3
+Version: 0.2.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -30,18 +30,18 @@
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-images.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-images)](https://pypi.org/project/katalytic-images/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-images.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-images)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-images?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-images)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-images/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-images?branch=main)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-images/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-images/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-images.svg)](https://katalytic-images.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-images
 ```
```

