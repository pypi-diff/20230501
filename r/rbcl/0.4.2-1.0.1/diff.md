# Comparing `tmp/rbcl-0.4.2.tar.gz` & `tmp/rbcl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rbcl-0.4.2.tar", last modified: Tue Jan 17 18:54:20 2023, max compression
+gzip compressed data, was "rbcl-1.0.1.tar", last modified: Mon May  1 16:23:23 2023, max compression
```

## Comparing `rbcl-0.4.2.tar` & `rbcl-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-01-17 18:54:20.873003 rbcl-0.4.2/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1093 2022-03-11 05:43:15.000000 rbcl-0.4.2/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8701 2023-01-17 18:54:20.873003 rbcl-0.4.2/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8385 2022-09-19 02:26:07.000000 rbcl-0.4.2/README.rst
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      267 2022-09-17 02:44:20.000000 rbcl-0.4.2/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      157 2023-01-17 18:54:20.877003 rbcl-0.4.2/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8544 2023-01-17 18:40:09.000000 rbcl-0.4.2/setup.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-01-17 18:54:20.873003 rbcl-0.4.2/src/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-01-17 18:54:20.873003 rbcl-0.4.2/src/rbcl/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1182 2022-09-19 00:38:13.000000 rbcl-0.4.2/src/rbcl/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    28148 2022-09-19 02:27:50.000000 rbcl-0.4.2/src/rbcl/rbcl.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2212 2022-09-15 23:39:20.000000 rbcl-0.4.2/src/rbcl/sodium_ffi.h
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      624 2022-09-15 23:39:20.000000 rbcl-0.4.2/src/rbcl/sodium_ffi.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-01-17 18:54:20.873003 rbcl-0.4.2/src/rbcl.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8701 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      325 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      231 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       13 2023-01-17 18:54:20.000000 rbcl-0.4.2/src/rbcl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:23:23.769936 rbcl-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2022-03-11 05:43:15.000000 rbcl-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     9364 2023-05-01 16:23:23.771169 rbcl-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8907 2023-04-24 06:11:43.000000 rbcl-1.0.1/README.rst
+-rw-rw-rw-   0        0        0      292 2023-05-01 16:09:32.000000 rbcl-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      939 2023-05-01 16:23:23.771169 rbcl-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 16:23:23.760061 rbcl-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 16:23:23.763422 rbcl-1.0.1/src/rbcl/
+-rw-rw-rw-   0        0        0     1276 2023-04-23 17:14:19.000000 rbcl-1.0.1/src/rbcl/__init__.py
+-rw-rw-rw-   0        0        0     1129 2023-04-22 01:28:49.000000 rbcl-1.0.1/src/rbcl/_sodium.tmpl
+-rw-rw-rw-   0        0        0    10031 2023-04-24 02:54:05.000000 rbcl-1.0.1/src/rbcl/_sodium_build.py
+-rw-rw-rw-   0        0        0    33672 2023-04-24 02:26:27.000000 rbcl-1.0.1/src/rbcl/rbcl.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:23:23.769936 rbcl-1.0.1/src/rbcl.egg-info/
+-rw-rw-rw-   0        0        0     9364 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      235 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-01 16:23:23.000000 rbcl-1.0.1/src/rbcl.egg-info/top_level.txt
```

### Comparing `rbcl-0.4.2/LICENSE` & `rbcl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rbcl-0.4.2/PKG-INFO` & `rbcl-1.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,161 +1,178 @@
-Metadata-Version: 2.1
-Name: rbcl
-Version: 0.4.2
-Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
-Home-page: https://github.com/nthparty/rbcl
-Author: Nth Party, Ltd.
-Author-email: team@nthparty.com
-License: MIT
-Description-Content-Type: text/x-rst
-Provides-Extra: build
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-====
-rbcl
-====
-
-Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
-   :target: https://badge.fury.io/py/rbcl
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
-   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
-   :target: https://github.com/nthparty/rbcl/actions
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
-   :alt: Coveralls test coverage summary.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__::
-
-    python -m pip install rbcl
-
-The library can be imported in the usual ways::
-
-    import rbcl
-    from rbcl import *
-
-Examples
-^^^^^^^^
-
-A few usage examples are presented below::
-
-    >>> from rbcl import *
-    >>> x = crypto_core_ristretto255_random()
-    >>> assert crypto_core_ristretto255_is_valid_point(x)
-    >>> y = crypto_core_ristretto255_from_hash(b'\xF0'*64)
-    >>> assert crypto_core_ristretto255_is_valid_point(y)
-    >>> z1 = crypto_core_ristretto255_add(x, y)
-    >>> z2 = crypto_core_ristretto255_add(y, x)
-    >>> assert z1 == z2  # Assert that point addition commutes.
-    >>> s1 = crypto_core_ristretto255_scalar_random()
-    >>> s2 = crypto_core_ristretto255_scalar_random()
-    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
-    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
-    >>> assert w1 == w2  # Assert that point multiplication (by a scalar) is repeated addition.
-
-This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
-
-Development, Build, and Manual Installation Instructions
---------------------------------------------------------
-All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.py``. The ``extras_require`` parameter is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Building from Source
-^^^^^^^^^^^^^^^^^^^^
-The library can be built manually from source **within Linux and macOS** using the sequence of commands below::
-
-    python -m pip install .[build]
-    python setup.py bdist_wheel
-
-Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python setup.py bdist_wheel`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location::
-
-    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
-
-The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
-
-Preparation for Local Development
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it)::
-
-    cp build/lib*/rbcl/_sodium*.* src/rbcl
-
-Manual Installation
-^^^^^^^^^^^^^^^^^^^
-Once the package is `built <#building-from-source>`_, it can be installed manually using the command below::
-
-    python -m pip install -f dist . --upgrade
-
-Documentation
-^^^^^^^^^^^^^
-Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../setup.py ../src/rbcl/sodium_ffi.py && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
-
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/rbcl/rbcl.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/rbcl
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``setup.py``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python setup.py sdist
-
-Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain::
-
-    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+====
+rbcl
+====
+
+Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
+   :target: https://badge.fury.io/py/rbcl
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
+   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
+   :target: https://github.com/nthparty/rbcl/actions
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
+   :alt: Coveralls test coverage summary.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__:
+
+.. code-block:: bash
+
+    python -m pip install rbcl
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import rbcl
+    from rbcl import *
+
+Examples
+^^^^^^^^
+
+A few usage examples are presented below:
+
+.. code-block:: python
+
+    >>> from rbcl import *
+    >>> x = crypto_core_ristretto255_random()
+    >>> assert crypto_core_ristretto255_is_valid_point(x)
+    >>> y = crypto_core_ristretto255_from_hash(b'\xF0' * 64)
+    >>> assert crypto_core_ristretto255_is_valid_point(y)
+    >>> z1 = crypto_core_ristretto255_add(x, y)
+    >>> z2 = crypto_core_ristretto255_add(y, x)
+    >>> assert z1 == z2 # Point addition commutes.
+    >>> s1 = crypto_core_ristretto255_scalar_random()
+    >>> s2 = crypto_core_ristretto255_scalar_random()
+    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
+    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
+    >>> assert w1 == w2 # Multiplication of a point by a scalar is repeated addition.
+
+This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
+
+Development, Build, and Manual Installation Instructions
+--------------------------------------------------------
+All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.cfg``. The ``extras_require`` option is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__ (assuming that the library has already been built successfully):
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Building from Source
+^^^^^^^^^^^^^^^^^^^^
+The library can be built manually from source **within Linux and macOS** using the sequence of commands below:
+
+.. code-block:: bash
+
+    python -m pip install .[build]
+    python -m build --sdist --wheel .
+
+Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python -m build --sdist --wheel .`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location:
+
+.. code-block:: bash
+
+    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
+
+The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
+
+Preparation for Local Development
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it):
+
+.. code-block:: bash
+
+    cp build/lib*/rbcl/_sodium.py src/rbcl
+
+Manual Installation
+^^^^^^^^^^^^^^^^^^^
+Once the package is `built <#building-from-source>`_, it can be installed manually using the command below:
+
+.. code-block:: bash
+
+    python -m pip install -f dist . --upgrade
+
+Documentation
+^^^^^^^^^^^^^
+Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../src/rbcl/_sodium_build.py && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
+
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/rbcl/rbcl.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/rbcl src/rbcl/_sodium.tmpl src/rbcl/_sodium_build.py --disable=duplicate-code
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``setup.cfg``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist .
+
+Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain:
+
+.. code-block:: bash
+
+    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `rbcl-0.4.2/README.rst` & `rbcl-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: rbcl
+Version: 1.0.1
+Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
+Home-page: https://github.com/nthparty/rbcl
+Author: Nth Party
+Author-email: team@nthparty.com
+License: MIT
+Requires-Python: >=3.7
+Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 ====
 rbcl
 ====
 
 Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -20,125 +37,159 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
    :target: https://coveralls.io/github/nthparty/rbcl?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__:
+
+.. code-block:: bash
 
     python -m pip install rbcl
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import rbcl
     from rbcl import *
 
 Examples
 ^^^^^^^^
 
-A few usage examples are presented below::
+A few usage examples are presented below:
+
+.. code-block:: python
 
     >>> from rbcl import *
     >>> x = crypto_core_ristretto255_random()
     >>> assert crypto_core_ristretto255_is_valid_point(x)
-    >>> y = crypto_core_ristretto255_from_hash(b'\xF0'*64)
+    >>> y = crypto_core_ristretto255_from_hash(b'\xF0' * 64)
     >>> assert crypto_core_ristretto255_is_valid_point(y)
     >>> z1 = crypto_core_ristretto255_add(x, y)
     >>> z2 = crypto_core_ristretto255_add(y, x)
-    >>> assert z1 == z2  # Assert that point addition commutes.
+    >>> assert z1 == z2 # Point addition commutes.
     >>> s1 = crypto_core_ristretto255_scalar_random()
     >>> s2 = crypto_core_ristretto255_scalar_random()
     >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
     >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
-    >>> assert w1 == w2  # Assert that point multiplication (by a scalar) is repeated addition.
+    >>> assert w1 == w2 # Multiplication of a point by a scalar is repeated addition.
 
 This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
 
 Development, Build, and Manual Installation Instructions
 --------------------------------------------------------
-All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.py``. The ``extras_require`` parameter is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.cfg``. The ``extras_require`` option is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__ (assuming that the library has already been built successfully):
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Building from Source
 ^^^^^^^^^^^^^^^^^^^^
-The library can be built manually from source **within Linux and macOS** using the sequence of commands below::
+The library can be built manually from source **within Linux and macOS** using the sequence of commands below:
+
+.. code-block:: bash
 
     python -m pip install .[build]
-    python setup.py bdist_wheel
+    python -m build --sdist --wheel .
+
+Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python -m build --sdist --wheel .`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location:
 
-Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python setup.py bdist_wheel`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location::
+.. code-block:: bash
 
     wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
 
 The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
 
 Preparation for Local Development
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it)::
+Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it):
 
-    cp build/lib*/rbcl/_sodium*.* src/rbcl
+.. code-block:: bash
+
+    cp build/lib*/rbcl/_sodium.py src/rbcl
 
 Manual Installation
 ^^^^^^^^^^^^^^^^^^^
-Once the package is `built <#building-from-source>`_, it can be installed manually using the command below::
+Once the package is `built <#building-from-source>`_, it can be installed manually using the command below:
+
+.. code-block:: bash
 
     python -m pip install -f dist . --upgrade
 
 Documentation
 ^^^^^^^^^^^^^
-Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../setup.py ../src/rbcl/sodium_ffi.py && make html
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../src/rbcl/_sodium_build.py && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
 Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
 
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/rbcl/rbcl.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
-    python -m pylint src/rbcl
+    python -m pylint src/rbcl src/rbcl/_sodium.tmpl src/rbcl/_sodium_build.py --disable=duplicate-code
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``setup.py``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``setup.cfg``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
-    python setup.py sdist
+    python -m build --sdist .
 
-Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain::
+Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain:
+
+.. code-block:: bash
 
     cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `rbcl-0.4.2/setup.py` & `rbcl-1.0.1/src/rbcl/_sodium_build.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 """
-Setup, package, and build file.
+Script for building a bundled instance of libsodium  (for invocation by
+setuptools via ``setup.cfg``).
 """
 import sys
 import platform
 import os
 import os.path
 import shutil
 import glob
 import subprocess
 import tarfile
 import errno
 import urllib.request
-from distutils.sysconfig import get_config_vars
-from setuptools import Distribution, setup
-from setuptools.command.build_ext import build_ext as _build_ext
-
-try:
-    from setuptools.command.build_clib import build_clib as _build_clib
-except ImportError:
-    from distutils.command.build_clib import build_clib as _build_clib
+from distutils.sysconfig import get_config_vars # pylint: disable=deprecated-module
+import pystache
+from setuptools.command.install import install
 
 def prepare_libsodium_source_tree(libsodium_folder='src/rbcl/libsodium'):
     """
     Retrieve the libsodium source archive and extract it
     to the location used by the build process.
     """
-
     # Return if libsodium source tree has already been prepared.
     if os.path.exists(libsodium_folder) and len(os.listdir(libsodium_folder)) != 0:
         return libsodium_folder
 
     # URL from which libsodium source archive is retrieved,
     # and paths into which it is extracted and then moved.
     url = (
@@ -61,90 +56,148 @@
             member_path = os.path.join(libsodium_tar_gz_folder, member.name)
             abs_directory = os.path.abspath(libsodium_tar_gz_folder)
             abs_target = os.path.abspath(member_path)
             prefix = os.path.commonprefix([abs_directory, abs_target])
             if not prefix == abs_directory:
                 raise PermissionError(
                     'the retrieved libsodium tarball had ' +
-                    'improper paths or a path travesal exploit'
+                    'improper paths or a path traversal exploit'
                 )
 
         libsodium_tar_gz.extractall(libsodium_tar_gz_folder)
 
     # Move the source tree to the destination folder (removing
     # the destination folder first, if it already exists).
     if os.path.exists(libsodium_folder):
         shutil.rmtree(libsodium_folder)
-    shutil.move(
-        libsodium_tar_gz_folder + '/libsodium-1.0.18',
-        libsodium_folder
-    )
+    shutil.move(libsodium_tar_gz_folder + '/libsodium-1.0.18', libsodium_folder)
 
     # Remove the archive and temporary folder.
     os.remove(libsodium_tar_gz_path)
     shutil.rmtree(libsodium_tar_gz_folder)
 
     return libsodium_folder
 
-class Distribution(Distribution):
-    def has_c_libraries(self):
-        # On Windows, only a precompiled dynamic library file is used.
-        return not sys.platform == 'win32'
+def emit_libsodium():
+    """
+    Emit compiled libsodium binary as hexadecimal string in ``_sodium.py`` file.
+    """
+    # Extract path to compiled libsodium binary.
+    path_libsodium = 'build/temp/lib/libsodium.so' # Default for non-Windows builds.
+    if sys.platform == 'win32':
+        path_directory = (
+            os.environ.get('LIB', None)
+            if os.environ.get('LIB', None) is not None else
+            os.path.join(os.environ['WINDIR'], 'System32') # Windows default.
+        )
+        path_libsodium = os.path.join(path_directory, 'libsodium.dll')
+        if not os.path.exists(path_libsodium):
+            raise EnvironmentError(
+                'libsodium DLL not found at ' + path_libsodium + ', ' +
+                'set environment variable $LIB to path of directory ' +
+                'containing libsodium DLL'
+            )
+
+    # pylint: disable=consider-using-with
+    data = {'SODIUM_HEX': open(path_libsodium, 'rb').read().hex()}
+    template = open('build/lib/rbcl/_sodium.tmpl', encoding='utf-8').read()
+
+    # Emit rendered file to build directory.
+    with open('build/lib/rbcl/_sodium.py', 'w', encoding='utf-8') as sodium_out:
+        sodium_out.write(pystache.render(template, data))
+
+def extract_libsodium_from_static_archive(lib_temp: str):
+    """
+    For certain versions of macOS, the ``libsodium.a`` file contains multiple
+    target architectures. Calls to ``subprocess`` are wrapped in a ``try``
+    block because only certain macOS GitHub runners contain these multi-target
+    files.
+    """
+    if platform.processor() == 'arm':
+        try:
+            subprocess.check_call(
+                ['lipo', 'libsodium.a', '-thin', 'arm64', '-output', 'libsodium.a'],
+                cwd=lib_temp
+            )
+        except: # pylint: disable=bare-except
+            pass
+    else:
+        try:
+            subprocess.check_call(
+                ['lipo', 'libsodium.a', '-thin', 'x86_64', '-output', 'libsodium.a'],
+                cwd=lib_temp
+            )
+        except: # pylint: disable=bare-except
+            pass
+
+try:
+    from wheel.bdist_wheel import bdist_wheel
+
+    # Override bdist_wheel options so that output wheel file has platform-specific tags.
+    class BdistWheel(bdist_wheel): # pylint: disable=invalid-name
+        # pylint: disable=missing-class-docstring,missing-function-docstring
+        def finalize_options(self):
+            bdist_wheel.finalize_options(self)
+            self.root_is_pure = False # pylint: disable=attribute-defined-outside-init
+
+        def get_tag(self):
+            python, abi, plat = bdist_wheel.get_tag(self)
+            python, abi = 'py3', 'none'
+            return python, abi, plat
+
+except ImportError:
+    BdistWheel = None # pylint: disable=invalid-name
+
+class Install(install):
+    # pylint: disable=missing-class-docstring,missing-function-docstring
+    BUILD_TEMP = 'build/temp'
 
-class build_clib(_build_clib):
     def get_source_files(self):
         return [
             file
             for i in range(1, 8)
             for file in glob.glob(os.path.relpath('src/rbcl/libsodium' + ('/*' * i)))
         ]
 
-    def build_libraries(self, libraries):
-        raise RuntimeError('`build_libraries` should not be invoked')
-
-    def check_library_list(self, libraries):
-        raise RuntimeError('`check_library_list` should not be invoked')
-
     def get_library_names(self):
         return ['sodium']
 
     def run(self):
+        install.run(self)
+
         # On Windows, only a precompiled dynamic library file is used.
         if sys.platform == 'win32':
+            emit_libsodium()
             return
 
         # Confirm that make utility can be found.
         found = False
         if not os.environ.get('PATH', None) is None:
             for p in os.environ.get('PATH', '').split(os.pathsep):
                 p = os.path.join(p, 'make')
                 if os.access(p, os.X_OK):
                     found = True
-                for e in filter(
-                    None,
-                    os.environ.get('PATHEXT', '').split(os.pathsep)
-                ):
+                for e in filter(None, os.environ.get('PATHEXT', '').split(os.pathsep)):
                     if os.access(p + e, os.X_OK):
                         found = True
         if not found:
             raise RuntimeError('make utility cannot be found')
 
         # Reproduce Python's build environment variables.
         os.environ.update({
             variable: value
             for (variable, value) in get_config_vars().items()
             if (
-                variable in [
-                    'LDFLAGS', 'CFLAGS', 'CC', 'CCSHARED', 'LDSHARED'
-                ] and variable not in os.environ
+                variable in ['LDFLAGS', 'CFLAGS', 'CC', 'CCSHARED', 'LDSHARED'] and
+                variable not in os.environ
             )
         })
 
         # Ensure the temporary build directory exists.
-        build_temp = os.path.abspath(self.build_temp)
+        build_temp = os.path.abspath(Install.BUILD_TEMP)
         try:
             os.makedirs(build_temp)
         except OSError as e:
             if e.errno != errno.EEXIST:
                 raise
 
         # Retrieve (if necessary) and extract the libsodium source tree.
@@ -162,80 +215,37 @@
         subprocess.check_call(
             [os.path.abspath(os.path.relpath('src/rbcl/libsodium/configure'))] +
             [
                 '--disable-shared', '--enable-static',
                 '--disable-debug', '--disable-dependency-tracking', '--with-pic',
             ] +
             (['--disable-ssp'] if platform.system() == 'SunOS' else []) +
-            ['--prefix', os.path.abspath(self.build_clib)],
+            ['--prefix', os.path.abspath(Install.BUILD_TEMP)],
             cwd=build_temp
         )
         make_args = os.environ.get('LIBSODIUM_MAKE_ARGS', '').split()
         subprocess.check_call(['make'] + make_args, cwd=build_temp)
         subprocess.check_call(['make', 'check'] + make_args, cwd=build_temp)
         subprocess.check_call(['make', 'install'] + make_args, cwd=build_temp)
 
-class build_ext(_build_ext):
-    def run(self):
-        if self.distribution.has_c_libraries():
-            build_clib = self.get_finalized_command('build_clib')
-            self.include_dirs.append(os.path.join(build_clib.build_clib, 'include'),)
-            self.library_dirs.insert(0, os.path.join(build_clib.build_clib, 'lib64'),)
-            self.library_dirs.insert(0, os.path.join(build_clib.build_clib, 'lib'),)
-
-        return _build_ext.run(self)
-
-with open('README.rst', 'r') as fh:
-    long_description = fh.read()
-
-name = 'rbcl'
-version = '0.4.2'
-
-setup(
-    name=name,
-    version=version,
-    packages=[name],
-    ext_package=name,
-    install_requires=[
-        'cffi~=1.15',
-        'barriers~=1.0'
-    ],
-    extras_require={
-        'build': [
-            'setuptools~=62.0',
-            'wheel~=0.37',
-            'cffi~=1.15'
-        ],
-        'docs': [
-            'sphinx~=4.2.0',
-            'sphinx-rtd-theme~=1.0.0'
-        ],
-        'test': [
-            'pytest~=7.0',
-            'pytest-cov~=3.0'
-        ],
-        'lint': [
-            'pylint~=2.14.0'
-        ],
-        'coveralls': [
-            'coveralls~=3.3.1'
-        ],
-        'publish': [
-            'twine~=4.0'
-        ]
-    },
-    license='MIT',
-    url='https://github.com/nthparty/rbcl',
-    author='Nth Party, Ltd.',
-    author_email='team@nthparty.com',
-    description='Python library that bundles libsodium and provides ' + \
-                'wrappers for its Ristretto group functions.',
-    long_description=long_description,
-    long_description_content_type='text/x-rst',
-    cffi_modules=['src/rbcl/sodium_ffi.py:sodium_ffi'],
-    cmdclass={
-        'build_clib': build_clib,
-        'build_ext': build_ext,
-    },
-    distclass=Distribution,
-    zip_safe=False
-)
+        # Build dynamic (shared object) library file from the statically compiled
+        # archive binary file.
+        lib_temp = os.path.join(Install.BUILD_TEMP, 'lib')
+
+        # Different macOS GitHub runners contain either single or multi-target static
+        # archives.
+        if sys.platform == 'darwin':
+            extract_libsodium_from_static_archive(lib_temp)
+
+        # Explode the archive into many individual object files.
+        subprocess.check_call(['ar', '-x', 'libsodium.a'], cwd=lib_temp)
+
+        object_file_relpaths = glob.glob(lib_temp + '/*.o')
+        object_file_names = [o.split('/')[-1] for o in object_file_relpaths]
+        # Invoke gcc to (re-)link dynamically.
+        subprocess.check_call(
+            ['gcc', '-shared'] + object_file_names + ['-o', 'libsodium.so'],
+            cwd=lib_temp
+        )
+
+        # Emit libsodium binary to ``_sodium.py`` file as a hex-encoded string.
+        emit_libsodium()
```

### Comparing `rbcl-0.4.2/src/rbcl/__init__.py` & `rbcl-1.0.1/src/rbcl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""Allow users to use functions directly."""
+"""Gives users direct access to functions."""
+from rbcl.rbcl import _sodium # pylint: disable=import-self
+
 from rbcl.rbcl import \
-    crypto_scalarmult_ristretto255, \
-    crypto_scalarmult_ristretto255_allow_scalar_zero, \
-    crypto_scalarmult_ristretto255_BYTES, \
-    crypto_scalarmult_ristretto255_SCALARBYTES, \
-    crypto_scalarmult_ristretto255_base, \
-    crypto_scalarmult_ristretto255_base_allow_scalar_zero, \
+    randombytes_SEEDBYTES, \
     crypto_core_ristretto255_BYTES, \
     crypto_core_ristretto255_HASHBYTES, \
     crypto_core_ristretto255_NONREDUCEDSCALARBYTES, \
     crypto_core_ristretto255_SCALARBYTES, \
-    crypto_core_ristretto255_add, \
-    crypto_core_ristretto255_from_hash, \
+    crypto_scalarmult_ristretto255_BYTES, \
+    crypto_scalarmult_ristretto255_SCALARBYTES, \
+    randombytes, \
+    randombytes_buf_deterministic, \
     crypto_core_ristretto255_is_valid_point, \
     crypto_core_ristretto255_random, \
-    crypto_core_ristretto255_scalar_add, \
-    crypto_core_ristretto255_scalar_complement, \
-    crypto_core_ristretto255_scalar_invert, \
-    crypto_core_ristretto255_scalar_mul, \
-    crypto_core_ristretto255_scalar_negate, \
+    crypto_core_ristretto255_from_hash, \
+    crypto_core_ristretto255_add, \
+    crypto_core_ristretto255_sub, \
     crypto_core_ristretto255_scalar_random, \
     crypto_core_ristretto255_scalar_reduce, \
+    crypto_core_ristretto255_scalar_negate, \
+    crypto_core_ristretto255_scalar_complement, \
+    crypto_core_ristretto255_scalar_invert, \
+    crypto_core_ristretto255_scalar_add, \
     crypto_core_ristretto255_scalar_sub, \
-    crypto_core_ristretto255_sub, \
-    randombytes, \
-    randombytes_buf_deterministic
+    crypto_core_ristretto255_scalar_mul, \
+    crypto_scalarmult_ristretto255_base, \
+    crypto_scalarmult_ristretto255_base_allow_scalar_zero, \
+    crypto_scalarmult_ristretto255, \
+    crypto_scalarmult_ristretto255_allow_scalar_zero
```

### Comparing `rbcl-0.4.2/src/rbcl/rbcl.py` & `rbcl-1.0.1/src/rbcl/rbcl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,712 +1,857 @@
 """
 Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__
 and provides wrappers for its Ristretto group functions.
 
-This library exports wrappers for all libsodium methods related to the Ristretto
-group and random number generation, including all ``crypto_scalarmult_*`` methods
-and the `randombytes*` methods.
+This library exports wrappers for all libsodium functions related to the Ristretto
+group and random element generation, including all functions with names of the form
+``crypto_scalarmult_*`` and relevant functions with names of the form
+``randombytes*``.
 """
 from __future__ import annotations
+from typing import Callable
 import doctest
+import ctypes
+import os
 import pathlib
 from barriers import barriers
 
-VALIDATION_ENABLED = 'site-packages' not in str(pathlib.Path(__file__).resolve())
+try:
+    VALIDATION_ENABLED = 'site-packages' not in str(pathlib.Path(__file__).resolve())
+except NameError: # pragma: no cover
+    VALIDATION_ENABLED = False
 safe = barriers(VALIDATION_ENABLED) @ globals()
 
 try:
-    from rbcl import _sodium # pylint: disable=cyclic-import
-except: # pylint: disable=bare-except # pragma: no cover
     # Support for direct invocation in order to execute doctests.
-    import _sodium
+    from _sodium import _sodium # pylint: disable=cyclic-import
+except: # pylint: disable=bare-except # pragma: no cover
+    from rbcl._sodium import _sodium # pylint: disable=cyclic-import
 
-crypto_scalarmult_ristretto255_BYTES: int = \
-    _sodium.lib.crypto_scalarmult_ristretto255_bytes()
-crypto_scalarmult_ristretto255_SCALARBYTES: int = \
-    _sodium.lib.crypto_scalarmult_ristretto255_scalarbytes()
-crypto_core_ristretto255_BYTES: int = \
-    _sodium.lib.crypto_core_ristretto255_bytes()
-crypto_core_ristretto255_HASHBYTES: int = \
-    _sodium.lib.crypto_core_ristretto255_hashbytes()
-crypto_core_ristretto255_NONREDUCEDSCALARBYTES: int = \
-    _sodium.lib.crypto_core_ristretto255_nonreducedscalarbytes()
-crypto_core_ristretto255_SCALARBYTES: int = \
-    _sodium.lib.crypto_core_ristretto255_scalarbytes()
-randombytes_SEEDBYTES: int = \
-    _sodium.lib.randombytes_seedbytes()
+# Public and private globals (defined within ``_sodium_init`` after libsodium is ready).
+randombytes_SEEDBYTES: int = None
+"""Length of seed for a pseudorandom byte sequence.
 
-def crypto_core_ristretto255_is_valid_point(p):  # (const unsigned char *p);
-    """
-    Check if ``p`` represents a point on the ristretto255 curve, in canonical
-    form, on the main subgroup, and that the point doesn't have a small order.
+:meta hide-value:
+"""
 
-    >>> p = crypto_core_ristretto255_random()
-    >>> crypto_core_ristretto255_is_valid_point(p)
-    True
+crypto_core_ristretto255_BYTES: int = None
+"""Length of a byte sequence that represents a point.
 
-    :param p: a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type p: bytes
-    :return: point validity
-    :rtype: bool
-    """
-    if not isinstance(p, bytes) or len(p) != crypto_core_ristretto255_BYTES:
-        raise TypeError(
-            'Point must be a ' + str(crypto_core_ristretto255_BYTES) +
-            'long bytes sequence'
-        ) # pragma: no cover
+:meta hide-value:
+"""
 
-    rc = _sodium.lib.crypto_core_ristretto255_is_valid_point(p)
-    return rc == 1
+crypto_core_ristretto255_HASHBYTES: int = None
+"""Length of hash digest to use for creating a point.
+
+:meta hide-value:
+"""
+
+crypto_core_ristretto255_NONREDUCEDSCALARBYTES: int = None
+"""
+Length of a byte sequence that represents a scalar (possibly using a
+non-reduced representation).
+
+:meta hide-value:
+"""
+
+crypto_core_ristretto255_SCALARBYTES: int = None
+"""Length of a byte sequence that represents a scalar.
+
+:meta hide-value:
+"""
+
+crypto_scalarmult_ristretto255_BYTES: int = None
+"""
+Length of a byte sequence that represents a point (provided to -- or
+returned by -- a scalar-point multiplication function).
+
+:meta hide-value:
+"""
+
+crypto_scalarmult_ristretto255_SCALARBYTES: int = None
+"""
+Length of a byte sequence that represents a scalar (to be used as
+an input to a scalar-point multiplication function).
 
-def crypto_core_ristretto255_add(p, q):
+:meta hide-value:
+"""
+
+_crypto_core_ristretto255_point_new: Callable[[], bytes] = (
+    lambda: None # pylint: disable=unnecessary-lambda-assignment
+)
+_crypto_core_ristretto255_scalar_new: Callable[[], bytes] = (
+    lambda: None # pylint: disable=unnecessary-lambda-assignment
+)
+_crypto_scalarmult_ristretto255_point_new: Callable[[], bytes] = (
+    lambda: None # pylint: disable=unnecessary-lambda-assignment
+)
+_buffer_create: Callable[[int], bytes] = (
+    lambda size: (ctypes.c_char * size)() # pylint: disable=unnecessary-lambda-assignment
+)
+
+def randombytes(length: int) -> bytes:
     """
-    Add two points on the ristretto255 curve.
+    Return a bytes-like object of length ``length`` containing random bytes
+    from a cryptographically suitable source of randomness.
 
-    Example - Point addition commutes in L:
+    :param length: Length of bytes-like object to return.
 
-    >>> x = crypto_core_ristretto255_random()
-    >>> y = crypto_core_ristretto255_from_hash(b'\x70'*64)
-    >>> z1 = crypto_core_ristretto255_add(x, y)
-    >>> z2 = crypto_core_ristretto255_add(y, x)
-    >>> z1 == z2
+    >>> len(randombytes(14)) == 14
     True
+    >>> r1 = randombytes(14)
+    >>> r2 = randombytes(14)
+    >>> r1 == r2 # Chances of equality succeeding are 1/(2^42).
+    False
+
+    An exception is raised if the input is not valid:
 
-    :param p: a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type p: bytes
-    :param q: a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type q: bytes
-    :return: a point on the ristretto255 curve represented as
-             a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
+    >>> randombytes('abc')
+    Traceback (most recent call last):
+      ...
+    TypeError: length must be an integer
+    >>> randombytes(-1)
+    Traceback (most recent call last):
+      ...
+    ValueError: length must be a non-negative integer
     """
-    if (
-        not isinstance(p, bytes) or len(p) != crypto_core_ristretto255_BYTES or \
-        not isinstance(q, bytes) or len(q) != crypto_core_ristretto255_BYTES
-    ):
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_BYTES} long bytes sequence'
-        ) # pragma: no cover
+    if not isinstance(length, int):
+        raise TypeError('length must be an integer')
+
+    if length < 0:
+        raise ValueError('length must be a non-negative integer')
 
-    r = _sodium.ffi.new('unsigned char[]', crypto_core_ristretto255_BYTES)
-    _sodium.lib.crypto_core_ristretto255_add(r, p, q)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_BYTES)[:]
+    buf = _buffer_create(length)
+    _sodium.randombytes(buf, length)
+    return buf.raw
 
-def crypto_core_ristretto255_sub(p, q):
+def randombytes_buf_deterministic(length: int, seed: bytes) -> bytes:
     """
-    Subtract a point from another on the ristretto255 curve.
+    Return a bytes-like object of length ``length`` containing pseudorandom
+    bytes that have been deterministically generated from the supplied seed
+    (a byte vector of length :obj:`randombytes_SEEDBYTES`).
 
-    Example - Point subtraction is the inverse of addition:
+    :param length: Length of bytes-like object to return.
+    :param seed: Seed to use for generating pseudorandom bytes.
 
-    >>> p = crypto_core_ristretto255_from_hash(b'\x70'*64)
-    >>> mask = crypto_core_ristretto255_random()
-    >>> masked = crypto_core_ristretto255_add(p, mask)
-    >>> unmasked = crypto_core_ristretto255_sub(masked, mask)
-    >>> p == unmasked
+    The example below shows that the first ``32`` bytes from the stream of
+    pseudorandom bytes seeded by ``b'\x70' * 32`` are consistent across
+    invocations:
+
+    >>> r1 = randombytes_buf_deterministic(32, b'\x70' * 32)
+    >>> r2 = randombytes_buf_deterministic(40, b'\x70' * 32)
+    >>> len(r1) == 32
+    True
+    >>> r1 == r2[:32]
     True
 
-    :param p: a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type p: bytes
-    :param q: a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type q: bytes
-    :return: a point on the ristretto255 curve represented as
-             a :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if (
-        not isinstance(p, bytes) or len(p) != crypto_core_ristretto255_BYTES or \
-        not isinstance(q, bytes) or len(q) != crypto_core_ristretto255_BYTES
-    ):
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_BYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new('unsigned char[]', crypto_core_ristretto255_BYTES)
-    _sodium.lib.crypto_core_ristretto255_sub(r, p, q)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_BYTES)[:]
+    An exception is raised if an input is not valid:
 
-def crypto_core_ristretto255_from_hash(h):
+    >>> randombytes_buf_deterministic('abc', b'\x70' * 32)
+    Traceback (most recent call last):
+      ...
+    TypeError: length must be an integer
+    >>> randombytes_buf_deterministic(-1, b'\x70' * 32)
+    Traceback (most recent call last):
+      ...
+    ValueError: length must be a non-negative integer
+    >>> try:
+    ...     randombytes_buf_deterministic(32, 123)
+    ... except TypeError as e:
+    ...     str(e) == 'seed must be a bytes object of length ' + str(randombytes_SEEDBYTES)
+    True
+    >>> try:
+    ...     randombytes_buf_deterministic(32, b'\x70'*16)
+    ... except ValueError as e:
+    ...     str(e) == 'seed must be a bytes object of length ' + str(randombytes_SEEDBYTES)
+    True
+    """
+    if not isinstance(length, int):
+        raise TypeError('length must be an integer')
+
+    if length < 0:
+        raise ValueError('length must be a non-negative integer')
+
+    well_typed = isinstance(seed, bytes)
+    if not well_typed or len(seed) != randombytes_SEEDBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'seed must be a bytes object of length ' +
+            str(randombytes_SEEDBYTES)
+        )
+
+    buf = _buffer_create(length)
+    _sodium.randombytes_buf_deterministic(buf, length, seed)
+    return buf.raw
+
+def crypto_core_ristretto255_is_valid_point(p: bytes) -> bool:
     """
-    Map a 64-byte vector ``h`` (usually the output of a hash function) to a ristretto255
-    group element (a point), and output its representation in bytes.
+    Return a boolean indiciating whether ``p`` is a representation of a valid
+    point on the main subgroup (in canonical form) and that the point does not
+    have a small order.
 
-    >>> p = crypto_core_ristretto255_from_hash(b'\x70'*64)
+    :param p: Byte vector of length :obj:`crypto_core_ristretto255_BYTES`.
+
+    >>> p = crypto_core_ristretto255_random()
     >>> crypto_core_ristretto255_is_valid_point(p)
     True
 
-    :param h: a :py:data:`.crypto_core_ristretto255_HASHBYTES`
-              long bytes sequence ideally representing a hash digest
-    :type h: bytes
+    For this and other functions that operate on points, a descriptive exception
+    is raised if an input is not valid:
 
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
+    >>> try:
+    ...     crypto_core_ristretto255_is_valid_point(123)
+    ... except TypeError as e:
+    ...     str(e) == (
+    ...         'point must be a bytes object of length ' +
+    ...         str(crypto_core_ristretto255_BYTES)
+    ...     )
+    True
+    >>> try:
+    ...     crypto_core_ristretto255_is_valid_point(bytes([0, 0 ,0]))
+    ... except ValueError as e:
+    ...     str(e) == (
+    ...         'point must be a bytes object of length ' +
+    ...         str(crypto_core_ristretto255_BYTES)
+    ...     )
+    True
     """
-    if not isinstance(h, bytes) or len(
-            h) != crypto_core_ristretto255_HASHBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_HASHBYTES} long bytes sequence'
-        ) # pragma: no cover
+    well_typed = isinstance(p, bytes)
+    if not well_typed or len(p) != crypto_core_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'point must be a bytes object of length ' +
+            str(crypto_core_ristretto255_BYTES)
+        )
 
-    r = _sodium.ffi.new('unsigned char[]', crypto_core_ristretto255_BYTES)
-    _sodium.lib.crypto_core_ristretto255_from_hash(r, h)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_BYTES)[:]
+    rc = _sodium.crypto_core_ristretto255_is_valid_point(p)
+    return rc == 1
 
-def crypto_core_ristretto255_random():
+def crypto_core_ristretto255_random() -> bytes:
     """
-    Returns a ristretto255 group element (point).
+    Return a valid random point (represented as a byte vector of length
+    :obj:`crypto_core_ristretto255_BYTES`).
 
     >>> p = crypto_core_ristretto255_random()
     >>> crypto_core_ristretto255_is_valid_point(p)
     True
+    """
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_random(r)
+    return r.raw
+
+def crypto_core_ristretto255_from_hash(h: bytes) -> bytes:
+    """
+    Map a 64-byte vector ``h`` (usually the output of a hash function) to a
+    a point (represented as a byte vector of length
+    :obj:`crypto_core_ristretto255_BYTES`).
+
+    :param h: Byte vector of length :obj:`crypto_core_ristretto255_HASHBYTES`
+        (usually representing a hash digest).
+
+    >>> p = crypto_core_ristretto255_from_hash(b'\x70'*64)
+    >>> crypto_core_ristretto255_is_valid_point(p)
+    True
+    """
+    well_typed = isinstance(h, bytes)
+    if not well_typed or len(h) != crypto_core_ristretto255_HASHBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'input must be a bytes object of length ' +
+            str(crypto_core_ristretto255_HASHBYTES)
+        ) # pragma: no cover
 
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_random(r)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
-
-def crypto_core_ristretto255_scalar_random():  # (unsigned char *r);
-    """
-    Returns a :py:data:`.crypto_core_ristretto255_SCALARBYTES` byte long
-    representation of the scalar in the ``[0..L]`` interval, ``L`` being the
-    order of the group ``(2^252 + 27742317777372353535851937790883648493)``.
+    r = _crypto_core_ristretto255_point_new()
+    _sodium.crypto_core_ristretto255_from_hash(r, h)
+    return r.raw
 
-    Example - All valid scalars have an inverse:
+def crypto_core_ristretto255_add(p: bytes, q: bytes) -> bytes:
+    """
+    Add two points ``p`` and ``q`` and return their sum (represented as
+    a byte vector of length :obj:`crypto_core_ristretto255_BYTES`).
+
+    :param p: Byte vector of length :obj:`crypto_core_ristretto255_BYTES`
+        representing a point.
+    :param q: Byte vector of length :obj:`crypto_core_ristretto255_BYTES`
+        representing a point.
+
+    Addition of points is commutative:
 
-    >>> s = crypto_core_ristretto255_scalar_random()
     >>> p = crypto_core_ristretto255_random()
-    >>> masked = crypto_scalarmult_ristretto255(s, p)
-    >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
-    >>> unmasked = crypto_scalarmult_ristretto255(s_inv, masked)
-    >>> unmasked == p
+    >>> q = crypto_core_ristretto255_from_hash(b'\x70'*64)
+    >>> pq = crypto_core_ristretto255_add(p, q)
+    >>> qp = crypto_core_ristretto255_add(q, p)
+    >>> pq == qp
     True
+    """
+    well_typed = isinstance(p, bytes)
+    if not well_typed or len(p) != crypto_core_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each point must be a bytes object of length ' +
+            str(crypto_core_ristretto255_BYTES)
+        ) # pragma: no cover
 
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_random(r)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
-
-def crypto_core_ristretto255_scalar_invert(p):
-    """
-    Return the multiplicative inverse of integer ``s`` modulo ``L``,
-    i.e an integer ``i`` such that ``s * i = 1 (mod L)``, where ``L``
-    is the order of the main subgroup.
+    well_typed = isinstance(q, bytes)
+    if not well_typed or len(q) != crypto_core_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each point must be a bytes object of length ' +
+            str(crypto_core_ristretto255_BYTES)
+        ) # pragma: no cover
+
+    r = _crypto_core_ristretto255_point_new()
+    _sodium.crypto_core_ristretto255_add(r, p, q)
+    return r.raw
 
-    Example - All scalars have a multiplicative inverse:
+def crypto_core_ristretto255_sub(p: bytes, q: bytes) -> bytes:
+    """
+    Subtract a point ``q`` from a point ``p`` and return their difference
+    (represented as a byte vector of length :obj:`crypto_core_ristretto255_BYTES`).
+
+    :param p: Byte vector of length :obj:`crypto_core_ristretto255_BYTES`
+        representing a point.
+    :param q: Byte vector of length :obj:`crypto_core_ristretto255_BYTES`
+        representing a point.
+
+    Subtraction between points is the inverse of point addition:
+
+    >>> p = crypto_core_ristretto255_from_hash(b'\x70'*64)
+    >>> q = crypto_core_ristretto255_random()
+    >>> masked = crypto_core_ristretto255_add(p, q)
+    >>> unmasked = crypto_core_ristretto255_sub(masked, q)
+    >>> p == unmasked
+    True
+    """
+    well_typed = isinstance(p, bytes)
+    if not well_typed or len(p) != crypto_core_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each point must be a bytes object of length ' +
+            str(crypto_core_ristretto255_BYTES)
+        ) # pragma: no cover
+
+    well_typed = isinstance(q, bytes)
+    if not well_typed or len(q) != crypto_core_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each point must be a bytes object of length ' +
+            str(crypto_core_ristretto255_BYTES)
+        ) # pragma: no cover
+
+    r = _crypto_core_ristretto255_point_new()
+    _sodium.crypto_core_ristretto255_sub(r, p, q)
+    return r.raw
+
+def crypto_core_ristretto255_scalar_random() -> bytes:
+    """
+    Return a random scalar, represented as a byte vector of length
+    :obj:`crypto_core_ristretto255_SCALARBYTES`.
 
     >>> s = crypto_core_ristretto255_scalar_random()
+    >>> len(s) == crypto_core_ristretto255_SCALARBYTES
+    True
+
+    When interpreted as an integer, the scalar is guaranteed to be
+    less than the order of the group (*i.e.*,
+    ``2^252 + 27742317777372353535851937790883648493``).
+    """
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_random(r)
+    return r.raw
+
+def crypto_core_ristretto255_scalar_reduce(s: bytes) -> bytes:
+    """
+    Given a byte vector of length :obj:`crypto_core_ristretto255_NONREDUCEDSCALARBYTES`
+    representing a scalar, return its reduced representation ``s`` modulo ``L``
+    (where ``L`` is the order of the main subgroup) as a byte vector of length
+    :obj:`crypto_core_ristretto255_SCALARBYTES` .
+
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_NONREDUCEDSCALARBYTES`
+        representing a scalar.
+
+    In the example below, a large integer representing a scalar is reduced to
+    a valid scalar:
+
+    >>> x = bytes.fromhex('FF' * 32)
+    >>> s = crypto_core_ristretto255_scalar_reduce(x)
     >>> p = crypto_core_ristretto255_random()
     >>> masked = crypto_scalarmult_ristretto255(s, p)
     >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
     >>> unmasked = crypto_scalarmult_ristretto255(s_inv, masked)
     >>> unmasked == p
     True
 
-    Raises a ``RuntimeError`` if ``s`` is the integer zero.
+    For this and other functions that operate on points, a descriptive exception
+    is raised if an input is not valid:
 
-    :param s: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type s: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(p, bytes) or len(
-            p) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_invert(r, p)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    >>> try:
+    ...     crypto_core_ristretto255_scalar_reduce(123)
+    ... except TypeError as e:
+    ...     str(e) == (
+    ...         'scalar must be a bytes object of length ' +
+    ...         str(crypto_core_ristretto255_SCALARBYTES)
+    ...     )
+    True
+    >>> try:
+    ...     crypto_core_ristretto255_scalar_reduce(bytes([0, 0 ,0]))
+    ... except ValueError as e:
+    ...     str(e) == (
+    ...         'scalar must be a bytes object of length ' +
+    ...         str(crypto_core_ristretto255_SCALARBYTES)
+    ...     )
+    True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        )
 
-def crypto_core_ristretto255_scalar_negate(p):
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_reduce(r, s)
+    return r.raw
+
+def crypto_core_ristretto255_scalar_negate(s: bytes) -> bytes:
     """
-    Return the integer ``n`` such that ``s + n = 0 (mod L)``, where ``L``
-    is the order of the main subgroup.
+    Return the additive inverse of the scalar ``s`` modulo ``L`` (*i.e.*,
+    a scalar ``t`` such that ``s + t == 0`` modulo ``L``, where ``L`` is the
+    order of the main subgroup). The input and output are each represented as
+    a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`.
+
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
 
-    Example - All scalars have an additive inverse:
+    All scalars have an additive inverse:
 
     >>> s = crypto_core_ristretto255_scalar_random()
-    >>> s_inv = crypto_core_ristretto255_scalar_negate(s)
-    >>> zero = crypto_core_ristretto255_scalar_add(s, s_inv)
+    >>> t = crypto_core_ristretto255_scalar_negate(s)
+    >>> zero = crypto_core_ristretto255_scalar_add(s, t)
     >>> s == crypto_core_ristretto255_scalar_add(s, zero)
     True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_negate(r, s)
+    return r.raw
+
+def crypto_core_ristretto255_scalar_complement(s: bytes) -> bytes:
+    """
+    Return the additive complement of the scalar ``s`` modulo ``L`` (*i.e.*,
+    a scalar ``t`` such that ``s + t == 1`` modulo ``L``, where ``L`` is the
+    order of the main subgroup). The input and output are each represented as
+    a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`.
 
-    Example - Multiplication by zero is not defined in the subgroup {point * s | scalars s}:
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
 
+    All scalars have an additive complement:
+
+    >>> s = crypto_core_ristretto255_scalar_random()
+    >>> t = crypto_core_ristretto255_scalar_complement(s)
+    >>> one = crypto_core_ristretto255_scalar_add(s, t)
     >>> p = crypto_core_ristretto255_random()
-    >>> try:
-    ...     zero_p = crypto_scalarmult_ristretto255(zero, p)
-    ... except RuntimeError as e:
-    ...     str(e) == '`n` cannot be larger than the size of ' + \
-                      'the group or p^n is the identity element'
+    >>> p == crypto_scalarmult_ristretto255(one, p)
     True
-
-    :param s: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type s: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
     """
-    if not isinstance(p, bytes) or len(
-            p) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
         ) # pragma: no cover
 
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_negate(r, p)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_complement(r, s)
+    return r.raw
 
-def crypto_core_ristretto255_scalar_complement(p):
+def crypto_core_ristretto255_scalar_invert(s: bytes) -> bytes:
     """
-    Return the complement of integer ``s`` modulo ``L``, i.e. an integer
-    ``c`` such that ``s + c = 1 (mod L)``, where ``L`` is the order of
-    the main subgroup.
+    Return the multiplicative inverse of the scalar ``s`` modulo ``L``
+    (*i.e.*, an integer ``t`` such that ``s * t == 1`` modulo ``L``, where
+    ``L`` is the order of the main subgroup). The input and output are each
+    represented as a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`.
 
-    Example - All scalars have an additive complement:
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
+
+    All scalars have a multiplicative inverse:
 
     >>> s = crypto_core_ristretto255_scalar_random()
-    >>> s_comp = crypto_core_ristretto255_scalar_complement(s)
-    >>> one = crypto_core_ristretto255_scalar_add(s, s_comp)
     >>> p = crypto_core_ristretto255_random()
-    >>> p == crypto_scalarmult_ristretto255(one, p)
+    >>> masked = crypto_scalarmult_ristretto255(s, p)
+    >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
+    >>> unmasked = crypto_scalarmult_ristretto255(s_inv, masked)
+    >>> unmasked == p
     True
 
-    :param s: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type s: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(p, bytes) or len(
-            p) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_complement(r, p)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    If ``s`` is the zero scalar, an exception is raised.
 
-def crypto_core_ristretto255_scalar_add(p, q):
+    >>> crypto_core_ristretto255_scalar_invert(bytes([0] * 32))
+    Traceback (most recent call last):
+      ...
+    ValueError: scalar must not be zero
     """
-    Add integers ``p`` and ``q`` modulo ``L``, where ``L`` is the order of
-    the main subgroup.
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    if sum(s) == 0:
+        raise ValueError('scalar must not be zero')
 
-    Example - Addition of two scalars is commutative:
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_invert(r, s)
+    return r.raw
+
+def crypto_core_ristretto255_scalar_add(s: bytes, t: bytes) -> bytes:
+    """
+    Add two scalars ``s`` and ``t`` modulo ``L`` (where ``L`` is the order
+    of the main subgroup) and return their scalar product (represented as
+    a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`).
+
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
+    :param t: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
+
+    Addition of scalars is commutative:
 
     >>> s1 = crypto_core_ristretto255_scalar_random()
     >>> s2 = crypto_core_ristretto255_scalar_random()
     >>> s12 = crypto_core_ristretto255_scalar_add(s1, s2)
     >>> s21 = crypto_core_ristretto255_scalar_add(s2, s1)
     >>> s12 == s21
     True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    :param p: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type p: bytes
-    :param q: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type q: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(
-            p, bytes) or len(p) != crypto_core_ristretto255_SCALARBYTES or not isinstance(
-            q, bytes) or len(q) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_add(r, p, q)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    well_typed = isinstance(t, bytes)
+    if not well_typed or len(t) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_add(r, s, t)
+    return r.raw
 
-def crypto_core_ristretto255_scalar_sub(p, q):
+def crypto_core_ristretto255_scalar_sub(s: bytes, t: bytes) -> bytes:
     """
-    Subtract integers ``p`` and ``q`` modulo ``L``, where ``L`` is the
-    order of the main subgroup.
+    Subtract a scalar ``t`` from a scalar ``s`` modulo ``L`` (where ``L`` is
+    the order of the main subgroup) and return their difference (represented
+    as a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`).
+
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
+    :param t: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
 
-    Example - Subtraction is the inverse of addition:
+    Subtraction between scalars is the inverse of scalar addition:
 
     >>> s1 = crypto_core_ristretto255_scalar_random()
     >>> s2 = crypto_core_ristretto255_scalar_random()
     >>> s1_plus_s2 = crypto_core_ristretto255_scalar_add(s1, s2)
     >>> s1 == crypto_core_ristretto255_scalar_sub(s1_plus_s2, s2)
     True
+    """
+    well_typed = isinstance(s, bytes)
+    if not isinstance(s, bytes) or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    well_typed = isinstance(t, bytes)
+    if not isinstance(t, bytes) or len(t) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    :param p: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type p: bytes
-    :param q: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type q: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(
-            p, bytes) or len(p) != crypto_core_ristretto255_SCALARBYTES or not isinstance(
-            q, bytes) or len(q) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_sub(r, p, q)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_sub(r, s, t)
+    return r.raw
 
-def crypto_core_ristretto255_scalar_mul(p, q):
+def crypto_core_ristretto255_scalar_mul(s: bytes, t: bytes) -> bytes:
     """
-    Multiply integers ``p`` and ``q`` modulo ``L``, where ``L`` is the
-    order of the main subgroup.
+    Multiply two scalars ``s`` and ``t`` modulo ``L`` (where ``L`` is the
+    order of the main subgroup) and return their scalar product (represented
+    as a byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`).
+
+    :param s: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
+    :param t: Byte vector of length :obj:`crypto_core_ristretto255_SCALARBYTES`
+        representing a scalar.
 
-    Example - Multiplication of two scalars is commutative:
+    Multiplication of two scalars is commutative:
 
     >>> s1 = crypto_core_ristretto255_scalar_random()
     >>> s2 = crypto_core_ristretto255_scalar_random()
     >>> s1s2 = crypto_core_ristretto255_scalar_mul(s1, s2)
     >>> s2s1 = crypto_core_ristretto255_scalar_mul(s2, s1)
     >>> s1s2 == s2s1
     True
-
-    :param p: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type p: bytes
-    :param q: a :py:data:`.crypto_core_ristretto255_SCALARBYTES`
-              long bytes sequence representing an integer
-    :type q: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(
-            p, bytes) or len(p) != crypto_core_ristretto255_SCALARBYTES or not isinstance(
-            q, bytes) or len(q) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_mul(r, p, q)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
-
-def crypto_core_ristretto255_scalar_reduce(p):
     """
-    Reduce integer ``s`` to ``s`` modulo ``L``, where ``L`` is the order
-    of the main subgroup.
-
-    Example - Reduce a large value to a valid scalar:
+    well_typed = isinstance(s, bytes)
+    if not isinstance(s, bytes) or len(s) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    >>> x = bytes.fromhex('FF'*32)
-    >>> s = crypto_core_ristretto255_scalar_reduce(x)
-    >>> p = crypto_core_ristretto255_random()
-    >>> masked = crypto_scalarmult_ristretto255(s, p)
-    >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
-    >>> unmasked = crypto_scalarmult_ristretto255(s_inv, masked)
-    >>> unmasked == p
-    True
+    well_typed = isinstance(t, bytes)
+    if not isinstance(t, bytes) or len(t) != crypto_core_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'each scalar must be a bytes object of length ' +
+            str(crypto_core_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    :param s: a :py:data:`.crypto_core_ristretto255_NONREDUCEDSCALARBYTES`
-              long bytes sequence representing an integer
-    :type s: bytes
-    :return: an integer represented as a
-              :py:data:`.crypto_core_ristretto255_SCALARBYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(p, bytes) or len(
-            p) != crypto_core_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Each integer must be a {crypto_core_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    r = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_core_ristretto255_SCALARBYTES
-    )
-    _sodium.lib.crypto_core_ristretto255_scalar_reduce(r, p)
-    return _sodium.ffi.buffer(r, crypto_core_ristretto255_SCALARBYTES)[:]
+    r = _crypto_core_ristretto255_scalar_new()
+    _sodium.crypto_core_ristretto255_scalar_mul(r, s, t)
+    return r.raw
 
-def crypto_scalarmult_ristretto255_base(n):
+def crypto_scalarmult_ristretto255_base(s: bytes) -> bytes:
     """
-    Computes and returns the scalar product of a standard group element and an
-    integer ``n`` on the ristretto255 curve.
+    Compute and return the product (represented as a byte vector of length
+    :obj:`crypto_scalarmult_ristretto255_BYTES`) of a standard group element
+    and a scalar ``s``. 
+
+    :param s: Byte vector of length :obj:`crypto_scalarmult_ristretto255_SCALARBYTES`
+        representing a scalar.
 
     >>> s = crypto_core_ristretto255_scalar_random()
     >>> gs = crypto_scalarmult_ristretto255_base(s)
     >>> crypto_core_ristretto255_is_valid_point(gs)
     True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_scalarmult_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    :param n: a :py:data:`.crypto_scalarmult_ristretto255_SCALARBYTES` long bytes
-              sequence representing a scalar
-    :type n: bytes
-    :return: a point on the ristretto255 curve, represented as a
-             :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(n, bytes) or len(
-            n) != crypto_scalarmult_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    q = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_scalarmult_ristretto255_BYTES
-    )
-    if _sodium.lib.crypto_scalarmult_ristretto255_base(q, n) == -1:
+    q = _crypto_scalarmult_ristretto255_point_new()
+    if _sodium.crypto_scalarmult_ristretto255_base(q, s) == -1:
         raise RuntimeError(
-            '`n` cannot be larger than the size of the group or g^n is the identity element'
+            'input cannot be larger than the size of the group and ' +
+            'cannot yield the identity element when applied as an exponent'
         ) # pragma: no cover
 
-    return _sodium.ffi.buffer(q, crypto_scalarmult_ristretto255_BYTES)[:]
+    return q.raw
 
-def crypto_scalarmult_ristretto255_base_allow_scalar_zero(n):
+def crypto_scalarmult_ristretto255_base_allow_scalar_zero(s: bytes) -> bytes:
     """
-    Computes and returns the scalar product of a standard group element and an
-    integer ``n`` on the ristretto255 curve.  Zero-valued scalars are allowed.
+    Compute and return the product (represented as a byte vector of length
+    :obj:`crypto_scalarmult_ristretto255_BYTES`) of a standard group element
+    and a scalar ``s``. Zero-valued scalars are permitted.
+
+    :param s: Byte vector of length :obj:`crypto_scalarmult_ristretto255_SCALARBYTES`
+        representing a scalar.
 
     >>> s = crypto_core_ristretto255_scalar_random()
     >>> gs = crypto_scalarmult_ristretto255_base_allow_scalar_zero(s)
     >>> crypto_core_ristretto255_is_valid_point(gs)
     True
     >>> crypto_scalarmult_ristretto255_base_allow_scalar_zero(
-    ...   crypto_core_ristretto255_scalar_sub(s, s)
+    ...     crypto_core_ristretto255_scalar_sub(s, s)
     ... ) == crypto_core_ristretto255_sub(gs, gs)
     True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_scalarmult_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    q = _crypto_scalarmult_ristretto255_point_new()
 
-    :param n: a :py:data:`.crypto_scalarmult_ristretto255_SCALARBYTES` long bytes
-              sequence representing a scalar
-    :type n: bytes
-    :return: a point on the ristretto255 curve, represented as a
-             :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(n, bytes) or len(
-            n) != crypto_scalarmult_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    q = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_scalarmult_ristretto255_BYTES
-    )
-
-    # If ``-1``, then ``q`` remains cleared (``b'\0'*32``).
-    _sodium.lib.crypto_scalarmult_ristretto255_base(q, n)
-    return _sodium.ffi.buffer(q, crypto_scalarmult_ristretto255_BYTES)[:]
+    # If the below returns ``-1``, then ``q`` remains cleared (``b'\0' * 32``).
+    _sodium.crypto_scalarmult_ristretto255_base(q, s)
+    return q.raw
 
-def crypto_scalarmult_ristretto255(n, p):
+def crypto_scalarmult_ristretto255(s: bytes, p: bytes) -> bytes:
     """
-    Computes and returns the scalar product of a *clamped* integer ``n``
-    and the given group element on the ristretto255 curve.
+    Compute and return the product (represented as a byte vector of length
+    :obj:`crypto_scalarmult_ristretto255_BYTES`) of a *clamped* integer ``s``
+    and the provided point (*i.e.*, group element).
+
+    :param s: Byte vector of length :obj:`crypto_scalarmult_ristretto255_SCALARBYTES`
+        representing a scalar.
+    :param p: Byte vector of length :obj:`crypto_scalarmult_ristretto255_BYTES`
+        representing a valid point.
+
     The scalar is clamped, as done in the public key generation case,
-    by setting to zero the bits in position [0, 1, 2, 255] and setting
-    to one the bit in position 254.
+    by setting to zero the bits in position ``[0, 1, 2, 255]`` and by
+    setting to ``1`` the bit in position ``254``.
 
-    Example - Scalar multiplication is an invertible operation:
+    Scalar multiplication is an invertible operation:
 
     >>> s = crypto_core_ristretto255_scalar_random()
     >>> p = crypto_core_ristretto255_random()
     >>> masked = crypto_scalarmult_ristretto255(s, p)
     >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
     >>> unmasked = crypto_scalarmult_ristretto255(s_inv, masked)
     >>> unmasked == p
     True
 
-    :param n: a :py:data:`.crypto_scalarmult_ristretto255_SCALARBYTES` long bytes
-              sequence representing a scalar
-    :type n: bytes
-    :param p: a :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type p: bytes
-    :return: a point on the ristretto255 curve, represented as a
-             :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(n, bytes) or len(
-            n) != crypto_scalarmult_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    if not isinstance(p, bytes) or len(
-            p) != crypto_scalarmult_ristretto255_BYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_BYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    q = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_scalarmult_ristretto255_BYTES
-    )
-    if _sodium.lib.crypto_scalarmult_ristretto255(q, n, p) == -1:
+    Multiplication by the zero scalar is not defined in the subgroup consisting
+    of products of valid points and scalars:
+
+    >>> p = crypto_core_ristretto255_random()
+    >>> s = crypto_core_ristretto255_scalar_random()
+    >>> t = crypto_core_ristretto255_scalar_negate(s)
+    >>> zero = crypto_core_ristretto255_scalar_add(s, t)
+    >>> try:
+    ...     crypto_scalarmult_ristretto255(zero, p)
+    ... except RuntimeError as e:
+    ...     str(e) == (
+    ...         'input cannot be larger than the size of the group and ' +
+    ...         'cannot yield the identity element when applied as an exponent'
+    ...     )
+    True
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_scalarmult_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
+
+    well_typed = isinstance(p, bytes)
+    if not well_typed or len(p) != crypto_scalarmult_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'point must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_BYTES)
+        ) # pragma: no cover
+
+    q = _crypto_scalarmult_ristretto255_point_new()
+    if _sodium.crypto_scalarmult_ristretto255(q, s, p) == -1:
         raise RuntimeError(
-            '`n` cannot be larger than the size of the group or p^n is the identity element'
+            'input cannot be larger than the size of the group and ' +
+            'cannot yield the identity element when applied as an exponent'
         )
-    return _sodium.ffi.buffer(q, crypto_scalarmult_ristretto255_BYTES)[:]
+
+    return q.raw
 
 @safe
 def crypto_scalarmult_ristretto255_allow_scalar_zero(
-        n, p
-    ): # pragma: no cover # The decorator recompiles this function body.
+        s: bytes, p: bytes
+    ) -> bytes: # pragma: no cover # The decorator recompiles this function body.
     """
-    Computes and returns the scalar product of a *clamped* integer ``n``
-    and the given group element on the ristretto255 curve.
+    Compute and return the product (represented as a byte vector of length
+    :obj:`crypto_scalarmult_ristretto255_BYTES`) of a *clamped* integer
+    ``s`` and the provided point (*i.e.*, group element).
+
+    :param s: Byte vector of length :obj:`crypto_scalarmult_ristretto255_SCALARBYTES`
+        representing a scalar.
+    :param p: Byte vector of length :obj:`crypto_scalarmult_ristretto255_BYTES`
+        representing a valid point.
+
     The scalar is clamped, as done in the public key generation case,
-    by setting to zero the bits in position [0, 1, 2, 255] and setting
-    to one the bit in position 254.  Zero-valued scalars are allowed.
+    by setting to zero the bits in position ``[0, 1, 2, 255]`` and by
+    setting to ``1`` the bit in position ``254``. Zero-valued scalars
+    are permitted.
 
-    Example - Scalar multiplication is an invertible operation:
+    Scalar multiplication is an invertible operation:
 
     >>> s = crypto_core_ristretto255_scalar_random()
     >>> p = crypto_core_ristretto255_random()
     >>> masked = crypto_scalarmult_ristretto255_allow_scalar_zero(s, p)
     >>> s_inv = crypto_core_ristretto255_scalar_invert(s)
     >>> unmasked = crypto_scalarmult_ristretto255_allow_scalar_zero(s_inv, masked)
     >>> unmasked == p
     True
 
-    Example - Multiplication by zero is allowed:
+    Multiplication by the zero scalar is permitted:
 
     >>> zero_scalar, zero_point = bytes(32), bytes(32)
     >>> crypto_scalarmult_ristretto255_allow_scalar_zero(zero_scalar, p) == zero_point
     True
 
-    Example - The scalar being zero does not raise an error, but the point being invalid does:
+    While the scalar input can be zero, the provided point must be valid:
 
-    >>> invalid_point = b'\1'*32
+    >>> invalid_point = b'\1' * 32
     >>> crypto_scalarmult_ristretto255_allow_scalar_zero(zero_scalar, invalid_point)
     Traceback (most recent call last):
       ...
-    TypeError: The second input must represent a valid Ristretto255 point
+    TypeError: second input must represent a valid point
+    """
+    well_typed = isinstance(s, bytes)
+    if not well_typed or len(s) != crypto_scalarmult_ristretto255_SCALARBYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'scalar must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_SCALARBYTES)
+        ) # pragma: no cover
 
-    :param n: a :py:data:`.crypto_scalarmult_ristretto255_SCALARBYTES` long bytes
-              sequence representing a scalar
-    :type n: bytes
-    :param p: a :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-              representing a point on the ristretto255 curve
-    :type p: bytes
-    :return: a point on the ristretto255 curve, represented as a
-             :py:data:`.crypto_scalarmult_ristretto255_BYTES` long bytes sequence
-    :rtype: bytes
-    """
-    if not isinstance(n, bytes) or len(n) != crypto_scalarmult_ristretto255_SCALARBYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_SCALARBYTES} long bytes sequence'
-        ) # pragma: no cover
-
-    if not isinstance(p, bytes) or len(p) != crypto_scalarmult_ristretto255_BYTES:
-        raise TypeError(
-            f'Input must be a {crypto_scalarmult_ristretto255_BYTES} long bytes sequence'
+    well_typed = isinstance(p, bytes)
+    if not well_typed or len(p) != crypto_scalarmult_ristretto255_BYTES:
+        raise (ValueError if well_typed else TypeError)(
+            'point must be a bytes object of length ' +
+            str(crypto_scalarmult_ristretto255_BYTES)
         ) # pragma: no cover
 
     safe # pylint: disable=pointless-statement # Marker for ``barriers`` decorator ``safe``.
     if not crypto_core_ristretto255_is_valid_point(p):
-        raise TypeError('The second input must represent a valid Ristretto255 point')
-
-    q = _sodium.ffi.new(
-        'unsigned char[]',
-        crypto_scalarmult_ristretto255_BYTES
-    )
+        raise TypeError('second input must represent a valid point')
 
-    # If ``-1``, then ``q`` remains cleared (``b'\0'*32``).
-    _sodium.lib.crypto_scalarmult_ristretto255(q, n, p)
-    return _sodium.ffi.buffer(q, crypto_scalarmult_ristretto255_BYTES)[:]
-
-def randombytes(size):
-    """
-    Returns ``size`` number of random bytes from a cryptographically secure
-    random source.
-
-    >>> r1 = randombytes(14)
-    >>> r2 = randombytes(14)
-    >>> r1 == r2  # 2^42 chance of one-off event (i.e. equality)
-    False
-
-    :param size: int
-    :rtype: bytes
-    """
-    buf = _sodium.ffi.new('unsigned char[]', size)
-    _sodium.lib.randombytes(buf, size)
-    return _sodium.ffi.buffer(buf, size)[:]
-
-def randombytes_buf_deterministic(size, seed):
-    """
-    Returns ``size`` number of deterministically generated pseudorandom bytes
-    from a seed
-
-    Example - Get the first 32 bytes from a stream seeded by 0x7070...70:
-
-    >>> r1 = randombytes_buf_deterministic(32, b'\x70'*32)
-    >>> r2 = randombytes_buf_deterministic(40, b'\x70'*32)
-    >>> r1 == r2[:32]
-    True
-
-    :param size: int
-    :param seed: bytes
-    :rtype: bytes
-    """
-    if len(seed) != randombytes_SEEDBYTES:
-        raise TypeError( # pragma: no cover
-            'Deterministic random bytes must be generated from 32 bytes'
-        )
-
-    buf = _sodium.ffi.new('unsigned char[]', size)
-    _sodium.lib.randombytes_buf_deterministic(buf, size, seed)
-    return _sodium.ffi.buffer(buf, size)[:]
-
-# Initializes sodium, picking the best implementations available for this
-# machine.
-
-def _sodium_init():
-    if _sodium.lib.sodium_init() == -1:
-        raise RuntimeError( # pragma: no cover
-            'libsodium error during initialization'
-        )
+    q = _crypto_scalarmult_ristretto255_point_new()
 
-_sodium.ffi.init_once(_sodium_init, 'libsodium')
+    # If ``-1``, then ``q`` remains cleared (``b'\0' * 32``).
+    _sodium.crypto_scalarmult_ristretto255(q, s, p)
+    return q.raw
+
+def _sodium_init() -> None:
+    """
+    Checks that libsodium is not already initialized, initializes it,
+    and defines globals whose definitions depend on functions exported
+    by libsodium.
+    """
+    if _sodium.sodium_init() == 1:
+        raise RuntimeError('libsodium is already initialized') # pragma: no cover
+
+    if not _sodium.sodium_init() == 1:
+        raise RuntimeError('libsodium error during initialization') # pragma: no cover
+
+    _sodium.ready = True
+
+    # Define values of public and private globals.
+    context = globals()
+    context['crypto_scalarmult_ristretto255_BYTES'] = \
+        _sodium.crypto_scalarmult_ristretto255_bytes()
+    context['crypto_scalarmult_ristretto255_SCALARBYTES'] = \
+        _sodium.crypto_scalarmult_ristretto255_scalarbytes()
+    context['crypto_core_ristretto255_BYTES'] = \
+        _sodium.crypto_core_ristretto255_bytes()
+    context['crypto_core_ristretto255_HASHBYTES'] = \
+        _sodium.crypto_core_ristretto255_hashbytes()
+    context['crypto_core_ristretto255_NONREDUCEDSCALARBYTES'] = \
+        _sodium.crypto_core_ristretto255_nonreducedscalarbytes()
+    context['crypto_core_ristretto255_SCALARBYTES'] = \
+        _sodium.crypto_core_ristretto255_scalarbytes()
+    context['randombytes_SEEDBYTES'] = \
+        _sodium.randombytes_seedbytes()
+
+    context['_crypto_core_ristretto255_point_new'] = \
+        ctypes.c_char * crypto_core_ristretto255_BYTES
+    context['_crypto_core_ristretto255_scalar_new'] = \
+        ctypes.c_char * crypto_core_ristretto255_SCALARBYTES
+    context['_crypto_scalarmult_ristretto255_point_new'] = \
+        ctypes.c_char * crypto_scalarmult_ristretto255_BYTES
+
+# Check that libsodium is not already initialized and initialize it
+# (unless documentation is being automatically generated).
+if not os.environ.get('RBCL_SPHINX_AUTODOC_BUILD', None) == '1':
+    _sodium_init()
 
 if __name__ == '__main__':
     doctest.testmod() # pragma: no cover
```

### Comparing `rbcl-0.4.2/src/rbcl.egg-info/PKG-INFO` & `rbcl-1.0.1/src/rbcl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,195 @@
-Metadata-Version: 2.1
-Name: rbcl
-Version: 0.4.2
-Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
-Home-page: https://github.com/nthparty/rbcl
-Author: Nth Party, Ltd.
-Author-email: team@nthparty.com
-License: MIT
-Description-Content-Type: text/x-rst
-Provides-Extra: build
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-====
-rbcl
-====
-
-Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
-   :target: https://badge.fury.io/py/rbcl
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
-   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
-   :target: https://github.com/nthparty/rbcl/actions
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
-   :alt: Coveralls test coverage summary.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__::
-
-    python -m pip install rbcl
-
-The library can be imported in the usual ways::
-
-    import rbcl
-    from rbcl import *
-
-Examples
-^^^^^^^^
-
-A few usage examples are presented below::
-
-    >>> from rbcl import *
-    >>> x = crypto_core_ristretto255_random()
-    >>> assert crypto_core_ristretto255_is_valid_point(x)
-    >>> y = crypto_core_ristretto255_from_hash(b'\xF0'*64)
-    >>> assert crypto_core_ristretto255_is_valid_point(y)
-    >>> z1 = crypto_core_ristretto255_add(x, y)
-    >>> z2 = crypto_core_ristretto255_add(y, x)
-    >>> assert z1 == z2  # Assert that point addition commutes.
-    >>> s1 = crypto_core_ristretto255_scalar_random()
-    >>> s2 = crypto_core_ristretto255_scalar_random()
-    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
-    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
-    >>> assert w1 == w2  # Assert that point multiplication (by a scalar) is repeated addition.
-
-This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
-
-Development, Build, and Manual Installation Instructions
---------------------------------------------------------
-All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.py``. The ``extras_require`` parameter is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Building from Source
-^^^^^^^^^^^^^^^^^^^^
-The library can be built manually from source **within Linux and macOS** using the sequence of commands below::
-
-    python -m pip install .[build]
-    python setup.py bdist_wheel
-
-Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python setup.py bdist_wheel`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location::
-
-    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
-
-The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
-
-Preparation for Local Development
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it)::
-
-    cp build/lib*/rbcl/_sodium*.* src/rbcl
-
-Manual Installation
-^^^^^^^^^^^^^^^^^^^
-Once the package is `built <#building-from-source>`_, it can be installed manually using the command below::
-
-    python -m pip install -f dist . --upgrade
-
-Documentation
-^^^^^^^^^^^^^
-Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../setup.py ../src/rbcl/sodium_ffi.py && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
-
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/rbcl/rbcl.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/rbcl
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``setup.py``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python setup.py sdist
-
-Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain::
-
-    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: rbcl
+Version: 1.0.1
+Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
+Home-page: https://github.com/nthparty/rbcl
+Author: Nth Party
+Author-email: team@nthparty.com
+License: MIT
+Requires-Python: >=3.7
+Provides-Extra: build
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+====
+rbcl
+====
+
+Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
+   :target: https://badge.fury.io/py/rbcl
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
+   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
+   :target: https://github.com/nthparty/rbcl/actions
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
+   :alt: Coveralls test coverage summary.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__:
+
+.. code-block:: bash
+
+    python -m pip install rbcl
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import rbcl
+    from rbcl import *
+
+Examples
+^^^^^^^^
+
+A few usage examples are presented below:
+
+.. code-block:: python
+
+    >>> from rbcl import *
+    >>> x = crypto_core_ristretto255_random()
+    >>> assert crypto_core_ristretto255_is_valid_point(x)
+    >>> y = crypto_core_ristretto255_from_hash(b'\xF0' * 64)
+    >>> assert crypto_core_ristretto255_is_valid_point(y)
+    >>> z1 = crypto_core_ristretto255_add(x, y)
+    >>> z2 = crypto_core_ristretto255_add(y, x)
+    >>> assert z1 == z2 # Point addition commutes.
+    >>> s1 = crypto_core_ristretto255_scalar_random()
+    >>> s2 = crypto_core_ristretto255_scalar_random()
+    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
+    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
+    >>> assert w1 == w2 # Multiplication of a point by a scalar is repeated addition.
+
+This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
+
+Development, Build, and Manual Installation Instructions
+--------------------------------------------------------
+All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.cfg``. The ``extras_require`` option is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__ (assuming that the library has already been built successfully):
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Building from Source
+^^^^^^^^^^^^^^^^^^^^
+The library can be built manually from source **within Linux and macOS** using the sequence of commands below:
+
+.. code-block:: bash
+
+    python -m pip install .[build]
+    python -m build --sdist --wheel .
+
+Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python -m build --sdist --wheel .`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location:
+
+.. code-block:: bash
+
+    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
+
+The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
+
+Preparation for Local Development
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it):
+
+.. code-block:: bash
+
+    cp build/lib*/rbcl/_sodium.py src/rbcl
+
+Manual Installation
+^^^^^^^^^^^^^^^^^^^
+Once the package is `built <#building-from-source>`_, it can be installed manually using the command below:
+
+.. code-block:: bash
+
+    python -m pip install -f dist . --upgrade
+
+Documentation
+^^^^^^^^^^^^^
+Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../src/rbcl/_sodium_build.py && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
+
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/rbcl/rbcl.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/rbcl src/rbcl/_sodium.tmpl src/rbcl/_sodium_build.py --disable=duplicate-code
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``setup.cfg``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist .
+
+Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain:
+
+.. code-block:: bash
+
+    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

