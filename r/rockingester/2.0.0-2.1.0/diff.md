# Comparing `tmp/rockingester-2.0.0.tar.gz` & `tmp/rockingester-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.0.0.tar", last modified: Thu Apr 27 05:48:01 2023, max compression
+gzip compressed data, was "rockingester-2.1.0.tar", last modified: Mon May  1 07:14:23 2023, max compression
```

## Comparing `rockingester-2.0.0.tar` & `rockingester-2.1.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 05:47:51.000000 rockingester-2.0.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 05:47:51.000000 rockingester-2.0.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-27 05:47:51.000000 rockingester-2.0.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.214316 rockingester-2.0.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 05:47:51.000000 rockingester-2.0.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-27 05:47:51.000000 rockingester-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-27 05:47:51.000000 rockingester-2.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 05:47:51.000000 rockingester-2.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 05:47:51.000000 rockingester-2.0.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 05:47:51.000000 rockingester-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-04-27 05:48:01.230316 rockingester-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-27 05:47:51.000000 rockingester-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-27 05:47:51.000000 rockingester-2.0.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.222316 rockingester-2.0.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 05:47:51.000000 rockingester-2.0.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-27 05:47:51.000000 rockingester-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:48:01.230316 rockingester-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.218316 rockingester-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.226316 rockingester-2.0.0/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 05:48:01.000000 rockingester-2.0.0/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-27 05:47:51.000000 rockingester-2.0.0/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:48:01.230316 rockingester-2.0.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-27 05:47:51.000000 rockingester-2.0.0/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 07:14:12.000000 rockingester-2.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 07:14:12.000000 rockingester-2.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-01 07:14:12.000000 rockingester-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-01 07:14:12.000000 rockingester-2.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 07:14:12.000000 rockingester-2.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 07:14:12.000000 rockingester-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-01 07:14:23.541447 rockingester-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 07:14:12.000000 rockingester-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-01 07:14:12.000000 rockingester-2.1.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-01 07:14:12.000000 rockingester-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:14:23.541447 rockingester-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/test_collector.py
```

### Comparing `rockingester-2.0.0/.dae-devops/Makefile` & `rockingester-2.1.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/conventions.rst` & `rockingester-2.1.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/developing.rst` & `rockingester-2.1.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/devops.rst` & `rockingester-2.1.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/docs_structure.rst` & `rockingester-2.1.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/installing.rst` & `rockingester-2.1.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/docs/testing.rst` & `rockingester-2.1.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.dae-devops/project.yaml` & `rockingester-2.1.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.devcontainer/Dockerfile` & `rockingester-2.1.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.devcontainer/devcontainer.json` & `rockingester-2.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/CONTRIBUTING.rst` & `rockingester-2.1.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/actions/install_requirements/action.yml` & `rockingester-2.1.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/dependabot.yml` & `rockingester-2.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/pages/make_switcher.py` & `rockingester-2.1.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/workflows/code.yml` & `rockingester-2.1.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/workflows/docs.yml` & `rockingester-2.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/workflows/docs_clean.yml` & `rockingester-2.1.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.github/workflows/linkcheck.yml` & `rockingester-2.1.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.gitignore` & `rockingester-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.gitlab-ci.yml` & `rockingester-2.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/.vscode/launch.json` & `rockingester-2.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/LICENSE` & `rockingester-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/PKG-INFO` & `rockingester-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.0.0
+Version: 2.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.0.0/README.rst` & `rockingester-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/configurations/development.yaml` & `rockingester-2.1.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/conf.py` & `rockingester-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/images/dls-favicon.ico` & `rockingester-2.1.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/images/dls-logo.svg` & `rockingester-2.1.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/index.rst` & `rockingester-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.1.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/docs/user/index.rst` & `rockingester-2.1.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/pyproject.toml` & `rockingester-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.1.0/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.0.0
+Version: 2.1.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.0.0/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.1.0/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.1.0/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/collectors/collectors.py` & `rockingester-2.1.0/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/collectors/context.py` & `rockingester-2.1.0/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/context_base.py` & `rockingester-2.1.0/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/exceptions.py` & `rockingester-2.1.0/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/thing.py` & `rockingester-2.1.0/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_api/things.py` & `rockingester-2.1.0/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_cli/main.py` & `rockingester-2.1.0/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_cli/subcommands/base.py` & `rockingester-2.1.0/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_cli/subcommands/service.py` & `rockingester-2.1.0/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_cli/version.py` & `rockingester-2.1.0/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/__main__.py` & `rockingester-2.1.0/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.1.0/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/collectors/base.py` & `rockingester-2.1.0/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.1.0/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/collectors/context.py` & `rockingester-2.1.0/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.1.0/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 # Crystal plate pydantic model.
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
 # Crystal well pydantic model.
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 
+# Crystal plate objects factory.
+from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
+
 # Base class for collector instances.
 from rockingester_lib.collectors.base import Base as CollectorBase
 
 logger = logging.getLogger(__name__)
 
 thing_type = "rockingester_lib.collectors.direct_poll"
 
@@ -258,14 +261,16 @@
         crystal_plate_model: CrystalPlateModel,
         visit_directory: Path,
     ) -> None:
         """
         Scrape a single directory looking for new files.
 
         Adds discovered files to internal list which gets pushed when it reaches a configurable size.
+
+        TODO: Consider some other flow where well images can be copied as they arrive instead of doing them all in a bunch.
         """
 
         # Name of the destination directory where we will permanently store ingested well image files.
         target = (
             visit_directory / self.__visit_plates_subdirectory / plate_directory.name
         )
 
@@ -285,16 +290,22 @@
             )
 
         # Get all the well images in the plate directory.
         well_names = [
             entry.name for entry in os.scandir(plate_directory) if entry.is_file()
         ]
 
+        # Make an object corresponding to the crystal plate model's type.
+        crystal_plate_object = CrystalPlateObjects().build_object(
+            {"type": crystal_plate_model.thing_type}
+        )
+
         # Don't handle the plate directory until all images have arrived.
-        if len(well_names) < 288:
+        # TODO: Put in some kind of failsafe in direct_poll.py to handle case where all the well images never arrive.
+        if len(well_names) < crystal_plate_object.get_well_count():
             return
 
         # Sort wells by name so that tests are deterministic.
         well_names.sort()
 
         crystal_well_models: List[CrystalWellModel] = []
         for well_name in well_names:
```

### Comparing `rockingester-2.0.0/src/rockingester_lib/contexts/base.py` & `rockingester-2.1.0/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/exceptions.py` & `rockingester-2.1.0/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/src/rockingester_lib/version.py` & `rockingester-2.1.0/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/tests/base.py` & `rockingester-2.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/tests/configurations/direct_poll.yaml` & `rockingester-2.1.0/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/tests/configurations/service.yaml` & `rockingester-2.1.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/tests/conftest.py` & `rockingester-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.0.0/tests/test_collector.py` & `rockingester-2.1.0/tests/test_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import asyncio
 import logging
 import time
 from pathlib import Path
 
 from dls_utilpack.visit import get_xchem_subdirectory
 
+# Types which the CrystalPlateObjects factory can use to build an instance.
+from xchembku_api.crystal_plate_objects.constants import (
+    ThingTypes as CrystalPlateObjectThingTypes,
+)
+
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
 # Client context creator.
@@ -137,14 +142,15 @@
         visit = "cm00001-1_otherstuff"
         created_crystal_plate_models = []
         created_crystal_plate_models.append(
             CrystalPlateModel(
                 formulatrix__plate__id=10,
                 barcode="98ab",
                 visit=visit,
+                thing_type=CrystalPlateObjectThingTypes.SWISS3,
             )
         )
 
         nobarcode_barcode = "98ac"
 
         # Create a crystal plate model with a good barcode but bad visit.
         novisit_barcode = "98ad"
```

