# Comparing `tmp/pynamer-0.5.0.tar.gz` & `tmp/pynamer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.5.0.tar", last modified: Sun Apr 30 20:16:46 2023, max compression
+gzip compressed data, was "pynamer-0.5.1.tar", last modified: Mon May  1 09:24:21 2023, max compression
```

## Comparing `pynamer-0.5.0.tar` & `pynamer-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.5.0/AUTHORS.md
--rw-rw-rw-   0        0        0     3397 2023-04-30 20:16:31.000000 pynamer-0.5.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12177 2023-04-30 20:16:46.346319 pynamer-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    10845 2023-04-30 20:14:17.000000 pynamer-0.5.0/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0     1808 2023-04-30 20:16:46.361953 pynamer-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.265598 pynamer-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.330677 pynamer-0.5.0/src/pynamer/
--rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.5.0/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1780 2023-04-30 20:16:31.000000 pynamer-0.5.0/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0       17 2023-04-30 20:13:43.000000 pynamer-0.5.0/src/pynamer/project_count.pickle
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.5.0/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    20074 2023-04-30 20:12:42.000000 pynamer-0.5.0/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0  7243286 2023-04-30 09:18:06.000000 pynamer-0.5.0/src/pynamer/pypi_index.txt
--rw-rw-rw-   0        0        0      427 2023-04-29 19:54:50.000000 pynamer-0.5.0/src/pynamer/setup.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.330677 pynamer-0.5.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    12177 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 20:16:46.000000 pynamer-0.5.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 20:16:46.346319 pynamer-0.5.0/tests/
--rw-rw-rw-   0        0        0      309 2023-04-30 20:14:15.000000 pynamer-0.5.0/tests/test_pynamer.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.811234 pynamer-0.5.1/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.5.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     3582 2023-05-01 09:24:09.000000 pynamer-0.5.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12177 2023-05-01 09:24:21.811234 pynamer-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10845 2023-04-30 20:14:17.000000 pynamer-0.5.1/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1808 2023-05-01 09:24:21.822864 pynamer-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.720585 pynamer-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.783074 pynamer-0.5.1/src/pynamer/
+-rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.5.1/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1780 2023-05-01 09:24:09.000000 pynamer-0.5.1/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0       17 2023-04-30 20:13:43.000000 pynamer-0.5.1/src/pynamer/project_count.pickle
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.795589 pynamer-0.5.1/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.5.1/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    19306 2023-05-01 08:51:55.000000 pynamer-0.5.1/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0  7243286 2023-04-30 09:18:06.000000 pynamer-0.5.1/src/pynamer/pypi_index.txt
+-rw-rw-rw-   0        0        0      427 2023-04-29 19:54:50.000000 pynamer-0.5.1/src/pynamer/setup.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.795589 pynamer-0.5.1/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    12177 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 09:24:21.000000 pynamer-0.5.1/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 09:24:21.811234 pynamer-0.5.1/tests/
+-rw-rw-rw-   0        0        0      309 2023-04-30 20:14:15.000000 pynamer-0.5.1/tests/test_pynamer.py
```

### Comparing `pynamer-0.5.0/CHANGELOG.md` & `pynamer-0.5.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.1 (2023-05-01)
+### Fix
+* Regex pattern for 10,000+ projects found ([`9ec94ea`](https://github.com/Stephen-RA-King/pynamer/commit/9ec94ea1bdd90244be0b4cf7e0941b40ad7bb2ba))
+
 ## v0.5.0 (2023-04-30)
 ### Feature
 * Add pypi search function and rich tables ([`089356b`](https://github.com/Stephen-RA-King/pynamer/commit/089356b574a3eca65dfcac69951f335a97e5e063))
 
 ### Fix
 * Total projects found ([`4b42701`](https://github.com/Stephen-RA-King/pynamer/commit/4b42701fc9655573918251179b44e21855adc09b))
```

### Comparing `pynamer-0.5.0/LICENSE` & `pynamer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.0/PKG-INFO` & `pynamer-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

### Comparing `pynamer-0.5.0/README.md` & `pynamer-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.0/pyproject.toml` & `pynamer-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.0/setup.cfg` & `pynamer-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.0/src/pynamer/__init__.py` & `pynamer-0.5.1/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import as_file, files
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-0.5.0/src/pynamer/pynamer.py` & `pynamer-0.5.1/src/pynamer/pynamer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,578 +1,569 @@
-#!/usr/bin/env python3
-
-# TODO: suppress verbose output from build.
-# TODO: add docstrings
-# TODO: add typing
-# TODO: add 'fix' function to check package structure and fix if necessary
-# TODO: add random standoff timer to prevent dossing PyPI
-# TODO: write tests
-# TODO: final version - turn off file logging
-# TODO: split and rename files into logical components
-
-
-# Core Library modules
-import argparse
-import contextlib
-import json
-import os
-import pickle
-import re
-import shutil
-import string
-import subprocess
-import sys
-from datetime import datetime
-from pathlib import Path
-
-# Third party modules
-import build
-import requests  # type: ignore
-import yaml  # type: ignore
-from bs4 import BeautifulSoup
-from colorama import Back, Fore, Style
-from jinja2 import Template
-from rich.console import Console
-from rich.table import Table
-from tqdm import tqdm
-
-# Local modules
-from . import logger, project_count, project_path, setup_text
-
-
-class Config:
-    PYPIRC = None
-    ORIGINAL_PROJECT_NAME = "project_name"
-    NO_CLEANUP: bool = False
-    PROJECT_COUNT = 0
-    PACKAGE_VERSION = "0.0.0"
-    pypi_search_url: str = "https://pypi.org/search/"
-    pypi_project_url: str = "https://pypi.org/project/"
-    pypi_json_url: str = "https://pypi.org/pypi/"
-    IDLEMODE = 1 if "idlelib.run" in sys.modules else 0
-
-
-config = Config()
-config.PROJECT_COUNT = project_count
-
-
-def _feedback(message: str, feedback_type: str) -> None:
-    """A utility method to generate formatted messages appropriate to the
-    environment.
-
-    Args:
-        message:        Text to be echoed.
-        feedback_type:  identifies type of message to display.
-    """
-    if feedback_type not in ["null", "nominal", "warning", "error"]:
-        return
-    if config.IDLEMODE == 1:
-        print(message)
-    else:
-        if feedback_type == "null":
-            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "nominal":
-            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "warning":
-            print(
-                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
-            )
-        elif feedback_type == "error":
-            print(Fore.RED + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-
-
-def find_pypirc_file():
-    filename = ".pypirc"
-    system_path = os.getenv("PATH")
-    path_directories = list()
-    path_directories.append(os.getcwd())
-    path_directories.extend(system_path.split(os.pathsep))
-    for directory in path_directories:
-        file_path = Path(directory) / filename
-        if file_path.exists():
-            logger.debug(
-                "%s is present in the system's PATH at %s", filename, directory
-            )
-            config.PYPIRC = file_path
-            break
-    else:
-        logger.debug("%s is not present in the system's PATH.", filename)
-
-
-@contextlib.contextmanager
-def suppress_stdout():
-    with open(os.devnull, "w") as devnull:
-        old_stdout = sys.stdout
-        sys.stdout = devnull
-        try:
-            yield
-        finally:
-            sys.stdout = old_stdout
-
-
-def rename_project_dir(old_name: str, new_name: str) -> None:
-    old_directory_path = Path(old_name)
-    new_directory_path = Path(new_name)
-    logger.debug("renaming project directory from %s to %s", old_name, new_name)
-    try:
-        old_directory_path.rename(new_directory_path)
-    except FileNotFoundError:
-        logger.error("directory %s cannot be found:", old_directory_path)
-
-
-def create_setup(new_project_name: str) -> None:
-    template = Template(setup_text)
-    content = template.render(
-        PROJECT_NAME=new_project_name,
-        PACKAGE_VERSION=config.PACKAGE_VERSION,
-    )
-    setup_file = project_path.joinpath("setup.py")
-    with open(setup_file, mode="w", encoding="utf-8") as message:
-        logger.debug("creating new setup.py with the following: \n %s", content)
-        message.write(content)
-
-
-def delete_director(items_to_delete: list) -> None:
-    """Utility function to delete files or directories"""
-    for item in items_to_delete:
-        if not item.exists():
-            logger.debug("trying to delete %s but it does not exist", item)
-            continue
-        if item.is_dir():
-            logger.debug("Deleting Directory: %s", item)
-            shutil.rmtree(item, ignore_errors=True)
-        else:
-            logger.debug("Deleting File: %s", item)
-            Path.unlink(item, missing_ok=True)
-
-
-def run_command(*arguments: str, shell=True, working_dir=None, project=None) -> None:
-    working_dir = os.getcwd() if working_dir is None else working_dir
-    try:
-        process = subprocess.Popen(
-            arguments,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            shell=shell,
-            text=True,
-            cwd=working_dir,
-        )
-        stdout, stderr = process.communicate()
-        if process.returncode != 0:
-            logger.error("Error running command: %s", arguments)
-            logger.error("stderr: %s", stderr)
-            cleanup(project)
-            return
-        logger.debug("%s", stdout)
-        return
-    except Exception as e:
-        logger.error("Exception running command: %s", arguments)
-        logger.error(e)
-        cleanup(project)
-        return
-
-
-def ping_project(new_project_name: str, output_file: str = None) -> bool:
-    url_project = "".join(["https://pypi.org/project/", new_project_name, "/"])
-    logger.debug("attempting to get url %s", url_project)
-    try:
-        project_ping = requests.get(url_project, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit(f"An error occurred with an HTTP request")
-    if project_ping.status_code == 200:
-        logger.debug("%s FOUND in the project area of PyPI", new_project_name)
-        if output_file is not None:
-            message = f"{new_project_name:20} is already registered"
-            write_output_file(output_file, message)
-        return True
-    else:
-        logger.debug("%s NOT FOUND in the project area of PyPI", new_project_name)
-        if output_file is not None:
-            message = f"{new_project_name:20} is available"
-            write_output_file(output_file, message)
-        return False
-
-
-def ping_json(new_project_name: str) -> str:
-    url_json = "".join(["https://pypi.org/pypi/", new_project_name, "/json"])
-    logger.debug("attempting to get url %s", url_json)
-    try:
-        project_json_raw = requests.get(url_json, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit(f"An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-        result = "".join(
-            [
-                project_json["info"]["author"],
-                "\n",
-                project_json["info"]["author_email"],
-                "\n",
-                project_json["info"]["version"],
-                "\n",
-                project_json["info"]["summary"],
-            ]
-        )
-        return result
-    else:
-        logger.debug("No response from JSON URL")
-        return ""
-
-
-def build_dist():
-    logger.debug("Building the distribution... ")
-    builder = build.ProjectBuilder(project_path)
-    builder.build("wheel", project_path / "dist")
-    builder.build("sdist", project_path / "dist")
-
-
-def upload_dist(project_name):
-    logger.debug("Uploading the distribution... ")
-    dir_path = os.fspath(project_path / "dist" / "*")
-    pypirc_path = os.fspath(config.PYPIRC)
-    run_command(
-        sys.executable,
-        "-m",
-        "twine",
-        "upload",
-        "--config-file",
-        pypirc_path,
-        dir_path,
-        project=project_name,
-    )
-
-
-def cleanup(new_project_name):
-    if config.NO_CLEANUP is True:
-        return
-    rename_project_dir(
-        project_path.joinpath(new_project_name),
-        project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
-    )
-    build_artifacts = [
-        project_path / "build",
-        project_path / "dist",
-        project_path / "".join([new_project_name, ".egg-info"]),
-        project_path / "setup.py",
-    ]
-    logger.debug("cleaning build artifacts %s", build_artifacts)
-    delete_director(build_artifacts)
-
-
-def generate_pypi_index() -> None:
-    new_count = 0
-    progress_bar = tqdm(total=config.PROJECT_COUNT)
-    pypi_index = project_path / "pypi_index.txt"
-    pypi_count = project_path / "project_count.pickle"
-    if pypi_index.exists():
-        Path.unlink(pypi_index, missing_ok=True)
-    try:
-        index_object_raw = requests.get("https://pypi.org/simple/", timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit(f"An error occurred with an HTTP request")
-    pattern = re.compile(r"(?:>)([\w\W]*?)(?:<)")
-    with pypi_index.open(mode="a") as file:
-        for line in index_object_raw.iter_lines():
-            line = str(line)
-            project_text = re.search(pattern, line)
-            if project_text is not None:
-                new_count += 1
-                progress_bar.update(1)
-                project = "".join([project_text.group(1), " \n"])
-                file.write(project)
-    progress_bar.close()
-    with open(pypi_count, "wb") as f:
-        pickle.dump(new_count, f)
-
-
-def pypi_search_index(project_name):
-    pypi_index = project_path / "pypi_index.txt"
-    if not pypi_index.exists():
-        generate_pypi_index()
-    with pypi_index.open(mode="r") as file:
-        projects = file.read()
-        if project_name in projects:
-            logger.debug("%s FOUND in the PyPI simple index", project_name)
-            return True
-        else:
-            logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-            return False
-
-
-def pypi_search(search_project):
-    api_url: str = "https://pypi.org/search/"
-    pattern = re.compile(r">([\d,]+?)<")
-    s = requests.Session()
-    projects_raw, match, others = [], [], []
-    params = {"q": {search_project}, "page": 1}
-    r = s.get(api_url, params=params)
-    soup = BeautifulSoup(r.text, "html.parser")
-    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
-    for project_raw in projects_raw:
-        project_name = project_raw.select_one(
-            'span[class*="package-snippet__name"]'
-        ).text.strip()
-        version = project_raw.select_one(
-            'span[class*="package-snippet__version"]'
-        ).text.strip()
-        released_iso_8601 = project_raw.select_one(
-            'span[class*="package-snippet__created"]'
-        ).find("time")["datetime"]
-        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
-            "%Y-%m-%d"
-        )
-        description = project_raw.select_one(
-            'p[class*="package-snippet__description"]'
-        ).text.strip()
-        if project_name.lower() == search_project.lower():
-            match.append([project_name, version, released, description])
-        else:
-            others.append([project_name, version, released, description])
-
-    total_div_raw = soup.select(
-        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
-    )
-    total_raw = re.search(pattern, str(total_div_raw)).group(1)
-    total_str = total_raw.translate(str.maketrans("", "", string.punctuation))
-    others_total = int(total_str) - len(match)
-    return match, others, others_total
-
-
-def process_input_file(file):
-    file_path = Path(file)
-    if not file_path.exists():
-        raise SystemExit(f"The file {file} does not exist")
-    with file_path.open(mode="r") as file:
-        file_contents = file.read()
-        projects = file_contents.split()
-        projects_list = list(projects)
-        return list(set(projects_list))
-
-
-def write_output_file(file, message):
-    file_path = Path(file)
-    with file_path.open(mode="w") as file:
-        file.write(message)
-
-
-def final_analysis(pattern: list) -> None:
-    table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("FINAL ANALYSIS", style="cyan")
-    if pattern == [0, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search facility.\n"
-            "It can only be found by searching the simple index which is not available "
-            "through the interface"
-        )
-    elif pattern == [1, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search facility.\n"
-            "However if appears in the simple index and can be displayed by simply browsing "
-            "to the projects URL"
-        )
-    elif sum(pattern) > 1:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row("The package name was found in at least one place")
-    elif sum(pattern) == 0:
-        table.add_row("[green]AVAILABLE![/green]\n")
-        table.add_row("The package name was found in any part of PyPI")
-
-    console = Console()
-    console.print(table)
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        prog="pynamer",
-        description="Determine if project name is available on pypi with the "
-        "option to 'register' it for future use if available",
-    )
-    parser.add_argument(
-        "projects",
-        nargs="*",
-        default="None",
-        help="Optional - one or more project names",
-    )
-    parser.add_argument(
-        "-r",
-        "--register",
-        action="store_true",
-        help="Register the name on PyPi if the name is available",
-    )
-    parser.add_argument(
-        "-d",
-        "--dryrun",
-        action="store_true",
-        help="Perform all tests but without uploading a dist to PyPI",
-    )
-    parser.add_argument(
-        "-f",
-        "--file",
-        default="None",
-        type=str,
-        help="File containing a list of projects to analyze",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        default="None",
-        type=str,
-        help="File to output the results to",
-    )
-    parser.add_argument(
-        "-n",
-        "--nocleanup",
-        action="store_true",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="output additional information",
-    )
-    parser.add_argument(
-        "-g",
-        "--generate",
-        action="store_true",
-        help="Generate a new PyPI simple index",
-    )
-
-    args = parser.parse_args()
-    logger.debug(" args: %s", args)
-
-    if args.generate is True:
-        generate_pypi_index()
-
-    if args.projects == "None" and args.file == "None":
-        parser.print_help()
-        raise SystemExit("No projects to analyse")
-
-    project_list = []
-    test_results = []
-    find_pypirc_file()
-    if args.nocleanup is True:
-        config.NO_CLEANUP = True
-
-    if args.projects != "None":
-        logger.debug("adding project names from command line %s", args.projects)
-        project_list.extend(list(set(args.projects)))
-        logger.debug("project_list = %s", project_list)
-
-    if args.file != "None":
-        logger.debug("adding project names from file %s", args.file)
-        project_list.extend(process_input_file(args.file))
-        logger.debug("project_list = %s", project_list)
-
-    # Main loop
-    for new_project in project_list:
-        test_table = Table(title=f"Test Results for {new_project}")
-        test_table.add_column("No.", style="blue")
-        test_table.add_column("Test", style="bold green")
-        test_table.add_column("Result", style="bold yellow")
-        test_table.add_column("Details", style="bold cyan")
-
-        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
-        match_table.add_column("Package", style="blue")
-        match_table.add_column("Version", style="bold green")
-        match_table.add_column("Released", style="bold yellow")
-        match_table.add_column("Description", style="bold cyan")
-
-        others_table = Table(title="Other Close Matches or Related Projects")
-        others_table.add_column("Package", style="blue")
-        others_table.add_column("Version", style="bold green")
-        others_table.add_column("Released", style="bold yellow")
-        others_table.add_column("Description", style="bold cyan")
-
-        # perform the tests
-        if ping_project(new_project):
-            test_results.append(1)
-            json_data = ping_json(new_project)
-            test_table.add_row("1", "Basic http get to project URL", "FOUND", json_data)
-        else:
-            test_results.append(0)
-            test_table.add_row("1", "Basic http get to project URL", "NOT FOUND", "")
-
-        if pypi_search_index(new_project):
-            test_results.append(1)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "FOUND",
-                f"Searched {project_count} projects",
-            )
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "NOT FOUND",
-                f"Searched {project_count} projects",
-            )
-        match, others, others_total = pypi_search(new_project)
-
-        if match:
-            test_results.append(1)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "FOUND",
-                f"Exact match found: {len(match)}, Others found: {others_total}",
-            )
-            for items in match:
-                match_table.add_row(items[0], items[1], items[2], items[3])
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "NOT FOUND",
-                f"Exact match found: 0, Others found: {others_total}",
-            )
-        if others:
-            for items in others:
-                others_table.add_row(items[0], items[1], items[2], items[3])
-
-        console = Console()
-        console.print(test_table)
-        if match:
-            console.print(match_table)
-
-        if args.verbose and others:
-            console.print(others_table)
-
-        # build and upload
-        if (
-            test_results == [0, 0, 0]
-            and args.register is True
-            and config.PYPIRC is not None
-        ):
-            rename_project_dir(
-                project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
-                project_path.joinpath(new_project),
-            )
-            create_setup(new_project)
-            build_dist()
-            if args.dryrun is False:
-                upload_dist(new_project)
-            else:
-                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
-            cleanup(new_project)
-        elif config.PYPIRC is None:
-            _feedback(
-                ".pypirc file cannot be located ... wont attempt to 'register'",
-                "warning",
-            )
-        elif sum(test_results) > 0 and args.register is True:
-            _feedback(
-                "Project already exists ... wont attempt to 'register'", "warning"
-            )
-        final_analysis(test_results)
-
-
-if __name__ == "__main__":
-    SystemExit(main())
+#!/usr/bin/env python3
+
+# TODO: suppress verbose output from build.
+# TODO: add docstrings
+# TODO: add typing
+# TODO: add 'fix' function to check package structure and fix if necessary
+# TODO: add random standoff timer to prevent dossing PyPI
+# TODO: write tests
+# TODO: final version - turn off file logging
+# TODO: split and rename files into logical components
+
+
+# Core Library modules
+import argparse
+import json
+import os
+import pickle
+import re
+import shutil
+import string
+import subprocess
+import sys
+from datetime import datetime
+from pathlib import Path
+
+# Third party modules
+import build
+import requests  # type: ignore
+import yaml  # type: ignore
+from bs4 import BeautifulSoup
+from colorama import Back, Fore, Style
+from jinja2 import Template
+from rich.console import Console
+from rich.table import Table
+from tqdm import tqdm
+
+# Local modules
+from . import logger, project_count, project_path, setup_text
+
+
+class Config:
+    PYPIRC = None
+    ORIGINAL_PROJECT_NAME = "project_name"
+    NO_CLEANUP: bool = False
+    PROJECT_COUNT = 0
+    PACKAGE_VERSION = "0.0.0"
+    pypi_search_url: str = "https://pypi.org/search/"
+    pypi_project_url: str = "https://pypi.org/project/"
+    pypi_json_url: str = "https://pypi.org/pypi/"
+    IDLEMODE = 1 if "idlelib.run" in sys.modules else 0
+
+
+config = Config()
+config.PROJECT_COUNT = project_count
+
+
+def _feedback(message: str, feedback_type: str) -> None:
+    """A utility method to generate formatted messages appropriate to the
+    environment.
+
+    Args:
+        message:        Text to be echoed.
+        feedback_type:  identifies type of message to display.
+    """
+    if feedback_type not in ["null", "nominal", "warning", "error"]:
+        return
+    if config.IDLEMODE == 1:
+        print(message)
+    else:
+        if feedback_type == "null":
+            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "nominal":
+            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "warning":
+            print(
+                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
+            )
+        elif feedback_type == "error":
+            print(Fore.RED + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+
+
+def find_pypirc_file():
+    filename = ".pypirc"
+    system_path = os.getenv("PATH")
+    path_directories = list()
+    path_directories.append(os.getcwd())
+    path_directories.extend(system_path.split(os.pathsep))
+    for directory in path_directories:
+        file_path = Path(directory) / filename
+        if file_path.exists():
+            logger.debug(
+                "%s is present in the system's PATH at %s", filename, directory
+            )
+            config.PYPIRC = file_path
+            break
+    else:
+        logger.debug("%s is not present in the system's PATH.", filename)
+
+
+def rename_project_dir(old_name: str, new_name: str) -> None:
+    old_directory_path = Path(old_name)
+    new_directory_path = Path(new_name)
+    logger.debug("renaming project directory from %s to %s", old_name, new_name)
+    try:
+        old_directory_path.rename(new_directory_path)
+    except FileNotFoundError:
+        logger.error("directory %s cannot be found:", old_directory_path)
+
+
+def create_setup(new_project_name: str) -> None:
+    template = Template(setup_text)
+    content = template.render(
+        PROJECT_NAME=new_project_name,
+        PACKAGE_VERSION=config.PACKAGE_VERSION,
+    )
+    setup_file = project_path.joinpath("setup.py")
+    with open(setup_file, mode="w", encoding="utf-8") as message:
+        logger.debug("creating new setup.py with the following: \n %s", content)
+        message.write(content)
+
+
+def delete_director(items_to_delete: list) -> None:
+    """Utility function to delete files or directories"""
+    for item in items_to_delete:
+        if not item.exists():
+            logger.debug("trying to delete %s but it does not exist", item)
+            continue
+        if item.is_dir():
+            logger.debug("Deleting Directory: %s", item)
+            shutil.rmtree(item, ignore_errors=True)
+        else:
+            logger.debug("Deleting File: %s", item)
+            Path.unlink(item, missing_ok=True)
+
+
+def run_command(*arguments: str, shell=True, working_dir=None, project=None) -> None:
+    working_dir = os.getcwd() if working_dir is None else working_dir
+    try:
+        process = subprocess.Popen(
+            arguments,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            shell=shell,
+            text=True,
+            cwd=working_dir,
+        )
+        stdout, stderr = process.communicate()
+        if process.returncode != 0:
+            logger.error("Error running command: %s", arguments)
+            logger.error("stderr: %s", stderr)
+            cleanup(project)
+            return
+        logger.debug("%s", stdout)
+        return
+    except Exception as e:
+        logger.error("Exception running command: %s", arguments)
+        logger.error(e)
+        cleanup(project)
+        return
+
+
+def ping_project(new_project_name: str, output_file: str = None) -> bool:
+    url_project = "".join(["https://pypi.org/project/", new_project_name, "/"])
+    logger.debug("attempting to get url %s", url_project)
+    try:
+        project_ping = requests.get(url_project, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit(f"An error occurred with an HTTP request")
+    if project_ping.status_code == 200:
+        logger.debug("%s FOUND in the project area of PyPI", new_project_name)
+        if output_file is not None:
+            message = f"{new_project_name:20} is already registered"
+            write_output_file(output_file, message)
+        return True
+    else:
+        logger.debug("%s NOT FOUND in the project area of PyPI", new_project_name)
+        if output_file is not None:
+            message = f"{new_project_name:20} is available"
+            write_output_file(output_file, message)
+        return False
+
+
+def ping_json(new_project_name: str) -> str:
+    url_json = "".join(["https://pypi.org/pypi/", new_project_name, "/json"])
+    logger.debug("attempting to get url %s", url_json)
+    try:
+        project_json_raw = requests.get(url_json, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit(f"An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+        result = "".join(
+            [
+                project_json["info"]["author"],
+                "\n",
+                project_json["info"]["author_email"],
+                "\n",
+                project_json["info"]["version"],
+                "\n",
+                project_json["info"]["summary"],
+            ]
+        )
+        return result
+    else:
+        logger.debug("No response from JSON URL")
+        return ""
+
+
+def build_dist():
+    logger.debug("Building the distribution... ")
+    builder = build.ProjectBuilder(project_path)
+    builder.build("wheel", project_path / "dist")
+    builder.build("sdist", project_path / "dist")
+
+
+def upload_dist(project_name):
+    logger.debug("Uploading the distribution... ")
+    dir_path = os.fspath(project_path / "dist" / "*")
+    pypirc_path = os.fspath(config.PYPIRC)
+    run_command(
+        sys.executable,
+        "-m",
+        "twine",
+        "upload",
+        "--config-file",
+        pypirc_path,
+        dir_path,
+        project=project_name,
+    )
+
+
+def cleanup(new_project_name):
+    if config.NO_CLEANUP is True:
+        return
+    rename_project_dir(
+        project_path.joinpath(new_project_name),
+        project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
+    )
+    build_artifacts = [
+        project_path / "build",
+        project_path / "dist",
+        project_path / "".join([new_project_name, ".egg-info"]),
+        project_path / "setup.py",
+    ]
+    logger.debug("cleaning build artifacts %s", build_artifacts)
+    delete_director(build_artifacts)
+
+
+def generate_pypi_index() -> None:
+    new_count = 0
+    progress_bar = tqdm(total=config.PROJECT_COUNT)
+    pypi_index = project_path / "pypi_index.txt"
+    pypi_count = project_path / "project_count.pickle"
+    if pypi_index.exists():
+        Path.unlink(pypi_index, missing_ok=True)
+    try:
+        index_object_raw = requests.get("https://pypi.org/simple/", timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit(f"An error occurred with an HTTP request")
+    pattern = re.compile(r">([\w\W]*?)<")
+    with pypi_index.open(mode="a") as file:
+        for line in index_object_raw.iter_lines():
+            line = str(line)
+            project_text = re.search(pattern, line)
+            if project_text is not None:
+                new_count += 1
+                progress_bar.update(1)
+                project = "".join([project_text.group(1), " \n"])
+                file.write(project)
+    progress_bar.close()
+    with open(pypi_count, "wb") as f:
+        pickle.dump(new_count, f)
+
+
+def pypi_search_index(project_name):
+    pypi_index = project_path / "pypi_index.txt"
+    if not pypi_index.exists():
+        generate_pypi_index()
+    with pypi_index.open(mode="r") as file:
+        projects = file.read()
+        if project_name in projects:
+            logger.debug("%s FOUND in the PyPI simple index", project_name)
+            return True
+        else:
+            logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+            return False
+
+
+def pypi_search(search_project):
+    api_url: str = "https://pypi.org/search/"
+    pattern = re.compile(r">([\d,+]*?)<")
+    s = requests.Session()
+    projects_raw, match, others = [], [], []
+    params = {"q": {search_project}, "page": 1}
+    r = s.get(api_url, params=params)
+    soup = BeautifulSoup(r.text, "html.parser")
+    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
+    for project_raw in projects_raw:
+        project_name = project_raw.select_one(
+            'span[class*="package-snippet__name"]'
+        ).text.strip()
+        version = project_raw.select_one(
+            'span[class*="package-snippet__version"]'
+        ).text.strip()
+        released_iso_8601 = project_raw.select_one(
+            'span[class*="package-snippet__created"]'
+        ).find("time")["datetime"]
+        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
+            "%Y-%m-%d"
+        )
+        description = project_raw.select_one(
+            'p[class*="package-snippet__description"]'
+        ).text.strip()
+        if project_name.lower() == search_project.lower():
+            match.append([project_name, version, released, description])
+        else:
+            others.append([project_name, version, released, description])
+
+    total_div_raw = soup.select(
+        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
+    )
+    total_raw = re.search(pattern, str(total_div_raw)).group(1)
+    total = int(total_raw.translate(str.maketrans("", "", string.punctuation)))
+    others_total = (
+        "".join([str(total), "+"]) if total == 10000 else (str(int(total) - len(match)))
+    )
+
+    return match, others, others_total
+
+
+def process_input_file(file):
+    file_path = Path(file)
+    if not file_path.exists():
+        raise SystemExit(f"The file {file} does not exist")
+    with file_path.open(mode="r") as file:
+        file_contents = file.read()
+        projects = file_contents.split()
+        projects_list = list(projects)
+        return list(set(projects_list))
+
+
+def write_output_file(file, message):
+    file_path = Path(file)
+    with file_path.open(mode="w") as file:
+        file.write(message)
+
+
+def final_analysis(pattern: list) -> None:
+    table = Table(show_header=True, header_style="bold magenta")
+    table.add_column("FINAL ANALYSIS", style="cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the interface"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search facility.\n"
+            "However if appears in the simple index and can be displayed by simply browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) > 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        prog="pynamer",
+        description="Determine if project name is available on pypi with the "
+        "option to 'register' it for future use if available",
+    )
+    parser.add_argument(
+        "projects",
+        nargs="*",
+        default="None",
+        help="Optional - one or more project names",
+    )
+    parser.add_argument(
+        "-r",
+        "--register",
+        action="store_true",
+        help="Register the name on PyPi if the name is available",
+    )
+    parser.add_argument(
+        "-d",
+        "--dryrun",
+        action="store_true",
+        help="Perform all tests but without uploading a dist to PyPI",
+    )
+    parser.add_argument(
+        "-f",
+        "--file",
+        default="None",
+        type=str,
+        help="File containing a list of projects to analyze",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        default="None",
+        type=str,
+        help="File to output the results to",
+    )
+    parser.add_argument(
+        "-n",
+        "--nocleanup",
+        action="store_true",
+        help=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="output additional information",
+    )
+    parser.add_argument(
+        "-g",
+        "--generate",
+        action="store_true",
+        help="Generate a new PyPI simple index",
+    )
+
+    args = parser.parse_args()
+    logger.debug(" args: %s", args)
+
+    if args.generate is True:
+        generate_pypi_index()
+
+    if args.projects == "None" and args.file == "None":
+        parser.print_help()
+        raise SystemExit("No projects to analyse")
+
+    project_list = []
+    test_results = []
+    find_pypirc_file()
+    if args.nocleanup is True:
+        config.NO_CLEANUP = True
+
+    if args.projects != "None":
+        logger.debug("adding project names from command line %s", args.projects)
+        project_list.extend(list(set(args.projects)))
+        logger.debug("project_list = %s", project_list)
+
+    if args.file != "None":
+        logger.debug("adding project names from file %s", args.file)
+        project_list.extend(process_input_file(args.file))
+        logger.debug("project_list = %s", project_list)
+
+    # Main loop
+    for new_project in project_list:
+        test_table = Table(title=f"Test Results for {new_project}")
+        test_table.add_column("No.", style="blue")
+        test_table.add_column("Test", style="bold green")
+        test_table.add_column("Result", style="bold yellow")
+        test_table.add_column("Details", style="bold cyan")
+
+        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
+        match_table.add_column("Package", style="blue")
+        match_table.add_column("Version", style="bold green")
+        match_table.add_column("Released", style="bold yellow")
+        match_table.add_column("Description", style="bold cyan")
+
+        others_table = Table(title="Other Close Matches or Related Projects")
+        others_table.add_column("Package", style="blue")
+        others_table.add_column("Version", style="bold green")
+        others_table.add_column("Released", style="bold yellow")
+        others_table.add_column("Description", style="bold cyan")
+
+        # perform the tests
+        if ping_project(new_project):
+            test_results.append(1)
+            json_data = ping_json(new_project)
+            test_table.add_row("1", "Basic http get to project URL", "FOUND", json_data)
+        else:
+            test_results.append(0)
+            test_table.add_row("1", "Basic http get to project URL", "NOT FOUND", "")
+
+        if pypi_search_index(new_project):
+            test_results.append(1)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "FOUND",
+                f"Searched {project_count} projects",
+            )
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "NOT FOUND",
+                f"Searched {project_count} projects",
+            )
+        match, others, others_total = pypi_search(new_project)
+
+        if match:
+            test_results.append(1)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "FOUND",
+                f"Exact match found: {len(match)}, Others found: {others_total}",
+            )
+            for items in match:
+                match_table.add_row(items[0], items[1], items[2], items[3])
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "NOT FOUND",
+                f"Exact match found: 0, Others found: {others_total}",
+            )
+        if others:
+            for items in others:
+                others_table.add_row(items[0], items[1], items[2], items[3])
+
+        console = Console()
+        console.print(test_table)
+        if match:
+            console.print(match_table)
+
+        if args.verbose and others:
+            console.print(others_table)
+
+        # build and upload
+        if (
+            test_results == [0, 0, 0]
+            and args.register is True
+            and config.PYPIRC is not None
+        ):
+            rename_project_dir(
+                project_path.joinpath(config.ORIGINAL_PROJECT_NAME),
+                project_path.joinpath(new_project),
+            )
+            create_setup(new_project)
+            build_dist()
+            if args.dryrun is False:
+                upload_dist(new_project)
+            else:
+                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
+            cleanup(new_project)
+        elif config.PYPIRC is None:
+            _feedback(
+                ".pypirc file cannot be located ... wont attempt to 'register'",
+                "warning",
+            )
+        elif sum(test_results) > 0 and args.register is True:
+            _feedback(
+                "Project already exists ... wont attempt to 'register'", "warning"
+            )
+        final_analysis(test_results)
+
+
+if __name__ == "__main__":
+    SystemExit(main())
```

### Comparing `pynamer-0.5.0/src/pynamer/pypi_index.txt` & `pynamer-0.5.1/src/pynamer/pypi_index.txt`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.0/src/pynamer.egg-info/PKG-INFO` & `pynamer-0.5.1/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
```

