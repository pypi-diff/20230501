# Comparing `tmp/cortex_cli-1.13.0.post1.tar.gz` & `tmp/cortex_cli-1.13.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.13.0.post1.tar", last modified: Thu Apr 27 21:05:55 2023, max compression
+gzip compressed data, was "cortex_cli-1.13.0.post2.tar", last modified: Mon May  1 14:57:34 2023, max compression
```

## Comparing `cortex_cli-1.13.0.post1.tar` & `cortex_cli-1.13.0.post2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.13.0.post1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-04-26 17:25:59.000000 cortex_cli-1.13.0.post1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-04-25 18:51:50.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2001 2023-04-26 16:12:30.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24439 2023-04-26 15:26:09.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.0.post1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.0.post1/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-27 21:05:55.000000 cortex_cli-1.13.0.post1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.0.post1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-27 21:05:55.502960 cortex_cli-1.13.0.post1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5211 2023-04-28 14:58:42.000000 cortex_cli-1.13.0.post2/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-05-01 14:57:21.000000 cortex_cli-1.13.0.post2/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-04-27 21:54:12.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-04-28 14:57:33.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24829 2023-05-01 14:57:13.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.0.post2/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post2/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.0.post2/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.0.post2/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-04-27 21:53:57.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.609032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-04-27 21:54:07.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.609032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.0.post2/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-01 14:57:34.000000 cortex_cli-1.13.0.post2/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.0.post2/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-01 14:57:34.619032 cortex_cli-1.13.0.post2/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.0.post2/setup.py
```

### Comparing `cortex_cli-1.13.0.post1/README.md` & `cortex_cli-1.13.0.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <p align="center">
     <img src="https://www.nearlyhuman.ai/wp-content/uploads/2022/04/virtual-copy.svg" width="200"/>
 </p>
 
-# Cortex CLI
+# Nearly Human Cortex CLI
 A simple CLI that abstracts the Cortex API.  The application should reflect all of the Cortex routes, and provide a way
 to interact with models within an approved client.
 
 ## Prerequisites
 - Mamba
 - Create a github token with repo permissions and set the `GH_TOKEN` environment variable
 
 ## Build
 ```
 mamba env create -f ./conda.yml
 
-# Build version of Cortex CLI for release
+# Build version of Nearly Human Cortex CLI for release
 python -m build
 ```
 
 ## Installing the CLI
 ```
 mamba create -n cortex_cli python=3.10 pip -c conda-forge
 mamba activate cortex_cli
```

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/configure.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
         help='The profile to save the configuration under.',
         default=None
     )
 
     _api_url = plumbum.cli.SwitchAttr(
         names=['-u', '--api-url'],
         argtype=str,
-        help='The Cortex API endpoint.',
+        help='The Nearly Human Cortex API endpoint.',
         default=None
     )
 
     _api_key = plumbum.cli.SwitchAttr(
         names=['-k', '--api-key'],
         argtype=str,
-        help='The Cortex API Key to use.',
+        help='The Nearly Human Cortex API Key to use.',
         default=None
     )
 
     def main(self, *args):
         config = ConfigParser(default_section=None)
 
         path = os.path.expanduser('~/.nearlyhuman/config')
```

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/inferences.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/models.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,20 +678,29 @@
 
         return f'Saved the pipeline artifacts to disk: ({self._artifacts_dir})'
 
 
     def _save_environment(self):
         self._info('Packing conda environment...')
 
-        conda_pack.pack(
-            output=f'{self._artifacts_dir}/environment.tar.gz',
-            force=True,
-            verbose=True,
-            ignore_editable_packages=False,
-            ignore_missing_files=True)
+        if 'CORTEX_ENV_PATH' in os.environ:
+            conda_pack.pack(
+                prefix=os.getenv('CORTEX_ENV_PATH'),
+                output=f'{self._artifacts_dir}/environment.tar.gz',
+                force=True,
+                verbose=True,
+                ignore_editable_packages=False,
+                ignore_missing_files=True)
+        else:
+            conda_pack.pack(
+                output=f'{self._artifacts_dir}/environment.tar.gz',
+                force=True,
+                verbose=True,
+                ignore_editable_packages=False,
+                ignore_missing_files=True)
 
         return f'Packed conda environment to disk: ({self._artifacts_dir})'
 
 
     def _upload_pipeline(self):
         self._info('Uploading pipeline artifacts to Cortex...')
```

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.13.0.post2/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.13.0.post2/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ```
 
 ## Modifying the cortex.yml
 The structure of the cortex.yml should be
 ```
 model_class: "{{cookiecutter.__model_class}}"
 model_path: "src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py"
+model_repo: "{{cookiecutter.model_repo}}"
 base_path: "src/{{cookiecutter.__model_name}}/base.py"
 params:
   - gamma: 0.002
 pipeline_steps:
   - download_data: "Download data"
   - transform_data: "Transform data"
   - data_contains_pii_ethics_check: "Data PII ethics check"
```

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ```
 
 ## Modifying the cortex.yml
 The structure of the cortex.yml should be
 ```
 model_class: "{{cookiecutter.__model_class}}"
 model_path: "src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py"
+model_repo: "{{cookiecutter.model_repo}}"
 base_path: "src/{{cookiecutter.__model_name}}/base.py"
 params:
   - gamma: 0.002
 pipeline_steps:
   - download_data: "Download data"
   - transform_data: "Transform data"
   - data_contains_pii_ethics_check: "Data PII ethics check"
```

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.0.post2/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.13.0.post2/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.13.0.post2/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.13.0.post2/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0.post1/setup.py` & `cortex_cli-1.13.0.post2/setup.py`

 * *Files identical despite different names*

