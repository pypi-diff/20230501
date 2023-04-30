# Comparing `tmp/fbench-0.2.0.tar.gz` & `tmp/fbench-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbench-0.2.0.tar", max compression
+gzip compressed data, was "fbench-0.3.0.tar", max compression
```

## Comparing `fbench-0.2.0.tar` & `fbench-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1523 2023-03-12 14:19:00.114818 fbench-0.2.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-03-12 14:19:00.114818 fbench-0.2.0/LICENSES/
--rw-r--r--   0        0        0     1543 2023-03-12 14:19:00.114818 fbench-0.2.0/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     1874 2023-03-12 14:19:00.114818 fbench-0.2.0/README.md
--rw-r--r--   0        0        0     1153 2023-03-12 14:20:40.127825 fbench-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-03-12 14:19:00.118818 fbench-0.2.0/src/fbench/__init__.py
--rw-r--r--   0        0        0      199 2023-03-12 14:19:00.118818 fbench-0.2.0/src/fbench/exception.py
--rw-r--r--   0        0        0     3241 2023-03-12 14:19:00.118818 fbench-0.2.0/src/fbench/function.py
--rw-r--r--   0        0        0     1089 2023-03-12 14:19:00.118818 fbench-0.2.0/src/fbench/validation.py
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 fbench-0.2.0/setup.py
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 fbench-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1523 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSES/
+-rw-r--r--   0        0        0     1543 2023-04-30 22:43:45.211215 fbench-0.3.0/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     1898 2023-04-30 22:43:45.211215 fbench-0.3.0/README.md
+-rw-r--r--   0        0        0     1193 2023-04-30 22:45:22.364355 fbench-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      259 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/__init__.py
+-rw-r--r--   0        0        0     1169 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/config.py
+-rw-r--r--   0        0        0      199 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/exception.py
+-rw-r--r--   0        0        0     3729 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/function.py
+-rw-r--r--   0        0        0      573 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/structure.py
+-rw-r--r--   0        0        0     1031 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/validation.py
+-rw-r--r--   0        0        0     8060 2023-04-30 22:43:45.235216 fbench-0.3.0/src/fbench/visualization.py
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 fbench-0.3.0/setup.py
+-rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 fbench-0.3.0/PKG-INFO
```

### Comparing `fbench-0.2.0/LICENSE` & `fbench-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-0.2.0/LICENSES/NUMPY_LICENSE` & `fbench-0.3.0/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `fbench-0.2.0/README.md` & `fbench-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </p>
 
 ## About
 
 A collection of benchmark functions:
 
 - [Documentation](https://fbench.readthedocs.io/en/stable/index.html)
-- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)
+- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)
 - [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
 
 ## Installation
 
 `fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:
 
 ```console
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
                              ****** fBench ******
                 [pypi] [docs] [ci_status] [coverage] [license]
 ## About A collection of benchmark functions: - [Documentation](https://
-fbench.readthedocs.io/en/stable/index.html) - [Example usage](https://
-fbench.readthedocs.io/en/stable/example.html) - [API Reference](https://
-fbench.readthedocs.io/en/stable/autoapi/fbench/index.html) ## Installation
-`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python
-3.8+: ```console pip install fbench ``` ## Examples The [`ackley`](https://
-fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley)
-function: ```python >>> import fbench >>> round(fbench.ackley([1, 1]), 4)
-3.6254 ``` ## Contributing to fBench Your contribution is greatly appreciated!
-See the following links to help you get started: - [Contributing Guide](https:/
-/fbench.readthedocs.io/en/latest/contributing.html) - [Developer Guide](https:/
-/fbench.readthedocs.io/en/latest/developers.html) - [Contributor Code of
-Conduct](https://fbench.readthedocs.io/en/latest/conduct.html) ## License
-`fbench` was created by fBench Developers. It is licensed under the terms of
-the BSD 3-Clause license.
+fbench.readthedocs.io/en/stable/index.html) - [Overview of fBench functions]
+(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [API
+Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
+## Installation `fbench` is available on [PyPI](https://pypi.org/project/
+fbench/) for Python 3.8+: ```console pip install fbench ``` ## Examples The
+[`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+index.html#fbench.ackley) function: ```python >>> import fbench >>> round
+(fbench.ackley([1, 1]), 4) 3.6254 ``` ## Contributing to fBench Your
+contribution is greatly appreciated! See the following links to help you get
+started: - [Contributing Guide](https://fbench.readthedocs.io/en/latest/
+contributing.html) - [Developer Guide](https://fbench.readthedocs.io/en/latest/
+developers.html) - [Contributor Code of Conduct](https://fbench.readthedocs.io/
+en/latest/conduct.html) ## License `fbench` was created by fBench Developers.
+It is licensed under the terms of the BSD 3-Clause license.
```

### Comparing `fbench-0.2.0/pyproject.toml` & `fbench-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbench"
-version = "0.2.0"
+version = "0.3.0"
 description = "A collection of benchmark functions."
 authors = ["fBench Developers"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/fbench"
 documentation = "https://fbench.readthedocs.io/en/stable/"
 include = ["LICENSES/"]
@@ -12,14 +12,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
+matplotlib = "^3.7.1"
+bumbag = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 black = {extras = ["jupyter"], version = "^22.6.0"}
 isort = "^5.10.1"
 flake8 = "^4.0.1"
```

### Comparing `fbench-0.2.0/src/fbench/validation.py` & `fbench-0.3.0/src/fbench/validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import numpy as np
 
-__all__ = ("check_vector",)
+from fbench import exception
 
-from fbench.exception import IncorrectNumberOfElements, NotAVectorError
+__all__ = ("check_vector",)
 
 
-def check_vector(x, min_number_of_elements):
+def check_vector(x, /, *, min_elements):
     """Validate an n-dimensional vector.
 
     Parameters
     ----------
     x : array_like
         Input data with :math:`n` elements that can be converted to an array.
-    min_number_of_elements : int
+    min_elements : int
         Specify the minimum number of elements ``x`` must have.
 
     Returns
     -------
     np.ndarray
-        An n-dimensional vector.
+        The :math:`n`-dimensional vector.
 
     Raises
     ------
     NotAVectorError
         If ``x`` is not vector-like.
     IncorrectNumberOfElements
-        If ``x`` does not satisfy the ``min_number_of_elements`` condition.
+        If ``x`` does not satisfy the ``min_elements`` condition.
     """
     x = np.asarray(x)
 
     if len(x.shape) != 1:
-        raise NotAVectorError(
+        raise exception.NotAVectorError(
             f"input must be vector-like object - it has shape={x.shape}"
         )
 
-    if not len(x) >= min_number_of_elements:
-        raise IncorrectNumberOfElements(
-            f"number of elements must be at least {min_number_of_elements} "
+    if not len(x) >= min_elements:
+        raise exception.IncorrectNumberOfElements(
+            f"number of elements must be at least {min_elements} "
             f"- it has {x.shape[0]}"
         )
 
     return x
```

### Comparing `fbench-0.2.0/setup.py` & `fbench-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 packages = \
 ['fbench']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.2,<2.0.0']
+['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'fbench',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A collection of benchmark functions.',
-    'long_description': '<h1 align="center">fBench</h1>\n\n<p align="center">\n<a href="https://pypi.org/project/fbench"><img alt="pypi" src="https://img.shields.io/pypi/v/fbench"></a>\n<a href="https://readthedocs.org/projects/fbench/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/fbench/badge/?version=latest"></a>\n<a href="https://github.com/estripling/fbench/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/fbench/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/fbench"><img alt="coverage" src="https://codecov.io/github/estripling/fbench/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/fbench/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/fbench"></a>\n</p>\n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation](https://fbench.readthedocs.io/en/stable/index.html)\n- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)\n- [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
+    'long_description': '<h1 align="center">fBench</h1>\n\n<p align="center">\n<a href="https://pypi.org/project/fbench"><img alt="pypi" src="https://img.shields.io/pypi/v/fbench"></a>\n<a href="https://readthedocs.org/projects/fbench/?badge=latest"><img alt="docs" src="https://readthedocs.org/projects/fbench/badge/?version=latest"></a>\n<a href="https://github.com/estripling/fbench/actions/workflows/ci.yml"><img alt="ci status" src="https://github.com/estripling/fbench/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n<a href="https://codecov.io/gh/estripling/fbench"><img alt="coverage" src="https://codecov.io/github/estripling/fbench/coverage.svg?branch=main"></a>\n<a href="https://github.com/estripling/fbench/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/pypi/l/fbench"></a>\n</p>\n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation](https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n- [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n## Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the following links to help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https://fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n## License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the terms of the BSD 3-Clause license.\n',
     'author': 'fBench Developers',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/estripling/fbench',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fbench'] package_data = \ {'': ['*']} install_requires =
-\ ['numpy>=1.24.2,<2.0.0'] setup_kwargs = { 'name': 'fbench', 'version':
-'0.2.0', 'description': 'A collection of benchmark functions.',
-'long_description': '
+\ ['bumbag>=5.0.0,<6.0.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0']
+setup_kwargs = { 'name': 'fbench', 'version': '0.3.0', 'description': 'A
+collection of benchmark functions.', 'long_description': '
                              ****** fBench ******
 \n\n
             \n[pypi]\n[docs]\n[ci_status]\n[coverage]\n[license]\n
 \n\n## About\n\nA collection of benchmark functions:\n\n- [Documentation]
-(https://fbench.readthedocs.io/en/stable/index.html)\n- [Example usage](https:/
-/fbench.readthedocs.io/en/stable/example.html)\n- [API Reference](https://
-fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)\n\n##
-Installation\n\n`fbench` is available on [PyPI](https://pypi.org/project/
-fbench/) for Python 3.8+:\n\n```console\npip install fbench\n```\n\n##
-Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/
-fbench/index.html#fbench.ackley) function:\n\n```python\n>>> import fbench\n>>>
-round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n## Contributing to
-fBench\n\nYour contribution is greatly appreciated!\nSee the following links to
-help you get started:\n\n- [Contributing Guide](https://fbench.readthedocs.io/
-en/latest/contributing.html)\n- [Developer Guide](https://
-fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of
+(https://fbench.readthedocs.io/en/stable/index.html)\n- [Overview of fBench
+functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)\n-
+[API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+index.html)\n\n## Installation\n\n`fbench` is available on [PyPI](https://
+pypi.org/project/fbench/) for Python 3.8+:\n\n```console\npip install
+fbench\n```\n\n## Examples\n\nThe [`ackley`](https://fbench.readthedocs.io/en/
+stable/autoapi/fbench/index.html#fbench.ackley) function:\n\n```python\n>>>
+import fbench\n>>> round(fbench.ackley([1, 1]), 4)\n3.6254\n```\n\n##
+Contributing to fBench\n\nYour contribution is greatly appreciated!\nSee the
+following links to help you get started:\n\n- [Contributing Guide](https://
+fbench.readthedocs.io/en/latest/contributing.html)\n- [Developer Guide](https:/
+/fbench.readthedocs.io/en/latest/developers.html)\n- [Contributor Code of
 Conduct](https://fbench.readthedocs.io/en/latest/conduct.html)\n\n##
 License\n\n`fbench` was created by fBench Developers.\nIt is licensed under the
 terms of the BSD 3-Clause license.\n', 'author': 'fBench Developers',
 'author_email': 'None', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'https://github.com/estripling/fbench', 'package_dir': package_dir,
 'packages': packages, 'package_data': package_data, 'install_requires':
 install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `fbench-0.2.0/PKG-INFO` & `fbench-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: fbench
-Version: 0.2.0
+Version: 0.3.0
 Summary: A collection of benchmark functions.
 Home-page: https://github.com/estripling/fbench
 License: BSD 3-Clause
 Keywords: fbench
 Author: fBench Developers
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: bumbag (>=5.0.0,<6.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Project-URL: Documentation, https://fbench.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/estripling/fbench
 Description-Content-Type: text/markdown
 
 <h1 align="center">fBench</h1>
 
@@ -30,15 +32,15 @@
 </p>
 
 ## About
 
 A collection of benchmark functions:
 
 - [Documentation](https://fbench.readthedocs.io/en/stable/index.html)
-- [Example usage](https://fbench.readthedocs.io/en/stable/example.html)
+- [Overview of fBench functions](https://fbench.readthedocs.io/en/stable/fBench-functions.html)
 - [API Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
 
 ## Installation
 
 `fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python 3.8+:
 
 ```console
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: fbench Version: 0.2.0 Summary: A collection of
+Metadata-Version: 2.1 Name: fbench Version: 0.3.0 Summary: A collection of
 benchmark functions. Home-page: https://github.com/estripling/fbench License:
 BSD 3-Clause Keywords: fbench Author: fBench Developers Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
-numpy (>=1.24.2,<2.0.0) Project-URL: Documentation, https://
+bumbag (>=5.0.0,<6.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
+Dist: numpy (>=1.24.2,<2.0.0) Project-URL: Documentation, https://
 fbench.readthedocs.io/en/stable/ Project-URL: Repository, https://github.com/
 estripling/fbench Description-Content-Type: text/markdown
                              ****** fBench ******
                 [pypi] [docs] [ci_status] [coverage] [license]
 ## About A collection of benchmark functions: - [Documentation](https://
-fbench.readthedocs.io/en/stable/index.html) - [Example usage](https://
-fbench.readthedocs.io/en/stable/example.html) - [API Reference](https://
-fbench.readthedocs.io/en/stable/autoapi/fbench/index.html) ## Installation
-`fbench` is available on [PyPI](https://pypi.org/project/fbench/) for Python
-3.8+: ```console pip install fbench ``` ## Examples The [`ackley`](https://
-fbench.readthedocs.io/en/stable/autoapi/fbench/index.html#fbench.ackley)
-function: ```python >>> import fbench >>> round(fbench.ackley([1, 1]), 4)
-3.6254 ``` ## Contributing to fBench Your contribution is greatly appreciated!
-See the following links to help you get started: - [Contributing Guide](https:/
-/fbench.readthedocs.io/en/latest/contributing.html) - [Developer Guide](https:/
-/fbench.readthedocs.io/en/latest/developers.html) - [Contributor Code of
-Conduct](https://fbench.readthedocs.io/en/latest/conduct.html) ## License
-`fbench` was created by fBench Developers. It is licensed under the terms of
-the BSD 3-Clause license.
+fbench.readthedocs.io/en/stable/index.html) - [Overview of fBench functions]
+(https://fbench.readthedocs.io/en/stable/fBench-functions.html) - [API
+Reference](https://fbench.readthedocs.io/en/stable/autoapi/fbench/index.html)
+## Installation `fbench` is available on [PyPI](https://pypi.org/project/
+fbench/) for Python 3.8+: ```console pip install fbench ``` ## Examples The
+[`ackley`](https://fbench.readthedocs.io/en/stable/autoapi/fbench/
+index.html#fbench.ackley) function: ```python >>> import fbench >>> round
+(fbench.ackley([1, 1]), 4) 3.6254 ``` ## Contributing to fBench Your
+contribution is greatly appreciated! See the following links to help you get
+started: - [Contributing Guide](https://fbench.readthedocs.io/en/latest/
+contributing.html) - [Developer Guide](https://fbench.readthedocs.io/en/latest/
+developers.html) - [Contributor Code of Conduct](https://fbench.readthedocs.io/
+en/latest/conduct.html) ## License `fbench` was created by fBench Developers.
+It is licensed under the terms of the BSD 3-Clause license.
```

