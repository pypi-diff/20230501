# Comparing `tmp/xchembku-1.3.0.tar.gz` & `tmp/xchembku-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.3.0.tar", last modified: Fri Apr 28 07:41:31 2023, max compression
+gzip compressed data, was "xchembku-1.4.0.tar", last modified: Mon May  1 05:33:30 2023, max compression
```

## Comparing `xchembku-1.3.0.tar` & `xchembku-1.4.0.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.815016 xchembku-1.3.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 07:41:21.000000 xchembku-1.3.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 07:41:21.000000 xchembku-1.3.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-28 07:41:21.000000 xchembku-1.3.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.803016 xchembku-1.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.819016 xchembku-1.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-28 07:41:21.000000 xchembku-1.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-28 07:41:21.000000 xchembku-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-28 07:41:21.000000 xchembku-1.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 07:41:21.000000 xchembku-1.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 07:41:21.000000 xchembku-1.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 07:41:21.000000 xchembku-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-28 07:41:31.835016 xchembku-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-28 07:41:21.000000 xchembku-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-28 07:41:21.000000 xchembku-1.3.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.807016 xchembku-1.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.823016 xchembku-1.3.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.827016 xchembku-1.3.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 07:41:21.000000 xchembku-1.3.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-28 07:41:21.000000 xchembku-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:41:31.835016 xchembku-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.811016 xchembku-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 07:41:31.000000 xchembku-1.3.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.831016 xchembku-1.3.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 07:41:21.000000 xchembku-1.3.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:41:31.835016 xchembku-1.3.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_crystal_well_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-28 07:41:21.000000 xchembku-1.3.0/tests/test_soakdb3_crystal_well.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.376048 xchembku-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-01 05:33:20.000000 xchembku-1.4.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-01 05:33:20.000000 xchembku-1.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-01 05:33:20.000000 xchembku-1.4.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.360047 xchembku-1.4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-01 05:33:20.000000 xchembku-1.4.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-01 05:33:20.000000 xchembku-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-01 05:33:20.000000 xchembku-1.4.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 05:33:20.000000 xchembku-1.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 05:33:20.000000 xchembku-1.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-01 05:33:20.000000 xchembku-1.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-01 05:33:20.000000 xchembku-1.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 05:33:20.000000 xchembku-1.4.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 05:33:20.000000 xchembku-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-01 05:33:30.376048 xchembku-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 05:33:20.000000 xchembku-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-01 05:33:20.000000 xchembku-1.4.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.360047 xchembku-1.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 05:33:20.000000 xchembku-1.4.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-01 05:33:20.000000 xchembku-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 05:33:30.376048 xchembku-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.364048 xchembku-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.368048 xchembku-1.4.0/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/crystal_plate_objects/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 05:33:30.000000 xchembku-1.4.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.372048 xchembku-1.4.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.376048 xchembku-1.4.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-01 05:33:20.000000 xchembku-1.4.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.376048 xchembku-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:33:30.376048 xchembku-1.4.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/test_crystal_well_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-01 05:33:20.000000 xchembku-1.4.0/tests/test_soakdb3_crystal_well.py
```

### Comparing `xchembku-1.3.0/.dae-devops/Makefile` & `xchembku-1.4.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/conventions.rst` & `xchembku-1.4.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/developing.rst` & `xchembku-1.4.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/devops.rst` & `xchembku-1.4.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.4.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/installing.rst` & `xchembku-1.4.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/docs/testing.rst` & `xchembku-1.4.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.dae-devops/project.yaml` & `xchembku-1.4.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.devcontainer/Dockerfile` & `xchembku-1.4.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.devcontainer/devcontainer.json` & `xchembku-1.4.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/CONTRIBUTING.rst` & `xchembku-1.4.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/actions/install_requirements/action.yml` & `xchembku-1.4.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/dependabot.yml` & `xchembku-1.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/pages/make_switcher.py` & `xchembku-1.4.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/workflows/code.yml` & `xchembku-1.4.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/workflows/docs.yml` & `xchembku-1.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/workflows/docs_clean.yml` & `xchembku-1.4.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.github/workflows/linkcheck.yml` & `xchembku-1.4.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.gitignore` & `xchembku-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.gitlab-ci.yml` & `xchembku-1.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/.vscode/launch.json` & `xchembku-1.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/LICENSE` & `xchembku-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/PKG-INFO` & `xchembku-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.3.0
+Version: 1.4.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.3.0/README.rst` & `xchembku-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/configurations/development.yaml` & `xchembku-1.4.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/conf.py` & `xchembku-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/images/dls-favicon.ico` & `xchembku-1.4.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/images/dls-logo.svg` & `xchembku-1.4.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/index.rst` & `xchembku-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.4.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/docs/user/index.rst` & `xchembku-1.4.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/pyproject.toml` & `xchembku-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.4.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.3.0
+Version: 1.4.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.3.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.4.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/context_base.py` & `xchembku-1.4.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.4.0/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.4.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.4.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.4.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/exceptions.py` & `xchembku-1.4.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.4.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.4.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.4.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     Typically this structure is populated and transmitted by the chimpflow.
     """
 
     uuid: str
     crystal_well_uuid: Optional[str] = None
     confirmed_target_x: Optional[int] = None
     confirmed_target_y: Optional[int] = None
+    confirmed_microns_x: Optional[int] = None
+    confirmed_microns_y: Optional[int] = None
     is_usable: Optional[bool] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
```

### Comparing `xchembku-1.3.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.4.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.4.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,31 +8,34 @@
     Model containing well information formed from a composite query of droplocation information.
 
     Typically this structure is returned by queries.
     """
 
     # Stuff from the original record.
     uuid: str
-    visit: str
     position: str
     filename: str
     width: Optional[int]
     height: Optional[int]
     error: Optional[str]
     created_on: str
 
+    # Stuff from the plate.
+    visit: str
+    crystal_plate_thing_type: str
+
     # Stuff from the autolocation.
     auto_target_x: Optional[int] = None
     auto_target_y: Optional[int] = None
     well_centroid_x: Optional[int] = None
     well_centroid_y: Optional[int] = None
     drop_detected: Optional[bool] = None
     number_of_crystals: Optional[int] = None
 
     # Stuff from the droplocation.
     crystal_well_droplocation_uuid: Optional[str] = None
     confirmed_target_x: Optional[int] = None
     confirmed_target_y: Optional[int] = None
-    echo_coordinate_x: Optional[int] = None
-    echo_coordinate_y: Optional[int] = None
+    confirmed_microns_x: Optional[int] = None
+    confirmed_microns_y: Optional[int] = None
 
     is_usable: Optional[bool] = None
```

### Comparing `xchembku-1.3.0/src/xchembku_cli/main.py` & `xchembku-1.4.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.4.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.4.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_cli/version.py` & `xchembku-1.4.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/__main__.py` & `xchembku-1.4.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/contexts/base.py` & `xchembku-1.4.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.4.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.4.0/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/databases/databases.py` & `xchembku-1.4.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/databases/normsql.py` & `xchembku-1.4.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.4.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from dls_normsql.constants import CommonFieldnames
 from dls_utilpack.describe import describe
 
 from xchembku_api.models.crystal_well_droplocation_model import (
     CrystalWellDroplocationModel,
 )
+from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
 from xchembku_lib.datafaces.direct_base import DirectBase
 
 logger = logging.getLogger(__name__)
 
 # Module-level lock to keep upsert atomic.
 upsert_lock = RLock()
 
@@ -60,14 +61,58 @@
         return await self.upsert_crystal_well_droplocations(
             models,
             only_fields=only_fields,
             why=why,
         )
 
     # ----------------------------------------------------------------------------------------
+    async def __add_confirmed_microns(self, model_dict: Dict, why=None) -> None:
+
+        if why is not None:
+            why = f"[CONFMIC] {why}"
+
+        # Input model not updating confirmed target?
+        if (
+            "confirmed_target_x" not in model_dict
+            or "confirmed_target_y" not in model_dict
+        ):
+            return
+
+        from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
+
+        filter = CrystalWellFilterModel(anchor=model_dict["crystal_well_uuid"])
+
+        # Get the well record.
+        crystal_well_models = await self.fetch_crystal_wells_needing_droplocation(
+            filter,
+            why=f"(crystal well for) {why}",
+        )
+
+        if len(crystal_well_models) == 0:
+            raise RuntimeError(
+                "database integrity error: no crystal well for droplocation upsert"
+            )
+        crystal_well_model = crystal_well_models[0]
+        crystal_well_model.confirmed_target_x = model_dict["confirmed_target_x"]
+        crystal_well_model.confirmed_target_y = model_dict["confirmed_target_y"]
+
+        crystal_plate_object = CrystalPlateObjects().build_object(
+            {"type": crystal_well_model.crystal_plate_thing_type}
+        )
+
+        x, y = crystal_plate_object.compute_drop_location_microns(
+            crystal_well_model.dict()
+        )
+
+        logger.debug(f"{why} x is {x}, y is {y}")
+
+        model_dict["confirmed_microns_x"] = x
+        model_dict["confirmed_microns_y"] = y
+
+    # ----------------------------------------------------------------------------------------
     async def upsert_crystal_well_droplocations(
         self,
         models: List[CrystalWellDroplocationModel],
         only_fields: Optional[List[str]] = None,
         why=None,
     ) -> Dict:
         """
@@ -83,37 +128,42 @@
 
         inserted_count = 0
         updated_count = 0
 
         # Loop over all the models to be upserted.
         for model in models:
             with upsert_lock:
+                model_dict = copy.deepcopy(model.dict())
+
                 # Find any existing record for this model object.
                 records = await self.query(
                     "SELECT * FROM crystal_well_droplocations WHERE crystal_well_uuid = ?",
                     subs=[model.crystal_well_uuid],
                     why=why,
                 )
 
                 if len(records) > 0:
                     logger.debug(
                         describe(
                             "crystal_well_droplocation record before update", records[0]
                         )
                     )
                     # Make a copy of the model record and remove some fields not to update.
-                    model_dict = copy.deepcopy(model.dict())
                     model_dict.pop(CommonFieldnames.UUID)
                     model_dict.pop(CommonFieldnames.CREATED_ON)
-                    model_dict.pop("crystal_well_uuid")
                     if only_fields is not None:
                         for field in list(model_dict.keys()):
                             if field not in only_fields:
                                 model_dict.pop(field)
 
+                    # Convert confirmed target to microns and store in the dict.
+                    await self.__add_confirmed_microns(model_dict, why=why)
+
+                    model_dict.pop("crystal_well_uuid")
+
                     result = await self.update(
                         "crystal_well_droplocations",
                         model_dict,
                         "(crystal_well_uuid = ?)",
                         subs=[model.crystal_well_uuid],
                         why=why,
                     )
@@ -128,17 +178,21 @@
                     logger.debug(
                         describe(
                             "crystal_well_droplocation record after update", records[0]
                         )
                     )
 
                 else:
+
+                    # Convert confirmed target to microns and store in the dict.
+                    await self.__add_confirmed_microns(model_dict, why=why)
+
                     await self.insert(
                         "crystal_well_droplocations",
-                        [model.dict()],
+                        [model_dict],
                         why=why,
                     )
                     inserted_count += 1
 
         return {
             "updated_count": updated_count,
             "inserted_count": inserted_count,
```

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,18 +195,19 @@
             "\n  crystal_well_autolocations.auto_target_y,"
             "\n  crystal_well_autolocations.well_centroid_x,"
             "\n  crystal_well_autolocations.well_centroid_y,"
             "\n  crystal_well_autolocations.drop_detected,"
             "\n  crystal_well_autolocations.number_of_crystals,"
             "\n  crystal_well_droplocations.confirmed_target_x,"
             "\n  crystal_well_droplocations.confirmed_target_y,"
-            "\n  (crystal_well_droplocations.confirmed_target_x - crystal_well_autolocations.well_centroid_x) AS echo_coordinate_x,"
-            "\n  (crystal_well_droplocations.confirmed_target_y - crystal_well_autolocations.well_centroid_y) AS echo_coordinate_y,"
+            "\n  crystal_well_droplocations.confirmed_microns_x,"
+            "\n  crystal_well_droplocations.confirmed_microns_y,"
             "\n  crystal_well_droplocations.is_usable,"
-            "\n  crystal_plates.visit"
+            "\n  crystal_plates.visit,"
+            "\n  crystal_plates.thing_type AS crystal_plate_thing_type"
             "\nFROM crystal_wells"
             "\nJOIN crystal_well_autolocations ON crystal_well_autolocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_well_droplocations ON crystal_well_droplocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_plates ON crystal_plates.uuid = crystal_wells.crystal_plate_uuid"
         )
 
         # Caller wants a glob of file?
```

### Comparing `xchembku-1.3.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.4.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/src/xchembku_lib/version.py` & `xchembku-1.4.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/base.py` & `xchembku-1.4.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/configurations/direct.yaml` & `xchembku-1.4.0/tests/configurations/direct.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/configurations/service.yaml` & `xchembku-1.4.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/conftest.py` & `xchembku-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/test_crystal_plate.py` & `xchembku-1.4.0/tests/test_crystal_plate.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,16 +228,32 @@
 
         assert upserted_models[0].uuid == upserted_model.uuid
         assert upserted_models[0].created_on == created_on
         assert upserted_models[0].visit == upserted_model.visit
 
         # Make sure that the model which came out of the database can be instantiated.
         specification = {"type": upserted_models[0].thing_type}
-        o = CrystalPlateObjects().build_object(specification)
-        assert o.get_well_count() == 288
+        crystal_plate_model = CrystalPlateObjects().build_object(specification)
+        assert crystal_plate_model.get_well_count() == 288
+
+        # TODO: Move testing of drop location in microns out of test_crystal_plate.py and into its own test file.
+        # Cook up a fake crystal well so we can use the plate to convert drop location to microns.
+        crystal_well_dict = {
+            "well_centroid_x": 100,
+            "well_centroid_y": 101,
+            "confirmed_target_x": 150,
+            "confirmed_target_y": 51,
+        }
+
+        # Let the plate decide how to convert pixels into microns.
+        x_microns, y_microns = crystal_plate_model.compute_drop_location_microns(
+            crystal_well_dict
+        )
+        assert x_microns == int(0.5 + 2.837 * 50)
+        assert y_microns == int(0.5 + 2.837 * -50)
 
     # ----------------------------------------------------------------------------------------
 
     async def __check(
         self,
         dataface,
         filter: CrystalPlateFilterModel,
```

### Comparing `xchembku-1.3.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.4.0/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.3.0/tests/test_crystal_well_droplocation.py` & `xchembku-1.4.0/tests/test_crystal_well_droplocation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import logging
 from typing import Optional
 
 # Base class for the tester.
 from tests.base import Base
 
+# Types which the CrystalPlateObjects factory can use to build an instance.
+from xchembku_api.crystal_plate_objects.constants import (
+    ThingTypes as CrystalPlateThingTypes,
+)
+
 # Client context creator.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 
 # Object managing datafaces.
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 from xchembku_api.models.crystal_well_autolocation_model import (
     CrystalWellAutolocationModel,
 )
 from xchembku_api.models.crystal_well_droplocation_model import (
     CrystalWellDroplocationModel,
 )
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_api.models.crystal_well_model import CrystalWellModel
+from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
 
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
@@ -111,14 +117,19 @@
         # Make a plate for the wells we will create.
         self.__visit = "cm00001-1"
         self.__barcode = "xyzw"
         self.__crystal_plate_model = CrystalPlateModel(
             formulatrix__plate__id=1,
             barcode=self.__barcode,
             visit=self.__visit,
+            thing_type=CrystalPlateThingTypes.SWISS3,
+        )
+
+        self.__crystal_plate_object = CrystalPlateObjects().build_object(
+            {"type": CrystalPlateThingTypes.SWISS3}
         )
 
         # Write plate record.
         await dataface.upsert_crystal_plates(
             [self.__crystal_plate_model],
         )
 
@@ -299,35 +310,38 @@
         filename = "%03d%s.jpg" % (self.__injected_count, letter)
         self.__injected_count += 1
 
         # Create the well object.
         m = CrystalWellModel(
             position="01A_1",
             crystal_plate_uuid=self.__crystal_plate_model.uuid,
+            crystal_plate_thing_type=self.__crystal_plate_model.thing_type,
             filename=filename,
         )
 
         # Write well record.
         await dataface.upsert_crystal_wells([m])
 
         if autolocation:
             # Add a crystal well autolocation.
             ta = CrystalWellAutolocationModel(
                 crystal_well_uuid=m.uuid,
                 number_of_crystals=10,
+                well_centroid_x=100,
+                well_centroid_y=100,
             )
 
             await dataface.originate_crystal_well_autolocations([ta])
 
         if droplocation:
             # Add a crystal well droplocation.
             td = CrystalWellDroplocationModel(
                 crystal_well_uuid=m.uuid,
-                confirmed_target_x=10,
-                confirmed_target_y=11,
+                confirmed_target_x=150,
+                confirmed_target_y=50,
                 is_usable=True,
             )
 
             await dataface.upsert_crystal_well_droplocations([td])
 
         return m
 
@@ -339,21 +353,43 @@
         filter: CrystalWellFilterModel,
         expected: int,
         note: str,
         filename: Optional[str] = None,
     ):
         """ """
 
+        # Get the full crystal well with auto and confirmed drop locations.
         crystal_well_models = await dataface.fetch_crystal_wells_needing_droplocation(
             filter
         )
 
+        # Make sure we got enough.
         assert len(crystal_well_models) == expected, note
 
-        # All wells should belong to the visit.
         for crystal_well_model in crystal_well_models:
+            # All wells should belong to the visit.
             assert crystal_well_model.visit == self.__visit, f"{note} visit"
 
+            # All present confirmed drop locations should be consistent.
+            if (
+                crystal_well_model.well_centroid_x is not None
+                and crystal_well_model.confirmed_target_x is not None
+                and crystal_well_model.well_centroid_y is not None
+                and crystal_well_model.confirmed_target_y is not None
+            ):
+
+                # Use the template plate to predict the microns.
+                (
+                    microns_x,
+                    microns_y,
+                ) = self.__crystal_plate_object.compute_drop_location_microns(
+                    crystal_well_model.dict()
+                )
+                assert crystal_well_model.confirmed_target_x == 150
+                assert crystal_well_model.confirmed_microns_x == microns_x
+                assert crystal_well_model.confirmed_target_y == 50
+                assert crystal_well_model.confirmed_microns_y == microns_y
+
         if filename is not None:
             assert crystal_well_models[0].filename == filename, f"{note} filename"
 
         return crystal_well_models
```

### Comparing `xchembku-1.3.0/tests/test_soakdb3_crystal_well.py` & `xchembku-1.4.0/tests/test_soakdb3_crystal_well.py`

 * *Files identical despite different names*

