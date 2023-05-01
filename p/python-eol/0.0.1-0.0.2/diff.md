# Comparing `tmp/python_eol-0.0.1.tar.gz` & `tmp/python_eol-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_eol-0.0.1.tar", last modified: Sun Apr 30 15:49:07 2023, max compression
+gzip compressed data, was "python_eol-0.0.2.tar", last modified: Mon May  1 07:25:15 2023, max compression
```

## Comparing `python_eol-0.0.1.tar` & `python_eol-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-30 15:49:07.614644 python_eol-0.0.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)       28 2023-04-30 12:26:27.000000 python_eol-0.0.1/.flake8
--rw-rw-r--   0 martin    (1000) martin    (1000)      103 2023-04-30 15:47:31.000000 python_eol-0.0.1/.gitignore
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-04-30 15:31:01.000000 python_eol-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 martin    (1000) martin    (1000)      303 2023-04-30 15:29:54.000000 python_eol-0.0.1/.pre-commit-hooks.yaml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1062 2023-04-30 15:40:38.000000 python_eol-0.0.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     1358 2023-04-30 15:49:07.614644 python_eol-0.0.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      893 2023-04-30 15:32:48.000000 python_eol-0.0.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1876 2023-04-30 15:42:55.000000 python_eol-0.0.1/pyproject.toml
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-30 15:49:07.610644 python_eol-0.0.1/python_eol/
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-04-30 12:53:47.000000 python_eol-0.0.1/python_eol/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1509 2023-04-24 16:42:44.000000 python_eol-0.0.1/python_eol/db.json
--rw-rw-r--   0 martin    (1000) martin    (1000)     2455 2023-04-30 15:19:38.000000 python_eol-0.0.1/python_eol/main.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-30 15:49:07.614644 python_eol-0.0.1/python_eol.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1358 2023-04-30 15:49:07.000000 python_eol-0.0.1/python_eol.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      397 2023-04-30 15:49:07.000000 python_eol-0.0.1/python_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-30 15:49:07.000000 python_eol-0.0.1/python_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       45 2023-04-30 15:49:07.000000 python_eol-0.0.1/python_eol.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-04-30 15:49:07.000000 python_eol-0.0.1/python_eol.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       96 2023-04-30 15:26:39.000000 python_eol-0.0.1/requirements-dev.in
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-04-30 15:49:07.614644 python_eol-0.0.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-30 15:49:07.614644 python_eol-0.0.1/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-30 06:43:54.000000 python_eol-0.0.1/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2118 2023-04-30 15:20:10.000000 python_eol-0.0.1/tests/test_main.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1224 2023-04-30 15:23:56.000000 python_eol-0.0.1/tox.ini
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      182 2023-05-01 07:24:31.000000 python_eol-0.0.2/.bumpversion.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)       28 2023-04-30 12:26:27.000000 python_eol-0.0.2/.flake8
+-rw-rw-r--   0 martin    (1000) martin    (1000)      103 2023-04-30 15:47:31.000000 python_eol-0.0.2/.gitignore
+-rw-rw-r--   0 martin    (1000) martin    (1000)      998 2023-05-01 07:21:13.000000 python_eol-0.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      303 2023-04-30 15:29:54.000000 python_eol-0.0.2/.pre-commit-hooks.yaml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1062 2023-04-30 15:40:38.000000 python_eol-0.0.2/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1477 2023-05-01 07:25:15.171445 python_eol-0.0.2/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1012 2023-05-01 07:21:13.000000 python_eol-0.0.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1894 2023-05-01 07:24:31.000000 python_eol-0.0.2/pyproject.toml
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/python_eol/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-04-30 12:53:47.000000 python_eol-0.0.2/python_eol/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      646 2023-05-01 07:13:42.000000 python_eol-0.0.2/python_eol/_docker_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1509 2023-04-24 16:42:44.000000 python_eol-0.0.2/python_eol/db.json
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3696 2023-05-01 05:45:39.000000 python_eol-0.0.2/python_eol/main.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/python_eol.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1477 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       45 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-05-01 07:25:15.000000 python_eol-0.0.2/python_eol.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      109 2023-05-01 07:23:55.000000 python_eol-0.0.2/requirements-dev.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-01 07:25:15.171445 python_eol-0.0.2/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-01 07:25:15.171445 python_eol-0.0.2/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-30 06:43:54.000000 python_eol-0.0.2/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1972 2023-05-01 07:12:56.000000 python_eol-0.0.2/tests/test_docker_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3597 2023-05-01 07:12:48.000000 python_eol-0.0.2/tests/test_main.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1228 2023-04-30 17:26:09.000000 python_eol-0.0.2/tox.ini
```

### Comparing `python_eol-0.0.1/.pre-commit-config.yaml` & `python_eol-0.0.2/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -29,10 +29,11 @@
     hooks:
       - id: black
   - repo: https://github.com/lyz-code/yamlfix/
     rev: 1.9.0
     hooks:
       - id: yamlfix
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: python-eol-check
+        args: [--fail-close-to-eol]
```

### Comparing `python_eol-0.0.1/LICENSE` & `python_eol-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_eol-0.0.1/PKG-INFO` & `python_eol-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_eol
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple tool to check if python version is past EOL
 Author-email: Martin Imre <martinimre25@gmail.com>
 Project-URL: Source, https://github.com/mimre25/python-eol
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
@@ -27,20 +27,21 @@
 
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
-```
-  --fail-close-to-eol  Fail if the python version is close to eol instead of just warn
+```sh
+  --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
+  --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.1/README.md` & `python_eol-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
-```
-  --fail-close-to-eol  Fail if the python version is close to eol instead of just warn
+```sh
+  --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
+  --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.1/pyproject.toml` & `python_eol-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_eol"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name = "Martin Imre", email = "martinimre25@gmail.com"}
 ]
 description = "Simple tool to check if python version is past EOL"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -30,21 +30,21 @@
 python_eol = ["*.json"]
 
 ###### Tooling #####
 
 ##### ruff #####
 [tool.ruff]
 select = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ",  "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI",  "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-ignore = ["D203", "D213"]
+ignore = ["D203", "D213", "G004"]
 
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ",  "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI",  "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 [tool.ruff.per-file-ignores]
-"tests/*"= ["S101", "D100", "D103", "D104"]
+"tests/*"= ["S101", "D100", "D103", "D104", "FBT001"]
 
 ##### pytest #####
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 source = ["python_eol"]
```

### Comparing `python_eol-0.0.1/python_eol/db.json` & `python_eol-0.0.2/python_eol/db.json`

 * *Files identical despite different names*

### Comparing `python_eol-0.0.1/python_eol/main.py` & `python_eol-0.0.2/python_eol/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 import argparse
 import json
 import logging
 import platform
 from datetime import date
 from pathlib import Path
+from typing import Any
+
+from ._docker_utils import _extract_python_version_from_docker_file, _find_docker_files
 
 EOL_WARN_DAYS = 60
 
+logger = logging.getLogger(__name__)
+
 
 def _get_major_minor() -> str:
     major, minor, patch = platform.python_version_tuple()
     return f"{major}.{minor}"
 
 
 def _get_db_file_path() -> Path:
@@ -31,63 +36,102 @@
             "python_eol",
             "db.json",
         )  # pragma: no cover
 
     return Path(db_file)
 
 
-logger = logging.getLogger(__name__)
-
-
-def _check_python_eol(*, fail_close_to_eol: bool = False) -> int:
-    db_file = _get_db_file_path()
-    with db_file.open() as f:
-        eol_data = json.load(f)
-
-    version_info = {entry["cycle"]: entry for entry in eol_data}
-
-    my_version = _get_major_minor()
-
-    my_version_info = version_info[my_version]
+def _check_eol(
+    python_version: str,
+    version_info: dict[str, dict[str, Any]],
+    *,
+    fail_close_to_eol: bool = False,
+    prefix: str = "",
+) -> int:
+    my_version_info = version_info[python_version]
     today = date.today()
     eol_date = date.fromisoformat(my_version_info["eol"])
     time_to_eol = eol_date - today
 
     if time_to_eol.days < 0:
-        logger.error("Your python version is beyond end of life")
+        logger.error(f"{prefix}Python {python_version} is beyond end of life")
         return 1
     if time_to_eol.days < EOL_WARN_DAYS:
-        msg = f"Your python version is going to be end of life in 2 months {eol_date}"
+        msg = (
+            f"{prefix}Python {python_version} is going to "
+            f"be end of life in 2 months {eol_date}"
+        )
 
         if fail_close_to_eol:
             logger.error(msg)
             return 1
         else:
             logger.warning(msg)
             return 0
-
-    logger.info("All good your python version has quite some time left")
     return 0
 
 
+def _check_python_eol(
+    *,
+    fail_close_to_eol: bool = False,
+    check_docker_files: bool = False,
+) -> int:
+    db_file = _get_db_file_path()
+    with db_file.open() as f:
+        eol_data = json.load(f)
+
+    version_info = {entry["cycle"]: entry for entry in eol_data}
+
+    my_version = _get_major_minor()
+
+    docker_res = 0
+    if check_docker_files:
+        for path in _find_docker_files():
+            version = _extract_python_version_from_docker_file(path)
+            if version:
+                docker_res = (
+                    _check_eol(
+                        version,
+                        version_info,
+                        fail_close_to_eol=fail_close_to_eol,
+                        prefix=f"{path}: ",
+                    )
+                    or docker_res
+                )
+    return (
+        _check_eol(my_version, version_info, fail_close_to_eol=fail_close_to_eol)
+        or docker_res
+    )
+
+
 def _get_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="eol check if your python version is beyond end of life",
     )
     parser.add_argument(
         "--fail-close-to-eol",
         action="store_true",
         help="Fail if the python version is close to eol instead of just warn",
     )
+    parser.add_argument(
+        "--check-docker-files",
+        action="store_true",
+        help=(
+            "Search for Dockerfile (**/*Dockerfile*) and check "
+            "the python versions specified inside them"
+        ),
+    )
     return parser
 
 
 def main() -> int:
     """Run main entry point."""
     parser = _get_argparser()
     args, unknown_args = parser.parse_known_args()
-
-    return _check_python_eol(fail_close_to_eol=args.fail_close_to_eol)
+    return _check_python_eol(
+        fail_close_to_eol=args.fail_close_to_eol,
+        check_docker_files=args.check_docker_files,
+    )
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
```

### Comparing `python_eol-0.0.1/python_eol.egg-info/PKG-INFO` & `python_eol-0.0.2/python_eol.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eol
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple tool to check if python version is past EOL
 Author-email: Martin Imre <martinimre25@gmail.com>
 Project-URL: Source, https://github.com/mimre25/python-eol
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
@@ -27,20 +27,21 @@
 
 ## Usage
 Simply invoke `eol` from your command line
 ```sh
 eol
 ```
 **Options**:
-```
-  --fail-close-to-eol  Fail if the python version is close to eol instead of just warn
+```sh
+  --fail-close-to-eol   Fail if the python version is close to eol instead of just warn
+  --check-docker-files  Search for Dockerfile (**/*Dockerfile*) and check the python versions specified inside them
 ```
 
 ## Pre-commit-hook
 Add the following to your `.pre-commit-config.yaml`:
 ```yaml
 repos:
   - repo: https://github.com/mimre25/python-eol/
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: python-eol-check
 ```
```

### Comparing `python_eol-0.0.1/tox.ini` & `python_eol-0.0.2/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     pytest
     coverage
     freezegun
 commands =
     coverage run -m pytest {posargs}
     coverage report
 
-[testenv:py{39-311}]
+[testenv:py{39,310,311}]
 commands =
     {[testenv]commands}
     coverage report --fail-under 100
 
 [testenv:py{37,38}]
 commands =
     {[testenv]commands}
```

