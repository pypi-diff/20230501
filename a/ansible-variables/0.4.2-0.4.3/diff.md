# Comparing `tmp/ansible-variables-0.4.2.tar.gz` & `tmp/ansible-variables-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.4.2.tar", last modified: Sun Apr 23 15:32:04 2023, max compression
+gzip compressed data, was "ansible-variables-0.4.3.tar", last modified: Mon May  1 16:10:58 2023, max compression
```

## Comparing `ansible-variables-0.4.2.tar` & `ansible-variables-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_variablesource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.647362 ansible-variables-0.4.3/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:10:58.000000 ansible-variables-0.4.3/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:10:58.651362 ansible-variables-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 16:10:37.000000 ansible-variables-0.4.3/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.4.2/LICENSE` & `ansible-variables-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.2/PKG-INFO` & `ansible-variables-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.2
+Version: 0.4.3
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
-Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
+Project-URL: Repository, https://github.com/hille721/ansible-variables
+Project-URL: Changelog, https://github.com/hille721/ansible-variables/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -27,30 +29,33 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ansible-variables
 
-[![PyPI version][pypi-version]][pypi-link]
-[![PyPI platforms][pypi-platforms]][pypi-link]
+[![PyPI version][pypi-version-badge]][pypi-link]
+[![PyPI platforms][pypi-platforms-badge]][pypi-link]
+[![pre-commit][pre-commit-badge]][pre-commit-link]
 
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
 There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
+Tested with `ansible-core` 2.11 - 2.15.
+
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
@@ -116,9 +121,11 @@
 * the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
 
 [pypi-link]:                https://pypi.org/project/ansible-variables/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
-[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
+[pypi-platforms-badge]:     https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version-badge]:       https://badge.fury.io/py/ansible-variables.svg
+[pre-commit-badge]:         https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>
+[pre-commit-link]:          https://pre-commit.com/
```

### Comparing `ansible-variables-0.4.2/README.md` & `ansible-variables-0.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # ansible-variables
 
-[![PyPI version][pypi-version]][pypi-link]
-[![PyPI platforms][pypi-platforms]][pypi-link]
+[![PyPI version][pypi-version-badge]][pypi-link]
+[![PyPI platforms][pypi-platforms-badge]][pypi-link]
+[![pre-commit][pre-commit-badge]][pre-commit-link]
 
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
 There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
+Tested with `ansible-core` 2.11 - 2.15.
+
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
@@ -85,9 +88,11 @@
 * the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
 
 [pypi-link]:                https://pypi.org/project/ansible-variables/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
-[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
+[pypi-platforms-badge]:     https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version-badge]:       https://badge.fury.io/py/ansible-variables.svg
+[pre-commit-badge]:         https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>
+[pre-commit-link]:          https://pre-commit.com/
```

### Comparing `ansible-variables-0.4.2/lib/ansible_variables/utils/vars.py` & `ansible-variables-0.4.3/lib/ansible_variables/utils/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import contextlib
-from dataclasses import dataclass
 import io
-from typing import Optional, List
 import re
+from dataclasses import dataclass
+from typing import List, Optional
 
 from ansible import constants as C
 from ansible.inventory.host import Host
-from ansible.utils.display import Display
 from ansible.parsing.dataloader import DataLoader
+from ansible.utils.display import Display
 from ansible.vars.manager import VariableManager, VarsWithSources
 
 display = Display()
 
 
 @dataclass
 class VariableSource:
```

### Comparing `ansible-variables-0.4.2/lib/ansible_variables.egg-info/PKG-INFO` & `ansible-variables-0.4.3/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.2
+Version: 0.4.3
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
-Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
+Project-URL: Repository, https://github.com/hille721/ansible-variables
+Project-URL: Changelog, https://github.com/hille721/ansible-variables/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -27,30 +29,33 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ansible-variables
 
-[![PyPI version][pypi-version]][pypi-link]
-[![PyPI platforms][pypi-platforms]][pypi-link]
+[![PyPI version][pypi-version-badge]][pypi-link]
+[![PyPI platforms][pypi-platforms-badge]][pypi-link]
+[![pre-commit][pre-commit-badge]][pre-commit-link]
 
 The Ansible inventory provides a very powerful framework to declare variables in a hierarchical manner.
 There a lof of different places where a variable can be defined (inventory, host_vars, groups_vars, ...) and Ansible will merge them in a specific order ([variable precedence](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence)).
 
 `ansible-variables` will help to keep track of your host context variables:
 
 * inventory file or script group vars
 * inventory group_vars/all
 * inventory group_vars/*
 * inventory file or script host vars
 * inventory host_vars/*
 
 Based on one host it will return a list with all variables, values and variable type.
 
+Tested with `ansible-core` 2.11 - 2.15.
+
 ## Installation
 
 ```bash
 pip install ansible-variables
 ```
 
 ## Usage
@@ -116,9 +121,11 @@
 * the screenshots used  in this README where created with [termshot](https://github.com/homeport/termshot)
 
 ## License
 
 This project is licensed under the [GNU General Public License v3.0](https://github.com/hille721/ansible-variables/blob/main/LICENSE)
 
 [pypi-link]:                https://pypi.org/project/ansible-variables/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/ansible-variables
-[pypi-version]:             https://badge.fury.io/py/ansible-variables.svg
+[pypi-platforms-badge]:     https://img.shields.io/pypi/pyversions/ansible-variables
+[pypi-version-badge]:       https://badge.fury.io/py/ansible-variables.svg
+[pre-commit-badge]:         https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>
+[pre-commit-link]:          https://pre-commit.com/
```

### Comparing `ansible-variables-0.4.2/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.4.3/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.2/setup.cfg` & `ansible-variables-0.4.3/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [metadata]
 name = ansible-variables
-version = 0.4.2
+version = 0.4.3
 description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls = 
-	Bug Tracker=https://github.com/hille721/ansible-variables/issues
 	Documentation=https://github.com/hille721/ansible-variables/blob/main/README.md
+	Repository=https://github.com/hille721/ansible-variables
+	Changelog=https://github.com/hille721/ansible-variables/blob/main/CHANGELOG.md
+	Bug Tracker=https://github.com/hille721/ansible-variables/issues
 license = GPLv3+
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
@@ -34,15 +36,15 @@
 zip_safe = False
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=lib
 packages = find:
 install_requires = 
-	ansible-core
+	ansible-core>=2.11.0
 	rich
 
 [options.packages.find]
 where = lib
 exclude = 
 	tests
```

### Comparing `ansible-variables-0.4.2/tests/test_cli.py` & `ansible-variables-0.4.3/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from ansible import constants as C
 
 from ansible_variables.cli.variables import VariablesCLI
 
 C.set_constant("CONFIG_FILE", "tests/test_data/ansible.cfg")
 C.set_constant("DEFAULT_HOST_LIST", "tests/test_data/inventory")
```

### Comparing `ansible-variables-0.4.2/tests/test_utils.py` & `ansible-variables-0.4.3/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ansible import constants as C
-from ansible.parsing.dataloader import DataLoader
 from ansible.inventory.manager import InventoryManager
+from ansible.parsing.dataloader import DataLoader
 from ansible.vars.manager import VariableManager
 
 from ansible_variables.utils.vars import variable_sources
 
 C.set_constant("CONFIG_FILE", "tests/test_data/ansible.cfg")
 
 loader = DataLoader()
```

### Comparing `ansible-variables-0.4.2/tests/test_variablesource.py` & `ansible-variables-0.4.3/tests/test_variablesource.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
-
 from ansible import constants as C
 from ansible.errors import AnsibleFileNotFound
 from ansible.parsing.dataloader import DataLoader
+
 from ansible_variables.utils.vars import VariableSource
 
 DEBUGLOG = """
 29355 1681471136.41205:  29355 1681471136.40830: in VariableManager get_vars()
 29355 1681471136.40839: Calling all_inventory to load vars for server1
 29355 1681471136.40842: Calling groups_inventory to load vars for server1
 29355 1681471136.40850: Calling all_plugins_inventory to load vars for server1
```

