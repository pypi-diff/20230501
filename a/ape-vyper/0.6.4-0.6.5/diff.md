# Comparing `tmp/ape-vyper-0.6.4.tar.gz` & `tmp/ape-vyper-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.4.tar", last modified: Tue Apr 25 12:31:34 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.5.tar", last modified: Mon May  1 16:01:52 2023, max compression
```

## Comparing `ape-vyper-0.6.4.tar` & `ape-vyper-0.6.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19829 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.009209 ape-vyper-0.6.4/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.009209 ape-vyper-0.6.4/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/erc20.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 16:01:52.000000 ape-vyper-0.6.5/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 16:01:51.000000 ape-vyper-0.6.5/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.044531 ape-vyper-0.6.5/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:01:52.048531 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-01 16:00:37.000000 ape-vyper-0.6.5/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/.github/release-drafter.yml` & `ape-vyper-0.6.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.5/.github/workflows/prtitle.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
-          run: pip install commitizen
+          run: |
+            python -m pip install --upgrade pip
+            pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
           run: cz check --message "$TITLE"
```

### Comparing `ape-vyper-0.6.4/.github/workflows/publish.yaml` & `ape-vyper-0.6.5/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-vyper-0.6.4/.github/workflows/test.yaml` & `ape-vyper-0.6.5/.github/workflows/test.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
-          run: pip install .[lint]
+          run: |
+            python -m pip install --upgrade pip
+            pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
         - name: Run isort
           run: isort --check-only .
 
@@ -44,18 +46,20 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
-          run: pip install .[lint,test]  # Might need test deps
+          run: |
+            python -m pip install --upgrade pip
+            pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
@@ -69,15 +73,17 @@
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
-          run: pip install .[test]
+          run: |
+            python -m pip install --upgrade pip
+            pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing" -n 0 -s --cov
 
 # NOTE: uncomment this block after you've marked tests with @pytest.mark.fuzzing
 #    fuzzing:
 #        runs-on: ubuntu-latest
@@ -87,14 +93,16 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
-#          run: pip install .[test]
+#          run: |
+#             python -m pip install --upgrade pip
+#             pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-vyper-0.6.4/.gitignore` & `ape-vyper-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/.pre-commit-config.yaml` & `ape-vyper-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/CONTRIBUTING.md` & `ape-vyper-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/LICENSE` & `ape-vyper-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/PKG-INFO` & `ape-vyper-0.6.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-vyper
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-vyper.git
-        cd ape-vyper
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, place Vyper contract source files (files with extension `.vy`) in your Ape project's contracts folder.
-        An example Vyper contract can be found [here](https://vyper.readthedocs.io/en/stable/vyper-by-example.html).
-        Then, from your root Ape project folder, run the command:
-        
-        ```bash
-        ape compile
-        ```
-        
-        The `.vy` files in your project will compile into `ContractTypes` that you can deploy and interact with in Ape.
-        
-        ### Interfaces
-        
-        You can not compile interface source files directly.
-        Thus, you must place interface files in a directory named `interfaces` in your `contracts_folder` e.g. `contracts/interfaces/IFace.vy`.
-        Then, these files can be imported in other `.vy` sources files via:
-        
-        ```python
-        import interfaces.IFace as IFace
-        ```
-        
-        Alternatively, use JSON interfaces from dependency contract types by listing them under the `import_remapping` key:
-        
-        ```yaml
-        # Use `voting` example contracts from Vyperlang repo.
-        dependencies:
-          - name: VyperVoting
-            github: vyperlang/vyper
-            contracts_folder: examples/voting/
-            version: v0.3.7
-        
-        # Automatically allow importing voting contracts in your project.
-        vyper:
-          import_remapping:
-            - "voting=VyperVoting@v0.3.7"
-        ```
-        
-        Import the voting contract types like this:
-        
-        ```python
-        # @version 0.3.7
-        
-        import voting.ballot as ballot
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -94,7 +19,82 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-vyper
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-vyper.git
+cd ape-vyper
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, place Vyper contract source files (files with extension `.vy`) in your Ape project's contracts folder.
+An example Vyper contract can be found [here](https://vyper.readthedocs.io/en/stable/vyper-by-example.html).
+Then, from your root Ape project folder, run the command:
+
+```bash
+ape compile
+```
+
+The `.vy` files in your project will compile into `ContractTypes` that you can deploy and interact with in Ape.
+
+### Interfaces
+
+You can not compile interface source files directly.
+Thus, you must place interface files in a directory named `interfaces` in your `contracts_folder` e.g. `contracts/interfaces/IFace.vy`.
+Then, these files can be imported in other `.vy` sources files via:
+
+```python
+import interfaces.IFace as IFace
+```
+
+Alternatively, use JSON interfaces from dependency contract types by listing them under the `import_remapping` key:
+
+```yaml
+# Use `voting` example contracts from Vyperlang repo.
+dependencies:
+  - name: VyperVoting
+    github: vyperlang/vyper
+    contracts_folder: examples/voting/
+    version: v0.3.7
+
+# Automatically allow importing voting contracts in your project.
+vyper:
+  import_remapping:
+    - "voting=VyperVoting@v0.3.7"
+```
+
+Import the voting contract types like this:
+
+```python
+# @version 0.3.7
+
+import voting.ballot as ballot
+```
```

### Comparing `ape-vyper-0.6.4/README.md` & `ape-vyper-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/ape_vyper/compiler.py` & `ape-vyper-0.6.5/ape_vyper/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,73 +239,92 @@
                     vyper_version=vyper_version,
                     vyper_binary=vyper_binary,
                 )
             except VyperError as err:
                 raise VyperCompileError(err) from err
 
             for source_id, output_items in result["contracts"].items():
+                content = {
+                    i + 1: ln
+                    for i, ln in enumerate((base_path / source_id).read_text().splitlines())
+                }
                 for name, output in output_items.items():
                     # De-compress source map to get PC POS map.
                     ast = ASTNode.parse_obj(result["sources"][source_id]["ast"])
+
+                    # Track function offsets.
+                    function_offsets = []
+                    for node in ast.children:
+                        lineno = node.lineno
+
+                        # NOTE: Constructor is handled elsewhere.
+                        if node.ast_type == "FunctionDef" and "__init__" not in content.get(
+                            lineno, ""
+                        ):
+                            function_offsets.append((node.lineno, node.end_lineno))
+
                     bytecode = output["evm"]["deployedBytecode"]
                     opcodes = bytecode["opcodes"].split(" ")
                     compressed_src_map = SourceMap(__root__=bytecode["sourceMap"])
                     src_map = list(compressed_src_map.parse())[1:]
                     pc = 0
                     pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
-                    content = {
-                        i + 1: ln
-                        for i, ln in enumerate((base_path / source_id).read_text().splitlines())
-                    }
                     last_value = None
                     revert_pc = -1
+                    revert_pc_offset = 18
                     if _is_nonpayable_check(opcodes):
                         # Starting in vyper 0.2.14, reverts without a reason string are optimized
                         # with a jump to the "end" of the bytecode.
                         revert_pc = (
                             len(opcodes)
                             + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
-                            - 18
+                            - revert_pc_offset
                         )
 
                     processed_opcodes = []
+                    last_pc = None
+                    non_payable_str = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
+
                     while src_map and opcodes:
                         src = src_map.pop(0)
                         op = opcodes.pop(0)
                         processed_opcodes.append(op)
-                        start_pc = pc
+                        if pc not in [x[0] for x in pc_map_list]:
+                            # Track the last unused PC location.
+                            last_pc = pc
+
                         pc += 1
-                        if opcodes and is_0x_prefixed(opcodes[0]):
-                            last_value = int(opcodes.pop(0), 16)
-                            pc += int(op[4:])
 
-                        # Check for special Payable case.
-                        if src.start is None:
-                            if (
-                                op == "REVERT"
-                                and len(processed_opcodes) > 6
-                                and processed_opcodes[-7] == "CALLVALUE"
-                            ) or _is_revert_jump(op, last_value, revert_pc, processed_opcodes):
-                                pc_map_item = {
-                                    "location": None,
-                                    "dev": f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}",
-                                }
-                                pc_map_list.append(
-                                    (pc if op == "REVERT" else start_pc, pc_map_item)
-                                )
+                        # Detect immutable state member load.
+                        # If this is the case, ignore increasing pc by push size.
+                        is_code_copy = len(opcodes) > 5 and opcodes[5] == "CODECOPY"
 
-                            continue
+                        if not is_code_copy and opcodes and is_0x_prefixed(opcodes[0]):
+                            last_value = int(opcodes.pop(0), 16)
+                            # Add the push number, e.g. PUSH1 adds `1`.
+                            num_pushed = int(op[4:])
+                            pc += num_pushed
 
                         # Add content PC item.
                         # Also check for compiler runtime error handling.
                         # Runtime error locations are marked in the PCMap for further analysis.
                         if src.start is not None and src.length is not None:
                             stmt = ast.get_node(src)
                             if stmt:
-                                item: Dict = {"location": list(stmt.line_numbers)}
+                                line_nos = list(stmt.line_numbers)
+                                # Add next non-payable check.
+                                if last_pc is not None and len(function_offsets) > 0:
+                                    next_fn = function_offsets[0]
+                                    if line_nos[0] >= next_fn[0] and line_nos[2] <= next_fn[1]:
+                                        np_check = {"location": None, "dev": non_payable_str}
+                                        pc_map_list.append((last_pc, np_check))
+                                        function_offsets.pop(0)
+
+                                # Add located item.
+                                item: Dict = {"location": line_nos}
                                 is_revert_jump = _is_revert_jump(
                                     op, last_value, revert_pc, processed_opcodes
                                 )
                                 if op == "REVERT" or is_revert_jump:
                                     dev = None
                                     if stmt.ast_type in ("AugAssign", "BinOp"):
                                         # SafeMath
```

### Comparing `ape-vyper-0.6.4/ape_vyper/exceptions.py` & `ape-vyper-0.6.5/ape_vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.5/ape_vyper.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-vyper
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-vyper.git
-        cd ape-vyper
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, place Vyper contract source files (files with extension `.vy`) in your Ape project's contracts folder.
-        An example Vyper contract can be found [here](https://vyper.readthedocs.io/en/stable/vyper-by-example.html).
-        Then, from your root Ape project folder, run the command:
-        
-        ```bash
-        ape compile
-        ```
-        
-        The `.vy` files in your project will compile into `ContractTypes` that you can deploy and interact with in Ape.
-        
-        ### Interfaces
-        
-        You can not compile interface source files directly.
-        Thus, you must place interface files in a directory named `interfaces` in your `contracts_folder` e.g. `contracts/interfaces/IFace.vy`.
-        Then, these files can be imported in other `.vy` sources files via:
-        
-        ```python
-        import interfaces.IFace as IFace
-        ```
-        
-        Alternatively, use JSON interfaces from dependency contract types by listing them under the `import_remapping` key:
-        
-        ```yaml
-        # Use `voting` example contracts from Vyperlang repo.
-        dependencies:
-          - name: VyperVoting
-            github: vyperlang/vyper
-            contracts_folder: examples/voting/
-            version: v0.3.7
-        
-        # Automatically allow importing voting contracts in your project.
-        vyper:
-          import_remapping:
-            - "voting=VyperVoting@v0.3.7"
-        ```
-        
-        Import the voting contract types like this:
-        
-        ```python
-        # @version 0.3.7
-        
-        import voting.ballot as ballot
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -94,7 +19,82 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-vyper
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-vyper.git
+cd ape-vyper
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, place Vyper contract source files (files with extension `.vy`) in your Ape project's contracts folder.
+An example Vyper contract can be found [here](https://vyper.readthedocs.io/en/stable/vyper-by-example.html).
+Then, from your root Ape project folder, run the command:
+
+```bash
+ape compile
+```
+
+The `.vy` files in your project will compile into `ContractTypes` that you can deploy and interact with in Ape.
+
+### Interfaces
+
+You can not compile interface source files directly.
+Thus, you must place interface files in a directory named `interfaces` in your `contracts_folder` e.g. `contracts/interfaces/IFace.vy`.
+Then, these files can be imported in other `.vy` sources files via:
+
+```python
+import interfaces.IFace as IFace
+```
+
+Alternatively, use JSON interfaces from dependency contract types by listing them under the `import_remapping` key:
+
+```yaml
+# Use `voting` example contracts from Vyperlang repo.
+dependencies:
+  - name: VyperVoting
+    github: vyperlang/vyper
+    contracts_folder: examples/voting/
+    version: v0.3.7
+
+# Automatically allow importing voting contracts in your project.
+vyper:
+  import_remapping:
+    - "voting=VyperVoting@v0.3.7"
+```
+
+Import the voting contract types like this:
+
+```python
+# @version 0.3.7
+
+import voting.ballot as ballot
+```
```

### Comparing `ape-vyper-0.6.4/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.5/ape_vyper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.5/ape_vyper.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 eth-ape<0.7,>=0.6.8
-ethpm-types>=0.4.3
+ethpm-types>=0.4.4
 tqdm
 vvm<0.2,>=0.1.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `ape-vyper-0.6.4/pyproject.toml` & `ape-vyper-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/setup.py` & `ape-vyper-0.6.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.8,<0.7",
-        "ethpm-types>=0.4.3",  # Use same version as eth-ape
+        "ethpm-types>=0.4.4",
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     license="Apache-2.0",
```

### Comparing `ape-vyper-0.6.4/tests/conftest.py` & `ape-vyper-0.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.6.5/tests/contracts/passing_contracts/erc20.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.4/tests/test_compiler.py` & `ape-vyper-0.6.5/tests/test_compiler.py`

 * *Files 25% similar despite different names*

```diff
@@ -177,32 +177,102 @@
     from `compile_src()` which includes the uncompressed source map data.
     """
 
     path = PASSING_BASE / "contract.vy"
     result = compiler.compile([path], base_path=PASSING_BASE)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
-    src_map = compile_source(code)["<stdin>"]["source_map"]
-
-    def item(dev: RuntimeErrorType, location=None):
-        return {"dev": f"dev: {dev.value}", "location": location}
+    compile_result = compile_source(code)["<stdin>"]
+    src_map = compile_result["source_map"]
+    lines = code.splitlines()
 
+    # Use the old-fashioned way of gathering PCMap to ensure our creative way works
     expected = {pc: {"location": ln} for pc, ln in src_map["pc_pos_map"].items()}
-    expected["23"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["52"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["73"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["94"] = item(RuntimeErrorType.INTEGER_OVERFLOW, [14, 12, 14, 20])
-    expected["151"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["188"] = item(RuntimeErrorType.INTEGER_UNDERFLOW, [19, 11, 19, 25])
-    expected["229"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["249"] = item(RuntimeErrorType.DIVISION_BY_ZERO, [24, 11, 24, 16])
-    expected["288"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["308"] = item(RuntimeErrorType.MODULO_BY_ZERO, [29, 11, 29, 16])
-    expected["351"] = item(RuntimeErrorType.INDEX_OUT_OF_RANGE, [34, 11, 34, 24])
-    expected["392"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    expected["405"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
-    assert actual == expected
+    missing_pcs = []
+    empty_locs = []
+    wrong_locs = []
+    for expected_pc, item_dict in expected.items():
+        expected_loc = item_dict["location"]
+
+        # Collect matching locations.
+        matching_locs = []
+        for mpc, loc in actual.items():
+            if loc["location"] == expected_loc:
+                matching_locs.append(mpc)
+
+        if expected_pc not in actual:
+            missing_pcs.append((expected_pc, expected_loc, matching_locs))
+            continue
+
+        if actual[expected_pc]["location"] is None:
+            empty_locs.append((expected_pc, expected_loc, matching_locs))
+            continue
+
+        if actual[expected_pc]["location"] != expected_loc:
+            wrong_locs.append((expected_pc, expected_loc, matching_locs))
+
+    limit = 10  # Only show first ten failures of each category.
+
+    def make_failure(title, ls):
+        fail_format = "PC={pc}, Expected={ex} (actual matches={match})"
+        suffix = ", ".join([fail_format.format(pc=m, ex=e, match=mat) for m, e, mat in ls[:limit]])
+        return f"{title}: {suffix}"
+
+    failures = []
+    if len(missing_pcs) != 0:
+        failures.append((missing_pcs[0][0], make_failure("Missing PCs", missing_pcs)))
+    if len(empty_locs) != 0:
+        failures.append((empty_locs[0][0], make_failure("Empty locations", empty_locs)))
+    if len(wrong_locs) != 0:
+        failures.append((wrong_locs[0][0], make_failure("Wrong locations", wrong_locs)))
+
+    # Show first failures to occur first.
+    failures.sort(key=lambda x: x[0])
+
+    assert len(failures) == 0, "\n".join([x[1] for x in failures])
+
+    # Test helper methods.
+    def _all(check):
+        return [x for x in actual.values() if x.get("dev") == f"dev: {check.value}"]
+
+    def line(cont: str) -> int:
+        # A helper for getting expected line numbers
+        return [i + 1 for i, x in enumerate(lines) if cont in x][0]
+
+    # Verify non-payable checks.
+    nonpayable_checks = _all(RuntimeErrorType.NONPAYABLE_CHECK)
+    assert len(nonpayable_checks) >= 8
+
+    # Verify integer overflow checks
+    overflows = _all(RuntimeErrorType.INTEGER_OVERFLOW)
+    overflow_no = line("return (2**127-1) + i")
+    assert len(overflows) == 2
+    assert overflows[0]["location"] == [overflow_no, 12, overflow_no, 20]
+
+    # Verify integer underflow checks
+    underflows = _all(RuntimeErrorType.INTEGER_UNDERFLOW)
+    underflow_no = line("return i - (2**127-1)")
+    assert len(underflows) == 2
+    assert underflows[0]["location"] == [underflow_no, 11, underflow_no, 25]
+
+    # Verify division by zero checks
+    div_zeros = _all(RuntimeErrorType.DIVISION_BY_ZERO)
+    div_no = line("return 4 / i")
+    assert len(div_zeros) == 1
+    assert div_zeros[0]["location"] == [div_no, 11, div_no, 16]
+
+    # Verify modulo by zero checks
+    mod_zeros = _all(RuntimeErrorType.MODULO_BY_ZERO)
+    mod_no = line("return 4 % i")
+    assert len(mod_zeros) == 1
+    assert mod_zeros[0]["location"] == [mod_no, 11, mod_no, 16]
+
+    # Verify index out of range checks
+    range_checks = _all(RuntimeErrorType.INDEX_OUT_OF_RANGE)
+    range_no = line("return self.dynArray[idx]")
+    assert len(range_checks) == 1
+    assert range_checks[0]["location"] == [range_no, 11, range_no, 24]
 
 
 def test_enrich_error(contract_logic_error, compiler):
     actual = compiler.enrich_error(contract_logic_error)
     assert isinstance(actual, NonPayableError)
```

