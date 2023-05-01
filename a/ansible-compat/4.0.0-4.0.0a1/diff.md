# Comparing `tmp/ansible-compat-4.0.0.tar.gz` & `tmp/ansible-compat-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.0.tar", last modified: Fri Apr 28 13:57:26 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.0a1.tar", last modified: Mon May  1 08:52:50 2023, max compression
```

## Comparing `ansible-compat-4.0.0.tar` & `ansible-compat-4.0.0a1.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.183455 ansible-compat-4.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.187455 ansible-compat-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.187455 ansible-compat-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.191455 ansible-compat-4.0.0/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.195455 ansible-compat-4.0.0/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/src/ansible_compat/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.195455 ansible-compat-4.0.0/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 13:57:26.000000 ansible-compat-4.0.0/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.199455 ansible-compat-4.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.203455 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/collections/acme.goodies/roles/baz/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.175455 ansible-compat-4.0.0/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.179455 ansible-compat-4.0.0/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:57:26.207455 ansible-compat-4.0.0/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-28 13:57:07.000000 ansible-compat-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.196787 ansible-compat-4.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.200787 ansible-compat-4.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.200787 ansible-compat-4.0.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.200787 ansible-compat-4.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.200787 ansible-compat-4.0.0a1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.180787 ansible-compat-4.0.0a1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.204788 ansible-compat-4.0.0a1/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.204788 ansible-compat-4.0.0a1/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.180787 ansible-compat-4.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.208788 ansible-compat-4.0.0a1/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.208788 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-01 08:52:50.000000 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-01 08:52:50.000000 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:52:50.000000 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 08:52:50.000000 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 08:52:50.000000 ansible-compat-4.0.0a1/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.212788 ansible-compat-4.0.0a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.216788 ansible-compat-4.0.0a1/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.184787 ansible-compat-4.0.0a1/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.216788 ansible-compat-4.0.0a1/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.216788 ansible-compat-4.0.0a1/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.184787 ansible-compat-4.0.0a1/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.216788 ansible-compat-4.0.0a1/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.184787 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.184787 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.184787 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/collections/acme.goodies/roles/baz/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.188787 ansible-compat-4.0.0a1/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.188787 ansible-compat-4.0.0a1/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.188787 ansible-compat-4.0.0a1/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.188787 ansible-compat-4.0.0a1/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.188787 ansible-compat-4.0.0a1/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:52:50.220788 ansible-compat-4.0.0a1/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24524 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-01 08:52:34.000000 ansible-compat-4.0.0a1/tox.ini
```

### Comparing `ansible-compat-4.0.0/.github/dependabot.yml` & `ansible-compat-4.0.0a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/.github/workflows/release.yml` & `ansible-compat-4.0.0a1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/.github/workflows/tox.yml` & `ansible-compat-4.0.0a1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/.gitignore` & `ansible-compat-4.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/.pre-commit-config.yaml` & `ansible-compat-4.0.0a1/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,21 @@
   python: python3.9
 exclude: |
   (?x)^(
     test/assets/.*
   )$
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.261"
+    rev: "v0.0.263"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.0-alpha.6"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
@@ -49,45 +49,39 @@
       - id: debug-statements
         language_version: python3
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.30.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        args:
-          # https://github.com/pre-commit/mirrors-isort/issues/9#issuecomment-624404082
-          - --filter-files
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
           - ansible-core
           - cached_property
           - packaging
           - pytest
           - pytest-mock
           - subprocess-tee>=0.4.1
+          - "typing-extensions>=4.5.0;python_version<'3.10'"
           - types-PyYAML
           - types-pkg_resources
           - types-jsonschema>=4.4.9
   - repo: https://github.com/pycqa/pylint
     rev: v3.0.0a6
     hooks:
       - id: pylint
@@ -99,21 +93,21 @@
   - repo: local
     hooks:
       - id: pip-compile-upgrade
         # To run it execute: `pre-commit run pip-compile-upgrade --hook-stage manual`
         name: Upgrade constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking --upgrade -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib
+        entry: python -m piptools compile --resolver=backtracking --upgrade -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib --unsafe-package typing_extensions
         pass_filenames: false
         stages:
           - manual
         additional_dependencies:
           - pip-tools>=6.11.0
       - id: pip-compile
         name: Check constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
-        entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib
+        entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib --unsafe-package typing_extensions
         pass_filenames: false
         additional_dependencies:
           - pip-tools>=6.11.0
```

### Comparing `ansible-compat-4.0.0/.readthedocs.yml` & `ansible-compat-4.0.0a1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/LICENSE` & `ansible-compat-4.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/PKG-INFO` & `ansible-compat-4.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.0
+Version: 4.0.0a1
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.0/README.md` & `ansible-compat-4.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/docs/images/favicon.ico` & `ansible-compat-4.0.0a1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/docs/images/logo.png` & `ansible-compat-4.0.0a1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/docs/images/logo.svg` & `ansible-compat-4.0.0a1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.0a1/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/mkdocs.yml` & `ansible-compat-4.0.0a1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/pyproject.toml` & `ansible-compat-4.0.0a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 dependencies = [
   # https://docs.ansible.com/ansible/latest/reference_appendices/release_and_maintenance.html
   "ansible-core>=2.12",
   "packaging",
   "PyYAML",
   "subprocess-tee>=0.4.1",
   "jsonschema>=4.6.0",
+  "typing-extensions>=4.5.0;python_version<'3.10'",
 ]
 
 [project.urls]
 homepage = "https://github.com/ansible/ansible-compat"
 documentation = "https://ansible-compat.readthedocs.io/"
 repository = "https://github.com/ansible/ansible-compat"
 changelog = "https://github.com/ansible/ansible-compat/releases"
@@ -89,15 +90,15 @@
   "f", # filename
   "i",
   "j",
   "k",
   "ns", # namespace
   "ex",
   "Run",
-  "_"
+  "_",
 ]
 
 [tool.pylint.IMPORTS]
 preferred-modules = ["unittest:pytest"]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
@@ -110,19 +111,35 @@
 ]
 
 [tool.pytest.ini_options]
 # ensure we treat warnings as error
 filterwarnings = ["error"]
 
 [tool.ruff]
-select = ["PT"]
+select = ["ALL"]
 ignore = [
+  # Disabled on purpose:
+  "ANN101", # Missing type annotation for `self` in method
+  "D203", # incompatible with D211
+  "D213", # incompatible with D212
   "E501", # we use black
+  "RET504", # Unnecessary variable assignment before `return` statement
+  # Temporary disabled during adoption:
+  "S607", # Starting a process with a partial executable path
 
 ]
 target-version = "py39"
 
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
+[tool.ruff.isort]
+known-first-party = ["ansible_compat"]
+
+[tool.ruff.per-file-ignores]
+"test/**/*.py" = ["SLF001", "S101", "FBT001"]
+
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `ansible-compat-4.0.0/requirements.txt` & `ansible-compat-4.0.0a1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib pyproject.toml
+#    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib --unsafe-package=typing_extensions pyproject.toml
 #
 argparse-manpage==4.1
     # via ansible-compat (pyproject.toml)
 attrs==23.1.0
     # via jsonschema
 beautifulsoup4==4.12.1
     # via
@@ -265,16 +265,17 @@
     #   mkdocs-ansible
 tomli==2.0.1
     # via
     #   black
     #   build
     #   pyproject-hooks
     #   pytest
-typing-extensions==4.5.0
+typing-extensions==4.5.0 ; python_version < "3.10"
     # via
+    #   ansible-compat (pyproject.toml)
     #   black
     #   mkdocs-ansible
     #   mkdocstrings
 urllib3==1.26.15
     # via
     #   mkdocs-ansible
     #   requests
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat/config.py` & `ansible-compat-4.0.0a1/src/ansible_compat/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,114 +1,108 @@
 """Store configuration options as a singleton."""
 import ast
 import copy
 import os
 import re
 import subprocess
 from collections import UserDict
-from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Union
+from typing import Literal, Optional, Union
 
 from packaging.version import Version
 
 from ansible_compat.constants import ANSIBLE_MIN_VERSION
 from ansible_compat.errors import InvalidPrerequisiteError, MissingAnsibleError
 from ansible_compat.ports import cache
 
-if TYPE_CHECKING:
-    # https://github.com/PyCQA/pylint/issues/3285
-    _UserDict = UserDict[str, object]  # pylint: disable=unsubscriptable-object
-else:
-    _UserDict = UserDict
-
 
 # do not use lru_cache here, as environment can change between calls
 def ansible_collections_path() -> str:
     """Return collection path variable for current version of Ansible."""
     return "ANSIBLE_COLLECTIONS_PATH"
 
 
 def parse_ansible_version(stdout: str) -> Version:
     """Parse output of 'ansible --version'."""
     # Ansible can produce extra output before displaying version in debug mode.
 
     # ansible-core 2.11+: 'ansible [core 2.11.3]'
     match = re.search(
-        r"^ansible \[(?:core|base) (?P<version>[^\]]+)\]", stdout, re.MULTILINE
+        r"^ansible \[(?:core|base) (?P<version>[^\]]+)\]",
+        stdout,
+        re.MULTILINE,
     )
     if match:
         return Version(match.group("version"))
-    raise InvalidPrerequisiteError(
-        f"Unable to parse ansible cli version: {stdout}\nKeep in mind that only {ANSIBLE_MIN_VERSION } or newer are supported."
-    )
+    msg = f"Unable to parse ansible cli version: {stdout}\nKeep in mind that only {ANSIBLE_MIN_VERSION } or newer are supported."
+    raise InvalidPrerequisiteError(msg)
 
 
 @cache
 def ansible_version(version: str = "") -> Version:
     """Return current Version object for Ansible.
 
     If version is not mentioned, it returns current version as detected.
     When version argument is mentioned, it return converts the version string
     to Version object in order to make it usable in comparisons.
     """
     if version:
         return Version(version)
 
     proc = subprocess.run(
-        ["ansible", "--version"],
-        universal_newlines=True,
+        ["ansible", "--version"],  # noqa: S603
+        text=True,
         check=False,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     if proc.returncode != 0:
-        raise MissingAnsibleError(
-            "Unable to find a working copy of ansible executable.", proc=proc
-        )
+        raise MissingAnsibleError(proc=proc)
 
     return parse_ansible_version(proc.stdout)
 
 
-class AnsibleConfig(_UserDict):  # pylint: disable=too-many-ancestors
+class AnsibleConfig(UserDict[str, object]):  # pylint: disable=too-many-ancestors
     """Interface to query Ansible configuration.
 
     This should allow user to access everything provided by `ansible-config dump` without having to parse the data himself.
     """
 
     _aliases = {
         "COLLECTIONS_PATH": "COLLECTIONS_PATHS",  # 2.9 -> 2.10
     }
     # Expose some attributes to enable auto-complete in editors, based on
     # https://docs.ansible.com/ansible/latest/reference_appendices/config.html
     action_warnings: bool = True
     agnostic_become_prompt: bool = True
     allow_world_readable_tmpfiles: bool = False
     ansible_connection_path: Optional[str] = None
-    ansible_cow_acceptlist: List[str]
+    ansible_cow_acceptlist: list[str]
     ansible_cow_path: Optional[str] = None
     ansible_cow_selection: str = "default"
     ansible_force_color: bool = False
     ansible_nocolor: bool = False
     ansible_nocows: bool = False
     ansible_pipelining: bool = False
     any_errors_fatal: bool = False
     become_allow_same_user: bool = False
-    become_plugin_path: List[str] = [
+    become_plugin_path: list[str] = [
         "~/.ansible/plugins/become",
         "/usr/share/ansible/plugins/become",
     ]
     cache_plugin: str = "memory"
     cache_plugin_connection: Optional[str] = None
     cache_plugin_prefix: str = "ansible_facts"
     cache_plugin_timeout: int = 86400
-    callable_accept_list: List[str] = []
-    callbacks_enabled: List[str] = []
+    callable_accept_list: list[str] = []
+    callbacks_enabled: list[str] = []
     collections_on_ansible_version_mismatch: Union[
-        Literal["warning"], Literal["warning"], Literal["ignore"]
+        Literal["warning"],
+        Literal["warning"],
+        Literal["ignore"],
     ] = "warning"
-    collections_paths: List[str] = [
+    collections_paths: list[str] = [
         "~/.ansible/collections",
         "/usr/share/ansible/collections",
     ]
     collections_scan_sys_path: bool = True
     color_changed: str = "yellow"
     color_console_prompt: str = "white"
     color_debug: str = "dark gray"
@@ -121,209 +115,215 @@
     color_ok: str = "green"
     color_skip: str = "cyan"
     color_unreachable: str = "bright red"
     color_verbose: str = "blue"
     color_warn: str = "bright purple"
     command_warnings: bool = False
     conditional_bare_vars: bool = False
-    connection_facts_modules: Dict[str, str]
+    connection_facts_modules: dict[str, str]
     controller_python_warning: bool = True
     coverage_remote_output: Optional[str]
-    coverage_remote_paths: List[str]
-    default_action_plugin_path: List[str] = [
+    coverage_remote_paths: list[str]
+    default_action_plugin_path: list[str] = [
         "~/.ansible/plugins/action",
         "/usr/share/ansible/plugins/action",
     ]
     default_allow_unsafe_lookups: bool = False
     default_ask_pass: bool = False
     default_ask_vault_pass: bool = False
     default_become: bool = False
     default_become_ask_pass: bool = False
     default_become_exe: Optional[str] = None
     default_become_flags: str
     default_become_method: str = "sudo"
     default_become_user: str = "root"
-    default_cache_plugin_path: List[str] = [
+    default_cache_plugin_path: list[str] = [
         "~/.ansible/plugins/cache",
         "/usr/share/ansible/plugins/cache",
     ]
-    default_callback_plugin_path: List[str] = [
+    default_callback_plugin_path: list[str] = [
         "~/.ansible/plugins/callback",
         "/usr/share/ansible/plugins/callback",
     ]
-    default_cliconf_plugin_path: List[str] = [
+    default_cliconf_plugin_path: list[str] = [
         "~/.ansible/plugins/cliconf",
         "/usr/share/ansible/plugins/cliconf",
     ]
-    default_connection_plugin_path: List[str] = [
+    default_connection_plugin_path: list[str] = [
         "~/.ansible/plugins/connection",
         "/usr/share/ansible/plugins/connection",
     ]
     default_debug: bool = False
     default_executable: str = "/bin/sh"
     default_fact_path: Optional[str] = None
-    default_filter_plugin_path: List[str] = [
+    default_filter_plugin_path: list[str] = [
         "~/.ansible/plugins/filter",
         "/usr/share/ansible/plugins/filter",
     ]
     default_force_handlers: bool = False
     default_forks: int = 5
     default_gathering: Union[
-        Literal["smart"], Literal["explicit"], Literal["implicit"]
+        Literal["smart"],
+        Literal["explicit"],
+        Literal["implicit"],
     ] = "smart"
-    default_gather_subset: List[str] = ["all"]
+    default_gather_subset: list[str] = ["all"]
     default_gather_timeout: int = 10
     default_handler_includes_static: bool = False
     default_hash_behaviour: str = "replace"
-    default_host_list: List[str] = ["/etc/ansible/hosts"]
-    default_httpapi_plugin_path: List[str] = [
+    default_host_list: list[str] = ["/etc/ansible/hosts"]
+    default_httpapi_plugin_path: list[str] = [
         "~/.ansible/plugins/httpapi",
         "/usr/share/ansible/plugins/httpapi",
     ]
     default_internal_poll_interval: float = 0.001
-    default_inventory_plugin_path: List[str] = [
+    default_inventory_plugin_path: list[str] = [
         "~/.ansible/plugins/inventory",
         "/usr/share/ansible/plugins/inventory",
     ]
-    default_jinja2_extensions: List[str] = []
+    default_jinja2_extensions: list[str] = []
     default_jinja2_native: bool = False
     default_keep_remote_files: bool = False
     default_libvirt_lxc_noseclabel: bool = False
     default_load_callback_plugins: bool = False
     default_local_tmp: str = "~/.ansible/tmp"
-    default_log_filter: List[str] = []
+    default_log_filter: list[str] = []
     default_log_path: Optional[str] = None
-    default_lookup_lugin_path: List[str] = [
+    default_lookup_lugin_path: list[str] = [
         "~/.ansible/plugins/lookup",
         "/usr/share/ansible/plugins/lookup",
     ]
     default_managed_str: str = "Ansible managed"
     default_module_args: str
     default_module_compression: str = "ZIP_DEFLATED"
     default_module_name: str = "command"
-    default_module_path: List[str] = [
+    default_module_path: list[str] = [
         "~/.ansible/plugins/modules",
         "/usr/share/ansible/plugins/modules",
     ]
-    default_module_utils_path: List[str] = [
+    default_module_utils_path: list[str] = [
         "~/.ansible/plugins/module_utils",
         "/usr/share/ansible/plugins/module_utils",
     ]
-    default_netconf_plugin_path: List[str] = [
+    default_netconf_plugin_path: list[str] = [
         "~/.ansible/plugins/netconf",
         "/usr/share/ansible/plugins/netconf",
     ]
     default_no_log: bool = False
     default_no_target_syslog: bool = False
     default_null_representation: Optional[str] = None
     default_poll_interval: int = 15
     default_private_key_file: Optional[str] = None
     default_private_role_vars: bool = False
     default_remote_port: Optional[str] = None
     default_remote_user: Optional[str] = None
-    default_roles_path: List[str] = [
+    default_roles_path: list[str] = [
         "~/.ansible/roles",
         "/usr/share/ansible/roles",
         "/etc/ansible/roles",
     ]
-    default_selinux_special_fs: List[str] = [
+    default_selinux_special_fs: list[str] = [
         "fuse",
         "nfs",
         "vboxsf",
         "ramfs",
         "9p",
         "vfat",
     ]
     default_stdout_callback: str = "default"
     default_strategy: str = "linear"
-    default_strategy_plugin_path: List[str] = [
+    default_strategy_plugin_path: list[str] = [
         "~/.ansible/plugins/strategy",
         "/usr/share/ansible/plugins/strategy",
     ]
     default_su: bool = False
     default_syslog_facility: str = "LOG_USER"
     default_task_includes_static: bool = False
-    default_terminal_plugin_path: List[str] = [
+    default_terminal_plugin_path: list[str] = [
         "~/.ansible/plugins/terminal",
         "/usr/share/ansible/plugins/terminal",
     ]
-    default_test_plugin_path: List[str] = [
+    default_test_plugin_path: list[str] = [
         "~/.ansible/plugins/test",
         "/usr/share/ansible/plugins/test",
     ]
     default_timeout: int = 10
     default_transport: str = "smart"
     default_undefined_var_behavior: bool = True
-    default_vars_plugin_path: List[str] = [
+    default_vars_plugin_path: list[str] = [
         "~/.ansible/plugins/vars",
         "/usr/share/ansible/plugins/vars",
     ]
     default_vault_encrypt_identity: Optional[str] = None
     default_vault_identity: str = "default"
-    default_vault_identity_list: List[str] = []
+    default_vault_identity_list: list[str] = []
     default_vault_id_match: bool = False
     default_vault_password_file: Optional[str] = None
     default_verbosity: int = 0
     deprecation_warnings: bool = False
     devel_warning: bool = True
     diff_always: bool = False
     diff_context: int = 3
     display_args_to_stdout: bool = False
     display_skipped_hosts: bool = True
     docsite_root_url: str = "https://docs.ansible.com/ansible/"
-    doc_fragment_plugin_path: List[str] = [
+    doc_fragment_plugin_path: list[str] = [
         "~/.ansible/plugins/doc_fragments",
         "/usr/share/ansible/plugins/doc_fragments",
     ]
     duplicate_yaml_dict_key: Union[
-        Literal["warn"], Literal["error"], Literal["ignore"]
+        Literal["warn"],
+        Literal["error"],
+        Literal["ignore"],
     ] = "warn"
     enable_task_debugger: bool = False
     error_on_missing_handler: bool = True
-    facts_modules: List[str] = ["smart"]
+    facts_modules: list[str] = ["smart"]
     galaxy_cache_dir: str = "~/.ansible/galaxy_cache"
     galaxy_display_progress: Optional[str] = None
     galaxy_ignore_certs: bool = False
     galaxy_role_skeleton: Optional[str] = None
-    galaxy_role_skeleton_ignore: List[str] = ["^.git$", "^.*/.git_keep$"]
+    galaxy_role_skeleton_ignore: list[str] = ["^.git$", "^.*/.git_keep$"]
     galaxy_server: str = "https://galaxy.ansible.com"
     galaxy_server_list: Optional[str] = None
     galaxy_token_path: str = "~/.ansible/galaxy_token"
     host_key_checking: bool = True
     host_pattern_mismatch: Union[
-        Literal["warning"], Literal["error"], Literal["ignore"]
+        Literal["warning"],
+        Literal["error"],
+        Literal["ignore"],
     ] = "warning"
     inject_facts_as_vars: bool = True
     interpreter_python: str = "auto_legacy"
-    interpreter_python_distro_map: Dict[str, str]
-    interpreter_python_fallback: List[str]
+    interpreter_python_distro_map: dict[str, str]
+    interpreter_python_fallback: list[str]
     invalid_task_attribute_failed: bool = True
     inventory_any_unparsed_is_failed: bool = False
     inventory_cache_enabled: bool = False
     inventory_cache_plugin: Optional[str] = None
     inventory_cache_plugin_connection: Optional[str] = None
     inventory_cache_plugin_prefix: str = "ansible_facts"
     inventory_cache_timeout: int = 3600
-    inventory_enabled: List[str] = [
+    inventory_enabled: list[str] = [
         "host_list",
         "script",
         "auto",
         "yaml",
         "ini",
         "toml",
     ]
     inventory_export: bool = False
     inventory_ignore_exts: str
-    inventory_ignore_patterns: List[str] = []
+    inventory_ignore_patterns: list[str] = []
     inventory_unparsed_is_failed: bool = False
     localhost_warning: bool = True
     max_file_size_for_diff: int = 104448
     module_ignore_exts: str
     netconf_ssh_config: Optional[str] = None
-    network_group_modules: List[str] = [
+    network_group_modules: list[str] = [
         "eos",
         "nxos",
         "ios",
         "iosxr",
         "junos",
         "enos",
         "ce",
@@ -355,71 +355,80 @@
     plugin_filters_cfg: Optional[str] = None
     python_module_rlimit_nofile: int = 0
     retry_files_enabled: bool = False
     retry_files_save_path: Optional[str] = None
     run_vars_plugins: str = "demand"
     show_custom_stats: bool = False
     string_conversion_action: Union[
-        Literal["warn"], Literal["error"], Literal["ignore"]
+        Literal["warn"],
+        Literal["error"],
+        Literal["ignore"],
     ] = "warn"
-    string_type_filters: List[str] = [
+    string_type_filters: list[str] = [
         "string",
         "to_json",
         "to_nice_json",
         "to_yaml",
         "to_nice_yaml",
         "ppretty",
         "json",
     ]
     system_warnings: bool = True
-    tags_run: List[str] = []
-    tags_skip: List[str] = []
+    tags_run: list[str] = []
+    tags_skip: list[str] = []
     task_debugger_ignore_errors: bool = True
     task_timeout: int = 0
     transform_invalid_group_chars: Union[
-        Literal["always"], Literal["never"], Literal["ignore"], Literal["silently"]
+        Literal["always"],
+        Literal["never"],
+        Literal["ignore"],
+        Literal["silently"],
     ] = "never"
     use_persistent_connections: bool = False
-    variable_plugins_enabled: List[str] = ["host_group_vars"]
-    variable_precedence: List[str] = [
+    variable_plugins_enabled: list[str] = ["host_group_vars"]
+    variable_precedence: list[str] = [
         "all_inventory",
         "groups_inventory",
         "all_plugins_inventory",
         "all_plugins_play",
         "groups_plugins_inventory",
         "groups_plugins_play",
     ]
     verbose_to_stderr: bool = False
     win_async_startup_timeout: int = 5
     worker_shutdown_poll_count: int = 0
     worker_shutdown_poll_delay: float = 0.1
-    yaml_filename_extensions: List[str] = [".yml", ".yaml", ".json"]
+    yaml_filename_extensions: list[str] = [".yml", ".yaml", ".json"]
 
     def __init__(
         self,
         config_dump: Optional[str] = None,
-        data: Optional[Dict[str, object]] = None,
+        data: Optional[dict[str, object]] = None,
     ) -> None:
         """Load config dictionary."""
         super().__init__()
 
         if data:
             self.data = copy.deepcopy(data)
             return
 
         if not config_dump:
             env = os.environ.copy()
             # Avoid possible ANSI garbage
             env["ANSIBLE_FORCE_COLOR"] = "0"
             config_dump = subprocess.check_output(
-                ["ansible-config", "dump"], universal_newlines=True, env=env
+                ["ansible-config", "dump"],  # noqa: S603
+                universal_newlines=True,
+                env=env,
             )
 
         for match in re.finditer(
-            r"^(?P<key>[A-Za-z0-9_]+).* = (?P<value>.*)$", config_dump, re.MULTILINE
+            r"^(?P<key>[A-Za-z0-9_]+).* = (?P<value>.*)$",
+            config_dump,
+            re.MULTILINE,
         ):
             key = match.groupdict()["key"]
             value = match.groupdict()["value"]
             try:
                 self[key] = ast.literal_eval(value)
             except (NameError, SyntaxError, ValueError):
                 self[key] = value
@@ -450,21 +459,14 @@
         """Allow users to run copy on Config."""
         return AnsibleConfig(data=self.data)
 
     def __deepcopy__(self, memo: object) -> "AnsibleConfig":
         """Allow users to run deeepcopy on Config."""
         return AnsibleConfig(data=self.data)
 
-    def _dump_config_attrs(self) -> None:  # pragma: no cover
-        """Dump config attributes using pytest typed format."""
-        for item in sorted(self.data):
-            name = item.lower()
-            kind = self.data[item].__class__.__name__
-            print(f"{name}: {kind}")
-
 
 __all__ = [
     "ansible_collections_path",
     "parse_ansible_version",
     "ansible_version",
     "AnsibleConfig",
 ]
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat/constants.py` & `ansible-compat-4.0.0a1/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/src/ansible_compat/errors.py` & `ansible-compat-4.0.0a1/src/ansible_compat/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 class AnsibleCompatError(RuntimeError):
     """Generic error originating from ansible_compat library."""
 
     code = 1  # generic error
 
     def __init__(
-        self, message: Optional[str] = None, proc: Optional[Any] = None
+        self,
+        message: Optional[str] = None,
+        proc: Optional[Any] = None,
     ) -> None:
         """Construct generic library exception."""
         super().__init__(message)
         self.proc = proc
 
 
 class AnsibleCommandError(RuntimeError):
@@ -34,15 +36,17 @@
 
 class MissingAnsibleError(AnsibleCompatError):
     """Reports a missing or broken Ansible installation."""
 
     code = ANSIBLE_MISSING_RC
 
     def __init__(
-        self, message: Optional[str] = None, proc: Optional[Any] = None
+        self,
+        message: Optional[str] = "Unable to find a working copy of ansible executable.",
+        proc: Optional[Any] = None,
     ) -> None:
         """."""
         super().__init__(message)
         self.proc = proc
 
 
 class InvalidPrerequisiteError(AnsibleCompatError):
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat/loaders.py` & `ansible-compat-4.0.0a1/src/ansible_compat/loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Utilities for loading various files."""
 from __future__ import annotations
 
-import os
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import yaml
 
 from ansible_compat.errors import InvalidPrerequisiteError
 
+if TYPE_CHECKING:
+    from pathlib import Path
 
-def yaml_from_file(filepath: str) -> Any:
+
+def yaml_from_file(path: Path) -> Any:  # noqa: ANN401
     """Return a loaded YAML file."""
-    with open(filepath, encoding="utf-8") as content:
-        return yaml.load(content, Loader=yaml.FullLoader)
+    with path.open(encoding="utf-8") as content:
+        return yaml.load(content, Loader=yaml.SafeLoader)
 
 
-def colpath_from_path(filepath: str) -> str | None:
+def colpath_from_path(path: Path) -> str | None:
     """Return a FQCN from a path."""
-    galaxy_file = f"{filepath}/galaxy.yml"
-    if os.path.exists(galaxy_file):
+    galaxy_file = path / "galaxy.yml"
+    if galaxy_file.exists():
         galaxy = yaml_from_file(galaxy_file)
         for k in ("namespace", "name"):
             if k not in galaxy:
-                raise InvalidPrerequisiteError(
-                    f"{galaxy_file} is missing the following mandatory field {k}"
-                )
+                msg = f"{galaxy_file} is missing the following mandatory field {k}"
+                raise InvalidPrerequisiteError(msg)
         return f"{galaxy['namespace']}/{galaxy['name']}"
     return None
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat/prerun.py` & `ansible-compat-4.0.0a1/src/ansible_compat/prerun.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Utilities for configuring ansible runtime environment."""
 import hashlib
 import os
 from pathlib import Path
 
 
-def get_cache_dir(project_dir: str) -> Path:
+def get_cache_dir(project_dir: Path) -> Path:
     """Compute cache directory to be used based on project path."""
     # we only use the basename instead of the full path in order to ensure that
     # we would use the same key regardless the location of the user home
     # directory or where the project is clones (as long the project folder uses
     # the same name).
-    basename = os.path.basename(os.path.abspath(project_dir)).encode(encoding="utf-8")
+    basename = project_dir.resolve().name.encode(encoding="utf-8")
     # 6 chars of entropy should be enough
     cache_key = hashlib.sha256(basename).hexdigest()[:6]
     cache_dir = (
-        os.getenv("XDG_CACHE_HOME", os.path.expanduser("~/.cache"))
-        + "/ansible-compat/"
-        + cache_key
+        Path(os.getenv("XDG_CACHE_HOME", "~/.cache")).expanduser()
+        / "ansible-compat"
+        / cache_key
     )
-    return Path(cache_dir)
+    return cache_dir
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat/runtime.py` & `ansible-compat-4.0.0a1/src/ansible_compat/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Ansible runtime environment manager."""
 import contextlib
 import importlib
 import json
 import logging
 import os
-import pathlib
 import re
 import shutil
 import subprocess
 import tempfile
 import warnings
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import packaging
 import subprocess_tee
 from packaging.version import Version
 
 from ansible_compat.config import (
@@ -47,23 +47,24 @@
     """Warnings related to Ansible runtime."""
 
 
 class Runtime:
     """Ansible Runtime manager."""
 
     _version: Optional[packaging.version.Version] = None
-    cache_dir: Optional[pathlib.Path] = None
+    cache_dir: Optional[Path] = None
     # Used to track if we have already initialized the Ansible runtime as attempts
     # to do it multiple tilmes will cause runtime warnings from within ansible-core
     initialized: bool = False
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
-        project_dir: Optional[str] = None,
+        project_dir: Optional[Path] = None,
+        *,
         isolated: bool = False,
         min_required_version: Optional[str] = None,
         require_module: bool = False,
         max_retries: int = 0,
         environ: Optional[dict[str, str]] = None,
     ) -> None:
         """Initialize Ansible runtime environment.
@@ -83,15 +84,15 @@
                                That is useful for consumers that expect to
                                also perform Python imports from Ansible.
         :param max_retries: Number of times it should retry network operations.
                             Default is 0, no retries.
         :param environ: Environment dictionary to use, if undefined
                         ``os.environ`` will be copied and used.
         """
-        self.project_dir = project_dir or os.getcwd()
+        self.project_dir = project_dir or Path.cwd()
         self.isolated = isolated
         self.max_retries = max_retries
         self.environ = environ or os.environ.copy()
         # Reduce noise from paramiko, unless user already defined PYTHONWARNINGS
         # paramiko/transport.py:236: CryptographyDeprecationWarning: Blowfish has been deprecated
         # https://github.com/paramiko/paramiko/issues/2038
         # As CryptographyDeprecationWarning is not a builtin, we cannot use
@@ -101,49 +102,51 @@
             self.environ["PYTHONWARNINGS"] = "ignore:Blowfish has been deprecated"
 
         if isolated:
             self.cache_dir = get_cache_dir(self.project_dir)
         self.config = AnsibleConfig()
 
         if not self.version_in_range(lower=min_required_version):
-            raise RuntimeError(
-                f"Found incompatible version of ansible runtime {self.version}, instead of {min_required_version} or newer.",
-            )
+            msg = f"Found incompatible version of ansible runtime {self.version}, instead of {min_required_version} or newer."
+            raise RuntimeError(msg)
         if require_module:
             self._ensure_module_available()
 
         # pylint: disable=import-outside-toplevel
         from ansible.utils.display import Display
 
         # pylint: disable=unused-argument
-        def warning(self: Display, msg: str, formatted: bool = False) -> None:
+        def warning(
+            self: Display,  # noqa: ARG001
+            msg: str,
+            *,
+            formatted: bool = False,  # noqa: ARG001
+        ) -> None:
             """Override ansible.utils.display.Display.warning to avoid printing warnings."""
             warnings.warn(msg, category=AnsibleWarning, stacklevel=2)
 
         # Monkey patch ansible warning in order to use warnings module.
         Display.warning = warning
 
     def _ensure_module_available(self) -> None:
         """Assure that Ansible Python module is installed and matching CLI version."""
         ansible_release_module = None
         with contextlib.suppress(ModuleNotFoundError, ImportError):
             ansible_release_module = importlib.import_module("ansible.release")
 
         if ansible_release_module is None:
-            raise RuntimeError("Unable to find Ansible python module.")
+            msg = "Unable to find Ansible python module."
+            raise RuntimeError(msg)
 
         ansible_module_version = packaging.version.parse(
             ansible_release_module.__version__,
         )
         if ansible_module_version != self.version:
-            raise RuntimeError(
-                f"Ansible CLI ({self.version}) and python module"
-                f" ({ansible_module_version}) versions do not match. This "
-                "indicates a broken execution environment.",
-            )
+            msg = f"Ansible CLI ({self.version}) and python module ({ansible_module_version}) versions do not match. This indicates a broken execution environment."
+            raise RuntimeError(msg)
 
         # For ansible 2.15+ we need to initialize the plugin loader
         # https://github.com/ansible/ansible-lint/issues/2945
         if not Runtime.initialized:
             col_path = [f"{self.cache_dir}/collections"]
             if self.version >= Version("2.15.0.dev0"):
                 # pylint: disable=import-outside-toplevel,no-name-in-module
@@ -155,34 +158,35 @@
                 from ansible.utils.collection_loader._collection_finder import (  # pylint: disable=import-outside-toplevel
                     _AnsibleCollectionFinder,
                 )
 
                 # noinspection PyProtectedMember
                 # pylint: disable=protected-access
                 col_path += self.config.collections_paths
-                col_path += os.path.dirname(
+                col_path += os.path.dirname(  # noqa: PTH120
                     os.environ.get(ansible_collections_path(), "."),
                 ).split(":")
-                _AnsibleCollectionFinder(
+                _AnsibleCollectionFinder(  # noqa: SLF001
                     paths=col_path,
                 )._install()  # pylint: disable=protected-access
             Runtime.initialized = True
 
     def clean(self) -> None:
         """Remove content of cache_dir."""
         if self.cache_dir:
             shutil.rmtree(self.cache_dir, ignore_errors=True)
 
-    def exec(
+    def run(
         self,
         args: Union[str, list[str]],
+        *,
         retry: bool = False,
         tee: bool = False,
         env: Optional[dict[str, str]] = None,
-        cwd: Optional[str] = None,
+        cwd: Optional[Path] = None,
     ) -> CompletedProcess:
         """Execute a command inside an Ansible environment.
 
         :param retry: Retry network operations on failures.
         :param tee: Also pass captured stdout/stderr to system while running.
         """
         if tee:
@@ -194,15 +198,15 @@
             result = run_func(
                 args,
                 universal_newlines=True,
                 check=False,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 env=env or self.environ,
-                cwd=cwd,
+                cwd=str(cwd) if cwd else None,
             )
             if result.returncode == 0:
                 break
             _logger.debug("Environment: %s", env or self.environ)
             _logger.warning(
                 "Retrying execution failure %s of: %s",
                 result.returncode,
@@ -217,15 +221,15 @@
         If version is not mentioned, it returns current version as detected.
         When version argument is mentioned, it return converts the version string
         to Version object in order to make it usable in comparisons.
         """
         if self._version:
             return self._version
 
-        proc = self.exec(["ansible", "--version"])
+        proc = self.run(["ansible", "--version"])
         if proc.returncode == 0:
             self._version = parse_ansible_version(proc.stdout)
             return self._version
 
         msg = "Unable to find a working copy of ansible executable."
         raise MissingAnsibleError(msg, proc=proc)
 
@@ -242,16 +246,17 @@
             return False
         if upper and self.version >= packaging.version.Version(upper):
             return False
         return True
 
     def install_collection(
         self,
-        collection: str,
-        destination: Optional[Union[str, pathlib.Path]] = None,
+        collection: Union[str, Path],
+        *,
+        destination: Optional[Path] = None,
         force: bool = False,
     ) -> None:
         """Install an Ansible collection.
 
         Can accept version constraints like 'foo.bar:>=1.2.3'
         """
         cmd = [
@@ -262,88 +267,88 @@
         ]
         if force:
             cmd.append("--force")
 
         # As ansible-galaxy install is not able to automatically determine
         # if the range requires a pre-release, we need to manuall add the --pre
         # flag when needed.
-        matches = version_re.search(collection)
+        matches = version_re.search(str(collection))
         if matches and Version(matches[1]).is_prerelease:
             cmd.append("--pre")
 
         cpaths: list[str] = self.config.collections_paths
         if destination and str(destination) not in cpaths:
             # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
             # we hack ansible_collections_path instead and inject our own path there.
             # pylint: disable=no-member
             cpaths.insert(0, str(destination))
         cmd.append(f"{collection}")
 
-        _logger.info("Running from %s : %s", os.getcwd(), " ".join(cmd))
-        run = self.exec(
+        _logger.info("Running from %s : %s", Path.cwd(), " ".join(cmd))
+        run = self.run(
             cmd,
             retry=True,
             env={**self.environ, ansible_collections_path(): ":".join(cpaths)},
         )
         if run.returncode != 0:
             msg = f"Command returned {run.returncode} code:\n{run.stdout}\n{run.stderr}"
             _logger.error(msg)
             raise InvalidPrerequisiteError(msg)
 
     def install_collection_from_disk(
         self,
-        path: str,
-        destination: Optional[Union[str, pathlib.Path]] = None,
+        path: Path,
+        destination: Optional[Path] = None,
     ) -> None:
         """Build and install collection from a given disk path."""
         if not self.version_in_range(upper="2.11"):
             self.install_collection(path, destination=destination, force=True)
             return
         # older versions of ansible able unable to install without building
         with tempfile.TemporaryDirectory() as tmp_dir:
             cmd = [
                 "ansible-galaxy",
                 "collection",
                 "build",
                 "--output-path",
-                tmp_dir,
-                path,
+                str(tmp_dir),
+                str(path),
             ]
             _logger.info("Running %s", " ".join(cmd))
-            run = self.exec(cmd, retry=False)
+            run = self.run(cmd, retry=False)
             if run.returncode != 0:
                 _logger.error(run.stdout)
                 raise AnsibleCommandError(run)
             for archive_file in os.listdir(tmp_dir):
                 self.install_collection(
-                    os.path.join(tmp_dir, archive_file),
+                    str(Path(tmp_dir) / archive_file),
                     destination=destination,
                     force=True,
                 )
 
     # pylint: disable=too-many-branches
-    def install_requirements(
+    def install_requirements(  # noqa: C901,PLR0912
         self,
-        requirement: str,
+        requirement: Path,
+        *,
         retry: bool = False,
         offline: bool = False,
     ) -> None:
         """Install dependencies from a requirements.yml.
 
         :param requirement: path to requirements.yml file
         :param retry: retry network operations on failures
         :param offline: bypass installation, may fail if requirements are not met.
         """
-        if not os.path.exists(requirement):
+        if not Path(requirement).exists():
             return
-        reqs_yaml = yaml_from_file(requirement)
+        reqs_yaml = yaml_from_file(Path(requirement))
         if not isinstance(reqs_yaml, (dict, list)):
-            raise InvalidPrerequisiteError(
-                f"{requirement} file is not a valid Ansible requirements file.",
-            )
+            msg = f"{requirement} file is not a valid Ansible requirements file."
+            raise InvalidPrerequisiteError(msg)
 
         if isinstance(reqs_yaml, list) or "roles" in reqs_yaml:
             cmd = [
                 "ansible-galaxy",
                 "role",
                 "install",
                 "-vr",
@@ -355,15 +360,15 @@
             if offline:
                 _logger.warning(
                     "Skipped installing old role dependencies due to running in offline mode.",
                 )
             else:
                 _logger.info("Running %s", " ".join(cmd))
 
-                result = self.exec(cmd, retry=retry)
+                result = self.run(cmd, retry=retry)
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     raise AnsibleCommandError(result)
 
         # Run galaxy collection install works on v2 requirements.yml
         if "collections" in reqs_yaml:
             cmd = [
@@ -373,143 +378,150 @@
                 "-v",
             ]
             if offline:
                 _logger.warning(
                     "Skipped installing collection dependencies due to running in offline mode.",
                 )
             else:
-                cmd.extend(["-r", requirement])
+                cmd.extend(["-r", str(requirement)])
                 cpaths = self.config.collections_paths
                 if self.cache_dir:
                     # we cannot use '-p' because it breaks galaxy ability to ignore already installed collections, so
                     # we hack ansible_collections_path instead and inject our own path there.
                     dest_path = f"{self.cache_dir}/collections"
                     if dest_path not in cpaths:
                         # pylint: disable=no-member
                         cpaths.insert(0, dest_path)
                 _logger.info("Running %s", " ".join(cmd))
-                result = self.exec(
+                result = self.run(
                     cmd,
                     retry=retry,
                     env={**os.environ, "ANSIBLE_COLLECTIONS_PATH": ":".join(cpaths)},
                 )
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     _logger.error(result.stderr)
                     raise AnsibleCommandError(result)
 
-    def prepare_environment(
+    def prepare_environment(  # noqa: C901
         self,
         required_collections: Optional[dict[str, str]] = None,
+        *,
         retry: bool = False,
         install_local: bool = False,
         offline: bool = False,
         role_name_check: int = 0,
     ) -> None:
         """Make dependencies available if needed."""
+        destination: Optional[Path] = None
         if required_collections is None:
             required_collections = {}
 
         # first one is standard for collection layout repos and the last two
         # are part of Tower specification
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#ansible-galaxy-support
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#collections-support
         for req_file in [
             "requirements.yml",
             "roles/requirements.yml",
             "collections/requirements.yml",
         ]:
-            self.install_requirements(req_file, retry=retry, offline=offline)
+            self.install_requirements(Path(req_file), retry=retry, offline=offline)
 
-        destination = f"{self.cache_dir}/collections" if self.cache_dir else None
+        if self.cache_dir:
+            destination = self.cache_dir / "collections"
         for name, min_version in required_collections.items():
             self.install_collection(
                 f"{name}:>={min_version}",
                 destination=destination,
             )
 
         self._prepare_ansible_paths()
 
         if not install_local:
             return
 
-        if os.path.exists("galaxy.yml"):
+        if Path("galaxy.yml").exists():
             if destination:
                 # while function can return None, that would not break the logic
-                colpath = f"{destination}/ansible_collections/{colpath_from_path(os.getcwd())}"
-                if os.path.islink(colpath):
-                    if os.path.realpath(colpath) == os.getcwd():
+                colpath = Path(
+                    f"{destination}/ansible_collections/{colpath_from_path(Path.cwd())}",
+                )
+                if colpath.is_symlink():
+                    if os.path.realpath(colpath) == Path.cwd():
                         _logger.warning(
                             "Found symlinked collection, skipping its installation.",
                         )
                         return
                     _logger.warning(
                         "Collection is symlinked, but not pointing to %s directory, so we will remove it.",
-                        os.getcwd(),
+                        Path.cwd(),
                     )
-                    os.unlink(colpath)
+                    colpath.unlink()
 
             # molecule scenario within a collection
-            self.install_collection_from_disk(".", destination=destination)
-        elif pathlib.Path().resolve().parent.name == "roles" and os.path.exists(
-            "../../galaxy.yml",
+            self.install_collection_from_disk(Path("."), destination=destination)
+        elif (
+            Path().resolve().parent.name == "roles"
+            and Path("../../galaxy.yml").exists()
         ):
             # molecule scenario located within roles/<role-name>/molecule inside
             # a collection
-            self.install_collection_from_disk("../..", destination=destination)
+            self.install_collection_from_disk(Path("../.."), destination=destination)
         else:
             # no collection, try to recognize and install a standalone role
             self._install_galaxy_role(
                 self.project_dir,
                 role_name_check=role_name_check,
                 ignore_errors=True,
             )
 
     def require_collection(
         self,
         name: str,
         version: Optional[str] = None,
+        *,
         install: bool = True,
     ) -> None:
         """Check if a minimal collection version is present or exits.
 
         In the future this method may attempt to install a missing or outdated
         collection before failing.
         """
         try:
             ns, coll = name.split(".", 1)
         except ValueError as exc:
+            msg = f"Invalid collection name supplied: {name}%s"
             raise InvalidPrerequisiteError(
-                f"Invalid collection name supplied: {name}%s",
+                msg,
             ) from exc
 
         paths: list[str] = self.config.collections_paths
         if not paths or not isinstance(paths, list):
+            msg = f"Unable to determine ansible collection paths. ({paths})"
             raise InvalidPrerequisiteError(
-                f"Unable to determine ansible collection paths. ({paths})",
+                msg,
             )
 
         if self.cache_dir:
             # if we have a cache dir, we want to be use that would be preferred
             # destination when installing a missing collection
             # https://github.com/PyCQA/pylint/issues/4667
             paths.insert(0, f"{self.cache_dir}/collections")  # pylint: disable=E1101
 
         for path in paths:
-            collpath = os.path.expanduser(
-                os.path.join(path, "ansible_collections", ns, coll),
-            )
-            if os.path.exists(collpath):
-                mpath = os.path.join(collpath, "MANIFEST.json")
-                if not os.path.exists(mpath):
+            collpath = Path(path) / "ansible_collections" / ns / coll
+            if collpath.exists():
+                mpath = collpath / "MANIFEST.json"
+                if not mpath.exists():
                     msg = f"Found collection at '{collpath}' but missing MANIFEST.json, cannot get info."
                     _logger.fatal(msg)
                     raise InvalidPrerequisiteError(msg)
 
-                with open(mpath, encoding="utf-8") as f:
+                with mpath.open(encoding="utf-8") as f:
                     manifest = json.loads(f.read())
                     found_version = packaging.version.parse(
                         manifest["collection_info"]["version"],
                     )
                     if version and found_version < packaging.version.parse(version):
                         if install:
                             self.install_collection(f"{name}:>={version}")
@@ -531,15 +543,16 @@
     def _prepare_ansible_paths(self) -> None:
         """Configure Ansible environment variables."""
         try:
             library_paths: list[str] = self.config.default_module_path.copy()
             roles_path: list[str] = self.config.default_roles_path.copy()
             collections_path: list[str] = self.config.collections_paths.copy()
         except AttributeError as exc:
-            raise RuntimeError("Unexpected ansible configuration") from exc
+            msg = "Unexpected ansible configuration"
+            raise RuntimeError(msg) from exc
 
         alterations_list = [
             (library_paths, "plugins/modules", True),
             (roles_path, "roles", True),
         ]
 
         alterations_list.extend(
@@ -548,47 +561,49 @@
                 (library_paths, f"{self.cache_dir}/modules", False),
                 (collections_path, f"{self.cache_dir}/collections", False),
             ]
             if self.isolated
             else [],
         )
 
-        for path_list, path, must_be_present in alterations_list:
-            if not os.path.exists(path):
+        for path_list, path_, must_be_present in alterations_list:
+            path = Path(path_)
+            if not path.exists():
                 if must_be_present:
                     continue
-                os.makedirs(path, exist_ok=True)
+                path.mkdir(parents=True, exist_ok=True)
             if path not in path_list:
-                path_list.insert(0, path)
+                path_list.insert(0, str(path))
 
         if library_paths != self.config.DEFAULT_MODULE_PATH:
             self._update_env("ANSIBLE_LIBRARY", library_paths)
         if collections_path != self.config.collections_paths:
             self._update_env(ansible_collections_path(), collections_path)
         if roles_path != self.config.default_roles_path:
             self._update_env("ANSIBLE_ROLES_PATH", roles_path)
 
-    def _get_roles_path(self) -> pathlib.Path:
+    def _get_roles_path(self) -> Path:
         """Return roles installation path.
 
         If `self.isolated` is set to `True`, `self.cache_dir` would be
         created, then it returns the `self.cache_dir/roles`. When `self.isolated` is
         not mentioned or set to `False`, it returns the first path in
         `default_roles_path`.
         """
         if self.cache_dir:
-            path = pathlib.Path(f"{self.cache_dir}/roles")
+            path = Path(f"{self.cache_dir}/roles")
         else:
-            path = pathlib.Path(os.path.expanduser(self.config.default_roles_path[0]))
+            path = Path(self.config.default_roles_path[0]).expanduser()
         return path
 
     def _install_galaxy_role(
         self,
-        project_dir: str,
+        project_dir: Path,
         role_name_check: int = 0,
+        *,
         ignore_errors: bool = False,
     ) -> None:
         """Detect standalone galaxy role and installs it.
 
         :param: role_name_check: logic to used to check role name
             0: exit with error if name is not compliant (default)
             1: warn if name is not compliant
@@ -599,17 +614,17 @@
         Our implementation aims to match ansible-galaxy's behaviour for installing
         roles from a tarball or scm. For example ansible-galaxy will install a role
         that has both galaxy.yml and meta/main.yml present but empty. Also missing
         galaxy.yml is accepted but missing meta/main.yml is not.
         """
         yaml = None
         galaxy_info = {}
-        meta_filename = os.path.join(project_dir, "meta", "main.yml")
+        meta_filename = Path(project_dir) / "meta" / "main.yml"
 
-        if not os.path.exists(meta_filename):
+        if not meta_filename.exists():
             if ignore_errors:
                 return
         else:
             yaml = yaml_from_file(meta_filename)
 
         if yaml and "galaxy_info" in yaml:
             galaxy_info = yaml["galaxy_info"]
@@ -620,30 +635,29 @@
             if not re.match(r"[a-z0-9][a-z0-9_]+\.[a-z][a-z0-9_]+$", fqrn):
                 msg = MSG_INVALID_FQRL.format(fqrn)
                 if role_name_check == 1:
                     _logger.warning(msg)
                 else:
                     _logger.error(msg)
                     raise InvalidPrerequisiteError(msg)
-        else:
+        elif "role_name" in galaxy_info:
             # when 'role-name' is in skip_list, we stick to plain role names
-            if "role_name" in galaxy_info:
-                role_namespace = _get_galaxy_role_ns(galaxy_info)
-                role_name = _get_galaxy_role_name(galaxy_info)
-                fqrn = f"{role_namespace}{role_name}"
-            else:
-                fqrn = pathlib.Path(project_dir).absolute().name
+            role_namespace = _get_galaxy_role_ns(galaxy_info)
+            role_name = _get_galaxy_role_name(galaxy_info)
+            fqrn = f"{role_namespace}{role_name}"
+        else:
+            fqrn = Path(project_dir).absolute().name
         path = self._get_roles_path()
         path.mkdir(parents=True, exist_ok=True)
         link_path = path / fqrn
         # despite documentation stating that is_file() reports true for symlinks,
         # it appears that is_dir() reports true instead, so we rely on exists().
-        target = pathlib.Path(project_dir).absolute()
+        target = Path(project_dir).absolute()
         if not link_path.exists() or (
-            link_path.is_symlink() and os.readlink(link_path) != str(target)
+            link_path.is_symlink() and link_path.readlink() != target
         ):
             # must call unlink before checking exists because a broken
             # link reports as not existing and we want to repair it
             link_path.unlink(missing_ok=True)
             # https://github.com/python/cpython/issues/73843
             link_path.symlink_to(str(target), target_is_directory=True)
         _logger.info(
@@ -663,36 +677,37 @@
             value = [*value, *orig_value.split(":")]
         value_str = ":".join(value)
         if value_str != self.environ.get(varname, ""):
             self.environ[varname] = value_str
             _logger.info("Set %s=%s", varname, value_str)
 
 
-def _get_role_fqrn(galaxy_infos: dict[str, Any], project_dir: str) -> str:
+def _get_role_fqrn(galaxy_infos: dict[str, Any], project_dir: Path) -> str:
     """Compute role fqrn."""
     role_namespace = _get_galaxy_role_ns(galaxy_infos)
     role_name = _get_galaxy_role_name(galaxy_infos)
 
     if len(role_name) == 0:
-        role_name = pathlib.Path(project_dir).absolute().name
+        role_name = Path(project_dir).absolute().name
         role_name = re.sub(r"(ansible-|ansible-role-)", "", role_name).split(
             ".",
             maxsplit=2,
         )[-1]
 
     return f"{role_namespace}{role_name}"
 
 
 def _get_galaxy_role_ns(galaxy_infos: dict[str, Any]) -> str:
     """Compute role namespace from meta/main.yml, including trailing dot."""
     role_namespace = galaxy_infos.get("namespace", "")
     if len(role_namespace) == 0:
         role_namespace = galaxy_infos.get("author", "")
     if not isinstance(role_namespace, str):
-        raise AnsibleCompatError(f"Role namespace must be string, not {role_namespace}")
+        msg = f"Role namespace must be string, not {role_namespace}"
+        raise AnsibleCompatError(msg)
     # if there's a space in the name space, it's likely author name
     # and not the galaxy login, so act as if there was no namespace
     if not role_namespace or re.match(r"^\w+ \w+", role_namespace):
         role_namespace = ""
     else:
         role_namespace = f"{role_namespace}."
     return role_namespace
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.0a1/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.0
+Version: 4.0.0a1
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.0/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.0a1/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 .github/CODE_OF_CONDUCT.md
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/workflows/ack.yml
 .github/workflows/push.yml
 .github/workflows/release.yml
 .github/workflows/tox.yml
+.vscode/extensions.json
+.vscode/settings.json
 docs/api.md
 docs/index.md
 docs/images/favicon.ico
 docs/images/logo.png
 docs/images/logo.svg
 examples/reqs_v1/requirements.yml
 examples/reqs_v2/community-molecule-0.1.0.tar.gz
@@ -34,14 +36,15 @@
 src/ansible_compat/errors.py
 src/ansible_compat/loaders.py
 src/ansible_compat/ports.py
 src/ansible_compat/prerun.py
 src/ansible_compat/py.typed
 src/ansible_compat/runtime.py
 src/ansible_compat/schema.py
+src/ansible_compat/types.py
 src/ansible_compat.egg-info/PKG-INFO
 src/ansible_compat.egg-info/SOURCES.txt
 src/ansible_compat.egg-info/dependency_links.txt
 src/ansible_compat.egg-info/requires.txt
 src/ansible_compat.egg-info/top_level.txt
 test/__init__.py
 test/conftest.py
```

### Comparing `ansible-compat-4.0.0/test/assets/validate0_expected.json` & `ansible-compat-4.0.0a1/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.0/test/conftest.py` & `ansible-compat-4.0.0a1/test/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Pytest fixtures."""
 import pathlib
-from typing import Generator
+from collections.abc import Generator
 
 import pytest
 
 from ansible_compat.runtime import Runtime
 
 
 @pytest.fixture()
 # pylint: disable=unused-argument
-def runtime(scope: str = "session") -> Generator[Runtime, None, None]:
+def runtime(scope: str = "session") -> Generator[Runtime, None, None]:  # noqa: ARG001
     """Isolated runtime fixture."""
     instance = Runtime(isolated=True)
     yield instance
     instance.clean()
 
 
 @pytest.fixture()
 # pylint: disable=unused-argument
 def runtime_tmp(
-    tmp_path: pathlib.Path, scope: str = "session"
+    tmp_path: pathlib.Path,
+    scope: str = "session",  # noqa: ARG001
 ) -> Generator[Runtime, None, None]:
     """Isolated runtime fixture using a temp directory."""
-    instance = Runtime(project_dir=str(tmp_path), isolated=True)
+    instance = Runtime(project_dir=tmp_path, isolated=True)
     yield instance
     instance.clean()
```

### Comparing `ansible-compat-4.0.0/test/test_config.py` & `ansible-compat-4.0.0a1/test/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     # check lowercase and older name aliasing
     assert isinstance(config.collections_paths, list)
     assert isinstance(config.collections_path, list)
     assert config.collections_paths == config.collections_path
 
     # check if we can access the special data member
-    assert config.ACTION_WARNINGS == config.data["ACTION_WARNINGS"]
+    assert config.data["ACTION_WARNINGS"] == config.ACTION_WARNINGS
 
     with pytest.raises(AttributeError):
-        print(config.THIS_DOES_NOT_EXIST)
+        _ = config.THIS_DOES_NOT_EXIST
 
 
 def test_config_with_dump() -> None:
     """Tests that config can parse given dumps."""
     config = AnsibleConfig(config_dump="ACTION_WARNINGS(default) = True")
     assert config.ACTION_WARNINGS is True
 
@@ -49,24 +49,28 @@
     assert isinstance(new_config, AnsibleConfig)
     assert new_config is not config
 
 
 def test_parse_ansible_version_fail() -> None:
     """Checks that parse_ansible_version raises an error on invalid input."""
     with pytest.raises(
-        InvalidPrerequisiteError, match="Unable to parse ansible cli version"
+        InvalidPrerequisiteError,
+        match="Unable to parse ansible cli version",
     ):
         parse_ansible_version("foo")
 
 
 def test_ansible_version_missing(monkeypatch: MonkeyPatch) -> None:
     """Validate ansible_version behavior when ansible is missing."""
     monkeypatch.setattr(
         "subprocess.run",
-        lambda *args, **kwargs: subprocess.CompletedProcess(args=[], returncode=1),
+        lambda *args, **kwargs: subprocess.CompletedProcess(  # noqa: ARG005
+            args=[],
+            returncode=1,
+        ),
     )
     with pytest.raises(
         MissingAnsibleError,
         match="Unable to find a working copy of ansible executable.",
     ):
         # bypassing lru cache
         ansible_version.__wrapped__()
```

### Comparing `ansible-compat-4.0.0/test/test_runtime.py` & `ansible-compat-4.0.0a1/test/test_runtime.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Tests for Runtime class."""
 # pylint: disable=protected-access
 import logging
 import os
 import pathlib
 import subprocess
+from collections.abc import Iterator
 from contextlib import contextmanager
+from pathlib import Path
 from shutil import rmtree
-from typing import Any, Iterator, List, Type, Union
+from typing import Any, Union
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from packaging.version import Version
 from pytest_mock import MockerFixture
 
 from ansible_compat.constants import INVALID_PREREQUISITES_RC
@@ -43,16 +45,20 @@
 
 def test_runtime_missing_ansible_module(monkeypatch: MonkeyPatch) -> None:
     """Checks that we produce a RuntimeError when ansible module is missing."""
 
     class RaiseException:
         """Class to raise an exception."""
 
-        def __init__(self, *args: Any, **kwargs: Any) -> None:
-            raise ModuleNotFoundError()
+        def __init__(
+            self,
+            *args: Any,  # noqa: ARG002,ANN401
+            **kwargs: Any,  # noqa: ARG002,ANN401
+        ) -> None:
+            raise ModuleNotFoundError
 
     monkeypatch.setattr("importlib.import_module", RaiseException)
 
     with pytest.raises(RuntimeError, match="Unable to find Ansible python module."):
         Runtime(require_module=True)
 
 
@@ -82,43 +88,48 @@
 def test_runtime_version_fail_module(mocker: MockerFixture) -> None:
     """Tests for failure to detect Ansible version."""
     patched = mocker.patch(
         "ansible_compat.runtime.parse_ansible_version",
         autospec=True,
     )
     patched.side_effect = InvalidPrerequisiteError(
-        "Unable to parse ansible cli version"
+        "Unable to parse ansible cli version",
     )
     runtime = Runtime()
     with pytest.raises(
-        InvalidPrerequisiteError, match="Unable to parse ansible cli version"
+        InvalidPrerequisiteError,
+        match="Unable to parse ansible cli version",
     ):
-        runtime.version  # pylint: disable=pointless-statement
+        _ = runtime.version  # pylint: disable=pointless-statement
 
 
 def test_runtime_version_fail_cli(mocker: MockerFixture) -> None:
     """Tests for failure to detect Ansible version."""
     mocker.patch(
-        "ansible_compat.runtime.Runtime.exec",
+        "ansible_compat.runtime.Runtime.run",
         return_value=CompletedProcess(
-            ["x"], returncode=123, stdout="oops", stderr="some error"
+            ["x"],
+            returncode=123,
+            stdout="oops",
+            stderr="some error",
         ),
         autospec=True,
     )
     runtime = Runtime()
     with pytest.raises(
-        RuntimeError, match="Unable to find a working copy of ansible executable."
+        RuntimeError,
+        match="Unable to find a working copy of ansible executable.",
     ):
-        runtime.version  # pylint: disable=pointless-statement
+        _ = runtime.version  # pylint: disable=pointless-statement
 
 
 def test_runtime_prepare_ansible_paths_validation() -> None:
     """Check that we validate collection_path."""
     runtime = Runtime()
-    runtime.config.collections_paths = "invalid-value"  # type: ignore
+    runtime.config.collections_paths = "invalid-value"  # type: ignore[assignment]
     with pytest.raises(RuntimeError, match="Unexpected ansible configuration"):
         runtime._prepare_ansible_paths()
 
 
 @pytest.mark.parametrize(
     ("folder", "role_name", "isolated"),
     (
@@ -133,127 +144,112 @@
     caplog: pytest.LogCaptureFixture,
     folder: str,
     role_name: str,
     isolated: bool,
 ) -> None:
     """Checks that we can install roles."""
     caplog.set_level(logging.INFO)
-    project_dir = os.path.join(os.path.dirname(__file__), "roles", folder)
+    project_dir = Path(__file__).parent / "roles" / folder
     runtime = Runtime(isolated=isolated, project_dir=project_dir)
     runtime.prepare_environment(install_local=True)
     # check that role appears as installed now
-    result = runtime.exec(["ansible-galaxy", "list"])
+    result = runtime.run(["ansible-galaxy", "list"])
     assert result.returncode == 0, result
     assert role_name in result.stdout
     if isolated:
         assert pathlib.Path(f"{runtime.cache_dir}/roles/{role_name}").is_symlink()
     else:
         assert pathlib.Path(
-            f"{os.path.expanduser(runtime.config.default_roles_path[0])}/{role_name}"
+            f"{Path(runtime.config.default_roles_path[0]).expanduser()}/{role_name}",
         ).is_symlink()
     runtime.clean()
     # also test that clean does not break when cache_dir is missing
     tmp_dir = runtime.cache_dir
     runtime.cache_dir = None
     runtime.clean()
     runtime.cache_dir = tmp_dir
 
 
 def test_prepare_environment_with_collections(tmp_path: pathlib.Path) -> None:
     """Check that collections are correctly installed."""
-    runtime = Runtime(isolated=True, project_dir=str(tmp_path))
+    runtime = Runtime(isolated=True, project_dir=tmp_path)
     runtime.prepare_environment(required_collections={"community.molecule": "0.1.0"})
 
 
 def test_runtime_install_requirements_missing_file() -> None:
     """Check that missing requirements file is ignored."""
     # Do not rely on this behavior, it may be removed in the future
     runtime = Runtime()
-    runtime.install_requirements("/that/does/not/exist")
+    runtime.install_requirements(Path("/that/does/not/exist"))
 
 
 @pytest.mark.parametrize(
     ("file", "exc", "msg"),
     (
         (
-            "/dev/null",
+            Path("/dev/null"),
             InvalidPrerequisiteError,
             "file is not a valid Ansible requirements file",
         ),
         (
-            os.path.join(
-                os.path.dirname(__file__),
-                "assets",
-                "requirements-invalid-collection.yml",
-            ),
+            Path(__file__).parent / "assets" / "requirements-invalid-collection.yml",
             AnsibleCommandError,
             "Got 1 exit code while running: ansible-galaxy",
         ),
         (
-            os.path.join(
-                os.path.dirname(__file__),
-                "assets",
-                "requirements-invalid-role.yml",
-            ),
+            Path(__file__).parent / "assets" / "requirements-invalid-role.yml",
             AnsibleCommandError,
             "Got 1 exit code while running: ansible-galaxy",
         ),
     ),
     ids=("empty", "invalid-collection", "invalid-role"),
 )
 def test_runtime_install_requirements_invalid_file(
-    file: str, exc: Type[Any], msg: str
+    file: Path,
+    exc: type[Any],
+    msg: str,
 ) -> None:
     """Check that invalid requirements file is raising."""
     runtime = Runtime()
     with pytest.raises(
         exc,
         match=msg,
     ):
         runtime.install_requirements(file)
 
 
 @contextmanager
-def remember_cwd(cwd: str) -> Iterator[None]:
-    """Context manager for chdir."""
-    curdir = os.getcwd()
+def cwd(path: Path) -> Iterator[None]:
+    """Context manager for temporary changing current working directory."""
+    old_pwd = Path.cwd()
+    os.chdir(path)
     try:
-        os.chdir(cwd)
         yield
     finally:
-        os.chdir(curdir)
+        os.chdir(old_pwd)
 
 
 def test_prerun_reqs_v1(caplog: pytest.LogCaptureFixture, runtime: Runtime) -> None:
     """Checks that the linter can auto-install requirements v1 when found."""
-    cwd = os.path.realpath(
-        os.path.join(
-            os.path.dirname(os.path.realpath(__file__)), "..", "examples", "reqs_v1"
-        )
-    )
-    with remember_cwd(cwd):
-        with caplog.at_level(logging.INFO):
-            runtime.prepare_environment()
+    path = Path(__file__).parent.parent / "examples" / "reqs_v1"
+    with cwd(path), caplog.at_level(logging.INFO):
+        runtime.prepare_environment()
     assert any(
         msg.startswith("Running ansible-galaxy role install") for msg in caplog.messages
     )
     assert all(
         "Running ansible-galaxy collection install" not in msg
         for msg in caplog.messages
     )
 
 
 def test_prerun_reqs_v2(caplog: pytest.LogCaptureFixture, runtime: Runtime) -> None:
     """Checks that the linter can auto-install requirements v2 when found."""
-    cwd = os.path.realpath(
-        os.path.join(
-            os.path.dirname(os.path.realpath(__file__)), "..", "examples", "reqs_v2"
-        )
-    )
-    with remember_cwd(cwd):
+    path = (Path(__file__).parent.parent / "examples" / "reqs_v2").resolve()
+    with cwd(path):
         with caplog.at_level(logging.INFO):
             runtime.prepare_environment()
         assert any(
             msg.startswith("Running ansible-galaxy role install")
             for msg in caplog.messages
         )
         assert any(
@@ -297,15 +293,17 @@
     (
         (["a"], "a"),
         (["a", "b"], "a:b"),
         (["a", "b", "c"], "a:b:c"),
     ),
 )
 def test__update_env_no_old_value_no_default(
-    monkeypatch: MonkeyPatch, value: List[str], result: str
+    monkeypatch: MonkeyPatch,
+    value: list[str],
+    result: str,
 ) -> None:
     """Values are concatenated using : as the separator."""
     monkeypatch.delenv("DUMMY_VAR", raising=False)
 
     runtime = Runtime()
     runtime._update_env("DUMMY_VAR", value)
 
@@ -316,15 +314,18 @@
     ("default", "value", "result"),
     (
         ("a:b", ["c"], "c:a:b"),
         ("a:b", ["c:d"], "c:d:a:b"),
     ),
 )
 def test__update_env_no_old_value(
-    monkeypatch: MonkeyPatch, default: str, value: List[str], result: str
+    monkeypatch: MonkeyPatch,
+    default: str,
+    value: list[str],
+    result: str,
 ) -> None:
     """Values are appended to default value."""
     monkeypatch.delenv("DUMMY_VAR", raising=False)
 
     runtime = Runtime()
     runtime._update_env("DUMMY_VAR", value, default)
 
@@ -335,15 +336,18 @@
     ("old_value", "value", "result"),
     (
         ("a:b", ["c"], "c:a:b"),
         ("a:b", ["c:d"], "c:d:a:b"),
     ),
 )
 def test__update_env_no_default(
-    monkeypatch: MonkeyPatch, old_value: str, value: List[str], result: str
+    monkeypatch: MonkeyPatch,
+    old_value: str,
+    value: list[str],
+    result: str,
 ) -> None:
     """Values are appended to preexisting value."""
     monkeypatch.setenv("DUMMY_VAR", old_value)
 
     runtime = Runtime()
     runtime._update_env("DUMMY_VAR", value)
 
@@ -358,68 +362,70 @@
         ("", "c", ["e"], "e"),
         ("a", "c", ["e:f"], "e:f:a"),
     ),
 )
 def test__update_env(
     monkeypatch: MonkeyPatch,
     old_value: str,
-    default: str,  # pylint: disable=unused-argument
-    value: List[str],
+    default: str,  # pylint: disable=unused-argument # noqa: ARG001
+    value: list[str],
     result: str,
 ) -> None:
     """Defaults are ignored when preexisting value is present."""
     monkeypatch.setenv("DUMMY_VAR", old_value)
 
     runtime = Runtime()
     runtime._update_env("DUMMY_VAR", value)
 
     assert runtime.environ["DUMMY_VAR"] == result
 
 
 def test_require_collection_wrong_version(runtime: Runtime) -> None:
     """Tests behaviour of require_collection."""
     subprocess.check_output(
-        [
+        [  # noqa: S603
             "ansible-galaxy",
             "collection",
             "install",
             "examples/reqs_v2/community-molecule-0.1.0.tar.gz",
             "-p",
             "~/.ansible/collections",
-        ]
+        ],
     )
     with pytest.raises(InvalidPrerequisiteError) as pytest_wrapped_e:
         runtime.require_collection("community.molecule", "9999.9.9")
     assert pytest_wrapped_e.type == InvalidPrerequisiteError
     assert pytest_wrapped_e.value.code == INVALID_PREREQUISITES_RC
 
 
 def test_require_collection_invalid_name(runtime: Runtime) -> None:
     """Check that require_collection raise with invalid collection name."""
     with pytest.raises(
-        InvalidPrerequisiteError, match="Invalid collection name supplied:"
+        InvalidPrerequisiteError,
+        match="Invalid collection name supplied:",
     ):
         runtime.require_collection("that-is-invalid")
 
 
 def test_require_collection_invalid_collections_path(runtime: Runtime) -> None:
     """Check that require_collection raise with invalid collections path."""
-    runtime.config.collections_paths = "/that/is/invalid"  # type: ignore
+    runtime.config.collections_paths = "/that/is/invalid"  # type: ignore[assignment]
     with pytest.raises(
-        InvalidPrerequisiteError, match="Unable to determine ansible collection paths"
+        InvalidPrerequisiteError,
+        match="Unable to determine ansible collection paths",
     ):
         runtime.require_collection("community.molecule")
 
 
 def test_require_collection_preexisting_broken(tmp_path: pathlib.Path) -> None:
     """Check that require_collection raise with broken pre-existing collection."""
-    runtime = Runtime(isolated=True, project_dir=str(tmp_path))
+    runtime = Runtime(isolated=True, project_dir=tmp_path)
     dest_path: str = runtime.config.collections_paths[0]
-    dest = os.path.join(dest_path, "ansible_collections", "foo", "bar")
-    os.makedirs(dest, exist_ok=True)
+    dest = pathlib.Path(dest_path) / "ansible_collections" / "foo" / "bar"
+    dest.mkdir(parents=True, exist_ok=True)
     with pytest.raises(InvalidPrerequisiteError, match="missing MANIFEST.json"):
         runtime.require_collection("foo.bar")
 
 
 def test_require_collection(runtime_tmp: Runtime) -> None:
     """Check that require collection successful install case."""
     runtime_tmp.require_collection("community.molecule", "0.1.0")
@@ -431,15 +437,18 @@
         ("fake_namespace.fake_name", None, True),
         ("fake_namespace.fake_name", "9999.9.9", True),
         ("fake_namespace.fake_name", None, False),
     ),
     ids=("a", "b", "c"),
 )
 def test_require_collection_missing(
-    name: str, version: str, install: bool, runtime: Runtime
+    name: str,
+    version: str,
+    install: bool,
+    runtime: Runtime,
 ) -> None:
     """Tests behaviour of require_collection, missing case."""
     with pytest.raises(AnsibleCompatError) as pytest_wrapped_e:
         runtime.require_collection(name=name, version=version, install=install)
     assert pytest_wrapped_e.type == InvalidPrerequisiteError
     assert pytest_wrapped_e.value.code == INVALID_PREREQUISITES_RC
 
@@ -448,15 +457,16 @@
     """Check that valid collection installs do not fail."""
     runtime.install_collection("examples/reqs_v2/community-molecule-0.1.0.tar.gz")
 
 
 def test_install_collection_dest(runtime: Runtime, tmp_path: pathlib.Path) -> None:
     """Check that valid collection to custom destination passes."""
     runtime.install_collection(
-        "examples/reqs_v2/community-molecule-0.1.0.tar.gz", destination=tmp_path
+        "examples/reqs_v2/community-molecule-0.1.0.tar.gz",
+        destination=tmp_path,
     )
     expected_file = (
         tmp_path / "ansible_collections" / "community" / "molecule" / "MANIFEST.json"
     )
     assert expected_file.is_file()
 
 
@@ -475,21 +485,23 @@
     pathlib.Path(f"{runtime_tmp.project_dir}/meta/main.yml").touch()
     # this should only raise a warning
     runtime_tmp._install_galaxy_role(runtime_tmp.project_dir, role_name_check=1)
     # this should test the bypass role name check path
     runtime_tmp._install_galaxy_role(runtime_tmp.project_dir, role_name_check=2)
     # this should raise an error
     with pytest.raises(
-        InvalidPrerequisiteError, match="does not follow current galaxy requirements"
+        InvalidPrerequisiteError,
+        match="does not follow current galaxy requirements",
     ):
         runtime_tmp._install_galaxy_role(runtime_tmp.project_dir, role_name_check=0)
 
 
 def test_install_galaxy_role_unlink(
-    runtime_tmp: Runtime, caplog: pytest.LogCaptureFixture
+    runtime_tmp: Runtime,
+    caplog: pytest.LogCaptureFixture,
 ) -> None:
     """Test ability to unlink incorrect symlinked roles."""
     caplog.set_level(logging.INFO)
     runtime_tmp.prepare_environment()
     pathlib.Path(f"{runtime_tmp.cache_dir}/roles").mkdir(parents=True, exist_ok=True)
     pathlib.Path(f"{runtime_tmp.cache_dir}/roles/acme.get_rich").symlink_to("/dev/null")
     pathlib.Path(f"{runtime_tmp.project_dir}/meta").mkdir()
@@ -502,22 +514,21 @@
     )
     runtime_tmp._install_galaxy_role(runtime_tmp.project_dir)
     assert "symlink to current repository" in caplog.text
 
 
 def test_install_galaxy_role_bad_namespace(runtime_tmp: Runtime) -> None:
     """Check install role with bad namespace in galaxy info."""
-    # pathlib.Path(f'{runtime_tmp.project_dir}/galaxy.yml').touch()
     pathlib.Path(f"{runtime_tmp.project_dir}/meta").mkdir()
     pathlib.Path(f"{runtime_tmp.project_dir}/meta/main.yml").write_text(
         """galaxy_info:
   role_name: foo
   author: bar
   namespace: ["xxx"]
-"""
+""",
     )
     # this should raise an error regardless the role_name_check value
     with pytest.raises(AnsibleCompatError, match="Role namespace must be string, not"):
         runtime_tmp._install_galaxy_role(runtime_tmp.project_dir, role_name_check=1)
 
 
 @pytest.mark.parametrize(
@@ -555,18 +566,18 @@
     runtime_tmp.prepare_environment()
     pathlib.Path(f"{runtime_tmp.project_dir}/meta").mkdir()
     pathlib.Path(f"{runtime_tmp.project_dir}/meta/main.yml").write_text(
         """galaxy_info:
   role_name: foo
   author: bar
   namespace: acme
-"""
+""",
     )
     runtime_tmp._install_galaxy_role(runtime_tmp.project_dir, role_name_check=2)
-    result = runtime_tmp.exec(["ansible-galaxy", "list"])
+    result = runtime_tmp.run(["ansible-galaxy", "list"])
     assert "- acme.foo," in result.stdout
     assert result.returncode == 0, result
 
 
 def test_upgrade_collection(runtime_tmp: Runtime) -> None:
     """Check that collection upgrade is possible."""
     # ensure that we inject our tmp folders in ansible paths
@@ -610,15 +621,17 @@
         ("1.0", None, True),
         ("9999.0", None, False),
         (None, "1.0", False),
     ),
     ids=("1", "2", "3", "4", "5"),
 )
 def test_runtime_version_in_range(
-    lower: Union[str, None], upper: Union[str, None], expected: bool
+    lower: Union[str, None],
+    upper: Union[str, None],
+    expected: bool,
 ) -> None:
     """Validate functioning of version_in_range."""
     runtime = Runtime()
     assert runtime.version_in_range(lower=lower, upper=upper) is expected
 
 
 @pytest.mark.parametrize(
@@ -630,76 +643,78 @@
     ids=("normal", "deep"),
 )
 def test_install_collection_from_disk(path: str, scenario: str) -> None:
     """Tests ability to install a local collection."""
     # ensure we do not have acme.google installed in user directory as it may
     # produce false positives
     rmtree(
-        os.path.expanduser("~/.ansible/collections/ansible_collections/acme/goodies"),
+        pathlib.Path(
+            "~/.ansible/collections/ansible_collections/acme/goodies",
+        ).expanduser(),
         ignore_errors=True,
     )
-    with remember_cwd(path):
+    with cwd(Path(path)):
         runtime = Runtime(isolated=True)
         # this should call install_collection_from_disk(".")
         runtime.prepare_environment(install_local=True)
         # that molecule converge playbook can be used without molecule and
         # should validate that the installed collection is available.
-        result = runtime.exec(["ansible-playbook", f"molecule/{scenario}/converge.yml"])
+        result = runtime.run(["ansible-playbook", f"molecule/{scenario}/converge.yml"])
         assert result.returncode == 0, result.stdout
         runtime.clean()
 
 
 def test_install_collection_from_disk_fail() -> None:
     """Tests that we fail to install a broken collection."""
-    with remember_cwd("test/collections/acme.broken"):
+    with cwd(Path("test/collections/acme.broken")):
         runtime = Runtime(isolated=True)
         with pytest.raises(RuntimeError) as exc_info:
             runtime.prepare_environment(install_local=True)
         # based on version of Ansible used, we might get a different error,
         # but both errors should be considered acceptable
         assert exc_info.type in (
             RuntimeError,
             AnsibleCompatError,
             AnsibleCommandError,
             InvalidPrerequisiteError,
         )
         assert exc_info.match(
-            "(is missing the following mandatory|Got 1 exit code while running: ansible-galaxy collection build)"
+            "(is missing the following mandatory|Got 1 exit code while running: ansible-galaxy collection build)",
         )
 
 
 def test_prepare_environment_offline_role() -> None:
     """Ensure that we can make use of offline roles."""
-    with remember_cwd("test/roles/acme.missing_deps"):
+    with cwd(Path("test/roles/acme.missing_deps")):
         runtime = Runtime(isolated=True)
         runtime.prepare_environment(install_local=True, offline=True)
 
 
 def test_runtime_run(runtime: Runtime) -> None:
     """Check if tee and non tee mode return same kind of results."""
-    result1 = runtime.exec(["seq", "10"])
-    result2 = runtime.exec(["seq", "10"], tee=True)
+    result1 = runtime.run(["seq", "10"])
+    result2 = runtime.run(["seq", "10"], tee=True)
     assert result1.returncode == result2.returncode
     assert result1.stderr == result2.stderr
     assert result1.stdout == result2.stdout
 
 
 def test_runtime_exec_cwd(runtime: Runtime) -> None:
     """Check if passing cwd works as expected."""
-    cwd = "/"
-    result1 = runtime.exec(["pwd"], cwd=cwd)
-    result2 = runtime.exec(["pwd"])
-    assert result1.stdout.rstrip() == cwd
+    path = Path("/")
+    result1 = runtime.run(["pwd"], cwd=path)
+    result2 = runtime.run(["pwd"])
+    assert result1.stdout.rstrip() == str(path)
     assert result1.stdout != result2.stdout
 
 
 def test_runtime_exec_env(runtime: Runtime) -> None:
     """Check if passing env works."""
-    result = runtime.exec(["printenv", "FOO"])
+    result = runtime.run(["printenv", "FOO"])
     assert not result.stdout
 
-    result = runtime.exec(["printenv", "FOO"], env={"FOO": "bar"})
+    result = runtime.run(["printenv", "FOO"], env={"FOO": "bar"})
     assert result.stdout.rstrip() == "bar"
 
     runtime.environ["FOO"] = "bar"
-    result = runtime.exec(["printenv", "FOO"])
+    result = runtime.run(["printenv", "FOO"])
     assert result.stdout.rstrip() == "bar"
```

### Comparing `ansible-compat-4.0.0/test/test_runtime_example.py` & `ansible-compat-4.0.0a1/test/test_runtime_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 def test_runtime_example() -> None:
     """Test basic functionality of Runtime class."""
     # instantiate the runtime using isolated mode, so installing new
     # roles/collections do not pollute the default setup.
     runtime = Runtime(isolated=True, max_retries=3)
 
     # Print Ansible core version
-    print(runtime.version)  # 2.9.10 (Version object)
+    _ = runtime.version  # 2.9.10 (Version object)
     # Get configuration info from runtime
-    print(runtime.config.collections_path)
+    _ = runtime.config.collections_path
 
     # Detect if current project is a collection and install its requirements
     runtime.prepare_environment(install_local=True)  # will retry 3 times if needed
 
     # Install a new collection (will retry 3 times if needed)
     runtime.install_collection("examples/reqs_v2/community-molecule-0.1.0.tar.gz")
 
     # Execute a command
-    result = runtime.exec(["ansible-doc", "--list"])
+    result = runtime.run(["ansible-doc", "--list"])
     assert result.returncode == 0
```

### Comparing `ansible-compat-4.0.0/test/test_schema.py` & `ansible-compat-4.0.0a1/test/test_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Tests for schema utilities."""
+from __future__ import annotations
+
 import json
-import os
-from typing import Any
+from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
 import pytest
 
 from ansible_compat.schema import JsonSchemaError, json_path, validate
 
+if TYPE_CHECKING:
+    from ansible_compat.types import JSON
+
 expected_results = [
     JsonSchemaError(
         message="False is not of type 'string'",
         data_path="environment.a",
         json_path="$.environment.a",
         schema_path="properties.environment.additionalProperties.type",
         relative_schema='{"type": "string"}',
@@ -27,24 +32,24 @@
         expected="string",
         validator="type",
         found="True",
     ),
 ]
 
 
-def json_from_asset(file_name: str) -> Any:
+def json_from_asset(file_name: str) -> JSON:
     """Load a json file from disk."""
-    file_name = os.path.join(os.path.dirname(os.path.abspath(__file__)), file_name)
-    with open(file_name, encoding="utf-8") as f:
-        return json.load(f)
+    file = Path(__file__).parent / file_name
+    with file.open(encoding="utf-8") as f:
+        return json.load(f)  # type: ignore[no-any-return]
 
 
-def jsonify(data: Any) -> Any:
+def jsonify(data: Any) -> JSON:  # noqa: ANN401
     """Convert object in JSON data structure."""
-    return json.loads(json.dumps(data, default=vars))
+    return json.loads(json.dumps(data, default=vars, sort_keys=True))  # type: ignore[no-any-return]
 
 
 @pytest.mark.parametrize("index", range(1))
 def test_schema(index: int) -> None:
     """Test the schema validator."""
     schema = json_from_asset(f"assets/validate{index}_schema.json")
     data = json_from_asset(f"assets/validate{index}_data.json")
```

### Comparing `ansible-compat-4.0.0/tox.ini` & `ansible-compat-4.0.0a1/tox.ini`

 * *Files identical despite different names*

