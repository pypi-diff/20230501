# Comparing `tmp/pytest_aioworkers-0.4.0.tar.gz` & `tmp/pytest_aioworkers-0.4.0a1.tar.gz`

## Comparing `pytest_aioworkers-0.4.0.tar` & `pytest_aioworkers-0.4.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/pytest_aioworkers/__init__.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/pytest_aioworkers/plugin.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/pytest_aioworkers/utils.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/LICENSE
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/README.rst
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/plugin.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pytest_aioworkers/utils.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/README.rst
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pytest_aioworkers-0.4.0a1/PKG-INFO
```

### Comparing `pytest_aioworkers-0.4.0/pytest_aioworkers/plugin.py` & `pytest_aioworkers-0.4.0a1/pytest_aioworkers/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_aioworkers-0.4.0/.gitignore` & `pytest_aioworkers-0.4.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_aioworkers-0.4.0/LICENSE` & `pytest_aioworkers-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aioworkers-0.4.0/README.rst` & `pytest_aioworkers-0.4.0a1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -23,55 +23,47 @@
 A plugin to test aioworkers projects with pytest
 
 
 
 Features
 --------
 
-* fixtures: aioworkers, context, config_yaml
+* fixtures
 
 
 Requirements
 ------------
 
 * pytest
 * aioworkers
 
 
 Installation
 ------------
 
 You can install "pytest-aioworkers" via `pip`_ from `PyPI`_::
 
-    $ pip install pytest-aioworkers[asyncio]
+    $ pip install pytest-aioworkers
 
 
 Contributing
 ------------
-Contributions are very welcome. Tests can be run with `hatch`_, please ensure
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
-To run tests::
-
-    hatch run pytest
-
-or::
-
-    hatch run cov
-
 License
 -------
 
 Distributed under the terms of the `Apache Software License 2.0`_ license, "pytest-aioworkers" is free and open source software
 
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`file an issue`: https://github.com/aioworkers/pytest-aioworkers/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`hatch`: https://hatch.pypa.io/latest/environment/#scripts
+.. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
```

### Comparing `pytest_aioworkers-0.4.0/pyproject.toml` & `pytest_aioworkers-0.4.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Testing",
     "Typing :: Typed",
 ]
 dependencies = [
     "aioworkers",
     "pytest >= 6.1.0",
 ]
@@ -41,16 +40,14 @@
 
 [project.entry-points.pytest11]
 aioworkers = "pytest_aioworkers.plugin"
 
 [project.urls]
 GitHub = "https://github.com/aioworkers/pytest-aioworkers"
 Homepage = "https://github.com/aioworkers/pytest-aioworkers"
-Documentation = "https://github.com/aioworkers/pytest-aioworkers/blob/master/README.rst"
-Issues = "https://github.com/aioworkers/pytest-aioworkers/issues"
 
 [tool.hatch.version]
 path = "pytest_aioworkers/__init__.py"
 
 [tool.hatch.build]
 include = [
     "/pytest_aioworkers",
@@ -92,15 +89,15 @@
 exclude_lines = [
     "no cov",
     "if TYPE_CHECKING:",
 ]
 
 [tool.black]
 line-length = 120
-target-version = ["py37", "py38", "py39", "py310", "py311"]
+target-version = ["py37", "py38", "py39", "py310"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 
 [tool.mypy]
```

### Comparing `pytest_aioworkers-0.4.0/PKG-INFO` & `pytest_aioworkers-0.4.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: pytest-aioworkers
-Version: 0.4.0
+Version: 0.4.0a1
 Summary: A plugin to test aioworkers project with pytest
 Project-URL: GitHub, https://github.com/aioworkers/pytest-aioworkers
 Project-URL: Homepage, https://github.com/aioworkers/pytest-aioworkers
-Project-URL: Documentation, https://github.com/aioworkers/pytest-aioworkers/blob/master/README.rst
-Project-URL: Issues, https://github.com/aioworkers/pytest-aioworkers/issues
 Author-email: Alexander Malev <malev@somedev.ru>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: aioworkers
 Requires-Dist: pytest>=6.1.0
 Provides-Extra: aiohttp
 Requires-Dist: pytest-aiohttp; extra == 'aiohttp'
@@ -55,55 +52,47 @@
 A plugin to test aioworkers projects with pytest
 
 
 
 Features
 --------
 
-* fixtures: aioworkers, context, config_yaml
+* fixtures
 
 
 Requirements
 ------------
 
 * pytest
 * aioworkers
 
 
 Installation
 ------------
 
 You can install "pytest-aioworkers" via `pip`_ from `PyPI`_::
 
-    $ pip install pytest-aioworkers[asyncio]
+    $ pip install pytest-aioworkers
 
 
 Contributing
 ------------
-Contributions are very welcome. Tests can be run with `hatch`_, please ensure
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
-To run tests::
-
-    hatch run pytest
-
-or::
-
-    hatch run cov
-
 License
 -------
 
 Distributed under the terms of the `Apache Software License 2.0`_ license, "pytest-aioworkers" is free and open source software
 
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`file an issue`: https://github.com/aioworkers/pytest-aioworkers/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
-.. _`hatch`: https://hatch.pypa.io/latest/environment/#scripts
+.. _`tox`: https://tox.readthedocs.io/en/latest/
 .. _`pip`: https://pypi.org/project/pip/
 .. _`PyPI`: https://pypi.org/project
```

