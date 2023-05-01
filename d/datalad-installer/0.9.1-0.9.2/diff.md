# Comparing `tmp/datalad-installer-0.9.1.tar.gz` & `tmp/datalad-installer-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad-installer-0.9.1.tar", last modified: Thu Jul 28 17:22:11 2022, max compression
+gzip compressed data, was "datalad-installer-0.9.2.tar", last modified: Tue Nov 22 15:34:12 2022, max compression
```

## Comparing `datalad-installer-0.9.1.tar` & `datalad-installer-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    12064 2022-07-28 17:22:01.000000 datalad-installer-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    21927 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20275 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      692 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/src/datalad_installer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21927 2022-07-28 17:22:10.000000 datalad-installer-0.9.1/src/datalad_installer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-07-28 17:22:10.000000 datalad-installer-0.9.1/src/datalad_installer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 17:22:10.000000 datalad-installer-0.9.1/src/datalad_installer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-07-28 17:22:10.000000 datalad-installer-0.9.1/src/datalad_installer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-28 17:22:10.000000 datalad-installer-0.9.1/src/datalad_installer.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    91065 2022-07-28 17:22:02.000000 datalad-installer-0.9.1/src/datalad_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 17:22:10.994149 datalad-installer-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    17803 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/test/test_install.py
--rw-r--r--   0 runner    (1001) docker     (121)    13811 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-07-28 17:21:51.000000 datalad-installer-0.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    13227 2022-11-22 15:34:02.000000 datalad-installer-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    21978 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    20275 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (121)      692 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/src/datalad_installer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    21978 2022-11-22 15:34:12.000000 datalad-installer-0.9.2/src/datalad_installer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-22 15:34:12.000000 datalad-installer-0.9.2/src/datalad_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 15:34:12.000000 datalad-installer-0.9.2/src/datalad_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-22 15:34:12.000000 datalad-installer-0.9.2/src/datalad_installer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-22 15:34:12.000000 datalad-installer-0.9.2/src/datalad_installer.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    92008 2022-11-22 15:34:03.000000 datalad-installer-0.9.2/src/datalad_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:34:12.326694 datalad-installer-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17916 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/test/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13811 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-11-22 15:33:50.000000 datalad-installer-0.9.2/tox.ini
```

### Comparing `datalad-installer-0.9.1/CHANGELOG.md` & `datalad-installer-0.9.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+# v0.9.2 (Tue Nov 22 2022)
+
+#### 🐛 Bug Fix
+
+- Retry failed downloads [#132](https://github.com/datalad/datalad-installer/pull/132) ([@jwodder](https://github.com/jwodder))
+- Install arm64 Miniconda on M1 Macs [#130](https://github.com/datalad/datalad-installer/pull/130) ([@jwodder](https://github.com/jwodder))
+- Handle moving files across filesystems [#125](https://github.com/datalad/datalad-installer/pull/125) ([@jwodder](https://github.com/jwodder))
+- Make `OSError.winerror` reference portable [#123](https://github.com/datalad/datalad-installer/pull/123) ([@jwodder](https://github.com/jwodder))
+
+#### 🏠 Internal
+
+- Update GitHub Actions action versions [#126](https://github.com/datalad/datalad-installer/pull/126) ([@jwodder](https://github.com/jwodder))
+
+#### 🧪 Tests
+
+- Test against Python 3.11 [#127](https://github.com/datalad/datalad-installer/pull/127) ([@jwodder](https://github.com/jwodder))
+- Fix test failures due to some sort of dependency hell [#128](https://github.com/datalad/datalad-installer/pull/128) ([@jwodder](https://github.com/jwodder))
+
+#### Authors: 1
+
+- John T. Wodder II ([@jwodder](https://github.com/jwodder))
+
+---
+
 # v0.9.1 (Thu Jul 28 2022)
 
 #### 🐛 Bug Fix
 
 - Smoke-test rclone with `--version` instead of `--help` [#122](https://github.com/datalad/datalad-installer/pull/122) ([@jwodder](https://github.com/jwodder))
 
 #### 📝 Documentation
```

### Comparing `datalad-installer-0.9.1/LICENSE` & `datalad-installer-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/PKG-INFO` & `datalad-installer-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-installer
-Version: 0.9.1
+Version: 0.9.2
 Summary: Installation script for Datalad and related components
 Home-page: https://github.com/datalad/datalad-installer
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Maintainer: John Thorvald Wodder II
 Maintainer-email: datalad-installer@varonathe.org
 License: MIT
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `datalad-installer-0.9.1/README.rst` & `datalad-installer-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/run-tests.sh` & `datalad-installer-0.9.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/setup.cfg` & `datalad-installer-0.9.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	License :: OSI Approved :: MIT License
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
```

### Comparing `datalad-installer-0.9.1/src/datalad_installer.egg-info/PKG-INFO` & `datalad-installer-0.9.2/src/datalad_installer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-installer
-Version: 0.9.1
+Version: 0.9.2
 Summary: Installation script for Datalad and related components
 Home-page: https://github.com/datalad/datalad-installer
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Maintainer: John Thorvald Wodder II
 Maintainer-email: datalad-installer@varonathe.org
 License: MIT
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `datalad-installer-0.9.1/src/datalad_installer.py` & `datalad-installer-0.9.2/src/datalad_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. _Datalad: https://www.datalad.org
 .. _git-annex: https://git-annex.branchable.com
 
 Visit <https://github.com/datalad/datalad-installer> for more information.
 """
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __author__ = "The DataLad Team and Contributors"
 __author_email__ = "team@datalad.org"
 __license__ = "MIT"
 __url__ = "https://github.com/datalad/datalad-installer"
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, suppress
@@ -49,14 +49,15 @@
     NamedTuple,
     Optional,
     Tuple,
     Type,
     Union,
     cast,
 )
+from urllib.error import HTTPError, URLError
 from urllib.request import Request, urlopen
 from zipfile import ZipFile
 
 log = logging.getLogger("datalad_installer")
 
 SYSTEM = platform.system()
 ON_LINUX = SYSTEM == "Linux"
@@ -652,25 +653,30 @@
                     self.sudo_confirm = SudoConfirm.OK
             runcmd("sudo", *args, **kwargs)
 
     def run_maybe_elevated(self, *args: Any, **kwargs: Any) -> None:
         try:
             runcmd(*args, **kwargs)
         except OSError as e:
-            if e.winerror == 740:  # type: ignore[attr-defined]
+            if getattr(e, "winerror", None) == 740:
                 log.info("Operation requires elevation; rerunning as administrator")
                 self.sudo(*args, **kwargs)
             else:
                 raise
 
     def move_maybe_elevated(self, path: Path, dest: Path) -> None:
         # `dest` must be a file path, not a directory path.
         log.info("Moving %s to %s", path, dest)
         try:
-            path.replace(dest)
+            if ON_POSIX:
+                # Handle cross-filesystem moves  (Don't use shutil.move() on
+                # Windows, as it fails when dest exists)
+                shutil.move(str(path), str(dest))
+            else:
+                path.replace(dest)
         except PermissionError:
             log.info("Operation requires elevation; rerunning as administrator")
             if ON_POSIX:
                 args = ["mv", "-f", "--", str(path), str(dest)]
             else:
                 args = ["move", str(path), str(dest)]
             self.sudo(*args)
@@ -993,15 +999,19 @@
         log.info("Python Match: %s", python_match)
         log.info("Extra args: %s", extra_args)
         if kwargs:
             log.warning("Ignoring extra component arguments: %r", kwargs)
         if ON_LINUX:
             miniconda_script = "Miniconda3-latest-Linux-x86_64.sh"
         elif ON_MACOS:
-            miniconda_script = "Miniconda3-latest-MacOSX-x86_64.sh"
+            arch = platform.machine().lower()
+            if arch in ("x86_64", "arm64"):
+                miniconda_script = f"Miniconda3-latest-MacOSX-{arch}.sh"
+            else:
+                raise RuntimeError(f"E: Unsupported architecture: {arch}")
         elif ON_WINDOWS:
             miniconda_script = "Miniconda3-latest-Windows-x86_64.exe"
         else:
             raise RuntimeError(f"E: Unsupported OS: {SYSTEM}")
         if python_match is not None:
             vparts: Tuple[int, ...]
             if python_match == "major":
@@ -2432,18 +2442,32 @@
     """
     Download a file from ``url``, saving it at ``path``.  Optional ``headers``
     are sent in the HTTP request.
     """
     log.info("Downloading %s", url)
     if headers is None:
         headers = {}
+    delays = iter([1, 2, 6, 15, 36])
     req = Request(url, headers=headers)
-    with urlopen(req) as r:
-        with open(path, "wb") as fp:
-            shutil.copyfileobj(r, fp)
+    while True:
+        try:
+            with urlopen(req) as r:
+                with open(path, "wb") as fp:
+                    shutil.copyfileobj(r, fp)
+            return
+        except URLError as e:
+            if isinstance(e, HTTPError) and e.code not in (500, 502, 503, 504):
+                raise
+            try:
+                delay = next(delays)
+            except StopIteration:
+                raise
+            else:
+                log.warning("Request to %s failed: %s", url, e)
+                log.info("Retrying in %d seconds", delay)
 
 
 def download_to_tempfile(
     url: str, suffix: Optional[str] = None, headers: Optional[Dict[str, str]] = None
 ) -> Path:
     # `suffix` should include the dot
     fd, tmpfile = tempfile.mkstemp(suffix=suffix)
```

### Comparing `datalad-installer-0.9.1/test/conftest.py` & `datalad-installer-0.9.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/test/test_install.py` & `datalad-installer-0.9.2/test/test_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     )
 
 
 @pytest.mark.skipif(
     sys.version_info[:2] < (3, 7),
     reason="Trying to install Python 3.6 on Conda gives package conflicts",
 )
+@pytest.mark.skipif(
+    sys.version_info[:2] == (3, 11),
+    reason="Python 3.11 not yet available on Conda",
+)
 @pytest.mark.miniconda
 def test_install_miniconda_python_match(tmp_path: Path) -> None:
     miniconda_path = tmp_path / "conda"
     r = main(
         [
             "datalad_installer.py",
             "miniconda",
```

### Comparing `datalad-installer-0.9.1/test/test_options.py` & `datalad-installer-0.9.2/test/test_options.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/test/test_util.py` & `datalad-installer-0.9.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `datalad-installer-0.9.1/tox.ini` & `datalad-installer-0.9.2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tox]
-envlist = lint,typing,py36,py37,py38,py39,py310,pypy3
+envlist = lint,typing,py36,py37,py38,py39,py310,py311,pypy3
 skip_missing_interpreters = True
 isolated_build = True
 minversion = 3.3.0
 
 [testenv]
 # HOME needs to be set in order for brew to work:
 passenv = GITHUB_TOKEN HOME
 deps =
-    pytest~=7.0
-    pytest-cov~=3.0
-    pytest-mock~=3.0
+    pytest
+    pytest-cov
+    pytest-mock
 commands =
     pytest {posargs} test
 
 [testenv:lint]
 deps =
     flake8~=4.0
     flake8-bugbear
```

