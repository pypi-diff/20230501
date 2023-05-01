# Comparing `tmp/lmql-0.0.5.1.tar.gz` & `tmp/lmql-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.5.1.tar", last modified: Wed Apr 19 15:29:32 2023, max compression
+gzip compressed data, was "lmql-0.0.6.tar", last modified: Mon May  1 11:40:54 2023, max compression
```

## Comparing `lmql-0.0.5.1.tar` & `lmql-0.0.6.tar`

### file list

```diff
@@ -1,231 +1,241 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.747986 lmql-0.0.5.1/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1618 2023-04-17 14:48:56.000000 lmql-0.0.5.1/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2733 2023-04-19 15:28:18.000000 lmql-0.0.5.1/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5.1/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.5.1/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4646 2023-04-19 15:29:32.767986 lmql-0.0.5.1/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4215 2023-04-18 06:55:18.000000 lmql-0.0.5.1/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.5.1/TODO.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.5.1/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.747986 lmql-0.0.5.1/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5777 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/_templates/layout.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2709 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     6564 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.5.1/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1078 2023-04-18 06:55:18.000000 lmql-0.0.5.1/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.5.1/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.5.1/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.5.1/pyproject.toml
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.5.1/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.5.1/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.5.1/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.5.1/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.5.1/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.5.1/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      828 2023-04-19 15:29:32.771986 lmql-0.0.5.1/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.5.1/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.751986 lmql-0.0.5.1/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6807 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/__init__.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     7529 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21177 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/model/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/model/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/async_generation_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/model/local_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17924 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8387 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/model/served_model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7565 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    39794 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18121 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1972 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    25946 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    17000 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/bopenai/openai_api.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      467 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18632 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27495 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    29933 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    20646 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/dclib/trie_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/hf_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    27896 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6076 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    43100 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8563 2023-04-19 15:28:18.000000 lmql-0.0.5.1/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5011 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/expr_test_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/str_in_str_tests.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2149 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/tests/test_sample_queries.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/tests/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3256 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.759986 lmql-0.0.5.1/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.763986 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.763986 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    68636 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    20848 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.767986 lmql-0.0.5.1/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.5.1/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1882 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-04-19 15:29:27.000000 lmql-0.0.5.1/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-04-19 15:29:32.755986 lmql-0.0.5.1/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4646 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     6409 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-04-19 15:29:32.000000 lmql-0.0.5.1/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.5.1/src/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.527314 lmql-0.0.6/.github/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.531314 lmql-0.0.6/.github/workflows/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1594 2023-05-01 11:40:25.000000 lmql-0.0.6/.github/workflows/lmql-web.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-01 11:40:25.000000 lmql-0.0.6/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6/MANIFEST.in
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4949 2023-05-01 11:40:54.571313 lmql-0.0.6/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4520 2023-05-01 11:40:25.000000 lmql-0.0.6/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)       75 2023-04-17 14:44:31.000000 lmql-0.0.6/TODO.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.531314 lmql-0.0.6/docs/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/Makefile
+-rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6/docs/RELEASE.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/make.bat
+-rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_ext/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5526 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_ext/lmql_snippets.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.527314 lmql-0.0.6/docs/source/_static/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/css/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-04-20 08:07:08.000000 lmql-0.0.6/docs/source/_static/css/lmql-docs.css
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/images/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_static/images/lmql.svg
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_static/js/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2191 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_static/js/lmql-playground.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/_templates/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/_templates/layout.html
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/blog/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-01 11:40:25.000000 lmql-0.0.6/docs/source/blog/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-01 11:40:25.000000 lmql-0.0.6/docs/source/blog/release-0.0.6.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/conf.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/dev-setup.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2762 2023-04-30 16:34:02.000000 lmql-0.0.6/docs/source/index.rst
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2484 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/installation.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.535314 lmql-0.0.6/docs/source/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/language/constraints.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/language/decoders.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/language/functions.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6564 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/models.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/overview.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/language/scripted_prompts.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/logo.png
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/docs/source/python/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/python/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10831 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/python/langchain.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-04-30 16:34:02.000000 lmql-0.0.6/docs/source/python/llama_index.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/python/lmql.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-04-20 08:07:08.000000 lmql-0.0.6/docs/source/python/pandas.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-04-19 15:28:18.000000 lmql-0.0.6/docs/source/python/python.ipynb
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/source/quickstart.md
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/docs/source/releases/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1078 2023-04-18 06:55:18.000000 lmql-0.0.6/docs/source/releases/misc-snippets.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6/docs/source/releases/release-0.0.5.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6/docs/todo.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6/pyproject.toml
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-04-17 14:44:31.000000 lmql-0.0.6/requirements.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/scripts/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6/scripts/activate-dev.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/scripts/conda/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      210 2023-04-19 15:28:18.000000 lmql-0.0.6/scripts/conda/requirements-no-gpu.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      344 2023-04-19 15:28:18.000000 lmql-0.0.6/scripts/conda/requirements.yml
+-rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6/scripts/pypi-release.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6/scripts/wheel.sh
+-rw-rw-r--   0 luca      (1000) luca      (1000)      826 2023-05-01 11:40:54.571313 lmql-0.0.6/setup.cfg
+-rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-03-14 15:27:49.000000 lmql-0.0.6/setup.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/lmql/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7077 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/__init__.py
+-rwxrwxr-x   0 luca      (1000) luca      (1000)     8087 2023-04-25 07:30:01.000000 lmql-0.0.6/src/lmql/cli.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/demo.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/http.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/language/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21491 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/language/compiler.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/language/fragment_parser.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      979 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/qstrings.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/language/validator.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/model/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/model/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    24468 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/model/async_generation_utils.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1299 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/model/local_client.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18118 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/model/serve.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8413 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/model/served_model.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/ops/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ops/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ops/follow_map.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    39435 2023-04-30 16:34:02.000000 lmql-0.0.6/src/lmql/ops/ops.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21044 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ops/token_set.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.543314 lmql-0.0.6/src/lmql/runtime/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/bopenai/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    27642 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/batched_openai.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    17239 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/bopenai/openai_api.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/dclib/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    18631 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_array.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    26024 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      538 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_global.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21668 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_model.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    30560 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/dclib_seq.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    20722 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/dclib/decoders.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4144 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/dclib/trie_cache.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3176 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/hf_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    34088 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/interpreter.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/interrupt.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1084 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/langchain.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6124 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/lmql_runtime.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1186 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/maiohttp.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/masks.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      732 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/runtime/model_registry.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5835 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/multi_head_interpretation.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)    47425 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/openai_integration.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/openai_secret.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2437 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/output_writer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/runtime/postprocessing/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3530 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/postprocessing/group_by.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1980 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/program_state.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/runtime/stats.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9327 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/runtime/tokenizer.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/tests/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5188 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/expr_test_utils.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/outdated/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/mask_product_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/monotonicity.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/one_of_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/sentences_op.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/stops_at.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/test_multi_head.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/outdated/token_set_test.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/tests/system/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/tests/system/basic_use_cases.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      971 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/tail_token_set.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2481 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/tests/test_sample_queries.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/ui/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/__init__.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.547314 lmql-0.0.6/src/lmql/ui/live/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/live/live.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3340 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/live/live.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/live/livelib.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/package.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/live/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.551313 lmql-0.0.6/src/lmql/ui/playground/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.dockerignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.env
+-rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/.gitignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/Dockerfile
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.551313 lmql-0.0.6/src/lmql/ui/playground/public/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/_headers
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/favicon.ico
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/index.html
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/lmql.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/manifest.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.563313 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5221 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/list.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/public/robots.txt
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.563313 lmql-0.0.6/src/lmql/ui/playground/public/snippets/
+-rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)   252806 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/ref.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/run-in-docker.sh
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.567313 lmql-0.0.6/src/lmql/ui/playground/src/
+-rw-rw-r--   0 luca      (1000) luca      (1000)    69215 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/playground/src/App.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/App.test.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/Configuration.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/DataListView.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)    21284 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/DecodingTree.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/Embed.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/Explore.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/SharedState.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3868 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/State.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5763 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/browser_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/build_info.js
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.567313 lmql-0.0.6/src/lmql/ui/playground/src/editor/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/editor/theme.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/explore.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/graph-layout.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/index.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/index.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/logo.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     8104 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/playground/src/queries.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/remote_process.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/screenshot.css
+-rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/setupTests.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/ui/playground/src/spinner.svg
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2949 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/playground/yarn.lock
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.gitattributes
+-rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.gitignore
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/.vscode/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.vscode/launch.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/.vscodeignore
+-rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/LICENSE
+-rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/README.md
+-rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/language-configuration.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/lmql-vscode.png
+-rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/ui/vscode/package.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/
+-rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.571313 lmql-0.0.6/src/lmql/utils/
+-rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6/src/lmql/utils/__init__.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     5384 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql/utils/graph.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-01 11:40:25.000000 lmql-0.0.6/src/lmql/utils/nputil.py
+-rw-rw-r--   0 luca      (1000) luca      (1000)      113 2023-05-01 11:40:49.000000 lmql-0.0.6/src/lmql/version.py
+drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-05-01 11:40:54.539314 lmql-0.0.6/src/lmql.egg-info/
+-rw-rw-r--   0 luca      (1000) luca      (1000)     4949 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/PKG-INFO
+-rw-rw-r--   0 luca      (1000) luca      (1000)     6764 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/SOURCES.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/dependency_links.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/entry_points.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/requires.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-05-01 11:40:54.000000 lmql-0.0.6/src/lmql.egg-info/top_level.txt
+-rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6/src/lmql.svg
```

### Comparing `lmql-0.0.5.1/.github/workflows/lmql-web.yml` & `lmql-0.0.6/.github/workflows/lmql-web.yml`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,24 @@
     - name: Clean permissions
       # You may pin to the exact commit or the version.
       # uses: main-quest/actions.clean-permissions@c8603ac2fddde3426082da840e0baff43a6505af
       uses: main-quest/actions.clean-permissions@v1.0.4
     - uses: actions/upload-artifact@v1
       with:
         name: DocumentationHTML
-        path: docs/build/html/doc-snippets
+        path: docs/build/html/
     - name: Prepare Node.js environment
       uses: actions/setup-node@v3
       with:
         node-version: 19.x
     - uses: actions/download-artifact@v3
       name: Restore docs/build/html
       with:
         name: DocumentationHTML
-        path: docs/build/html/doc-snippets
+        path: docs/build/html/
     - name: Build web/ and In-Browser LMQL Distribution
       run: cd web && bash deploy.sh
     
     - name: Deploy to web branch
       uses: JamesIves/github-pages-deploy-action@v4
       with:
         folder: web-deploy
```

### Comparing `lmql-0.0.5.1/.gitignore` & `lmql-0.0.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -168,7 +168,9 @@
 cython_debug/
 
 # End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks
 
 wip-snippets
 .vscode
 .lmql-algorithms-cache
+
+*.tokens
```

### Comparing `lmql-0.0.5.1/LICENSE` & `lmql-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/PKG-INFO` & `lmql-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.5.1
+Version: 0.0.6
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,16 @@
     <a href="https://lmql.ai">Explore Examples</a>
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
+    <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.5.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
           A query language for programming (large) language models.
                                Documentation_Â»
 
                Explore_Examples Â· Playground_IDE Â· Report_Bug
 
+                       [https://img.shields.io/discord/
+1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white]
+                                [PyPI_version]
 LMQL is a query language for large language models (LLMs). It facilitates LLM
 interaction by combining the benefits of natural language prompting with the
 expressiveness of Python. With only a few lines of LMQL code, users can express
 advanced, multi-part and tool-augmented LM queries, which then are optimized by
 the LMQL runtime to run efficiently as part of the LM decoding loop. ![lmql-
 overview](https://user-images.githubusercontent.com/17903049/222918379-
 84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

### Comparing `lmql-0.0.5.1/README.md` & `lmql-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     <a href="https://lmql.ai">Explore Examples</a>
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
+    <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
                                     [Logo]
                                 **** LMQL ****
           A query language for programming (large) language models.
                                Documentation_Â»
 
                Explore_Examples Â· Playground_IDE Â· Report_Bug
 
+                       [https://img.shields.io/discord/
+1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white]
+                                [PyPI_version]
 LMQL is a query language for large language models (LLMs). It facilitates LLM
 interaction by combining the benefits of natural language prompting with the
 expressiveness of Python. With only a few lines of LMQL code, users can express
 advanced, multi-part and tool-augmented LM queries, which then are optimized by
 the LMQL runtime to run efficiently as part of the LM decoding loop. ![lmql-
 overview](https://user-images.githubusercontent.com/17903049/222918379-
 84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

### Comparing `lmql-0.0.5.1/docs/Makefile` & `lmql-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/make.bat` & `lmql-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6/docs/source/_ext/lmql_snippets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6/docs/source/_static/css/lmql-docs.css`

 * *Files 2% similar despite different names*

```diff
@@ -270,8 +270,15 @@
 .val3 {
     background-color: rgb(130, 140, 249) !important;
     cursor: default;
 }
 
 .val3:hover, .val3.hover, .val3-hover .val3 {
     background-color: rgba(107, 119, 255, 1.0) !important;
+}
+
+.dataframe th {
+    width: 120pt !important;
+}
+.dataframe th:first-child {
+    width: auto !important;
 }
```

### Comparing `lmql-0.0.5.1/docs/source/_static/images/lmql.svg` & `lmql-0.0.6/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6/docs/source/_static/js/lmql-playground.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/conf.py` & `lmql-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/dev-setup.md` & `lmql-0.0.6/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/index.rst` & `lmql-0.0.6/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,16 @@
    
 .. toctree::
     :maxdepth: 1
     :caption: 🔗 Python Integration
     
     python/python.ipynb
     python/langchain.ipynb
+    python/llama_index.ipynb
+    python/pandas.ipynb
    
 .. toctree::
     :maxdepth: 1
     :caption: 💬 Contribute
     
     dev-setup
     Discord <https://discord.gg/7eJP4fcyNT>
```

#### html2text {}

```diff
@@ -20,12 +20,12 @@
 ð¬_Discord_Server ð¥_Twitter âï¸_E-Mail
 Contents -------- .. toctree:: :maxdepth: 1 quickstart installation â¡ï¸
 Playground IDE
 lmql.ai/playground> .. toctree:: :maxdepth: 1 :caption: ð LMQL Language
 language/overview.md language/scripted_prompts.md language/constraints.md
 language/decoders.md language/models.md language/functions.md .. toctree:: :
 maxdepth: 1 :caption: ð Python Integration python/python.ipynb python/
-langchain.ipynb .. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup
-Discord
+langchain.ipynb python/llama_index.ipynb python/pandas.ipynb .. toctree:: :
+maxdepth: 1 :caption: ð¬ Contribute dev-setup Discord
 discord.gg/7eJP4fcyNT> GitHub Issues
 github.com/eth-sri/lmql/issues> E-Mail
 lmql.ai>
```

### Comparing `lmql-0.0.5.1/docs/source/installation.md` & `lmql-0.0.6/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/constraints.md` & `lmql-0.0.6/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/decoders.md` & `lmql-0.0.6/docs/source/language/decoders.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/functions.md` & `lmql-0.0.6/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/models.md` & `lmql-0.0.6/docs/source/language/models.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/overview.md` & `lmql-0.0.6/docs/source/language/overview.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/language/scripted_prompts.md` & `lmql-0.0.6/docs/source/language/scripted_prompts.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/lmql.svg` & `lmql-0.0.6/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/logo.png` & `lmql-0.0.6/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/python/langchain.ipynb` & `lmql-0.0.6/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/python/lmql.txt` & `lmql-0.0.6/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/python/python.ipynb` & `lmql-0.0.6/docs/source/python/python.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/quickstart.md` & `lmql-0.0.6/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/docs/source/releases/misc-snippets.md` & `lmql-0.0.6/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/scripts/wheel.sh` & `lmql-0.0.6/scripts/wheel.sh`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/setup.cfg` & `lmql-0.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.5.1
+version = 0.0.6
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.5.1/src/lmql/__init__.py` & `lmql-0.0.6/src/lmql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,8 +183,15 @@
     for a in argnames:
         if a not in args_of_query:
             print(f"warning: @lmql.query {fct.__name__} has an argument '{a}' that is not used in the query.")
     
     # set the function context of the query based on the function context of the decorated function
     module.query.function_context = FunctionContext(argnames, args_of_query, scope)
     
-    return module.query
+    return module.query
+
+async def static_prompt(query_fct, *args, **kwargs):
+    """
+    Returns the static prompt prefix that is generated by the given query function up until the first variable.
+    """
+    res = await query_fct(*args, **kwargs, return_prompt_string=True)
+    return res[0]
```

### Comparing `lmql-0.0.5.1/src/lmql/cli.py` & `lmql-0.0.6/src/lmql/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,19 @@
     absolute_path = os.path.abspath(args.lmql_file)
     from lmql.runtime.output_writer import PrintingDebuggerOutputWriter
 
     writer = PrintingDebuggerOutputWriter()
     writer.clear = not args.no_clear
     writer.print_output = not args.no_realtime
 
-    results = asyncio.run(lmql.run_file(absolute_path, output_writer=writer))
+    if os.path.exists(absolute_path):
+        results = asyncio.run(lmql.run_file(absolute_path, output_writer=writer))
+    else:
+        code = args.lmql_file
+        results = asyncio.run(lmql.run(code, output_writer=writer))
     
     if type(results) is not list:
         results = [results]
     
     for r in results:
         if isinstance(r, LMQLResult):
             for v in [v for v in r.variables if v.startswith("P(")]:
@@ -155,25 +159,35 @@
         print(f"  commit: {version_info.commit}")
     print(f"  path: {project_root}/lmql")
     if version_info.build_on != "dev":
         print(f"  build on: {version_info.build_on}")
 
 def hello():
     import asyncio
-    code_local = """
-argmax "Hello[WHO]" from "local:gpt2-medium" where len(WHO) < 10    
-"""
-    print("[Greeting 🤗 Transformers]")
-    asyncio.run(lmql.run(code_local, output_writer=lmql.printing))
-    
-    print("[Greeting OpenAI]")
-    code_openai = """
-argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
-"""
-    asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
+    backend = None
+    # check for additional arg
+    if len(sys.argv) > 2:
+        backend = sys.argv[2]
+        if backend not in ["hf", "openai"]:
+            print("Invalid backend, please specify one of {}".format(", ".join(["hf", "openai"])))
+            sys.exit(1)
+    
+    if backend is None or backend == "hf":
+        code_local = """
+    argmax "Hello[WHO]" from "local:gpt2-medium" where len(WHO) < 10    
+    """
+        print("[Greeting 🤗 Transformers]")
+        asyncio.run(lmql.run(code_local, output_writer=lmql.printing))
+    
+    if backend is None or backend == "openai":
+        print("[Greeting OpenAI]")
+        code_openai = """
+    argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
+    """
+        asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
 
 hidden_commands = {
     "hello": hello
 }
 
 def main():
     if len(sys.argv) < 2:
```

### Comparing `lmql-0.0.5.1/src/lmql/demo.py` & `lmql-0.0.6/src/lmql/demo.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/http.py` & `lmql-0.0.6/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/language/compiler.py` & `lmql-0.0.6/src/lmql/language/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 from lmql.ops.ops import lmql_operation_registry
 
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable
 from lmql.language.validator import LMQLValidator, LMQLValidationError
 from lmql.language.fragment_parser import LMQLDecoderConfiguration, LMQLQuery, LanguageFragmentParser, FragmentParserError
 from lmql.runtime.model_registry import model_name_aliases
 import lmql.runtime.lmql_runtime as lmql_runtime
+from lmql.runtime.dclib import get_all_decoders
 
 OPS_NAMESPACE = "lmql.ops"
 
 class FreeVarCollector(ast.NodeVisitor):
-    def __init__(self, free_vars):
+    def __init__(self, free_vars, exclude=None):
         self.free_vars = free_vars
+        self.exclude = exclude or set()
 
     def visit_Name(self, node):
         if type(node.ctx) is ast.Load:
+            if node.id in self.exclude:
+                return
             self.free_vars.add(node.id)
 
 class PromptScope(ast.NodeVisitor):
     def scope(self, query: LMQLQuery):
         self.distribution_vars = set([query.distribution.variable_name]) if query.distribution is not None else set()    
         self.defined_vars = set()
 
@@ -37,15 +41,17 @@
         
         # also collect variable reads from where clause
         if query.where is not None:
             FreeVarCollector(self.free_vars).visit(query.where)
         if query.from_ast is not None:
             FreeVarCollector(self.free_vars).visit(query.from_ast)
         if query.decode is not None:
-            FreeVarCollector(self.free_vars).visit(query.decode)
+            FreeVarCollector(self.free_vars, exclude=get_all_decoders()).visit(query.decode)
+        if query.distribution is not None:
+            FreeVarCollector(self.free_vars).visit(query.distribution.values)
 
         query.scope = self
 
     def visit_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
```

### Comparing `lmql-0.0.5.1/src/lmql/language/fragment_parser.py` & `lmql-0.0.6/src/lmql/language/fragment_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/language/qstrings.py` & `lmql-0.0.6/src/lmql/language/qstrings.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/language/validator.py` & `lmql-0.0.6/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/model/async_generation_utils.py` & `lmql-0.0.6/src/lmql/model/async_generation_utils.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/model/local_client.py` & `lmql-0.0.6/src/lmql/model/local_client.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/model/serve.py` & `lmql-0.0.6/src/lmql/model/serve.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,26 +169,27 @@
             throughput,
             self.request_count, 
             self.state.queue.qsize(), 
             ", ".join(gpu_usage)), end="\r")
 
     def run(self):
         dtype = self.state.dtype
+        load_in_8bit = dtype == "8bit"
         if dtype == "float16":
             dtype = torch.float16
         else:
             dtype = None
         
         # load model
         if not self.cuda:
             print("Loading {} (CPU)".format(self.model_identifier))
             self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True)
         else:
             print("Loading {} (Multi-GPU)".format(self.model_identifier))
-            self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True, device_map="auto")
+            self.model = AutoModelForCausalLM.from_pretrained(self.model_identifier, torch_dtype=dtype, resume_download=True, load_in_8bit=load_in_8bit, device_map="auto")
         self.model.eval()
         
         print("Ready!".format(self.model_identifier))
 
         if self.ready_event:
             self.ready_event.set()
 
@@ -447,15 +448,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("model", type=str)
     parser.add_argument("--tokenizer", type=str, default=None)
     parser.add_argument("--port", type=int, default=8080)
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--cuda", action="store_true", default=False)
     parser.add_argument("--cache", type=str, default=None)
-    parser.add_argument("--dtype", type=str, default="none")
+    parser.add_argument("--dtype", type=str, default="none", help="What format to load the model weights. Options: 'float16' (not available on all models), '8bit' (requires bitsandbytes)")
     parser.add_argument("--wait_until_ready", action="store_true", default=False, help="Whether the server should start only after the model and tokenizer have been loaded.")
     parser.add_argument("--num-tokenizer-processes", type=int, default=2, dest="num_tokenizer_processes")
     
     args = parser.parse_args()
     
     manager = multiprocessing.Manager()
```

### Comparing `lmql-0.0.5.1/src/lmql/model/served_model.py` & `lmql-0.0.6/src/lmql/model/served_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,16 @@
         self.num_queries = 0
 
     def forward(self, input_ids, attention_mask=None):
         assert input_ids.numel() > 0, "input_ids must not be empty"
         # keep stats
         num_input_tokens = sum(len(x) for x in input_ids)
         self.consumed_tokens = self.consumed_tokens + num_input_tokens
-        
+        self.billable_tokens += 1
+
         assert input_ids.dtype == torch.long, "input_ids must be of dtype torch.long"
         # count prompt tokens + 1 generated output token per sequence
         
         # use local client if hosted in process
         if self.local_client is not None:
             return self.local_client.forward(input_ids, attention_mask)
```

### Comparing `lmql-0.0.5.1/src/lmql/ops/follow_map.py` & `lmql-0.0.6/src/lmql/ops/follow_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,20 +65,20 @@
         """
 
         fm = FollowMap()
         handled = tset()
 
         for p2, component in self.components:
             assert handled != "*", "Cannot intersect further patterns if '*' has already been handled."
-            
+        
             p1 = setminus(p1, handled)
             # p2 = setminus(p2, handled)
-            # print("intersect", p1, "and", p2, end="  ")
+            # print("intersect", p1, "and", p2)
             intersected_pattern = intersect(p1, p2)
-            # print(" gives", intersected_pattern, end=" ")
+            # print(" gives", intersected_pattern)
             intersected_pattern = setminus(intersected_pattern, handled)
             # print("minus", handled, " ", intersected_pattern)
 
             # empty patterns can be skipped
             if intersected_pattern == "∅": continue
 
             fm.components.append((intersected_pattern, component))
```

### Comparing `lmql-0.0.5.1/src/lmql/ops/ops.py` & `lmql-0.0.6/src/lmql/ops/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,25 +344,16 @@
             v = str(v)
             assert type(v) is str, "len() can only be applied to strings, lists, or tuples"
             if NextToken not in v:
                 return len(v)
             v = strip_next_token(v)
             
             len_masks = []
-            all = "∅"
-            l = 1
-            while True:
-                tmask = tset(charlen=l)
-                all = tmask.union(all)
-                # if 'all' encompasses all possible tokens, then we have enumerated all possible lengths
-                if len(all) == VocabularyMatcher.instance().vocab_size:
-                    break
-                if len(tmask) > 0:
-                    len_masks.append((tmask, len(v) + l))
-                l += 1
+            for l,tmask in charlen_tsets().items():
+                len_masks.append((tmask, len(v) + l))
             
             return fmap(*len_masks)
 
     def final(self, x, operands=None, result=None, **kwargs):
         return x[0]
 
 class NotOp(Node):
@@ -949,15 +940,15 @@
         
         return 0 # other constraints cannot be compared
 
 @LMQLOp(["STOPS_BEFORE", "stops_before"])
 class StopBeforeOp(StopAtOp):
     def postprocess(self, operands, value):
         op2 = operands[1]
-        matched_phrase_index = value.rfind(op2)
+        matched_phrase_index = value.find(op2)
         if matched_phrase_index != -1:
             value = value[:matched_phrase_index]
 
         return postprocessed_rewrite(value), postprocessed_value(value)
 
 class OpaqueLambdaOp(Node):
     def forward(self, *args, **kwargs):
```

### Comparing `lmql-0.0.5.1/src/lmql/ops/token_set.py` & `lmql-0.0.6/src/lmql/ops/token_set.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,15 @@
 from typing import Iterable, Tuple
 from itertools import product
 
 from lmql.utils import nputil
 import numpy as np
 from lmql.runtime.stats import Stats
 
-def get_vocab(tokenizer):
-    if hasattr(tokenizer, "vocab"):
-        return tokenizer.vocab
-    elif hasattr(tokenizer, "get_vocab"):
-        return tokenizer.get_vocab()
-    elif hasattr(tokenizer, "tokenizer_impl"):
-        return get_vocab(tokenizer.tokenizer_impl)
-    else:
-        assert False, "Could not obtain full vocabulary from unknown tokenizer type: {}".format(type(tokenizer))
+from lmql.runtime.tokenizer import get_vocab
 
 class VocabularyMatcher:
     """
     Generates sub-token level logit masks from provided tokens.
     """
     def __init__(self, tokenizer, model_identifier):
         self.tokenizer = tokenizer
@@ -111,18 +103,14 @@
             raise Exception("VocabularyMatcher not initialized.")
         return VocabularyMatcher._instance
 
     @staticmethod
     def ensure_ready():
         VocabularyMatcher.instance()
 
-    @property
-    def vocab_size(self):
-        return len(self.vocab)
-
     @staticmethod
     def with_cache(keys, provider):
         keys = [k for k in keys if k is not None]
         for k in keys:
             if k in VocabularyMatcher.cache.keys():
                 return VocabularyMatcher.cache[k]
         else:
@@ -173,14 +161,18 @@
         pattern = re.compile(regex, re.UNICODE)
         for id, subtoken in self.vocab.items():
             if pattern.match(subtoken) is not None:
                 mask[id] = True
 
         return mask
 
+    @property
+    def vocab_size(self):
+        return self.tokenizer.vocab_size
+
     def _make_mask_from_char_length(self, length):
         if self.token_lengths is None:
             token_lengths = np.zeros([self.vocab_size], dtype=np.int32)
             for id, subtoken in self.vocab.items():
                 token_lengths[id] = len(subtoken)
             self.token_lengths = token_lengths
         
@@ -245,67 +237,132 @@
         for i in mask.reshape(-1).nonzero()[0]:
             if len(tokens) > 5 and not full:
                 truncated = True
                 break
             if i == self.eos_token_id:
                 tokens.append("eos")
             else:
+                # invalid token
+                if not i in self.vocab:
+                    continue
+
                 s = self.vocab[i]
                 # replace nl and space
                 s = self.tokenizer.convert_tokens_to_string([s])
                 s = s.encode("unicode_escape").decode("utf-8")
                 tokens.append(tstr(s))
 
         return prefix + "{{{}}}".format(
             ", ".join([t for t in sorted(list(tokens))]) + ("..." if truncated else "")
         )
 
 VocabularyMatcher._instance = None
 VocabularyMatcher.cache = {}
 
+def has_tail(mask):
+    if mask is None: return False
+    if type(mask) is str: return False
+    assert type(mask) is TokenSet
+    return mask.tail is not None
 class TokenSetConcrete:
-    def __init__(self, tokens=None, minus=False, mask=None, regex=None, prefix=False, exact=False, charlen=None, name=None):
+    def __init__(self, tokens=None, minus=False, mask=None, regex=None, prefix=False, exact=False, charlen=None, name=None, tail=None):
         VocabularyMatcher.ensure_ready()
 
         if mask is not None:
             self.mask = mask.copy()
         else: 
             self.mask = VocabularyMatcher.instance().make_mask(tokens=tokens, regex=regex, minus=minus, prefix=prefix, exact=exact, charlen=charlen, name=name)
 
         self._token_str = None
         # for TokenSetSymbolic compatibility
         self.minusset = False
 
+        # long tail, if mask models deterministic token sequence
+        self.tail = tail
+
+        # if we in a deterministic long-tailed mask, extract the full tail
+        if self.tail is None and prefix and self.mask.sum() == 1 and tokens is not None and len(tokens) == 1:
+            tail_str = list(tokens)[0]
+            # deterministic_next_id = self.mask.nonzero()[0][0]
+            # deterministic_next_subtoken_str = VocabularyMatcher.instance().tokenizer.decode([deterministic_next_id])
+            # if len(tail_str) > len(deterministic_next_subtoken_str):
+            self.tail = tail_str
+
+    def merge_tail(self, mask, other):
+        """
+        Check which of the self.tail and other.tail are still valid under 'mask' and 
+        returns the merged tail. If no tail is valid, returns None.
+        """
+
+        # tails are only defined for deterministic masks
+        if mask.sum() != 1:
+            return None
+        deterministic_id = mask.nonzero()[0][0]
+
+        # check which of self.tail and other.tail are still valid under 'mask'
+        available_tails = []
+        for m,t in [(self.mask, self.tail), (other.mask, other.tail)]:
+            if t is None: 
+                continue
+            if m[deterministic_id]: 
+                available_tails.append(t)
+        
+        if len(available_tails) == 0: 
+            return None
+        elif len(available_tails) == 1: 
+            return available_tails[0]
+        else:
+            assert len(available_tails) == 2
+            if available_tails[0] != available_tails[1]:
+                # find common tail
+                for i in range(min(len(available_tails[0]), len(available_tails[1]))):
+                    if available_tails[0][i] != available_tails[1][i]:
+                        break
+                tail_str = available_tails[0][:i]
+                if len(tail_str) == 0: return None
+
+                deterministic_next_id = self.mask.nonzero()[0][0]
+                deterministic_next_subtoken_str = VocabularyMatcher.instance().tokenizer.decode([deterministic_next_id])
+                if len(tail_str) <= len(deterministic_next_subtoken_str):
+                    return None
+                else: 
+                    return tail_str
+            return available_tails[0]
+
     def union(self, other):
         if other == "∅": 
-            return TokenSetConcrete(mask=self.mask)
+            return TokenSetConcrete(mask=self.mask, tail=self.merge_tail(self.mask, other))
         if other == "*": 
             return "*"
 
         assert type(other) is TokenSetConcrete, "Can only union over two TokenSetConcrete."
 
-        return TokenSetConcrete(mask=np.logical_or(self.mask, other.mask))
+        mask = np.logical_or(self.mask, other.mask)
+        return TokenSetConcrete(mask=mask, tail=self.merge_tail(mask, other))
 
     def intersect(self, other):
         if other == "∅": return "∅"
         if other == "*": return self
 
         assert type(other) is TokenSetConcrete, "Can only intersect two TokenSetConcrete."
 
-        return TokenSetConcrete(mask=np.logical_and(self.mask, other.mask))
+
+        mask = np.logical_and(self.mask, other.mask)
+        return TokenSetConcrete(mask=mask, tail=self.merge_tail(mask, other))
      
     def setminus(self, other):
         if other == "*": 
             return "∅"
         if other == "∅":
             return TokenSetConcrete(mask=self.mask)
         
         assert type(other) is TokenSetConcrete, "Can only setminus two TokenSetConcrete."
 
-        return TokenSetConcrete(mask=np.logical_and(self.mask, np.logical_not(other.mask)))
+        mask = np.logical_and(self.mask, np.logical_not(other.mask))
+        return TokenSetConcrete(mask=mask, tail=self.merge_tail(mask, other))
     
 
     def starts_with(self, s):
         if s in self.tokens: 
             return not self.minusset # returns True if not minusset and s in self.tokens
         else:
             for s in self.tokens:
@@ -320,14 +377,17 @@
         return str(self)
 
     def __str__(self, full=False):
         if self._token_str is not None:
             return self._token_str
 
         self._token_str = VocabularyMatcher.instance().str(self.mask, full=full)
+
+        if self.tail is not None:
+            self._token_str += f" ⤖ '{self.tail}'"
         
         return self._token_str
 
     def __eq__(self, other):
         if other == "∅": 
             if self.mask.sum() == 0: 
                 return True
@@ -335,15 +395,15 @@
         if other == "*": 
             if self.mask.sum() == self.mask.shape[0]: 
                 return True
             return False
 
         assert type(other) is TokenSetConcrete, "Can only compare (==) two TokenSets."
 
-        return np.all(self.mask == other.mask)
+        return np.all(self.mask == other.mask) and self.tail == other.tail
 TokenSetConcrete.cache = {}
 
 class TokenSetSymbolic:
     def __init__(self, tokens=None, minus=False):
         assert token_set_vocabulary is not None, "TokenSetConcrete: token_set_vocabulary must be set before any TokenSets are instantiated."
 
         if tokens is None: tokens = set()
@@ -479,14 +539,22 @@
     if regex:
         assert len(tokens) == 1, "cannot create a TokenSet from multiple regexes."
         return TokenSet(regex=tokens[0], name=name)
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=False, name=name)
     return TokenSet(set(tokens), minus=False, prefix=prefix, exact=exact, name=name)
 
+def charlen_tsets():
+    l1 = tset(charlen=1)
+    token_lengths = VocabularyMatcher.instance().token_lengths
+    assert token_lengths is not None, "VocabularyMatcher.instance().token_lengths is None even though it should be fully initialized."
+    # get unique values in token_lengths (numpy)
+    length_values = np.unique(token_lengths)
+    return {l: tset(charlen=l) for l in length_values}
+
 def ntset(*tokens):
     if len(tokens) == 1 and type(tokens[0]) is set:
         return TokenSet(set(list(tokens[0])), minus=True)
     return TokenSet(set(tokens), minus=True)
 
 class ArgTuple(tuple): 
     def __repr__(self) -> str:
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6/src/lmql/runtime/bopenai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 
 def get_stats():
     global _api
     if _api is None:
         _api = AsyncOpenAIAPI()
     return _api.stats
 
+def reset_latency_stats():
+    global _api
+    if _api is None:
+        _api = AsyncOpenAIAPI()
+    _api.reset_latency_stats()
+
+def get_first_token_latency():
+    global _api
+    if _api is None:
+        _api = AsyncOpenAIAPI()
+    return _api.first_token_latency
 class AsyncConfiguration:
     @staticmethod
     def set_batch_size(bs):
         global _api
         if _api is None:
             _api = AsyncOpenAIAPI()
         _api.batch_size = bs
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 logit_bias_logging = True
 
 def set_logit_bias_logging(value):
     global logit_bias_logging
     logit_bias_logging = value
 
 class EmptyStreamError(Exception): pass
-
 class ChaosException(openai.APIError): pass
+class APIShutDownException(RuntimeError): pass
 class MaximumRetriesExceeded(Exception): 
     def __init__(self, error: Exception, retries: int):
         self.error = error
         self.retries = retries
     
     def __str__(self):
         print(self.error)
@@ -360,14 +360,16 @@
 class ResponseStreamSliceIterator:
     def __init__(self, slice):
         self.slice = slice
         self.retries = 0
         self.text = ""
         self.consumed_tokens = []
 
+        self.done = asyncio.Event()
+
     async def recover(self):
         recovery_kwargs = self.slice.kwargs.copy()
         # reconstruct the prompt by tokenizing the consumed tokens
         if len(self.consumed_tokens) > 0:
             prompt = self.consumed_tokens
             recovery_kwargs["prompt"] = [t[0] for t in prompt]
         
@@ -403,30 +405,55 @@
                 return partial_data
         self.text = new_it.text
         self.consumed_tokens = new_it.consumed_tokens
         self.slice = new_slice
         # otherwise the chunking aligns with the old stream, so we return the next chunk
         return await self.__anext__()
 
+    async def get_next(self):
+        if self.done.is_set(): 
+            raise StopAsyncIteration
+        check_done_task = asyncio.create_task(self.done.wait())
+        get_next_item_task = asyncio.create_task(self.slice.data_queue.get())
+        done, pending = await asyncio.wait([get_next_item_task, check_done_task], 
+            return_when=asyncio.FIRST_COMPLETED, timeout=2.0)
+        
+        if check_done_task in done:
+            # this indicates the end of this response stream
+            for t in pending: t.cancel()
+            raise StopAsyncIteration
+        elif len(done) > 0:
+            assert get_next_item_task in done, f"expected get_next_item_task to be done, but only {done} is done."
+            # cancel self.done waiting task
+            for t in pending: t.cancel()
+            # return with new data chunk
+            return get_next_item_task.result()
+        else:
+            # if after timeout this response has been fully consumed, we are done
+            if self.done.is_set():
+                raise StopAsyncIteration
+            # otherwise return a RecoveryAttempt for retrying this request
+            return RecoveryAttempt(self.slice.kwargs, TimeoutError(), self.slice.maximum_retries)
+
     async def __anext__(self):
         try:
-            try:
-                data = await asyncio.wait_for(self.slice.data_queue.get(), 2.0)
-            except asyncio.TimeoutError as e:
-                data = RecoveryAttempt(self.slice.kwargs, e, self.slice.maximum_retries)
+            data = await self.get_next()
             # None indicates end of stream
-            if data is None: raise StopAsyncIteration
+            if data is None:
+                raise StopAsyncIteration
             # exceptions that are queued are definitive (all retries failed)
             if isinstance(data, Exception): raise data
             # RecoveryAttempt indicates that the underlying stream errored out and we need to recover (still retries left)
             if isinstance(data, RecoveryAttempt):
+                if not self.slice.stream.scheduler.is_available():
+                    # fail quietly, if parent scheduler is no longer available (results of this query will be discarded anyway)
+                    raise StopAsyncIteration()
                 # if the stream of our self.slice errors out, we can recover by creating a new 
                 # stream via a new call to openai.Completion.create
                 attempt: RecoveryAttempt = data
-                traceback.print_exc()
                 print("OpenAI API: Underlying stream of OpenAI complete() call failed with error", type(attempt.error), attempt.error, f"Retrying... (attempt: {self.retries})", flush=True)
                 self.retries += 1
                 # if we have exceeded the maximum number of retries, raise the error
                 if self.retries > attempt.maximum_retries:
                     raise MaximumRetriesExceeded(attempt.error, retries=self.retries)
                 if self.slice.stream.scheduler.tokenizer is None:
                     print("Cannot recover from stream error without a configured tokenizer", flush=True)
@@ -513,14 +540,19 @@
         self.tokenizer = None
         
         self.cache = {}
         self.cache_dir = "."
         self.futures = set()
         self.restore_cache()
 
+        self.first_token_latency = 0
+
+    def reset_latency_stats(self):
+        self.first_token_latency = 0
+
     def restore_cache(self):
         if not self.use_cache:
             return
         cache_file = "openai.completions.cache"
         if os.path.exists(os.path.join(self.cache_dir, cache_file)):
             with open(os.path.join(self.cache_dir, cache_file), "rb") as f:
                 self.cache = pickle.load(f)
@@ -585,16 +617,14 @@
 
         num_prompt_tokens = sum([len(p) for p in kwargs["prompt"]])
         self.stats.prompt_tokens += num_prompt_tokens
 
         res = complete(**kwargs)
         first = await anext(res)
         return first_buffered(res, first)
-        
-        return res
 
     def is_definitive_error(self, e):
         if "logit biases, but can provide at most" in str(e):
             return True
         return False
 
     async def complete_request_worker(self, queue: asyncio.Queue):
@@ -620,16 +650,16 @@
                         await asyncio.sleep(0.5)
                         if retries <= 0 or self.is_definitive_error(e):
                             raise e
                         if type(e) is TimeoutError or type(e) is OpenAIRateLimitError:
                             t = (2.0 * random.random()) ** (self.maximum_retries - retries)
                             print("Backing off for", t , "seconds")
                             await asyncio.sleep(t)
-            except asyncio.CancelledError:
-                return
+            except asyncio.CancelledError as e:
+                break
             except Exception as e:
                 print("error", type(e))
                 for future in futures:
                     future.set_exception(e)
                 continue
 
             self.warn_chaos() # warns about self.chaos if set
@@ -667,9 +697,13 @@
 
 
         assert kwargs.get("echo", False), f"bopenai requires echo=True for to enable proper error recovery. Please handle proper prompt removal in client code."
 
         r = RequestQueueItem(kwargs, request_id)
         await self.complete_api_call_queue.put(r)
         self.request_ctr += 1
-        
-        return await result_fut
+        if not self.is_available():
+            raise APIShutDownException(f"bopenai requires at least one worker to be running to issue new complete requests.")
+        return await result_fut
+
+    def is_available(self):
+        return len([w for w in self.complete_request_workers if not w.done()]) > 0
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6/src/lmql/runtime/bopenai/openai_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 
 
 import json
 import time
 import asyncio
 
 from lmql.runtime.tokenizer import load_tokenizer
+from lmql.runtime.stats import Stats
 
 class OpenAIStreamError(Exception): pass
 class OpenAIRateLimitError(OpenAIStreamError): pass
 
 class Capacity: pass
 Capacity.total = 32000 # defines the total capacity available to allocate to different token streams that run in parallel
 # a value of 80000 averages around 130k tok/min on davinci with beam_var (lower values will decrease the rate and avoid rate limiting)
 Capacity.reserved = 0
 
 stream_semaphore = None
 
+api_stats = Stats("openai-api")
+
 class CapacitySemaphore:
     def __init__(self, capacity):
         self.capacity = capacity
 
     async def __aenter__(self):
         # wait for self.capacity > capacity
         while True:
@@ -206,15 +209,15 @@
                             complete_chunk = chunks[0].strip()
                             current_chunk = "data: ".join(chunks[1:])
 
                             if len(complete_chunk.strip()) == 0: 
                                 continue
                             if complete_chunk == "[DONE]": 
                                 return
-                            
+
                             n_chunks += 1
                             sum_chunk_times += time.time() - last_chunk_time
                             last_chunk_time = time.time()
                             
                             data = json.loads(complete_chunk)
 
                             if "error" in data.keys():
@@ -336,14 +339,17 @@
                             current_chunk = "data: ".join(chunks[1:])
 
                             if len(complete_chunk.strip()) == 0: 
                                 continue
                             if complete_chunk == "[DONE]": 
                                 return
                             
+                            if n_chunks == 0:
+                                api_stats.times["first-chunk-latency"] = api_stats.times.get("first-chunk-latency", 0) + (time.time() - stream_start)
+
                             n_chunks += 1
                             sum_chunk_times += time.time() - last_chunk_time
                             last_chunk_time = time.time()
                             
                             data = json.loads(complete_chunk)
 
                             if "error" in data.keys():
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6/src/lmql/runtime/dclib/dclib_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from lmql.utils import nputil
 
 @dataclass
 class Continuation:
     token: Any
     logprob: Any
     user_data: Any
-
 class criterion: 
     def __and__(self, other):
         return logical_and(self, other)
 
     def __or__(self, other):
         return logical_or(self, other)
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,596 +1,549 @@
 import asyncio
-from collections import namedtuple
-from typing import List, Union
-
-from .dclib_array import DataArray
-from .dclib_global import stats
-from .dclib_seq import DecoderSequence, detseq, deepcopy, deepmerge, DecoderSequence, DeterministicDecoderSequence, Continuation
+from lmql.runtime.dclib.dclib_seq import DecoderSequence
 import numpy as np
-from lmql.utils import nputil
+import pickle
+import os
+from typing import List, Union, Any
 from dataclasses import dataclass
-import sys
 
-from lmql.runtime.stats import Stats
+from .dclib_array import DataArray
+from .dclib_seq import DecoderSequence, Continuation, DeterministicDecoderSequence, deepcopy, deepmerge, detseq
+from .dclib_model import DcModel, CacheDelegate
+from .dclib_rewrite import DcModelRewriteMixin
+import lmql.runtime.masks as masks
+from lmql.utils.nputil import ensure_iterable
 
-@dataclass
-class DcModelLogitsTask:
-    model: any
-    input_ids: np.ndarray
-    logits_mask: np.ndarray
-    kwargs: dict
-    result_fut: asyncio.Future
-
-class ModelQueue:
-    @staticmethod
-    def get(model_identifier):
-        if model_identifier not in ModelQueue._instances.keys():
-            ModelQueue._instances[model_identifier] = ModelQueue(model_identifier)
-        return ModelQueue._instances[model_identifier]
-    
-    def __init__(self, model_identifier):
-        self.model_identifier = model_identifier
-        self.logits_queue = asyncio.Queue()
-        self.logits_workers = [asyncio.create_task(self.queue_worker_logits()) for _ in range(8)]
-    
-    def __del__(self):
-        for w in self.logits_workers:
-            w.cancel()
-        
-    def put(self, task):
-        self.logits_queue.put_nowait(task)
+class CachedDcModel(DcModelRewriteMixin, CacheDelegate):
+    delegate: DcModel
     
-    async def queue_worker_logits(self):
-        max_batch_size = DcModel.batch_size
-        while True:
-            try:
-                batch: List[DcModelLogitsTask] = []
-                task = await self.logits_queue.get()
-                batch.append(task)
-                if self.logits_queue.qsize() == 0:
-                    await asyncio.sleep(0.05)
-
-                while len(batch) < max_batch_size:
-                    try:
-                        task = self.logits_queue.get_nowait()
-                        batch.append(task)
-                    except asyncio.QueueEmpty:
-                        break
-                
-                # group by parameters
-                groups = [[]]
-                for t in batch:
-                    if len(groups[-1]) == 0:
-                        groups[-1].append(t)
-                        continue
-                    current_group_model = groups[-1][0].model
-                    current_group_kwargs = str(groups[-1][0].kwargs)
-                    if t.model == current_group_model and str(t.kwargs) == current_group_kwargs:
-                        groups[-1].append(t)
-                    else:
-                        groups.append([t])
-
-                # run groups in batches
-                for group in groups:
-                    kwargs = group[0].kwargs
-                    model = group[0].model
-                    logits, raw = await model.logits(
-                        [task.input_ids for task in group],
-                        logits_mask=self.stack_logit_masks([task.logits_mask for task in group]),
-                        **kwargs
-                    )
-                    for logits, raw, fut in zip(logits, raw, [task.result_fut for task in group]):
-                        fut.set_result((logits, raw))
-                    # print("batch of size", len(group), len(batch), self.logits_queue.qsize(), flush=True)
-            except Exception as e:
-                import traceback
-                traceback.print_exc()
-                print("Exception in queue worker logits: ", e)
-
-    def stack_logit_masks(self, logit_masks):
-        if all([m is None for m in logit_masks]):
-            return None
-        else:
-            existing = [m for m in logit_masks if m is not None]
-            vocab_size = existing[0].shape[1] if existing[0].ndim == 2 else existing[0].shape[0]
-            lm = np.stack([m if m is not None else np.zeros((vocab_size), dtype=np.bool) for m in logit_masks])
-            return lm
-
-ModelQueue._instances = {}
-
-class DcModel:
-    def __init__(self, model, tokenizer, truncation_threshold=-3e38, init_workers=True, **kwargs):
-        """
-        Parameters:
-        
-        model: The model to use for inference.
-        bos_token_id: The token id to use for the beginning of a sequence.
-        eos_token_id: The token id to use for the end of a sequence.
-        truncation_threshold: The threshold to use for logit truncation (cf. DecoderSequence.truncation_threshold). Logits below this threshold are considered to be -inf and will never be considered as next token.
-        """
-        self.model = model
-        self.tokenizer = tokenizer
-        self.model_identifier = model.model_identifier
-        self.model_args = kwargs
-
-        self.bos_token_id = tokenizer.bos_token_id
-        self.eos_token_id = tokenizer.eos_token_id
-        self.truncation_threshold = truncation_threshold
-
-        self.stats = Stats("dcmodel")
-
-        if init_workers: self.logits_queue = ModelQueue.get(self.model_identifier)
-        else: self.logits_queue = None
-
-    def log_billable_tokens(self, n: int):
-        if hasattr(self.model, "billable_tokens"):
-            self.model.billable_tokens += n
+    def __new__(cls, delegate: DcModel, initial_prompt_ids=None, cache_file=None, show_speculative=False):
+        mc = super().__new__(cls)
         
-    def log_queries(self, n: int):
-        if hasattr(self.model, "num_queries"):
-            self.model.num_queries += n
+        mc.delegate: DcModel = delegate
 
-    async def detokenize(self, *args, **kwargs):
-        return await self.model.detokenize(*args, **kwargs)
-    
-    async def tokenize(self, *args, **kwargs):
-        return await self.model.tokenize(*args, **kwargs)
+        # setup cache delegate
+        assert delegate.cache_delegate is None, "cannot cache a model that is already cached by another cache_delegate"
+        delegate.cache_delegate = mc
 
-    async def model_logits_async(self, model, input_ids, logits_mask=None, **kwargs):
-        loop = asyncio.get_running_loop()
-        result_fut = loop.create_future()
+        mc.token_streams = []
         
-        # print(kwargs)
-        model_args = {
-            "temperature": kwargs.get("temperature", None),
-            "eos_token_id": kwargs.get("eos_token_id", None),
-        }
+        mc.cache = {}
+        mc.user_data_cache = {}
+        mc.cache_lock = asyncio.Lock()
+
+        mc.mask_cache = {}
+        mc.show_speculative = show_speculative
         
-        self.logits_queue.put(DcModelLogitsTask(model, input_ids, logits_mask, model_args, result_fut))
+        mc.input_id_key_offset = len(initial_prompt_ids) if initial_prompt_ids else 0
+        mc.cache["initial_prompt_ids"] = str(initial_prompt_ids) if initial_prompt_ids is not None else None
+        mc.cache["model"] = delegate.model_identifier
+    
+        mc.calls = 0
+        mc.hits = 0
 
-        return await result_fut
+        mc.cache_file = cache_file
 
-    async def autobatch_logits_with_cache(self, model, input_ids, max_batch_size, cache=None, logits_mask=None, **kwargs):
-        kwargs = {**self.model_args, **kwargs}
+        try:
+            if cache_file is not None and os.path.exists(cache_file):
+                with open(cache_file, "rb") as f:
+                    cache = pickle.load(f)
+                    if cache["initial_prompt_ids"] != str(initial_prompt_ids):
+                        print("warning: cache file is from a different query (revision). Its contents will be overwritten.")
+                    elif cache["model"] != delegate.model_identifier:
+                        print("warning: cache file is from a different model. Its contents will be overwritten.")
+                    else:
+                        mc.cache = cache
+        except Exception as e:
+            print("error: failed to load token cache from file", e)
+            pass
 
-        if cache is not None: 
-            input_ids_to_process = [ids for cache, ids in zip(cache, input_ids) if cache is None]
-        else: 
-            input_ids_to_process = input_ids
-
-        # print("call model for ", len(input_ids_to_process), " sequences", [len(ids) for ids in input_ids_to_process])
-
-        # automatic batching
-        results = await asyncio.gather(*[self.model_logits_async(
-            model, 
-            input_ids_to_process[i],
-            logits_mask=logits_mask[i] if logits_mask is not None else None,
-            eos_token_id=self.eos_token_id,
-            **model.model_kwargs,
-            **kwargs
-        ) for i in range(len(input_ids_to_process))])
-
-        # call model only for non-cached input_ids
-        processed_logits = np.stack([r[0] for r in results], axis=0)
-        processed_logits_raw = np.stack([r[1] for r in results], axis=0)
-
-        # shortcut if no cache
-        if cache is None: return processed_logits, processed_logits_raw
-
-        # merge with cache
-        result_logits = []
-        result_raw = []
-        ptr = 0
-        for c in cache:
-            if c is not None:
-                result_logits.append(c[0])
-                result_raw.append(c[1])
+        return mc
+    
+    def close(self):
+        self.model.cache_delegate = None
+        for ts in self.token_streams:
+            ts.cancel()
+        self.token_streams = []
+
+    def save(self):
+        if self.cache_file is not None:
+            with open(self.cache_file, "wb") as f:
+                pickle.dump(self.cache, f)
+
+    def base_key(self, ids, *args):
+        if isinstance(ids, DecoderSequence):
+            return self.base_key(ids.input_ids)
+        return str(ids[self.input_id_key_offset:])
+
+    async def get_mask(self, s: DecoderSequence, **kwargs):
+        if s.id in self.mask_cache:
+            return self.mask_cache[s.id]
+        if hasattr(s, "logits_mask"):
+            return s.logits_mask
+
+        constrained_seqs = np.array([True], dtype=np.bool_)
+        logits_mask_result = await self.delegate.compute_logits_mask(s.input_ids.reshape(1, -1), [s.user_data], constrained_seqs, [s], **kwargs, required=True)
+        self.mask_cache[s.id] = logits_mask_result
+
+        if s.user_data is None:
+            s.user_data = {}
+        s.user_data = deepmerge(deepcopy(s.user_data), logits_mask_result.user_data[0])
+        s.user_data["set_by"] = "where"
+
+        setattr(s, "logits_mask", logits_mask_result)
+
+        return logits_mask_result
+
+    async def get_keys(self, s: DecoderSequence, edge_type: str, **kwargs):
+        kwargs = {**self.delegate.model_args, **kwargs}
+
+        keys = []
+
+        # compute logits mask
+        mask = (await self.get_mask(s, **kwargs)).logits_mask[0]
+
+        if type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0:
+            keys.append((self.base_key(s), str(s.next_ids[0])))
+
+        if mask is not None:
+            if masks.mask_num_allowed(mask) == 1:
+                keys.append((self.base_key(s), str(masks.mask_get_only_allowed(mask))))
             else:
-                result_logits.append(processed_logits[ptr])
-                result_raw.append(processed_logits_raw[ptr])
-                ptr += 1
-        
-        return np.stack(result_logits, axis=0), np.stack(result_raw, axis=0)
-
-    async def compute_logits_mask(self, input_ids, user_data, is_constrained, seqs, **kwargs):
-        if "modern_logits_processor" in kwargs:
-            processor = kwargs["modern_logits_processor"]
-            mask = await processor(seqs, additional_logits_processor_mask=is_constrained)
-            return mask
+                if masks.is_fixed_int_mask(mask):
+                    keys.append((self.base_key(s), edge_type, "-".join([str(i) for i in mask])))
 
-        if "dclib_additional_logits_processor" not in kwargs:
-            return namedtuple("LogitsMaskResult", ["logits_mask", "user_data"])([None], user_data)
-        
-        processor = kwargs["dclib_additional_logits_processor"]
-        mask = await processor(input_ids, user_data=user_data, additional_logits_processor_mask=is_constrained)
+                    if edge_type == "top-1":
+                        argmax_token, argmax_score = self.cache.get((self.base_key(s), "top-1"), (None, None))
+                        if type(argmax_token) is int and argmax_token in mask:
+                            keys.append((self.base_key(s), str(argmax_token)))
+                else:
+                    keys.append((self.base_key(s), edge_type, "-".join([str(i) for i in np.where(mask >= 0)[0]])))
+        else:
+            if edge_type != "sample":
+                # standard key is sequence id + edge type
+                keys.append((self.base_key(s), edge_type))
 
-        return mask
+        return keys
+    
+    async def get_cache(self, s: DecoderSequence, edge_type: str, user_data=False, **kwargs):
+        keys = await self.get_keys(s, edge_type, **kwargs)
 
-    async def logits(self, seqs, max_batch_size=16, **kwargs):
-        with self.stats.timer("logits"):
-            input_ids = [s.input_ids for s in seqs]
-            user_data = [s.data() for s in seqs]
-            cache = [(s.logits, s.raw_logits) if s.logits is not None else None for s in seqs]
-
-            # determine set of sequences that are constrained
-            constrained_seqs = np.array([s.is_query_constrained for s in seqs], dtype=np.bool_)
-
-            # compute logits mask
-            logits_mask_result = await self.compute_logits_mask(input_ids, user_data, constrained_seqs, seqs, **kwargs)
-            logits_mask = logits_mask_result.logits_mask
-            if len(logits_mask) == 1 and logits_mask[0] is None: logits_mask = None
-            
-            # update user data with new information obtained when computing logits masks
-            for s, updated_user_data in zip(seqs, logits_mask_result.user_data):
-                if updated_user_data is None: continue
-                # TODO: update instead of reassign
-                s.user_data = updated_user_data
-                s.user_data["set_by"] = "where"
-
-            # compute logits with automatic batching
-            result_logits, result_raw = await self.autobatch_logits_with_cache(self.model, input_ids, max_batch_size=max_batch_size, cache=cache, logits_mask=logits_mask, **kwargs)
-
-            # cache logits in nodes (if self.input_ids is used)
-            for s,logits,raw in zip(seqs, result_logits, result_raw):
-                s.logits = logits
-                s.raw_logits = raw
+        for k in keys:
+            token, score = None, None
             
-            return result_logits, result_raw
+            async with self.cache_lock:
+                if k in self.cache:
+                    token, score = self.cache[k]
+            
+            if token is None:
+                continue
+
+            if type(token) is asyncio.Future: 
+                awaited_result = await token
+                if awaited_result is None:
+                    continue
+                else:
+                    assert type(awaited_result) is tuple and len(awaited_result) == 2
+                    token, score = awaited_result
+            if user_data:
+                return keys, (token, score, self.user_data_cache.get(k, None))
+            return keys, (token, score)
 
-    async def argmax(self, sequences, **kwargs):
-        """
-        Returns a pool with `n` sampled successor nodes per node in the pool.
-        """
-        kwargs = {**self.model_args, **kwargs}
+        return keys, None
+    
+    def set_cache(self, key, c: Union[Continuation, tuple], user_data=None, verbose=False):
+        for k in key:
+            if verbose:
+                print("    cached", k)
+            
+            # check if the existing entry is a future
+            existing = self.cache.get(k, (None, None))[0]
+            fut = existing if type(existing) is asyncio.Future else None
+            
+            if type(c) is Continuation:
+                self.cache[k] = (c.token, c.logprob)
+                if user_data is not None:
+                    self.user_data_cache[k] = user_data
+                if fut is not None and not fut.done():
+                    fut.set_result((c.token, c.logprob))
+            else:
+                assert type(c) is tuple and len(c) == 2
+                self.cache[k] = c
+                if user_data is not None:
+                    self.user_data_cache[k] = user_data
+                if fut is not None and not fut.done():
+                    fut.set_result(c)
 
+    async def argmax(self, arr: DataArray, **kwargs):
         async def op_argmax(seqs):
-            if len(seqs) == 0:
-                return []
-            
-            if all(type(s) is DeterministicDecoderSequence for s in seqs) and all(len(s.next_ids) > 0 for s in seqs):
-                next_token_ids = np.array([s.next_ids[0] for s in seqs])
-                next_token_scores = np.array([s.next_logprobs[0] for s in seqs])
-                return [s.make_successors(next_token_ids[i].reshape(1), next_token_scores[i], logits=None) for i,s in enumerate(seqs)]
-            
-            self.model.num_queries += len(seqs)
-            logits, raw_logits = await self.logits(seqs, **kwargs)
-
-            next_token_ids = logits.argmax(axis=-1)
-            next_token_scores = np.take_along_axis(logits, next_token_ids.reshape(-1,1), axis=-1)
-            return [s.make_successors(next_token_ids[i].reshape(1), next_token_scores[i], logits=raw_logits[i]) for i,s in enumerate(seqs)]
-        
-        return await sequences.aelement_wise(op_argmax)
-
+            self.calls += len(seqs)
 
-    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False):
-        with self.stats.timer("score"):
-            assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
+            # check cache for all
+            cache_entries = [await self.get_cache(s, 'top-1', user_data=True, **kwargs) for s in seqs]
+            cached_tokens = [e[1] for e in cache_entries]
+            cache_keys = [e[0] for e in cache_entries]
+
+            # apply operation for non-cached
+            non_cached = [s for s, c in zip(seqs, cached_tokens) if c is None]
+            # generator over new results
+            non_cached_argmax = iter((await self.delegate.argmax(DataArray(non_cached), **kwargs)).items())
             
-            if max_batch_size is None:
-                max_batch_size = DcModel.batch_size
-            
-            completion = [np.array(cont) for cont in tokens]
-
-            def make_detseq(s, token_score, completion):
-                # compose deterministic flags
-                if type(deterministic) is bool:
-                    deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
-                    next_deterministic = np.array([deterministic] * len(completion[1:]))
-                else:
-                    assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored"
-                    deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
-                    next_deterministic = np.array(deterministic[1:])
-
-                return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
-                        next_ids=completion[1:],
-                        logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
-                        next_logprobs=token_score[1:],
-                        deterministic=deterministic_flags,
-                        next_deterministic=next_deterministic,
-                        predecessor=s,
-                        user_data=user_data,
-                        stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
-                        needs_rewrite=needs_rewrite,
-                        sticky_user_data_keys=s.sticky_user_data_keys)
             results = []
-
-            for i in range(0, len(sqs), max_batch_size):
-                batch_sqs = sqs[i:i+max_batch_size]
-                batch_input_ids = np.stack([s.input_ids for s in batch_sqs], axis=0)
-                batch_completion = np.stack(self.model.right_pad(completion[i:i+max_batch_size], pad_token_id=self.eos_token_id)["input_ids"], axis=0)
-
-                if noscore:
-                    token_scores = np.zeros_like(batch_completion)
+            # put new results in cache
+            for i, (s, key, c) in enumerate(zip(seqs, cache_keys, cached_tokens)):
+                if c is None: 
+                    r = next(non_cached_argmax)
+                    results.append(r)
+                    self.set_cache(key, r)
                 else:
-                    token_scores, _ = await self.model.score(
-                        batch_input_ids,
-                        batch_completion,
-                        eos_token_id=self.eos_token_id
-                    )
-                for s,c,ts in zip(batch_sqs,completion[i:i+max_batch_size], token_scores):
-                    results.append(make_detseq(s, ts[:len(c)], c))
-
-            return results
+                    token, logprob, cached_user_data = c
+                    logit_mask_result = await self.get_mask(s, **kwargs)
+                    user_data = deepmerge(logit_mask_result.user_data[0], cached_user_data) if cached_user_data is not None else logit_mask_result.user_data[0]
+                    continuation = s.make_successors(token.reshape(1), logprob.reshape(1), logits=None, user_data=[user_data])
+                    results.append(continuation)
 
-    async def score_old(self, seqs: Union[DataArray, DecoderSequence], tokens: Union[List[int], List[List[int]]], max_batch_size=4, deterministic=False, stop_phrase=False):
-        if type(tokens[0]) is int:
-            tokens = [tokens]
-        
-        unwrap = False
-        if type(seqs) is DecoderSequence:
-            seqs = DataArray([seqs] * len(tokens))
-            unwrap = True
-        
-        sqs = list(seqs.items())
-        original_shape = seqs.shape
-        seqs = seqs.flatten()
-        assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
-
-        input_ids = np.stack([s.input_ids for s in sqs], axis=0)
-        completion = [np.array(cont) for cont in tokens]
-
-        all_token_scores = []
-        all_logits = []
-        all_completions = []
-
-        # automatic batching
-        for i in range(0, len(input_ids), max_batch_size):
-            batch_completion = np.stack(self.model.right_pad(completion[i:i+max_batch_size], pad_token_id=self.eos_token_id)["input_ids"], axis=0)
-            
-            token_scores, logits = await self.model.score(
-                input_ids[i:i+max_batch_size],
-                batch_completion,
-                eos_token_id=self.eos_token_id
-            )
-            for c,ts,logs in zip(completion[i:i+max_batch_size], token_scores, logits):
-                all_completions.append(c)
-                all_token_scores.append(ts[:len(c)])
-                all_logits.append(logs[:len(c)])
-
-        def make_detseq(s, token_score, logits, completion, user_data):
-            return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
-                    next_ids=completion[1:],
-                    logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
-                    next_logprobs=token_score[1:],
-                    deterministic=np.concatenate([s.deterministic, np.array([deterministic])]),
-                    next_deterministic=np.array([deterministic] * len(completion[1:])),
-                    predecessor=s,
-                    user_data=user_data,
-                    stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
-                    needs_rewrite=True,
-                    sticky_user_data_keys=s.sticky_user_data_keys)
+                    self.hits += 1
 
-        s = DataArray([make_detseq(s, token_score, logits, completion, s.user_data) for s,token_score,logits,completion in zip(sqs, all_token_scores, all_logits, all_completions)])
-        
-        if unwrap: 
-            return list(s.items())
-        else:
-            return s.reshape(original_shape)
+            # read full result from cache
+            return results
 
-    async def sample(self, sequences, num_samples=1, **kwargs):
-        """
-        Returns a pool with `n` sampled successor nodes per node in the pool.
-        """
-        kwargs = {**self.model_args, **kwargs}
+        return await arr.aelement_wise(op_argmax)
 
+    async def sample(self, arr: DataArray, num_samples=1, **kwargs):
         async def op_sample(seqs):
-            if len(seqs) == 0:
-                return []
-
-            logits, raw_logits = await self.logits(seqs, **kwargs)
-            vocab_size = logits.shape[-1]
-
-            next_token_ids = []
-            for i in range(len(logits)):
-                probs = np.exp(logits[i])
-                num_possible = (probs > 0).sum()
-                next_token_ids.append(np.random.choice(vocab_size, size=max(num_samples, num_possible), p=probs, replace=False))
-            next_token_ids = np.stack(next_token_ids, axis=0)
-
-            next_token_scores = np.take_along_axis(logits, next_token_ids.reshape(-1,1), axis=-1)
+            self.calls += len(seqs)
 
-            return [s.make_successors(next_token_ids[i], next_token_scores[i], logits=raw_logits[i]) for i,s in enumerate(seqs)]
-        
-        return await sequences.aelement_wise(op_sample)
-
-    async def topk_continuations(self, sequences, k, **kwargs):
-        kwargs = {**self.model_args, **kwargs}
+            # check cache for all
+            cache_entries = [await self.get_cache(s, 'sample', **kwargs) for s in seqs]
+            cached_tokens = [e[1] for e in cache_entries]
+            cache_keys = [e[0] for e in cache_entries]
+            
+            # apply operation for non-cached
+            non_cached = [s for s, c in zip(seqs, cached_tokens) if c is None]
+            # generator over new results
+            non_cached_sample = iter((await self.delegate.sample(DataArray(non_cached), num_samples=num_samples, **kwargs)).items())
+            
+            results = []
+            # put new results in cache
+            for i, (s, key, c) in enumerate(zip(seqs, cache_keys, cached_tokens)):
+                if c is None: 
+                    r = next(non_cached_sample)
+                    results.append(r)
+                    self.set_cache(key, r)
+                else:
+                    token, logprob = c
+                    user_data = (await self.get_mask(s, **kwargs)).user_data
+                    continuation = s.make_successors(token.reshape(1), logprob, logits=None, user_data=user_data)
+                    results.append(continuation)
+                    self.hits += 1
 
-        async def op_topk(path, seqs, k):
-            if len(seqs) == 0:
-                return path, []
+            # read full result from cache
+            return results
 
-            logits, raw_logits = await self.logits(seqs, **kwargs)
+        return await arr.aelement_wise(op_sample)
 
-            next_token_scores, next_tokens = nputil.topk(
-                logits, k, sorted=True, axis=1
-            )
+    async def topk_continuations(self, arr: DataArray, k: int, **kwargs):
+        async def op_topk(seqs):
+            self.calls += len(seqs)
+            
+            # construct possible cache entries for all seqs (min(k, num_possible))
+            cache_entries_topk = [] 
+            for s in seqs:
+                max_k = k
+                if type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0:
+                    max_k = 1
+                mask = await self.get_mask(s, **kwargs)
+                if mask is not None:
+                    mask = mask.logits_mask[0]
+                    if mask is not None:
+                        max_k = min(k, masks.mask_num_allowed(mask))
+                cache_entries_topk.append([await self.get_cache(s, f'top-{i}', **kwargs) for i in range(1, max_k+1)])
+
+            # per seq, top 1-k cached tokens 
+            cached_tokens = [[e[1] for e in cache_entries] for cache_entries in cache_entries_topk]
+            # per seq, top 1-k cache keys (multiple per entry)
+            cache_keys = [[e[0] for e in cache_entries] for cache_entries in cache_entries_topk]
+
+            # apply operation for non-cached
+            non_cached = [s for s, c in zip(seqs, cached_tokens) if any(ct is None for ct in c)]
+            # generator over new results
+            non_cached_sample = iter((await self.delegate.topk_continuations(DataArray(non_cached), k=k, **kwargs)).items())
+            
+            results = []
+            # put new results in cache
+            for i, (s, key, c) in enumerate(zip(seqs, cache_keys, cached_tokens)):
+                if any(ct is None for ct in c):
+                    r = next(non_cached_sample)
+                    if any(ct is not None for ct in c):
+                        mask = (await self.get_mask(s, **kwargs)).logits_mask[0]
+                        print("WARNING: some cache entries are None, but some are not", len([e for e in c if e is not None]), len(r.token))
+                        print([await s.text()])
+                    results.append(r)
+                    next_token_ids = ensure_iterable(r.token)
+                    next_token_scores = ensure_iterable(r.logprob)
+                    # cache each continuation separately
+                    assert len(next_token_ids) <= len(key)
+                    for i,ck in zip(range(len(next_token_ids)), key):
+                        self.set_cache(ck, (next_token_ids[i], next_token_scores[i]))
+                    
+                    # fill remaining top-k slots with empty result
+                    for i in range(len(next_token_ids) + 1, k + 1):
+                        self.set_cache([(self.base_key(s), "top-{}".format(i))], (None, None))
+                else:
+                    tokens = []
+                    logprobs = []
+                    user_data = []
+                    for token, logprob in c:
+                        if token is None and logprob is None:
+                            # empty cache slot (top-i is not possible due to masking or truncation)
+                            continue
+                        c_user_data = (await self.get_mask(s, **kwargs)).user_data
+                        continuation = s.make_successors(token.reshape(1), logprob.reshape(1), logits=None, user_data=c_user_data)
+                        tokens.append(continuation.token)
+                        logprobs.append(continuation.logprob)
+                        user_data.append(continuation.user_data)
+                    self.hits += 1
+                    results.append(Continuation(np.array(tokens), np.array(logprobs), user_data))
 
-            return path, [s.make_successors(next_tokens[i], next_token_scores[i], logits=raw_logits[i]) for i,s in enumerate(seqs)]
+            # read full result from cache
+            return results
 
-        result_items = await asyncio.gather(*[op_topk(path, seqs, k) for path, seqs in sequences.sequences.items()])
-        return DataArray(dict(result_items))
+        return await arr.aelement_wise(op_topk)
     
-    def report_stats(self, printer, decoder_step=None):
-        self.model.report_stats(printer, decoder_step)
-        
-    async def _rewrite_seq(self, seqs_or_seq, noscore=False):
-        # check self.model_args for a "modern_rewriter" key
-        if "modern_rewriter" not in self.model_args:
-            return seqs_or_seq
+    def expand_through_cache(self, sq: DecoderSequence, tok: List[int], det: List[bool], user_data: List[Any], initial_user_data=None):
+        """
+        Steps along the cache based on 'tok' until no more cache entries are found.
+        """
+        while (self.base_key(sq), str(tok[0])) in self.cache.keys():
+            token, logprob = self.cache[(self.base_key(sq), str(tok[0]))]
+            c = Continuation(token, logprob, user_data[0])
+            sq = sq.extend(c, internal=True)
+            tok = tok[1:]
+            if type(det) is not bool:
+                det = det[1:]
+            user_data = user_data[1:]
+            if len(tok) == 0:
+                return sq, tok, det, user_data
+        return sq, tok, det, user_data
+
+    async def prescore_tokens(self, sq: DecoderSequence, tok: List[int], noscore=False):
+        user_data = sq.user_data
+
+        # expand through cache
+        while (self.base_key(sq), str(tok[0])) in self.cache.keys():
+            token, logprob = self.cache[(self.base_key(sq), str(tok[0]))]
+            c = Continuation(token, logprob, sq.user_data)
+            sq = sq.extend(c, internal=True)
+            tok = tok[1:]
+            if len(tok) == 0:
+                break
+
+        if len(tok) == 0: return
+        # do actual scoring with delegate model
+        sq, tokens, scores = await anext(self.delegate.score_tokens([sq], [tok], noscore=noscore))
+        self.save_cached(sq.input_ids, tokens, scores, user_data)
+        
+    def save_cached(self, ids: List[int], tokens, scores, user_data):
+        # add cache entries along pre-scored trajectory
+        for tok, score in zip(tokens, scores):
+            value = (np.array(tok).reshape(1), np.array(score).reshape(1))
+            self.set_cache([(self.base_key(ids, user_data), str(int(tok)))], value)
+            ids = np.append(ids, tok)
+
+    # async def prescore(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, 
+    #                 deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, 
+    #                 user_data=None, noscore=False):
+    #     async def op_score(sq, tok, max_batch_size, det, stop_phrase, needs_rewrite, user_data, noscore):
+    #         assert len(user_data) == len(tok)
+    #         sq, tok, det, user_data = self.expand_through_cache(sq, tok, det, user_data)
+
+    #         # handle short and fully cached sequences
+    #         if len(tok) == 0:
+    #             return [sq]
+    #         elif len(tok) <= 1 and not noscore:
+    #             return
+
+    #         # do actual scoring with delegate model
+    #         result = await self.delegate.score([sq], [tok], max_batch_size, det, stop_phrase, needs_rewrite, None, noscore, internal=True)
+
+    #         # add initial cache entry
+    #         s = result[0]
+    #         s.user_data = user_data[0]
+    #         c = Continuation(np.array([s.input_ids[-1]]), np.array([s.logprobs[-1]]), [user_data[0]])
+    #         self.set_cache([(self.base_key(sq), str(int(s.input_ids[-1])))], c)
+    #         user_data_offset = 1
+            
+    #         # add additional cache entries for deterministic tokens
+    #         while type(s) is DeterministicDecoderSequence and len(s.next_ids) > 0:
+    #             c = Continuation(np.array([s.next_ids[0]]), np.array([s.next_logprobs[0]]), [user_data[user_data_offset]])
+    #             sq = s
+    #             s = sq.extend(c)
+    #             user_data_offset += 1
+    #             self.set_cache([(self.base_key(sq), str(s.input_ids[-1]))], c)
         
-        # accept both a single sequence or a list of sequences
-        unwrap = lambda v: v
-        seqs = seqs_or_seq 
-        if type(seqs_or_seq) is not list:
-            seqs = [seqs_or_seq]
-            unwrap = lambda v: v[0] if type(v) is list and len(v) == 1 else v
-
-        # do not rewrite deterministic sequences (rewrite mask set to False)
-        mask_seq_to_rewrite = np.array([s.needs_rewrite for s in seqs], dtype=np.bool_)
-
-        rewriter = self.model_args["modern_rewriter"]
-        rewritten_ids = await rewriter(seqs, mask_seq_to_rewrite)
-    
-        # update user data, if rewriter provides it
-        for s, user_data in zip(seqs, rewritten_ids.user_data):
-            s.user_data = deepmerge(deepcopy(s.user_data), user_data) if user_data is not None else s.user_data
-            s.user_data["set_by"] = "rewrite"
-
-        all_updated_ids = rewritten_ids.appended_input_ids
-        if all_updated_ids is None:
-            all_updated_ids = [None for _ in range(len(seqs))]
-
-        # extract the offset of value tokens in appended_ids, before the sequence is deterministic
-        value_offset = rewritten_ids.value_offset
-        if value_offset is None:
-            value_offset = [0 for _ in range(len(seqs))]
-
-        # concat existing input_ids (minus eos if strip_eos) with appended input_ids
-        rewriting_tasks = []
-        for seqidx, (s, updated_ids, offset) in enumerate(zip(seqs, all_updated_ids, value_offset)):
-            # run actually rewrites asynchronously
-            rewriting_tasks.append(self._rewrite_seq_task(s, seqidx, seqs, rewritten_ids, updated_ids, offset, noscore=noscore))
-        rewritten_seqs = [s for s in await asyncio.gather(*rewriting_tasks) if s is not None]
-        return unwrap(rewritten_seqs)
-
-    async def _rewrite_seq_task(self, s, seqidx, seqs, rewritten_ids, updated_ids, value_offset, noscore=False):
-        if (updated_ids is None or len(updated_ids) == 0) and not get_strip_eos(seqidx, rewritten_ids.strip_eos):
-            return s
-        else:
-            ids = _stripped_ids(seqs, seqidx, rewritten_ids.strip_eos)
+    #     assert len(sqs) == len(tokens)
+    #     return await asyncio.gather(*[op_score(sq, tok, max_batch_size, det, stop_phrase, needs_rewrite, ud, noscore) for sq, tok, det, ud in zip(sqs, tokens, deterministic, user_data)])
+    
+    @property
+    def model_args(self):
+        return self.delegate.model_args
+
+    @property
+    def bos_token_id(self):
+        return self.delegate.bos_token_id
+    
+    @property
+    def eos_token_id(self):
+        return self.delegate.eos_token_id
+    
+    @property
+    def truncation_threshold(self):
+        return self.delegate.truncation_threshold
+    
+    @property
+    def model(self):
+        return self.delegate.model
+    
+    def report_stats(self, *args):
+        # print("Cache hits: %d/%d (%.2f%%)" % (self.hits, self.calls, 100 * self.hits / max(1,self.calls)))
+        return self.delegate.report_stats(*args)
+    
+    def log_billable_tokens(self, *args, **kwargs):
+        return self.delegate.log_billable_tokens(*args, **kwargs)
+    
+    async def tokenize(self, *args, **kwargs):
+        return await self.delegate.tokenize(*args, **kwargs)
+    
+    async def detokenize(self, *args, **kwargs):
+        return await self.delegate.detokenize(*args, **kwargs)
 
-            # if the rewritten sequence is identical to the original sequence, we can just keep the original sequence (with updated user data)
-            if (updated_ids is not None) and (len(ids) == len(s.input_ids) - 1 and len(updated_ids) == 1 and updated_ids[0] == s.input_ids[-1]):
-                return s
-            
-            # find the common prefix between the original sequence and the rewritten sequence
-            continued_seq = s
-            # keep track of current continuation seqs, to potentially traverse forward again (matching updated ids)
-            successors = [] 
-            # traverse backwards until continued_seq matches ids in length - 1
-            while len(continued_seq.input_ids) > len(ids) and continued_seq.predecessor is not None:
-                successors.insert(0, continued_seq)
-                continued_seq = continued_seq.predecessor
-
-            # traverse forward again, until the sequence no longer matches with updated_ids
-            last_rewrite_offset = len(continued_seq.input_ids)
-            offset = last_rewrite_offset
-            while offset < len(successors) + last_rewrite_offset and \
-                updated_ids is not None and \
-                offset < len(updated_ids) and \
-                successors[offset - last_rewrite_offset].input_ids[-1] == updated_ids[offset]:
+    def log_queries(self, n: int):
+        return self.delegate.log_queries(n)
+    
+    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
+        async def op_score(sq, tok):
+            unexpanded_tok = tok
+            # create continuation sequence at cache boundary
+            continued_seq, tok, det, _ = self.expand_through_cache(sq, tok, deterministic, [user_data for _ in tok])
+
+            if len(tok) == 0:
+                completion = np.array(unexpanded_tok)
+                token_scores = continued_seq.logprobs[-len(completion):]
+            else:
+                # run actual score() call for remaining non-cached part of 'tokens' (tok)
+                result: DeterministicDecoderSequence = (await self.delegate.score([continued_seq], [tok], max_batch_size, det, stop_phrase, needs_rewrite=needs_rewrite, user_data=user_data, noscore=noscore, internal=True))[0]
+                
+                # extract scores and tokens for new, scored part of 'tokens'
+                token_scores = np.array(result.logprobs[len(sq.input_ids):].tolist() + result.next_logprobs.tolist())
+                completion = np.array(unexpanded_tok)
+                assert len(token_scores) == len(completion), f"Expected {len(completion)} scores, but got {len(token_scores)}"
+
+                # store in cache
+                ids = continued_seq.input_ids
+                for i, (score, token) in enumerate(zip(token_scores[-len(tok):], tok)):
+                    # TODO: is this the correct user_data?
+                    self.set_cache([(self.base_key(ids, user_data if i > 0 else sq.user_data), str(token))], (np.array(token), np.array(score)))
+                    ids = np.append(ids, token)
                 
-                offset += 1
-                continued_seq = successors[offset - last_rewrite_offset - 1]
+            # determine detseq deterministic flags
+            if type(deterministic) is bool:
+                deterministic_flags = np.concatenate([sq.deterministic, np.array([deterministic])])
+                next_deterministic = np.array([deterministic] * len(completion[1:]))
+            else:
+                assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
+                deterministic_flags = np.concatenate([sq.deterministic, np.array(deterministic[:1])])
+                next_deterministic = np.array(deterministic[1:])
 
-            assert continued_seq is not None, "error: a rewritten sequence is not a continuation of any sequence already decoded. Going from {} to {} with common text {}".format(
-                await s.text(),
-                await self.detokenize(updated_ids),
-                # common ids
-                await self.detokenize(ids),
+            # create actual detseq
+            return detseq(ids=np.concatenate([sq.input_ids, completion[:1]], axis=0), 
+                    next_ids=completion[1:],
+                    logprobs=np.concatenate([sq.logprobs, token_scores[:1]], axis=0),
+                    next_logprobs=token_scores[1:],
+                    deterministic=deterministic_flags,
+                    next_deterministic=next_deterministic,
+                    predecessor=sq,
+                    user_data=user_data,
+                    stop_phrase=np.concatenate([sq.stop_phrase, np.array([stop_phrase])]),
+                    needs_rewrite=needs_rewrite,
+                    sticky_user_data_keys=sq.sticky_user_data_keys,
+                    internal=internal
             )
+        return await asyncio.gather(*[op_score(sq, tok) for sq, tok in zip(sqs, tokens)])
 
-            # align user data
-            user_data = continued_seq.extend_user_data(user_data=s.user_data)
-
-            if updated_ids is None:
-                s = DecoderSequence(continued_seq.input_ids, continued_seq.logprobs, continued_seq.deterministic, stop_phrase=continued_seq.stop_phrase, 
-                                    predecessor=continued_seq, user_data=user_data, sticky_user_data_keys=continued_seq.sticky_user_data_keys, epsilon_node=True)
-                s.needs_rewrite = False
-                return s
-
-            # offset updated_ids to the number of tokens that are already present as continued_seq
-            appended_ids = updated_ids[offset:]
-
-            if len(appended_ids) == 0:
-                return DecoderSequence(continued_seq.input_ids, continued_seq.logprobs, continued_seq.deterministic, stop_phrase=continued_seq.stop_phrase,
-                                    predecessor=continued_seq, user_data=user_data, sticky_user_data_keys=continued_seq.sticky_user_data_keys, epsilon_node=True)
-
-            # check if rewriting action provides user data specifically for the rewritten sequence
-            # user_data = rewritten_ids.rewritten_seq_user_data[seqidx] or user_data
-
-            # value tokens
-            num_value_tokens = value_offset - offset
-            deterministic = [True if i + 1 > num_value_tokens else False for i in range(len(appended_ids))]
-            continuation = (await self.score([continued_seq], [appended_ids], deterministic=deterministic, stop_phrase=False, needs_rewrite=False, user_data=user_data, noscore=noscore))[0]
-            
-            continuation.stop_phrase = s.stop_phrase[:len(continuation.input_ids)]
-            continuation.needs_rewrite = False
-            
-            steps = 0
-            while type(continuation) is DeterministicDecoderSequence and len(continuation.next_ids) > 0 and steps < num_value_tokens:
-                continuation.user_data = deepcopy(s.predecessor.user_data)
-                # print("continuation.user_data", continuation.user_data, flush=True)
-                continuation = continuation.extend(Continuation(continuation.next_ids[0], continuation.next_logprobs[0], continuation.user_data))
-                steps += 1
-            
-            continuation.user_data = rewritten_ids.rewritten_seq_user_data[seqidx] or user_data
-
-            return continuation
+    def register_token_stream(self, token_iterator: callable):
+        async def token_consumer(itr):
+            try:
+                ids = None
+                keys = None
+                sq = None
+                waiting_token_keys = []
+
+                async for (s, tokens, scores, edge_types, user_data) in itr():
+                    if type(tokens) is int or len(tokens) == 1:
+                        tokens = ensure_iterable(tokens)
+                        scores = ensure_iterable(scores)
+                        if type(edge_types) is str:
+                            edge_types = [edge_types]
+                    else:
+                        assert len(tokens) == len(scores) == len(edge_types), f"token_consumer: expected all lists to have the same length, but got {len(tokens)}, {len(scores)}, {len(edge_type)}"
+                        # print("setting entries for", edge_types)
+                    
+                    waiting_token_keys = []
+                    
+                    async with self.cache_lock:
+                        for token, score, edge_type in zip(tokens, scores, edge_types):
+                            assert type(edge_type) is str, "edge_types is {}".format(edge_types)
+                            if ids is None:
+                                ids = s.input_ids
+                                keys = await self.get_keys(s, edge_type, **self.model_args)
+                                sq = s
+                            token_keys = [(self.base_key(ids), edge_type, *k[2:]) for k in keys]
+                            token_keys += [(self.base_key(ids), str(token))]
+
+                            # for tk in token_keys:
+                            #     if tk in self.cache and type(self.cache[tk][0]) is not asyncio.Future:
+                            #         print("token_consumer: token for {} from stream already in cache ({} streams): {}".format(tk, len(self.token_streams), self.cache[tk]))
+
+                            self.set_cache(token_keys, (np.array(token).reshape(1), np.array(score).reshape(1)), user_data=user_data)
+
+                            if self.show_speculative:
+                                c = Continuation(np.array(token), np.array(score), None)
+                                sq = sq.extend(c)
+
+                            # set future for next token (so get_cache can wait for it if needed)
+                            fut_keys = [(self.base_key(ids), edge_type, *k[2:]) for k in keys]
+                            waiting_token_keys.append(fut_keys)
+                            # set future for next token (if k is not already set)
+                            fut = asyncio.Future()
+                            unset_keys = [k for k in fut_keys if k not in self.cache]
+                            self.set_cache(unset_keys, (fut, fut))
+
+                    # extend ids
+                    ids = np.append(ids, tokens[0])
+                        # print(waiting_token_keys)
+                
+                # remove last waiting token entry (since it will not be provided by this stream)
+                for future_keys in waiting_token_keys:
+                    for k in future_keys:
+                        fut = self.cache.get(k, (None, None))[0]
+                        if type(fut) is asyncio.Future:
+                            # resolve future as invalid (handled in get_cache)
+                            fut.set_result(None)
+                            del self.cache[k]
+            except Exception as e:
+                print("DcCachedModel: token_consumer failed with:", e)
+                import traceback
+                traceback.print_exc()
+                raise e
 
-    async def rewrite(self, ar: Union[DataArray, List[DecoderSequence], DecoderSequence], noscore=False):
-        """
-        Applies the active rewriting strategy (e.g. the LMQL interpreter) to the provided (array of) sequences.
+        self.token_streams = [s for s in self.token_streams if not s.done()]
+        self.token_streams.append(asyncio.create_task(token_consumer(token_iterator)))
         
-        This may add, remove or change tokens in the sequence, including the EOS token.
+    async def wait_for_active_streams(self):
         """
-        if type(ar) is not DataArray:
-            return await self._rewrite_seq(ar)
-
-        async def op_rewrite(path, seqs):
-            """
-            Rewrites the sequences in the pool using the rewriting strategy provided in kwargs.
-
-            If no rewriting strategy is provided, no rewriting is performed.
-            """
-            return path, await self._rewrite_seq(seqs, noscore=noscore)
-        
-        with stats.timer("rewrite"):
-            result_items = await asyncio.gather(*[op_rewrite(path, seqs) for path, seqs in ar.sequences.items()])
-        return DataArray(dict(result_items))
-
-DcModel.batch_size = 1
-
-
-def model(model=None, **kwargs) -> DcModel:
-    if "dcmodel" in kwargs:
-        return kwargs["dcmodel"]
-    if issubclass(type(model), DcModel):
-        model.model_args = {**model.model_args, **kwargs}
-        return model
-    return DcModel(model, **kwargs)
-
-def tokenizer(name, tokenize, detokenize, bos_token_id, eos_token_id):
-    class AsyncTokenizer:
-        def __init__(self, eos_token_id, bos_token_id):
-            self.name = name
-            self.eos_token_id = eos_token_id
-            self.bos_token_id = bos_token_id
-        async def __call__(self, text):
-            return await tokenize(text)
-        async def decode(self, tokens):
-            return await detokenize(tokens)
-    return AsyncTokenizer(eos_token_id=eos_token_id, bos_token_id=bos_token_id)
-
-def _stripped_ids(seqs, seqidx, strip_eos):
-    if strip_eos == True:
-        return seqs[seqidx].input_ids[:-1]
-    elif type(strip_eos) is list:
-        sequence_strip = strip_eos[seqidx]
-        if sequence_strip == True:
-            return seqs[seqidx].input_ids[:-1]
-        elif type(sequence_strip) is int:
-            return seqs[seqidx].input_ids[:sequence_strip] 
-        else:
-            return seqs[seqidx].input_ids
-    else:
-        return seqs[seqidx].input_ids
-
-def get_strip_eos(seqidx, strip_eos):
-    if strip_eos == True: return True
-    elif type(strip_eos) is list:
-        sequence_strip = strip_eos[seqidx]
-        if sequence_strip == True: return True
-        elif type(sequence_strip) is int: return True
-        else: return False
-    else: return False
+        Waits until all active cache streams have been processed.
+        """
+        caches = self.token_streams
+        # remove all done cache streams
+        self.token_streams = [f for f in self.token_streams if not f.done()]
+        return await asyncio.gather(*caches)
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         return {
             "nodes": nodes,
             "edges": self.edges
         }
 
 class DecoderSequence:
-    def __init__(self, input_ids_or_str, logprobs=None, deterministic=None, stop_phrase=None, predecessor=None, user_data=None, sticky_user_data_keys=None, epsilon_node=False):
+    def __init__(self, input_ids_or_str, logprobs=None, deterministic=None, stop_phrase=None, predecessor=None, user_data=None, sticky_user_data_keys=None, epsilon_node=False, internal=False):
         assert all([p > DecoderSequence.truncation_threshold for p in logprobs]) if logprobs is not None else True
 
         if type(input_ids_or_str) == str:
             assert False, "constructing dc.seq() directly from string is not supported anymore"
         elif type(input_ids_or_str) == list:
             input_ids = np.array(input_ids_or_str)
         else:
@@ -146,15 +146,15 @@
         return self._id
 
     def __new__(cls, *args, **kwargs):
         s = super().__new__(cls)
 
         setattr(s, "_id", f"s_{DecoderSequence.seq_ctr}")
 
-        if DecoderSequence.graph is not None:
+        if DecoderSequence.graph is not None and not kwargs.get("internal"):
             DecoderSequence.graph.add_node(s)
 
             predecessor = kwargs.get("predecessor")
             if predecessor is not None:
                 DecoderSequence.graph.add_edge(predecessor, s)
         
         DecoderSequence.seq_ctr += 1
@@ -287,43 +287,50 @@
 
     def extend_user_data(self, continuation=None, user_data=None):
         assert continuation is None or user_data is None, f"continuation and user_data are mutually exclusive arguments"
         # prepares the user_data dictionary to use with sucessor sequences
         if continuation is None and user_data is None:
             user_data = {}
         elif continuation is not None:
-            user_data = deepcopy(continuation.user_data)
+            if type(continuation.user_data) is list:
+                assert len(continuation.user_data) == 1, f"continuation.user_data is a list of length {len(continuation.user_data)} but should be a list of length 1"
+                user_data = deepcopy(continuation.user_data[0])
+            else:
+                user_data = deepcopy(continuation.user_data)
         elif user_data is not None:
             user_data = deepcopy(user_data)
         else:
             user_data = deepcopy(continuation.user_data)
         for sk in self.sticky_user_data_keys:
             if user_data is None:
                 user_data = {}
             set_path(user_data, sk, self.data(sk), create_missing=True, replace=False)
         return user_data
 
-    def extend(self, continuation):
+    def extend(self, continuation, internal=False):
         stop_phrase = self.detect_stop_phrase(continuation)
+
         return DecoderSequence(
             input_ids_or_str=np.concatenate([self.input_ids, continuation.token.reshape(1)]), 
             logprobs=np.concatenate([self.logprobs, continuation.logprob.reshape(1)]),
             # deterministic tokens are only extended in DeterministicDecoderSequence.extend.
             # So here, all extended tokens are non-deterministic, i.e. model predictions.
             deterministic=np.concatenate([self.deterministic, np.array([False])]),
             stop_phrase=stop_phrase,
             predecessor=self,
             user_data=self.extend_user_data(continuation),
-            sticky_user_data_keys=self.sticky_user_data_keys
+            sticky_user_data_keys=self.sticky_user_data_keys,
+            internal=internal
         )
 
     def detect_stop_phrase(self, continuation):
         old_stop_phrase = self.stop_phrase
         new_stop_phrase = np.concatenate([old_stop_phrase, np.array([False])])
-        stop_phrases = self.data("head").stopping_phrases["tokenized"]
+        
+        stop_phrases = self.data("head").stopping_phrases["tokenized"] if self.data("head") is not None else []
 
         if stop_phrases is None:
             return new_stop_phrase
 
         ids = np.concatenate([self.input_ids, continuation.token.reshape(1)]),
         for stop in stop_phrases:
             len_stop = len(stop)
@@ -422,21 +429,22 @@
         if k in a and isinstance(a[k], dict) and isinstance(b[k], dict):
             deepmerge(a[k], b[k])
         else:
             a[k] = b[k]
     return a
 
 class DeterministicDecoderSequence(DecoderSequence):
-    def __init__(self, input_ids, logprobs, deterministic, stop_phrase, next_ids, next_logprobs=None, next_deterministic=None, predecessor=None, user_data=None, needs_rewrite=False, sticky_user_data_keys=None):
-        super().__init__(input_ids, logprobs, deterministic, stop_phrase, predecessor, user_data=user_data.copy() if user_data is not None else None, sticky_user_data_keys=sticky_user_data_keys)
+    def __init__(self, input_ids, logprobs, deterministic, stop_phrase, next_ids, next_logprobs=None, next_deterministic=None, predecessor=None, user_data=None, needs_rewrite=False, sticky_user_data_keys=None, internal=False):
+        super().__init__(input_ids, logprobs, deterministic, stop_phrase, predecessor, user_data=user_data.copy() if user_data is not None else None, sticky_user_data_keys=sticky_user_data_keys, internal=internal)
         self.next_ids = next_ids
         self.next_logprobs = next_logprobs
         self.next_deterministic = next_deterministic
 
         self.needs_rewrite = needs_rewrite
+        self.internal = internal
 
         if next_logprobs is not None: assert len(next_logprobs) == len(next_ids), "Length of deterministic continuation did not match length of provided logprobs"
         if next_deterministic is not None: assert len(next_deterministic) == len(next_ids), "Length of determinism status did not match length of provided logrprobs"
 
         self.align_user_data()
 
     # async def text(self, offset: int = None, limit: int = None, pretty=True) -> str:
@@ -513,15 +521,15 @@
             s = s.extend(Continuation(s.next_ids[0], s.next_logprobs[0], s.user_data))
         return s
 
     def extend_user_data(self, continuation=None, user_data=None):
         # additionally add self.user_data for deterministic sequence extensions
         return deepmerge(deepcopy(self.user_data), super().extend_user_data(continuation=continuation, user_data=user_data))
 
-    def extend(self, continuation):
+    def extend(self, continuation, internal=False):
         # if not more predetermined tokens are left, just extend as usual and return a regular seq()
         if len(self.next_ids) <= 0:
             return super().extend(continuation)
 
         assert continuation.token == self.next_ids[0], "deterministic sequences must be extended by the predetermined next token: provided: " + str(continuation.token) + ", predetermined: " + str(self.next_ids[0])
 
         extended_input_ids = np.concatenate([self.input_ids, continuation.token.reshape(1)])
@@ -547,14 +555,15 @@
             next_ids=reduced_next_ids,
             next_logprobs=reduced_next_logprobs,
             next_deterministic=reduced_deterministic,
             predecessor=self, 
             user_data=user_data,
             needs_rewrite=self.needs_rewrite,
             sticky_user_data_keys=self.sticky_user_data_keys,
+            internal=internal or self.internal
         )
 
     def __repr__(self) -> str:
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         if (len(self.next_ids) > 0): 
             ids = "... " + ids
         next_ids = ", ".join([str(i) for i in self.next_ids[:10]])
@@ -621,28 +630,30 @@
     stop_phrase: np.ndarray,
     next_ids: List[int],
     next_logprobs: List[float] = None,
     next_deterministic: Optional[np.ndarray] = None,
     predecessor=None, 
     user_data=None,
     needs_rewrite=True,
-    sticky_user_data_keys=None):
+    sticky_user_data_keys=None,
+    internal=False):
     
     return DeterministicDecoderSequence(
         input_ids=ids, 
         logprobs=logprobs, 
         deterministic=deterministic,
         stop_phrase=stop_phrase,
         next_ids=next_ids,
         next_logprobs=next_logprobs,
         next_deterministic=next_deterministic,
         predecessor=predecessor, 
         user_data=user_data,
         needs_rewrite=needs_rewrite,
         sticky_user_data_keys=sticky_user_data_keys,
+        internal=internal
     )
 
 def seq(ids: List[int], logprobs:Optional[np.ndarray]=None, deterministic:Optional[np.ndarray]=None):
     return DecoderSequence(ids, logprobs=logprobs, deterministic=deterministic)
 
 def named(seqs: List[DecoderSequence] = None, name=None):
     for s in seqs:
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6/src/lmql/runtime/dclib/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     done = dc.seqs()
     step = 0
     
     # provide early first result to user
     yield h
 
     while len(h) > 0:
-        h = h.extend(await model.argmax(h))
+        h = h.extend(await model.argmax(h, noscore=True))
         h = await model.rewrite(h, noscore=True)
         h, done = (h + done).separate_by(dc.logical_not(dc.eos), dc.lt(max_len))
         
         step += 1
 
         yield (h, done)
 
@@ -32,15 +32,15 @@
 @dc.decoder
 async def sample(prompt_ids: np.ndarray, temperature=1, n=1, max_len=2048, **kwargs):
     model = dc.model(**kwargs)
     h = dc.seqs([dc.seq(prompt_ids)] * n)
     done = dc.seqs()
 
     while len(h) > 0:
-        h = h.extend(await model.sample(h, temperature=temperature))
+        h = h.extend(await model.sample(h, temperature=temperature, noscore=True))
         h = await model.rewrite(h, noscore=True)
         h, done = (h + done).separate_by(dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len)))
 
         yield (h, done)
     
     yield (h, done)
 
@@ -126,21 +126,23 @@
         h = await model.rewrite(h)
         h, done = (h + done).separate_by(not_done)
 
         h = dc.topk(h, n, name = "h_" + str(num_steps))
         done = dc.topk(done, n, name = "done_" + str(num_steps))
 
         # stop when done already tracks topk results
-        if len(done) == n and dc.max_score(h) < dc.min_score(done):
+        if len(done) == n and (len(h) == 0 or dc.max_score(h) < dc.min_score(done)):
             break
 
         yield (h, done)
     
     yield (h, done)
 
+    dc.finish(done)
+
 @dc.decoder
 async def beam_search(prompt_ids: np.ndarray, n=4, max_len=None, **kwargs):
     n = kwargs.get("num_beams", n)
     max_len = max_len or 2048
     model = dc.model(**kwargs)
 
     # keep track of active beams and finished sequences
@@ -150,15 +152,15 @@
 
     # stopping criteria for the beam search
     not_done = dc.logical_and(dc.logical_not(dc.eos), dc.lt(max_len))
 
     for num_steps in range(0, max_len):
         if len(h) == 0: break
 
-        h = h.extend(await model.topk_continuations(h, k=n))
+        h = h.extend(await model.topk_continuations(h, k=n, **kwargs))
         h = await model.rewrite(h)
         h, done = (h + done).separate_by(not_done)
 
         h = dc.topk(h, n, name = "h_" + str(num_steps))
         done = dc.topk(done, n, name = "done_" + str(num_steps))
 
         # stop when done already tracks topk results
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/dclib/trie_cache.py` & `lmql-0.0.6/src/lmql/runtime/dclib/trie_cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/hf_integration.py` & `lmql-0.0.6/src/lmql/runtime/hf_integration.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/interpreter.py` & `lmql-0.0.6/src/lmql/runtime/interpreter.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, List, Union, NamedTuple
 import numpy as np
 from lmql.runtime.multi_head_interpretation import InterpretationHead, InterpreterCall, InterpretationHeadDone
 from lmql.runtime.program_state import ProgramState
 import lmql.runtime.dclib as dc
 from lmql.runtime.stats import Stats
+from lmql.runtime.tokenizer import LMQLTokenizer
 from lmql.runtime.interrupt import interrupt
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, DistributionVariable
 from lmql.utils.nputil import replace_inf_nan_with_str
 
-from lmql.ops.token_set import VocabularyMatcher
+from lmql.ops.token_set import VocabularyMatcher, has_tail
 from lmql.runtime.model_registry import LMQLModelRegistry
 
 from lmql.ops.token_set import tset
 import lmql.ops.ops as ops
 
 class _DCLibDebugPrinter: pass
 _DCLibDebugPrinter.printer = None
@@ -135,19 +136,22 @@
 
     def __init__(self, force_model=None) -> None:
         assert force_model is None, "force_model is not supported in P2"
         
         # model-specific components
         self.model = None
         self.model_identifier = None
-        self.tokenizer = None
+        self.tokenizer: LMQLTokenizer = None
 
         # decoder configuration
         self.decoder = None
-        self.decoder_kwargs = None
+        self.decoder_kwargs = {}
+        
+        # extra interpreter flags passed via @lmql.query/@lmql.compiled_query
+        self.extra_kwargs = {}
 
         # query program
         self.fct = None
         self.root_state = None
 
         # constraints
         self.where = None
@@ -155,18 +159,28 @@
         # distribution variable if any
         self.distribution_variable = None
         self.distribution_values = None
 
         # logging and debugger output
         self.output_writer = None
         self.prefers_compact_mask  = False
+        self.caching = True
+        self.cache_file = None
+        self.show_speculative = False
+        
+        self.eager_followmap_expansion = True
 
     def set_where_clause(self, where):
         self.where = where
 
+    def set_extra_args(self, **kwargs):
+        if "output_writer" in kwargs:
+            self.output_writer = kwargs["output_writer"]
+        self.extra_kwargs.update(kwargs)
+
     def set_decoder(self, method, **kwargs):
         self.decoder_kwargs = kwargs
         self.decoder_kwargs["decoder"] = method
 
     def set_model(self, model_name):
         self.model = model_name
         self.model_identifier = model_name
@@ -180,15 +194,15 @@
         if self.model.startswith("openai/"):
             self.prefers_compact_mask = True
 
         self.model = client
 
     async def advance(self, state: PromptState):
         if state.variable is not None:
-            return
+            return state
         
         variable = state.variable
         stmt_buffer = state.stmt_buffer
         prompt = state.prompt
 
         distribution_variable = None
         distribution_values = None
@@ -269,18 +283,76 @@
                 return None
         state_dict = seq.data("head")
         if state_dict is None and not noroot:
             return self.root_state
         return state_dict
 
     async def where_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, **kwargs):
+        mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, **kwargs)
+
+        # check for tail and prescore
+        if hasattr(self.dcmodel, "prescore_tokens"):
+            if has_tail(mask):
+                tail_tokenized = self.tokenizer(mask.tail)["input_ids"]
+                await self.dcmodel.prescore_tokens(s, tail_tokenized, noscore=kwargs.get("noscore", False))
+        
+        return logit_mask, state
+
+        # eager follow map expansion (w/o) model prediction in between
+
+        # # if we cannot predict the next token deterministically
+        # if mask is None or len(mask) > 1 or not needs_masking:
+        #     # ask the model to predict the next token
+        #     return logit_mask, state
+
+        # # otherwise, we can expand the sequence deterministically, until a probabilistic token mask is encountered
+        # masks = [mask]
+        # logit_masks = [logit_mask]
+        # states = [state]
+
+        # #  checks if current mask can be expanded further
+        # mask_can_be_expanded_further = lambda: mask is not None and len(mask) == 1 and mask.mask.argmax() != self.model.get_tokenizer().eos_token_id
+
+        # unexpanded_offset = len(s.input_ids)
+        # initial_s = s
+
+        # # expand as far as possible
+        # while mask_can_be_expanded_further() and self.eager_followmap_expansion:
+        #     # extend the sequence with the next token
+        #     s = s.extend(dc.Continuation(mask.mask.argmax(), np.array([0]), None), internal=True)
+        #     # do not futher expand sequences at <eos>
+        #     if s.is_done(): break
+
+        #     # rewrite to get next-token user data and set it on the sequence
+        #     rewrite_result: RewrittenInputIds = await self.rewrite_for_sequence(s, True, assert_no_advance=True)
+        #     s.user_data = rewrite_result.user_data
+        #     s.user_data["set_by"] = "rewrite"
+
+        #     # call another step of where_for_sequence
+        #     mask, logit_mask, state = await self.where_step_for_sequence(s, needs_masking, seqidx, **kwargs)
+
+        #     if mask_can_be_expanded_further():
+        #         # save the current mask
+        #         masks.append(mask)
+        #         logit_masks.append(logit_mask)
+        #         states.append(state)
+
+        # # pre-score the expanded sequences
+        # if len(s.input_ids) - unexpanded_offset > 0:
+        #     num_to_score = len(s.input_ids) - unexpanded_offset
+        #     if hasattr(self.dcmodel, "prescore"):
+        #         await self.dcmodel.prescore([initial_s], [s.input_ids[-num_to_score:]], deterministic=[[False] * num_to_score], user_data=[states[-num_to_score:]], noscore=kwargs.get("noscore", False))
+
+        # return logit_masks[0], states[0]
+
+    async def where_step_for_sequence(self, s: dc.DecoderSequence, needs_masking, seqidx, **kwargs):
         state = self.interpreter_state_from_user_data(s)
         
         if not needs_masking:
-            return None, self.interpreter_state_user_data(state)
+            return None, None, self.interpreter_state_user_data(state)
 
         is_done = state.query_head.result is not None
 
         # default results (if no where clause is run)
         valid = True
         is_final = "var"
         program_state = state.program_state.copy()
@@ -292,14 +364,15 @@
 
         text = ""
 
         if is_done:
             mask = tset("eos")
             logit_mask = mask.mask
             stopping_phrases = {"text": [], "tokenized": []}
+            follow_trace = None
         elif variable is not None:
             if ":before" in variable:
                 variable = variable.split(":before",1)[0]
 
             text = await s.text(variable_offset, pretty=False)
             diff_text = text[len(await s.text(variable_offset, limit=-1, pretty=False)):]
 
@@ -345,20 +418,23 @@
                         program_state=program_state,
                         stopping_phrases=stopping_phrases,
                         where=await self.where_graph_with_trace(trace, follow_trace)
         )
 
         # no mask, no logits processing
         if logit_mask is None:
-            return None, self.interpreter_state_user_data(state)
+            return None, None, self.interpreter_state_user_data(state)
         
         # translate boolean mask to logit bias mask
-        logit_mask = np.logical_not(logit_mask) * np.finfo(np.float32).min
+        if len(mask) == 1:
+            logit_mask = mask.mask.argmax()
+        else:
+            logit_mask = np.logical_not(logit_mask) * np.finfo(np.float32).min
         
-        return logit_mask, self.interpreter_state_user_data(state)
+        return mask, logit_mask, self.interpreter_state_user_data(state)
 
     async def where_graph_with_trace(self, trace, follow_trace):
         from lmql.utils.graph import CytoscapeGraphWriter
 
         def node_data(op):
             result = "-"
             follow_map = "-"
@@ -385,15 +461,15 @@
     async def where_processor(self, seqs, additional_logits_processor_mask, **kwargs):
         zipped_task_inputs = zip(seqs, additional_logits_processor_mask, range(len(seqs)))
         token_mask_tasks = [self.where_for_sequence(s, needs_masking, seqidx, **kwargs) for s,needs_masking, seqidx in zipped_task_inputs]
         results = [(mask, user_data) for mask, user_data in await asyncio.gather(*token_mask_tasks)]
         
         return TokenMask([r[0] for r in results], [r[1] for r in results])
 
-    async def rewrite_for_sequence(self, seq: dc.DecoderSequence, needs_rewrite):
+    async def rewrite_for_sequence(self, seq: dc.DecoderSequence, needs_rewrite, assert_no_advance=False):
         if not needs_rewrite:
             return None
 
         # obtain interpreter state from predecessor node
         state = self.interpreter_state_from_user_data(seq.predecessor, noroot=True)
         
         assert state is not None, "prompt interpreter state must be set in predecessor node"
@@ -424,15 +500,16 @@
             prompt_length_before = len(prompt) # prompt without current variable
             old_prompt = prompt + text # prompt with current variable in raw form
             prompt += postprocessed_prompt # prompt with current variable in postprocessed form
             
             appended_value_prompt = prompt[prompt_length_before:]
 
             #  advance to next variable in prompt program (appends intermediate instructions to prompt)
-            
+            assert not assert_no_advance, f"error: prompt interpreter tried to advance query program even though assert_no_advance was set"
+
             state = state.updated(variable=variable, prompt=prompt, program_state=program_state)
             while state.variable is None and state.query_head.result is None:
                 state = await self.advance(state)
             reached_end = state.query_head.result is not None
             
             prompt = state.prompt
 
@@ -535,14 +612,19 @@
         self.tokenizer = self.model.get_tokenizer()
 
         assert issubclass(type(self.dcmodel), dc.DcModel), "The provided dcmodel must be a subclass of DcModel"
 
         if "no_repeat_ngram_size" in decoder_args:
             print("warning: no_repeat_ngram_size is known to cause issues when used with constrained decoding, including non-termination.")
 
+        # alternative mode where we only extract the prompt string
+        return_prompt_string = self.extra_kwargs.pop("return_prompt_string", False)
+        if return_prompt_string:
+            return self.root_state.prompt
+
         # tokenize initial prompt
         prompt_ids = await self.tokenize(self.root_state.prompt)
         if self.dcmodel.bos_token_id is not None:
             prompt_ids = [self.dcmodel.bos_token_id] + prompt_ids
         n = len(prompt_ids)
         
         # make sure that the initial prompt is not considered part of a variable
@@ -569,70 +651,95 @@
         mode = decoder_args["decoder"].lower()
         decoder_fct = dc.get_decoder(mode)
         self.validate_args(decoder_args, decoder_fct)
 
         # alias max_length -> max_len
         if "max_length" in decoder_args:
             decoder_args["max_len"] = decoder_args["max_length"]
+        if not "max_len" in decoder_args.keys():
+            decoder_args["max_len"] = 2048
+        
+        # parse show_speculative argument
+        if "show_speculative" in decoder_args.keys():
+            self.show_speculative = decoder_args.pop("show_speculative")
+            assert self.caching, "warning: show_speculative is only supported when caching is enabled."
+
+        # parse cache argument
+        if "cache" in decoder_args.keys():
+            cache_value = decoder_args.pop("cache")
+            if type(cache_value) is bool:
+                if cache_value == False:
+                    print("info: disabling model output caching")
+                self.caching = cache_value
+            elif type(cache_value) is str:
+                self.caching = True
+                self.cache_file = cache_value
+            else:
+                assert False, "Invalid value for 'cache' parameter. Expected either a boolean (to enable/disable) or a string (to enable with a disk-based cache file)"
 
         # setup dcmodel for use
         self.dcmodel.model_args = decoder_args
+        if self.caching:
+            self.dcmodel = dc.CachedDcModel(self.dcmodel, prompt_ids, cache_file=self.cache_file, show_speculative=self.show_speculative)
         decoder_args["dcmodel"] = self.dcmodel
         dc.set_truncation_threshold(self.dcmodel.truncation_threshold)
 
-        step_budget = decoder_args.get("step_budget", 1024)
+        assert len(prompt_ids) < decoder_args["max_len"], "The initial prompt already exceeds the provided max_len. Please increase the max_len or reduce the initial prompt (Initial prompt: '{}', max_len: {})".format(len(prompt_ids), decoder_args["max_len"])
+
+        # set step budget at least to max_len
+        step_budget = decoder_args.get("step_budget", max(1024, decoder_args.get("max_len", 1024)))
         
         async def debug_out(decoder_step):
             if _DCLibDebugPrinter.printer is not None and dc.DecoderSequence.graph is not None:
                 data = await dc.DecoderSequence.graph.json(diff=True)
                 data = replace_inf_nan_with_str(data)
                 _DCLibDebugPrinter.printer.add_decoder_state(data)
             self.dcmodel.report_stats(_DCLibDebugPrinter.printer, decoder_step)
 
         try:
             import time
 
-            decoder_step = 0
+            self.decoder_step = 0
             average_step_time = None
             start = time.time()
             async for _ in decoder_fct(prompt_ids, **decoder_args):
-                await debug_out(decoder_step)
-                decoder_step += 1
+                await debug_out(self.decoder_step)
+                self.decoder_step += 1
 
-                if step_budget is not None and decoder_step >= step_budget:
+                if step_budget is not None and self.decoder_step >= step_budget:
                     print("warning: step budget exceeded")
                     break
 
                 if interrupt.check():
                     interrupt.clear()
                     raise InterruptedError("lmql.runtime.interrupt")
                 
                 average_step_time = (time.time() - start) if average_step_time is None else (average_step_time * 0.9 + (time.time() - start) * 0.1)
 
                 if "performance_stats" in decoder_args:
-                    if decoder_step % 10 == 0:
+                    if self.decoder_step % 10 == 0:
                         Stats.print_all()
-                        print("step", decoder_step, "time", average_step_time)
+                        print("step", self.decoder_step, "time", average_step_time)
 
                 start = time.time()
             
             assert False, "decoder {} did not finish with dc.finish(), which means no result sequences were returned. \n\nThe reason for this may be a too small max_len value (max_len={}) ".format(decoder_args["decoder"], decoder_args["max_len"])
                 
         except dc.FinishException as fe:
             # one last call to debug_out to get the final state
-            await debug_out(decoder_step)
+            await debug_out(self.decoder_step)
             # if dc.finish is used, the decoder sets the sequences it considers 
             # finished (return them to prompt interpreter)
             result_sequences = fe.result_sequences
             
             billable_tokens = 0
             for s in result_sequences:
                 upper = len(s.input_ids)
                 has_deterministic_tail = False
-                while s.deterministic[upper-1]:
+                while s.deterministic[upper-1] and upper >= 0:
                     upper -= 1
                     has_deterministic_tail = True
                 # +1 for the eos token
                 billable_tokens += upper + (1 if has_deterministic_tail else 0)
             
             self.dcmodel.log_billable_tokens(billable_tokens)
 
@@ -640,24 +747,34 @@
 
             for i,s in enumerate(result_sequences):
                 state = self.interpreter_state_from_user_data(s)
                 if state.query_head.result is not None:
                     results.append(state.query_head.result)
                 else:
                     state = await self.advance(state)
+                    assert len(s.input_ids) < decoder_args["max_len"], "The decoder returned a sequence that exceeds the provided max_len (max_len={}, sequence length={}). To increase the max_len, please provide a corresponding max_len argument to the decoder function.".format(decoder_args["max_len"], len(s.input_ids))
+
                     assert state.query_head.result is not None, "decoder designates sequence {} as finished but the underyling query program has not produced a result. This is likekly a decoder bug. Decoder in use {}".format(await s.str(), decoder_args["decoder"])
                     results.append(state.query_head.result)
             
+            # set decoder step +1, for all stats logging that happens in postprocessing
+            self.decoder_step += 1
+
             return results
+        finally:
+            # make sure token cache is saved if possible
+            self.dcmodel.save()
+            if hasattr(self.dcmodel, "close"):
+                self.dcmodel.close()
 
     def validate_args(self, decoder_args, decoder_fct):
-        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats"]
+        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", "show_speculative"]
 
         # get all arg names and kwarg names of decoder function
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
 
     def print_stats(self):
-        pass
+        self.dcmodel.report_stats(self.output_writer, self.decoder_step)
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/langchain.py` & `lmql-0.0.6/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6/src/lmql/runtime/lmql_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,18 @@
         else:
             return super().__call__(*args, **kwargs)
 
     async def __acall__(self, *args, **kwargs):
         kwargs = self.make_kwargs(*args, **kwargs)
 
         interpreter = PromptInterpreter(force_model=self.model)
-        if self.output_writer is not None:
-            interpreter.output_writer = self.output_writer
+        interpreter.set_extra_args(
+            output_writer = self.output_writer,
+            **kwargs
+        )
 
         query_kwargs = {}
         for a in self.args:
             if a in kwargs.keys():
                 query_kwargs[a] = kwargs[a]
             else:
                 query_kwargs[a] = self.scope.resolve(a)
@@ -146,14 +148,15 @@
 
         # apply remaining postprocessors
         if self.postprocessors is not None:
             for postprocessor in self.postprocessors:
                 results = await postprocessor.process(results, self.output_writer)
         
         interpreter.print_stats()
+        interpreter.dcmodel.save()
 
         return results
 
 def context_call(fct_name, *args, **kwargs):
     return ("call:" + fct_name, args, kwargs)
 
 def interrupt_call(fct_name, *args, **kwargs):
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/model_registry.py` & `lmql-0.0.6/src/lmql/runtime/model_registry.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6/src/lmql/runtime/openai_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import os
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import Any, Callable, List, Optional, Union
 
 import numpy as np
 
+import lmql.runtime.masks as masks
 import lmql.runtime.bopenai as openai
 import lmql.runtime.dclib as dc
+import lmql.utils.nputil as nputil
 from lmql.runtime.dclib.dclib_model import DcModel
 from lmql.runtime.dclib.dclib_seq import (DecoderSequence, deepcopy, deepmerge,
                                           detseq, is_deterministic)
 from lmql.runtime.stats import Stats
 from lmql.runtime.tokenizer import load_tokenizer
 from lmql.utils import nputil
 
@@ -110,16 +112,14 @@
         self.model_identifier = "openai/" + self.model.model_identifier
 
         self.model.chunk_size = kwargs.get("openai_chunksize", 64)
         self.num_billed_tokens = {}
         self.num_requests = 0
 
         self.stats = Stats("openai")
-
-        # openai.Completion.set_chaos(0.05) # for unreliably testing
         openai.AsyncConfiguration.set_tokenizer(self.tokenize)
 
     def log_billable_tokens(self, n: int):
         pass # openai keeps track of billable tokens vai bopenai
     
     def log_queries(self, n: int):
         pass # openai keeps track of queries via bopenai
@@ -136,26 +136,26 @@
         """
         stopping_phrases = s.data("head").stopping_phrases["text"]
 
         if mask is None:
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         invert = False
-        num_allowed = is_allowed(mask).sum(axis=-1)
-        assert num_allowed > 0, "DclibOpenAiModel: encountered logits mask with no allowed tokens"
+        num_allowed = masks.mask_num_allowed(mask)
+        assert num_allowed > 0, "DclibOpenAiModel: encountered logits mask with no allowed tokens: mask: {} mask type:{}".format(mask, type(mask))
 
         if num_allowed == 1:
             # check for <eos> case
-            if is_allowed(mask[self.eos_token_id]):
+            if masks.mask_is_allowed(mask, self.eos_token_id):
                 return CompletionCall("fixed", self.eos_token_id, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
             else:
                 # otherwise we can treat this as a score call
-                return CompletionCall("fixed", mask.argmax(axis=-1), s.input_ids, kwargs, stopping_phrases=stopping_phrases)
-        elif num_allowed < mask.shape[-1]:
-            if mask.shape[-1] - num_allowed > num_allowed:
+                return CompletionCall("fixed", masks.mask_get_only_allowed(mask), s.input_ids, kwargs, stopping_phrases=stopping_phrases)
+        elif num_allowed < self.tokenizer.vocab_size:
+            if self.tokenizer.vocab_size - num_allowed > num_allowed:
                 # if we have to mask more than half of the tokens, we should just invert the masking
                 invert = True
         else: # num_allowed == mask.shape[-1] (full vocabulary)
             return CompletionCall("*", None, s.input_ids, kwargs, stopping_phrases=stopping_phrases)
 
         # num_allowed < mask.shape[-1] and num_allowed > 1 (needs mask)
         return CompletionCall("complete", mask, s.input_ids, kwargs, invert=invert, stopping_phrases=stopping_phrases)
@@ -184,56 +184,63 @@
         return await result_fut
 
     async def _score_next_tokens(self, s, next_tokens, noscore=False):
         if noscore:
             return np.zeros(len(next_tokens), dtype=np.float32)
         return (await self.api_score(np.concatenate([s.input_ids, next_tokens], axis=0), len(s.input_ids)))
     
-    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False):
+    async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
         assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
-        
-        completion = [np.array(cont) for cont in tokens]
 
         def make_detseq(s, token_score, completion):
             # compose deterministic flags
             if type(deterministic) is bool:
                 deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
-                assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored"
+                assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
                 deterministic_flags = np.concatenate([s.deterministic, np.array(deterministic[:1])])
                 next_deterministic = np.array(deterministic[1:])
 
             return detseq(ids=np.concatenate([s.input_ids, completion[:1]], axis=0), 
                     next_ids=completion[1:],
                     logprobs=np.concatenate([s.logprobs, token_score[:1]], axis=0),
                     next_logprobs=token_score[1:],
                     deterministic=deterministic_flags,
                     next_deterministic=next_deterministic,
                     predecessor=s,
                     user_data=user_data,
                     stop_phrase=np.concatenate([s.stop_phrase, np.array([stop_phrase])]),
                     needs_rewrite=needs_rewrite,
-                    sticky_user_data_keys=s.sticky_user_data_keys)
+                    sticky_user_data_keys=s.sticky_user_data_keys,
+                    internal=internal
+            )
         results = []
 
-        for s,compl,result in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl, noscore=noscore) for s, compl in zip(sqs, completion)))):
-            results.append(make_detseq(s, result, compl))
+        async for (s, tokens, scores) in self.score_tokens(sqs, tokens, max_batch_size=max_batch_size, noscore=noscore):
+            results.append(make_detseq(s, scores, tokens))
 
         return results
+    
+    async def score_tokens(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, noscore=False):
+        completion = [np.array(cont) for cont in tokens]
+
+        for s, tokens,scores in zip(sqs, completion, await asyncio.gather(*(self._score_next_tokens(s, compl, noscore=noscore) for s, compl in zip(sqs, completion)))):
+            yield (s, tokens, scores)
 
     async def async_complete(self, completion_call: Union[CompletionCall, List[CompletionCall]], **kwargs) -> openai.response_buffer:
         assert type(completion_call) is CompletionCall
 
         batch_size = 1
         input_ids = completion_call.input_ids.reshape(-1)
         assert input_ids.ndim == 1, f"_complete expects input_ids to be a 1D tensor when only one completion_call is passed, got {input_ids.ndim}D tensor."
 
         temperature = completion_call.kwargs.get("temperature", 0.0)
         logprobs = completion_call.kwargs.get("logprobs", 5)
+        noscore = completion_call.kwargs.get("noscore", False)
 
         kwargs = {
             "model": self.model.model_identifier,
             "prompt": input_ids.tolist(), # no more batching at this point
             "max_tokens": self.model.chunk_size,
             "temperature": temperature,
             "logprobs": logprobs,
@@ -244,45 +251,55 @@
 
         mode = completion_call.mode
         
         if mode == "*": # complete without mask
             pass
         elif mode == "complete": # complete with mask
             logit_bias = completion_call.api_mask
+            # reduce chunk size, if logit mask seems very sparse
+            if len(logit_bias) > 0 and max(logit_bias.values()) == 100 and len(logit_bias) < 10:
+                kwargs["max_tokens"] = min(kwargs["max_tokens"], 4)
             kwargs.update({"logit_bias": logit_bias})
         elif mode == "fixed": # complete with fixed token
             fixed_next_token = completion_call.logit_mask_or_fixed_id # special return value case for prepare function
             # TODO revisit this, what kind of probability do we want here (masked or unmasked/scored)
             if fixed_next_token == self.eos_token_id:
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=0), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
             else:
                 fixed_next_token = nputil.ensure_array(fixed_next_token, dtype=np.int64)
-                logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids)))
+                if noscore: logprob = 0.0
+                else: logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids)))
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=logprob), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
         elif len(completion_call.stopping_phrases) > 0:
             if len(completion_call.stopping_phrases) > 4:
                 # same but blaming it more on OpenAI
                 print("warning: the number of stopping phrases that would need to be passed to the OpenAI API is greater than 4. Since the OpenAI API only supports up to 4 stopping phrases, the first 4 stopping phrases will be passed to the API. Other stopping phrases will also be enforced, but may lead to an increase in the number of tokens billed to the user.")
-            kwargs.update({"stop": completion_call.stopping_phrases[:4]})
+            # skip stopping phrases for more speculative execution
+            # kwargs.update({"stop": completion_call.stopping_phrases[:4]})
         else:
             assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
 
         # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
         self.count_billed_tokens(input_ids.size + kwargs.get("max_tokens") * batch_size, self.model_identifier)
         
         if self.model_args.get("chatty_openai", False):
-            print("Completion with", kwargs)
+            args = kwargs.copy()
+            args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
+            print(f"openai complete: {args}")
 
         return CompletionResult((await openai.async_buffer(await openai.Completion.create(**kwargs), tokenizer=self.tokenize_list))[input_ids.size:], completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
     
     async def tokenize_list(self, tokens: List[str]):
         if len(tokens) > 0 and type(tokens[0]) is str:
             return [[t[0]] for t in await self.model.tokenize(tokens)]
         return tokens
     
+    async def openai_cache_delegate(self, kwargs, tokens, scores):
+        print(tokens, scores, self.cache_delegate)
+
     async def _complete(self, completion_call: Union[CompletionCall, List[CompletionCall]], **kwargs):
         if type(completion_call) is list:
             input_ids = np.stack([c.input_ids for c in completion_call], axis=0)
             assert input_ids.ndim == 2, f"_complete expects input_ids to be a 1D tensor per completion call, when multiple completion calls are passed, got {input_ids.ndim}D tensor."
             # all other call parameters are assumed to be the same
             batch_size = len(completion_call)
             completion_call = completion_call[0]
@@ -321,15 +338,15 @@
                     fixed_next_token = np.array(fixed_next_token)
                 logprob = (await self.api_score(np.concatenate([input_ids, fixed_next_token.reshape(1)], axis=0), len(input_ids))).result
                 return OpenAIModelOutputBuffer.fixed_output(fixed_next_token, logprob)
         elif len(completion_call.stopping_phrases) > 0:
             if len(completion_call.stopping_phrases) > 4:
                 # same but blaming it more on OpenAI
                 print("warning: the number of stopping phrases that would need to be passed to the OpenAI API is greater than 4. Since the OpenAI API only supports up to 4 stopping phrases, the first 4 stopping phrases will be passed to the API. Other stopping phrases will also be enforced, but may lead to an increase in the number of tokens billed to the user.")
-            kwargs.update({"stop": completion_call.stopping_phrases[:4]})
+            # kwargs.update({"stop": completion_call.stopping_phrases[:4]})
         else:
             assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
 
         # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
         self.count_billed_tokens(input_ids.size + kwargs.get("max_tokens") * batch_size, self.model_identifier)
         
         if self.model_args.get("chatty_openai", False):
@@ -382,20 +399,76 @@
             if is_deterministic(s) and len(s.next_ids) > 0:
                 return CompletionResult(
                     openai.response_buffer.singleton(token=s.next_ids[0], token_logprob=s.next_logprobs[0]),
                     None,
                     None,
                 )
 
-            return await self.async_complete(completion_call)
+            completion_result = await self.async_complete(completion_call)
+            # eagerly expand and cache full completion if a cache_delegate is available
+            if self.cache_delegate is not None:
+                await self.expand_and_cache(s, completion_result, "top-1", logprobs=kwargs.get("logprobs", 1))
+            return completion_result
 
         return await asyncio.gather(*[get_buffer(i, s) for i, s in enumerate(seqs)])
 
+    async def expand_and_cache(self, s: DecoderSequence, completion_result: CompletionResult, edge_type, logprobs=1):
+        async def token_stream():
+            nonlocal edge_type, s, completion_result
+            response_buffer = completion_result.buffer
+            
+            try:
+                tokens = []
+                scores = []
+
+                while True:
+                    try:
+                        if await response_buffer.empty():
+                            break
+
+                        res = await response_buffer.get(0)
+                        tokens = nputil.ensure_iterable(res["logprobs"]["tokens"])
+                        scores = res["logprobs"]["token_logprobs"]
+
+                        topprobs = res["logprobs"]["top_logprobs"]
+                        if topprobs is not None and logprobs > 1:
+                            topk_tokens = list(topprobs.items())
+                            topk_tokens = [(tok[0], score) for (tok_str, score), tok in zip(topk_tokens, await self.tokenize_list([s for s,_ in topk_tokens]))]
+                            topk_tokens += [(tokens[0], scores)]
+                            topk_tokens = list(dict.fromkeys(topk_tokens))
+                            topk_tokens = sorted(topk_tokens, key=lambda x: x[1], reverse=True)
+                            topk_tokens = topk_tokens[:logprobs]
+                            
+                            tokens = [tok for tok, _ in topk_tokens]
+                            scores = [score for _, score in topk_tokens]
+                            edge_type = ["top-{}".format(i+1) for i in range(len(topk_tokens))]
+                        
+                        # future continuation
+                        response_buffer = response_buffer[1:]
+                        continuation = CompletionResult(response_buffer, completion_result.continuation_type, completion_result.logit_mask_or_fixed_id)
+
+                        user_data = {
+                            "openai-continuations": {
+                                continuation.continuation_type: continuation
+                            }
+                        }
+                        yield (s, tokens, scores, edge_type, user_data)
+                    except IndexError:
+                        break
+                # print("fully expanded speculativate continuation:", [await self.detokenize(tokens)], flush=True)
+                # if len(tokens) > 1:
+                #     await self.cache(s, tokens, scores, edge_type)
+            except Exception as e:
+                import traceback
+                traceback.print_exc()
+                print("error in expand_and_cache worker:", e, flush=True)
+        self.register_token_stream(token_stream)
+
     async def argmax(self, sequences, **kwargs):
-        return await self.sample(sequences, num_samples=1, temperature=0)
+        return await self.sample(sequences, num_samples=1, temperature=0, **kwargs)
 
     def report_stats(self, printer, decoder_step=None):
         if printer is None:
             return
         if hasattr(printer, "report_model_stats"):
             s = openai.Completion.get_stats()
             data = {
@@ -411,15 +484,15 @@
     async def sample(self, sequences, num_samples=1, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
         kwargs = {**self.model_args, **kwargs}
 
         async def op_sample(seqs):
-            completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=5, **kwargs)
+            completions: List[CompletionResult] = await self.completion_buffer(seqs, logprobs=1, **kwargs)
             
             next_token_ids = []
             next_token_scores = []
             logits = []
             continuation_buffers: List[CompletionResult] = []
 
             for s, completion in zip(seqs, completions):
@@ -492,17 +565,16 @@
                     "openai-continuations": {
                         continuation_buffer.continuation_type: continuation_buffer
                     },
                     **(default_user_data.copy())
                 }
                 return [continuation_as_user_data] + [default_user_data.copy()] * (num_successors - 1)
 
-            s = [s.make_successors(next_token_ids[i], next_token_scores[i], logits=logits[i], 
+            return [s.make_successors(next_token_ids[i], next_token_scores[i], logits=logits[i], 
                 user_data=successor_user_data(continuation_buffers[i], len(next_token_ids[i]))) for i,s in enumerate(seqs)]
-            return s
         with self.stats.timer("sample"):
             return await sequences.aelement_wise(op_sample)
 
     async def topk_continuations(self, sequences, k, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
@@ -928,29 +1000,34 @@
     
     class OpenAIModel:
         def __init__(self) -> None:
             self.model_identifier = model_identifier
             self.served_model = None
             self._tokenizer = None
 
-            self.chunk_size = 64
+            self.decoder_args = {
+                "openai_chunksize": 64
+            }
 
         def get_tokenizer(self):
             if self._tokenizer is None:
                 self._tokenizer = load_tokenizer("gpt2")
             self.served_model = self
             return self._tokenizer
 
         def get_dclib_model(self):
             bos_token_id = self.get_tokenizer().bos_token_id
             eos_token_id = self.get_tokenizer().eos_token_id
 
             dc.set_dclib_tokenizer(dc.tokenizer("lmql-adapter-tokenizer", self.tokenize, self.detokenize, bos_token_id, eos_token_id))
 
-            return DclibOpenAiModel(self.served_model, self.get_tokenizer())
+            return DclibOpenAiModel(self, self.get_tokenizer(), **self.decoder_args)
 
         async def tokenize(self, text):
             return self.get_tokenizer()(text)["input_ids"]
         
         async def detokenize(self, input_ids):
             return self.get_tokenizer().decode(input_ids)
+
+        def sync_tokenize(self, text):
+            return self.get_tokenizer()(text)["input_ids"]
     return OpenAIModel
```

### Comparing `lmql-0.0.5.1/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/output_writer.py` & `lmql-0.0.6/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/program_state.py` & `lmql-0.0.6/src/lmql/runtime/program_state.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/stats.py` & `lmql-0.0.6/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6/src/lmql/runtime/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             else:
                 return tokens
          
         def decode(self, input_ids, clean_up_tokenization_spaces=None):
             # set typed array type of input_ids to int
             return str(js.detokenize_gpt(to_js([int(i) for i in input_ids])))
 
-        def __call__(self, s: str):
+        def __call__(self, s: str, add_special_tokens=False):
             unpack = False
             if type(s) is not list:
                 s = [s]
                 unpack = True
             input_ids = [[int(v) for v in js.tokenize_gpt(se)] for se in s]
             
             if unpack:
@@ -63,17 +63,22 @@
 
 class LMQLTokenizer:
     def __init__(self, tokenizer_impl, model_identifier):
         self.tokenizer_impl = tokenizer_impl
         self.model_identifier = model_identifier
         self.detokenizer_cache = {}
 
+        self._vocab = get_vocab(self.tokenizer_impl)
+        self.vocab_range = max(self._vocab.values()) + 1
+
     @property
     def vocab_size(self):
-        return self.tokenizer_impl.vocab_size
+        # in LMQL vocab_size is the vocab_range (the highest vocabulary ID + 1)
+        # this allows us to use a dense one hot array where no IDs are skipped
+        return self.vocab_range
 
     @property
     def bos_token_id(self):
         return self.tokenizer_impl.bos_token_id
     
     @property
     def eos_token_id(self):
@@ -103,15 +108,15 @@
                 # print("cache hit")
                 return self.detokenizer_cache[n][key]
         if n-1 in self.detokenizer_cache.keys():
             key = str(input_ids[:-1])
             if key in self.detokenizer_cache[n-1].keys():
                 global reverse_special_token_mappings
                 # print("secondary cache hit")
-                if input_ids[-1] >= self.tokenizer_impl.vocab_size:
+                if input_ids[-1] >= self.vocab_size:
                     extended = self.detokenizer_cache[n-1][key] + "<" + reverse_special_token_mappings[input_ids[-1]] + "/>"
                 else:
                     extended = self.detokenizer_cache[n-1][key] + self.tokenizer_impl.decode([input_ids[-1]], clean_up_tokenization_spaces=False)
                 if not n in self.detokenizer_cache.keys():
                     self.detokenizer_cache[n] = {}
                 self.detokenizer_cache[n][str(input_ids)] = extended
                 return extended
@@ -125,43 +130,44 @@
 
         if not n in self.detokenizer_cache.keys():
             self.detokenizer_cache[n] = {}
         self.detokenizer_cache[n][key] = s
 
         return s
 
-    def __call__(self, s: str):
+    def __call__(self, s: str, add_special_tokens=False):
         input_ids = []
         unpack = False
         if type(s) is not list:
             s = [s]
             unpack = True
         
         for seq in s:
             chunk_input_ids = []
             for chunk in self.chunk_out_by_tags(seq):
                 if type(chunk) is int:
                     chunk_input_ids.append(chunk)
                 else:
-                    chunk_input_ids += self.tokenizer_impl(chunk)["input_ids"]
+                    result = self.tokenizer_impl(chunk, add_special_tokens=add_special_tokens)["input_ids"]
+                    chunk_input_ids += result
             input_ids.append(chunk_input_ids)
         
         if unpack:
             return {"input_ids": input_ids[0]}
         else:
             return {"input_ids": input_ids}
     
     def special_token_id(self, identifier):
         global special_token_mappings
         global reverse_special_token_mappings
         
         if identifier not in special_token_mappings:
             if len(special_token_mappings) == 0:
                 # offset vocabulary IDs by at least the next decimal power of 10
-                offset = 10 ** (len(str(self.vocab_size)))
+                offset = 10 ** (len(str(self.vocab_range)))
                 special_token_mappings[identifier] = offset
                 reverse_special_token_mappings[offset] = identifier
             else:
                 next_id = max(special_token_mappings.values()) + 1
                 special_token_mappings[identifier] = next_id
                 reverse_special_token_mappings[next_id] = identifier
         return special_token_mappings[identifier]
@@ -219,14 +225,24 @@
     else:
         from transformers import AutoTokenizer
         t = AutoTokenizer.from_pretrained(model_identifier)
         with open(cache_path, "wb") as f:
             pickle.dump(t, f)
         return LMQLTokenizer(t, model_identifier)
 
+def get_vocab(tokenizer):
+    if hasattr(tokenizer, "vocab"):
+        return tokenizer.vocab
+    elif hasattr(tokenizer, "get_vocab"):
+        return tokenizer.get_vocab()
+    elif hasattr(tokenizer, "tokenizer_impl"):
+        return get_vocab(tokenizer.tokenizer_impl)
+    else:
+        assert False, "Could not obtain full vocabulary from unknown tokenizer type: {}".format(type(tokenizer))
+
 if __name__ == "__main__":
     import sys
 
     model_identifier = sys.argv[1]
     t = load_tokenizer(model_identifier)
 
     to_tokenize = sys.argv[2]
@@ -245,8 +261,8 @@
             # contains digit
             digits = "0123456789"
             if len(t) < 4 and any(c in digits for c in t):
                 print(t,id)
                 n += 1
                 result += f""""{t}","""
         print(n)
-        print(result)
+        print(result)
```

### Comparing `lmql-0.0.5.1/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6/src/lmql/tests/expr_test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import ast
 import types
 import astunparse
 import inspect
+import termcolor
 from lmql.language.fragment_parser import LMQLQuery
 from lmql.language.compiler import PromptScope, SNFList, WhereClauseTransformation
 from lmql.ops.ops import NextToken, digest
 from lmql.runtime.program_state import ProgramState
 
 
 global show_transformed
@@ -141,18 +142,21 @@
 
 def run_all_tests(g):
     g = g.copy()
     num_errors = 0
     for k in list(g.keys()):
         try:
             if k.startswith("test"): 
+                print("Running", k, "." * (40 - len(k)), end=" ")
                 g[k]()
+                termcolor.cprint("OK", "green")
         except AssertionError as e:
             print(e)
             num_errors += 1
+            termcolor.cprint("FAILED", "red")
     
     if num_errors != 0: 
         print(num_errors, "test(s) failed.")
         sys.exit(1)
     else: 
         print("All tests passed.")
         sys.exit(0)
```

### Comparing `lmql-0.0.5.1/src/lmql/tests/mask_product_test.py` & `lmql-0.0.6/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/monotonicity.py` & `lmql-0.0.6/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/one_of_tests.py` & `lmql-0.0.6/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/sentences_op.py` & `lmql-0.0.6/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/starts_with_op_test.py` & `lmql-0.0.6/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/stops_at.py` & `lmql-0.0.6/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/str_in_str_tests.py` & `lmql-0.0.6/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/test_multi_head.py` & `lmql-0.0.6/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/tests/token_set_test.py` & `lmql-0.0.6/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/live/live.js` & `lmql-0.0.6/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/live/live.py` & `lmql-0.0.6/src/lmql/ui/live/live.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,19 @@
         add_debugger_output("stdin-request", {})
         return await LiveApp.ainput(*args, web=self.web)
 
     def add_interpreter_head_state(self, variable, head, prompt, where, trace, is_valid, is_final, mask, num_tokens, program_variables):
         from lmql.utils.graph import CytoscapeGraphWriter
         
         def node_data(op):
+            follow_map = "<follow_map output not supported>"
+
             result = "-"
             if trace is not None and op in trace:
                 result = trace[op]
-                follow_map = "<follow_map output not supporte>"
             
             return {
                 "result": result,
                 "follow_map": follow_map,
                 "repr": repr(op)
             }
 
@@ -71,14 +72,18 @@
     output_writer = LiveDebuggerOutputWriter(web=web)
 
     result = await lmql.run(code, output_writer=output_writer)
 
     for r in (result if type(result) is list else [result]):
         if r is None:
             continue
+
+        if type(r) is not lmql.LMQLResult:
+            print(r)
+            continue
         
         for v in [v for v in r.variables if v.startswith("P(")]:
             distribution = r.variables[v]
             max_prob = max([p for _,p in distribution])
             labels = []
             for value, prob in distribution:
                 label = value if prob != max_prob else f"{value} (*)"
```

### Comparing `lmql-0.0.5.1/src/lmql/ui/live/livelib.py` & `lmql-0.0.6/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/README.md` & `lmql-0.0.6/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/package.json` & `lmql-0.0.6/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6/src/lmql/ui/playground/src/App.jsx`

 * *Files 1% similar despite different names*

```diff
@@ -166,24 +166,25 @@
   text-align: right;
   right: 20pt;
   z-index: -1;
   padding: 5pt;
   white-space: pre-line;
   max-height: 10pt;
 
-  :hover .tooltip {
-    visibility: visible;
-    opacity: 1;
-  }
+  /* indicate copy */
+  cursor: pointer;
 `
 
 function TokenCountIndicator() {
   const [stats, setStats] = useState({})
 
   const format_cost = (c, precision) => {
+    if (c == 0) {
+      return "$0.00"
+    }
     c = c.toFixed(precision)
     if (c === (0).toFixed(precision))
       return "<$" + (Math.pow(10, -precision)).toFixed(precision);
     return "$" + c;
   }
 
   const cost_estimate = (model, k_tokens, precision = 2) => {
@@ -258,40 +259,47 @@
     }
   }, [])
 
   let text = ""
   let tokenCount = 0;
   let model = ""
   let steps = 1;
-  if (stats.tokens) {
+  let copyString = ""
+  if (stats.tokens || stats._step) {
     tokenCount = stats.tokens
     model = stats.model
     steps = stats._step || 1
     // first upper 
     const otherKeys = Object.keys(stats)
       .filter(k => k != "tokens")
       .filter(k => !k.startsWith("_"))
       .filter(k => k != "model")
     const toFirstUpper = k => k.charAt(0).toUpperCase() + k.slice(1)
     text = `Tokens: ${tokenCount}, ${otherKeys.map(k => `${toFirstUpper(k)}: ${stats[k]}`).join(", ")}`
 
+    copyString = `Tokens: ${tokenCount}\n${otherKeys.map(k => `${toFirstUpper(k)}: ${stats[k]}`).join("\n")}`
+
     // time elapsed
     if (stats._start) {
       const end = stats._end || stats._now || Date.now();
       const elapsed = (end - stats._start) / 1000
       text += `\n Time: ${elapsed.toFixed(1)}s, `
+      copyString += `\nTime: ${elapsed.toFixed(1)}s, `
     }
 
     text += `${(tokenCount / steps).toFixed(2)} tok/step`
     if (model.includes("openai")) {
       text += ` Est. Cost ${cost_estimate(model, tokenCount / 1000, 4)}`
+      copyString += `\nEst. Cost ${cost_estimate(model, tokenCount / 1000, 4)}`
     }
   }
 
-  return <TokenCountDiv>
+  return <TokenCountDiv onClick={() => {
+    navigator.clipboard.writeText(copyString)
+  }}>
     {text}
   </TokenCountDiv>
 }
 
 // const PlotContainer = styled.div`
 //   flex: 1;
 //   padding: 10pt;
@@ -397,15 +405,15 @@
   }, props);
 
   props.status = props.processState
   props.processState = props.status.status
 
   function handleEditorDidMount(editor, monaco) {
     ResizeObservers.addResizeListener(() => {
-      let fontSize = window.innerWidth < 700 ? 10 : 16
+      let fontSize = window.innerWidth < 700 ? 12 : 16
       editor.updateOptions({ "fontSize": fontSize })
       window.setTimeout(() => {
         editor.layout()
       }, 100)
     })
 
     registerLmqlLanguage(monaco);
@@ -449,14 +457,16 @@
           fontSize: fontSize,
           // line wrap
           wordWrap: "on",
           // tabs are spaces
           // tabSize: 6,
           // show whitespace
           renderWhitespace: "all",
+          // set font family
+          fontFamily: "Fira Code, monospace",
           automaticLayout: true
         }}
         // custom language
         defaultLanguage="lmql"
         style={{ maxHeight: "80%" }}
         onMount={handleEditorDidMount}
       />
@@ -546,14 +556,15 @@
 
   /* if screen < 320pt */
   @media (max-width: 40em) {
     &.simple-mode {
       flex-direction: column;
       height: calc(100%);
       padding: 0;
+      margin-right: 4pt;
     }
 
     &.simple-mode.simple .panel {
       flex: 1;
       margin: 0;
       margin-top: 1pt;
       width: calc(100% - 10pt);
@@ -678,14 +689,15 @@
 const ModelResultText = styled.div`
   flex: 1; 
   display: flex;
   flex-direction: column;
   line-height: 1.6em;
   white-space: pre-wrap;
   overflow-y: auto;
+  font-size: 10pt;
 
   &.chat-mode {
     padding-bottom: 50pt;
   }
 
   &.chat-mode .system-message {
     text-align: center;
@@ -802,20 +814,20 @@
 
   div .variable:hover {
     position: relative;
     transform: scale(1.1);
   }
 
   div .badge {
-    padding: 2.5pt 4pt;
+    padding: 1.0pt 4pt;
     border-radius: 2pt;
-    font-size: 8pt;
+    font-size: 0.9em;
     background-color: rgba(0, 0, 0, 0.5);
     position:relative; 
-    top: -1.25pt;
+    top: -0.05em;
     margin-right: 2pt;
     user-select: none;
     /* exclude from text selection */
     -webkit-user-select: none;
     -moz-user-select: none;
     -ms-user-select: none;
   }
@@ -2017,15 +2029,16 @@
   const fitTrigger = useState(new TriggerState())[0];
   const [eagerLayout, setEagerLayout] = useState(false);
 
   const derivedNodeFeatures = (data) => {
     return {
       "_finfalse": data.user_data && data.user_data.head && data.user_data.head.valid == "False",
       "_isRoot": data.root,
-      "_isDone": data.user_data && data.user_data.head && data.user_data.head.variable == "__done__"
+      "_isDone": data.user_data && data.user_data.head && data.user_data.head.variable == "__done__",
+      "_noUserData": !data.user_data || (data.user_data && data.user_data == "None")
     }
   }
 
   return <Panel className='stretch' id="decoder">
     <h2>
       Decoder Graph
       <ToolbarSpacer />
```

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -184,14 +184,15 @@
     let mostLikelyMostRecentNode = null;
     let mostLikelyDepth = 0;
 
     cy.elements().depthFirstSearch({
         roots: rootNodes,
         visit: (node, edge, previous, i, depth) => {
             if (node.hasClass("compound")) return;
+            if (node.data("_noUserData")) return;
 
             if (depth >= mostLikelyDepth) {
                 if (depth > mostLikelyDepth) {
                     mostLikelyMostRecentNode = null
                 }
                 mostLikelyDepth = depth
                 if (mostLikelyMostRecentNode) {
@@ -285,14 +286,24 @@
                     'background-color': 'rgb(146, 185, 146)',
                     'background-opacity': 1.0,
                     'color': 'white',
                     'border-color': 'green',
                     'border-width': '0px',
                 }
             }, {
+                selector: 'node[_noUserData]',
+                style: {
+                    // light blue
+                    'background-color': 'rgb(249, 209, 248)',
+                    'background-opacity': 0.7,
+                    'color': 'white',
+                    'border-color': 'red',
+                    'border-width': '0px',
+                }
+            }, {
                 selector: 'node.inactive',
                 style: {
                     'opacity': 0.5
                 }
             },
             //   active nodes
             {
```

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6/src/lmql/ui/playground/src/editor/theme.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6/src/lmql/ui/playground/src/queries.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/package.json` & `lmql-0.0.6/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/utils/graph.py` & `lmql-0.0.6/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.5.1/src/lmql/utils/nputil.py` & `lmql-0.0.6/src/lmql/utils/nputil.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,29 @@
     else: return a
 
 def ensure_array(v, dtype=None):
     if v is None: return None
     if is_array(v): return v
     else: return np.array(v, dtype=dtype)
 
+def ensure_iterable(v):
+    if type(v) is np.float32 or type(v) is np.float64 or type(v) is np.int32 or type(v) is np.int64 or type(v) is float or type(v) is int:
+        return [v]
+    elif type(v) is np.ndarray:
+        if v.ndim == 0:
+            return [v.item()]
+        else:
+            return v
+    elif type(v) is list:
+        return v
+    elif hasattr(v, "numpy"):
+        return ensure_iterable(v.numpy())
+    else:
+        assert False, f"ensure_iterable(): type {type(v)} cannot be converted to iterable"
+
 
 def log_softmax(a):
     return a - np.log(np.sum(np.exp(a)))
 
 def topk(a, k:int, sorted: bool = False, axis=-1):
     assert k > 0, "topk(): k must be > 0"
     idx = np.argpartition(a, -k, axis=axis)[..., -k:]
```

### Comparing `lmql-0.0.5.1/src/lmql.egg-info/PKG-INFO` & `lmql-0.0.6/src/lmql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmql
-Version: 0.0.5.1
+Version: 0.0.6
 Summary: A query language for language models.
 Home-page: https://lmql.ai
 Author: Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 Author-email: hello@lmql.ai
 Project-URL: Docs, https://docs.lmql.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,16 @@
     <a href="https://lmql.ai">Explore Examples</a>
     ·
     <a href="https://lmql.ai/playground">Playground IDE</a>
     ·
     <a href="https://github.com/eth-sri/lmql/issues">Report Bug</a>
     <br/>
     <br/>
+    <a href="https://discord.gg/7eJP4fcyNT"><img src="https://img.shields.io/discord/1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white" height=18/></a>
+    <a href="https://badge.fury.io/py/Lmql"><img src="https://badge.fury.io/py/Lmql.svg" alt="PyPI version" height=18></a>
   </p>
 </div>
 
 LMQL is a query language for large language models (LLMs). It facilitates LLM interaction by combining the benefits of natural language prompting with the expressiveness of Python. With only a few lines of LMQL code, users can express advanced, multi-part and tool-augmented LM queries, which then are optimized by the LMQL runtime to run efficiently as part of the LM decoding loop.
 
 ![lmql-overview](https://user-images.githubusercontent.com/17903049/222918379-84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 2.1 Name: lmql Version: 0.0.5.1 Summary: A query language for
+Metadata-Version: 2.1 Name: lmql Version: 0.0.6 Summary: A query language for
 language models. Home-page: https://lmql.ai Author: Luca Beurer-Kellner, Marc
 Fischer, Martin Vechev Author-email: hello@lmql.ai Project-URL: Docs, https://
 docs.lmql.ai Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
                                 **** LMQL ****
           A query language for programming (large) language models.
                                Documentation_Â»
 
                Explore_Examples Â· Playground_IDE Â· Report_Bug
 
+                       [https://img.shields.io/discord/
+1091288833997410414?style=plastic&logo=discord&color=blueviolet&logoColor=white]
+                                [PyPI_version]
 LMQL is a query language for large language models (LLMs). It facilitates LLM
 interaction by combining the benefits of natural language prompting with the
 expressiveness of Python. With only a few lines of LMQL code, users can express
 advanced, multi-part and tool-augmented LM queries, which then are optimized by
 the LMQL runtime to run efficiently as part of the LM decoding loop. ![lmql-
 overview](https://user-images.githubusercontent.com/17903049/222918379-
 84a00b9a-1ef0-45bf-9384-15a20f2874f0.png)
```

### Comparing `lmql-0.0.5.1/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6/src/lmql.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,27 @@
 docs/source/logo.png
 docs/source/quickstart.md
 docs/source/_ext/lmql_snippets.py
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
+docs/source/blog/release-0.0.5.md
+docs/source/blog/release-0.0.6.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/models.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/python/.gitignore
 docs/source/python/langchain.ipynb
+docs/source/python/llama_index.ipynb
 docs/source/python/lmql.txt
+docs/source/python/pandas.ipynb
 docs/source/python/python.ipynb
 docs/source/releases/misc-snippets.md
 docs/source/releases/release-0.0.5.md
 scripts/activate-dev.sh
 scripts/pypi-release.sh
 scripts/wheel.sh
 scripts/conda/requirements-no-gpu.yml
@@ -71,47 +75,51 @@
 src/lmql/runtime/__init__.py
 src/lmql/runtime/hf_integration.py
 src/lmql/runtime/interpreter.py
 src/lmql/runtime/interrupt.py
 src/lmql/runtime/langchain.py
 src/lmql/runtime/lmql_runtime.py
 src/lmql/runtime/maiohttp.py
+src/lmql/runtime/masks.py
 src/lmql/runtime/model_registry.py
 src/lmql/runtime/multi_head_interpretation.py
 src/lmql/runtime/openai_integration.py
 src/lmql/runtime/openai_secret.py
 src/lmql/runtime/output_writer.py
 src/lmql/runtime/program_state.py
 src/lmql/runtime/stats.py
 src/lmql/runtime/tokenizer.py
 src/lmql/runtime/bopenai/__init__.py
 src/lmql/runtime/bopenai/batched_openai.py
 src/lmql/runtime/bopenai/openai_api.py
 src/lmql/runtime/dclib/__init__.py
 src/lmql/runtime/dclib/dclib_array.py
+src/lmql/runtime/dclib/dclib_cache.py
 src/lmql/runtime/dclib/dclib_global.py
 src/lmql/runtime/dclib/dclib_model.py
+src/lmql/runtime/dclib/dclib_rewrite.py
 src/lmql/runtime/dclib/dclib_seq.py
 src/lmql/runtime/dclib/decoders.py
 src/lmql/runtime/dclib/trie_cache.py
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
 src/lmql/tests/README.md
 src/lmql/tests/expr_test_utils.py
-src/lmql/tests/mask_product_test.py
-src/lmql/tests/monotonicity.py
-src/lmql/tests/one_of_tests.py
-src/lmql/tests/sentences_op.py
-src/lmql/tests/starts_with_op_test.py
-src/lmql/tests/stops_at.py
-src/lmql/tests/str_in_str_tests.py
-src/lmql/tests/test_multi_head.py
+src/lmql/tests/tail_token_set.py
 src/lmql/tests/test_sample_queries.py
-src/lmql/tests/token_set_test.py
+src/lmql/tests/outdated/mask_product_test.py
+src/lmql/tests/outdated/monotonicity.py
+src/lmql/tests/outdated/one_of_tests.py
+src/lmql/tests/outdated/sentences_op.py
+src/lmql/tests/outdated/starts_with_op_test.py
+src/lmql/tests/outdated/stops_at.py
+src/lmql/tests/outdated/str_in_str_tests.py
+src/lmql/tests/outdated/test_multi_head.py
+src/lmql/tests/outdated/token_set_test.py
 src/lmql/tests/system/basic_use_cases.py
 src/lmql/ui/.gitignore
 src/lmql/ui/__init__.py
 src/lmql/ui/live/__init__.py
 src/lmql/ui/live/live.js
 src/lmql/ui/live/live.py
 src/lmql/ui/live/livelib.py
```

### Comparing `lmql-0.0.5.1/src/lmql.svg` & `lmql-0.0.6/src/lmql.svg`

 * *Files identical despite different names*

