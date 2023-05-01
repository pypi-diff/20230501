# Comparing `tmp/autora-workflow-0.2.0.tar.gz` & `tmp/autora-workflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-workflow-0.2.0.tar", last modified: Fri Apr 28 22:15:15 2023, max compression
+gzip compressed data, was "autora-workflow-0.2.1.tar", last modified: Mon May  1 16:03:43 2023, max compression
```

## Comparing `autora-workflow-0.2.0.tar` & `autora-workflow-0.2.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.771377 autora-workflow-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/autora-workflow.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/accessing-state-dependent-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/basic-usage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/controller/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/cli/controller/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/basic-usage/controller.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.783377 autora-workflow-0.2.0/docs/cli/controller/custom-function/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function/func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/global.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000001-PARAMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.775377 autora-workflow-0.2.0/docs/cli/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/regressor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/cli/theorist/basic-usage/variables.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/passing-static-parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/docs/using-alternative-planners-and-executors.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.787377 autora-workflow-0.2.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.779377 autora-workflow-0.2.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/serializer/yaml_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora/workflow/state/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/src/autora/workflow/state/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/src/autora_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:15:15.000000 autora-workflow-0.2.0/src/autora_workflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:15:15.791377 autora-workflow-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-04-28 22:15:01.000000 autora-workflow-0.2.0/tests/test_controller_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/autora-workflow.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.367570 autora-workflow-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/accessing-state-dependent-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/basic-usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/controller/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/basic-usage/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/basic-usage/controller.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function/func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000001-PARAMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/global.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.371570 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/00000001-PARAMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/docs/cli/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/parameters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 16:03:23.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/regressor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/cli/theorist/basic-usage/variables.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/passing-static-parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31206 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/docs/using-alternative-planners-and-executors.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.375570 autora-workflow-0.2.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.363570 autora-workflow-0.2.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/serializer/yaml_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora/workflow/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/src/autora/workflow/state/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/src/autora_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 16:03:43.000000 autora-workflow-0.2.1/src/autora_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:43.379570 autora-workflow-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-01 16:03:24.000000 autora-workflow-0.2.1/tests/test_controller_plots.py
```

### Comparing `autora-workflow-0.2.0/.github/workflows/python-publish.yml` & `autora-workflow-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/.gitignore` & `autora-workflow-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/.idea/autora-workflow.iml` & `autora-workflow-0.2.1/.idea/autora-workflow.iml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/.idea/inspectionProfiles/Project_Default.xml` & `autora-workflow-0.2.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/.idea/runConfigurations/pytest_in_tests.xml` & `autora-workflow-0.2.1/.idea/runConfigurations/pytest_in_tests.xml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/.pre-commit-config.yaml` & `autora-workflow-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/LICENSE.md` & `autora-workflow-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/PKG-INFO` & `autora-workflow-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai/
+Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # AutoRA Workflow
```

### Comparing `autora-workflow-0.2.0/docs/accessing-state-dependent-properties.ipynb` & `autora-workflow-0.2.1/docs/accessing-state-dependent-properties.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/basic-usage.ipynb` & `autora-workflow-0.2.1/docs/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/basic-usage/controller.yml` & `autora-workflow-0.2.1/docs/cli/controller/basic-usage/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function/controller.yml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/controller.yml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/flow.cylc` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/controller.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/environment.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/flow.cylc`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml` & `autora-workflow-0.2.1/docs/cli/controller/custom-function-with-cylc-slurm/history/00000000-METADATA.yaml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/passing-static-parameters.ipynb` & `autora-workflow-0.2.1/docs/passing-static-parameters.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/docs/using-alternative-planners-and-executors.ipynb` & `autora-workflow-0.2.1/docs/using-alternative-planners-and-executors.ipynb`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/mkdocs/base.yml` & `autora-workflow-0.2.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/mkdocs/gen_ref_pages.py` & `autora-workflow-0.2.1/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/pyproject.toml` & `autora-workflow-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
 
 [project.urls]
-homepage = "https://www.empiricalresearch.ai/"
+homepage = "http://www.empiricalresearch.ai/"
 repository = "https://github.com/AutoResearch/autora-workflow"
 documentation = "https://hollandjg.github.io/autora-workflow/"
 
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `autora-workflow-0.2.0/src/autora/workflow/__init__.py` & `autora-workflow-0.2.1/src/autora/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/__main__.py` & `autora-workflow-0.2.1/src/autora/workflow/__main__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/base.py` & `autora-workflow-0.2.1/src/autora/workflow/base.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/controller.py` & `autora-workflow-0.2.1/src/autora/workflow/controller.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/cycle.py` & `autora-workflow-0.2.1/src/autora/workflow/cycle.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/executor.py` & `autora-workflow-0.2.1/src/autora/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/planner.py` & `autora-workflow-0.2.1/src/autora/workflow/planner.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/plotting.py` & `autora-workflow-0.2.1/src/autora/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/protocol.py` & `autora-workflow-0.2.1/src/autora/workflow/protocol.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/serializer/__init__.py` & `autora-workflow-0.2.1/src/autora/workflow/serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/state/history.py` & `autora-workflow-0.2.1/src/autora/workflow/state/history.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/state/param.py` & `autora-workflow-0.2.1/src/autora/workflow/state/param.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora/workflow/state/snapshot.py` & `autora-workflow-0.2.1/src/autora/workflow/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/src/autora_workflow.egg-info/PKG-INFO` & `autora-workflow-0.2.1/src/autora_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autora-workflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Workflow tools for the Autonomous Research Assistant (AutoRA) package.
 Author-email: John Gerrard Holland <john_holland1@brown.edu>
 License: MIT License
-Project-URL: homepage, https://www.empiricalresearch.ai/
+Project-URL: homepage, http://www.empiricalresearch.ai/
 Project-URL: repository, https://github.com/AutoResearch/autora-workflow
 Project-URL: documentation, https://hollandjg.github.io/autora-workflow/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # AutoRA Workflow
```

### Comparing `autora-workflow-0.2.0/src/autora_workflow.egg-info/SOURCES.txt` & `autora-workflow-0.2.1/src/autora_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-workflow-0.2.0/tests/test_controller_plots.py` & `autora-workflow-0.2.1/tests/test_controller_plots.py`

 * *Files identical despite different names*

