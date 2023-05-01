# Comparing `tmp/explainable-rl-0.0.1.tar.gz` & `tmp/explainable-rl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainable-rl-0.0.1.tar", last modified: Mon May  1 07:24:22 2023, max compression
+gzip compressed data, was "explainable-rl-0.0.2.tar", last modified: Mon May  1 08:55:14 2023, max compression
```

## Comparing `explainable-rl-0.0.1.tar` & `explainable-rl-0.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.457658 explainable-rl-0.0.1/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1165 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/LICENSE
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1318 2023-05-01 07:24:22.457770 explainable-rl-0.0.1/PKG-INFO
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)      787 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/PYPIREADME.md
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4197 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/README.md
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.444582 explainable-rl-0.0.1/explainable_rl/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/__init__.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.447524 explainable-rl-0.0.1/explainable_rl/agents/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3654 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/double_q_learner.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1359 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/q_learner.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1386 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/sarsa.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1685 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/sarsa_lambda.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)    10532 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/agents/td.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.448057 explainable-rl-0.0.1/explainable_rl/data_handler/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)       87 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/data_handler/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     6533 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/data_handler/data_handler.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.449048 explainable-rl-0.0.1/explainable_rl/environments/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/environments/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     7316 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3896 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing_prediction.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4207 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing_suggestion.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.449503 explainable-rl-0.0.1/explainable_rl/evaluation/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/evaluation/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     8823 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/evaluation/evaluator.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.450214 explainable-rl-0.0.1/explainable_rl/explainability/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/explainability/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     5663 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/explainability/pdp.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)    10210 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/explainability/shap_values.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.452053 explainable-rl-0.0.1/explainable_rl/foundation/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)       87 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3403 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/agent.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     8681 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/engine.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)      972 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/environment.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)      319 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/library.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2631 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/foundation/utils.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.452526 explainable-rl-0.0.1/explainable_rl/performance/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/performance/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)    14576 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/explainable_rl/performance/performance_evaluator.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.446050 explainable-rl-0.0.1/explainable_rl.egg-info/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1318 2023-05-01 07:24:22.000000 explainable-rl-0.0.1/explainable_rl.egg-info/PKG-INFO
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2095 2023-05-01 07:24:22.000000 explainable-rl-0.0.1/explainable_rl.egg-info/SOURCES.txt
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        1 2023-05-01 07:24:22.000000 explainable-rl-0.0.1/explainable_rl.egg-info/dependency_links.txt
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        1 2023-05-01 07:19:20.000000 explainable-rl-0.0.1/explainable_rl.egg-info/not-zip-safe
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)      124 2023-05-01 07:24:22.000000 explainable-rl-0.0.1/explainable_rl.egg-info/requires.txt
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)       21 2023-05-01 07:24:22.000000 explainable-rl-0.0.1/explainable_rl.egg-info/top_level.txt
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)       98 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/pyproject.toml
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1051 2023-05-01 07:24:22.458311 explainable-rl-0.0.1/setup.cfg
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.452993 explainable-rl-0.0.1/tests/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-18 13:00:21.000000 explainable-rl-0.0.1/tests/__init__.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.454448 explainable-rl-0.0.1/tests/test_agents/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.1/tests/test_agents/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2148 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_agents/test_double_q_learner.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1991 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_agents/test_q_learner.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2022 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_agents/test_sarsa.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1394 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_agents/test_sarsa_lambda.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2898 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_agents/test_td.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.454888 explainable-rl-0.0.1/tests/test_data_handler/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-13 16:03:36.000000 explainable-rl-0.0.1/tests/test_data_handler/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4365 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_data_handler/test_data_handler.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.455912 explainable-rl-0.0.1/tests/test_environments/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.1/tests/test_environments/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3250 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3120 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing_prediction.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2798 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing_suggestion.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.456703 explainable-rl-0.0.1/tests/test_explainability/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.1/tests/test_explainability/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1923 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_explainability/test_pdp.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3848 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_explainability/test_shap_values.py
-drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 07:24:22.457446 explainable-rl-0.0.1/tests/test_foundation/
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-13 16:03:36.000000 explainable-rl-0.0.1/tests/test_foundation/__init__.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4004 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_foundation/test_engine.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1636 2023-04-29 17:06:56.000000 explainable-rl-0.0.1/tests/test_foundation/test_utils.py
--rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1033 2023-04-26 20:03:40.000000 explainable-rl-0.0.1/tests/test_hyperparams.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.583455 explainable-rl-0.0.2/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1165 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/LICENSE
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1318 2023-05-01 08:55:14.583759 explainable-rl-0.0.2/PKG-INFO
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)      787 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/PYPIREADME.md
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4197 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/README.md
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.536495 explainable-rl-0.0.2/explainable_rl/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/__init__.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.547749 explainable-rl-0.0.2/explainable_rl/agents/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3654 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/double_q_learner.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1359 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/q_learner.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1386 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/sarsa.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1685 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/sarsa_lambda.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)    10532 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/agents/td.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.549138 explainable-rl-0.0.2/explainable_rl/data_handler/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)       87 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/data_handler/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     6533 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/data_handler/data_handler.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.552032 explainable-rl-0.0.2/explainable_rl/environments/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/environments/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     7316 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3896 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing_prediction.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4207 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing_suggestion.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.553374 explainable-rl-0.0.2/explainable_rl/evaluation/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/evaluation/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     8823 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/evaluation/evaluator.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.555778 explainable-rl-0.0.2/explainable_rl/explainability/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/explainability/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     5663 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/explainability/pdp.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)    10208 2023-05-01 08:53:37.000000 explainable-rl-0.0.2/explainable_rl/explainability/shap_values.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.563126 explainable-rl-0.0.2/explainable_rl/foundation/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)       87 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3403 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/agent.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     8681 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/engine.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)      972 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/environment.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)      319 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/library.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2631 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/foundation/utils.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.564445 explainable-rl-0.0.2/explainable_rl/performance/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/performance/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)    14576 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/explainable_rl/performance/performance_evaluator.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.543239 explainable-rl-0.0.2/explainable_rl.egg-info/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1318 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/PKG-INFO
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2095 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        1 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        1 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/not-zip-safe
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)      140 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/requires.txt
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)       21 2023-05-01 08:55:14.000000 explainable-rl-0.0.2/explainable_rl.egg-info/top_level.txt
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)       98 2023-04-29 17:06:56.000000 explainable-rl-0.0.2/pyproject.toml
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1068 2023-05-01 08:55:14.585225 explainable-rl-0.0.2/setup.cfg
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.565852 explainable-rl-0.0.2/tests/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-18 13:00:21.000000 explainable-rl-0.0.2/tests/__init__.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.570507 explainable-rl-0.0.2/tests/test_agents/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.2/tests/test_agents/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2148 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_agents/test_double_q_learner.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1991 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_agents/test_q_learner.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2022 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_agents/test_sarsa.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1394 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_agents/test_sarsa_lambda.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2898 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_agents/test_td.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.573402 explainable-rl-0.0.2/tests/test_data_handler/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-13 16:03:36.000000 explainable-rl-0.0.2/tests/test_data_handler/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4365 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_data_handler/test_data_handler.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.578292 explainable-rl-0.0.2/tests/test_environments/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.2/tests/test_environments/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3250 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3120 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing_prediction.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     2798 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing_suggestion.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.580530 explainable-rl-0.0.2/tests/test_explainability/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-20 11:00:15.000000 explainable-rl-0.0.2/tests/test_explainability/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1923 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_explainability/test_pdp.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     3848 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_explainability/test_shap_values.py
+drwxr-xr-x   0 ludovicobuizza   (501) staff       (20)        0 2023-05-01 08:55:14.582866 explainable-rl-0.0.2/tests/test_foundation/
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)        0 2023-04-13 16:03:36.000000 explainable-rl-0.0.2/tests/test_foundation/__init__.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     4004 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_foundation/test_engine.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1636 2023-05-01 08:45:01.000000 explainable-rl-0.0.2/tests/test_foundation/test_utils.py
+-rw-r--r--   0 ludovicobuizza   (501) staff       (20)     1033 2023-04-26 20:03:40.000000 explainable-rl-0.0.2/tests/test_hyperparams.py
```

### Comparing `explainable-rl-0.0.1/LICENSE` & `explainable-rl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/PKG-INFO` & `explainable-rl-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-rl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for explainable tabular reinforcement learning.
 Home-page: https://github.com/gsassatelli/explainable-rl
 Author: Giulia Sassatelli, Ludovico Buizza, Teresa Delgado de las Heras, Mireia Hernandez Caralt, Matteo Gabriel Mecattaf
 Author-email: lcb216@ic.ac.uk
 License: : MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `explainable-rl-0.0.1/PYPIREADME.md` & `explainable-rl-0.0.2/PYPIREADME.md`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/README.md` & `explainable-rl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/agents/double_q_learner.py` & `explainable-rl-0.0.2/explainable_rl/agents/double_q_learner.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/agents/q_learner.py` & `explainable-rl-0.0.2/explainable_rl/agents/q_learner.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/agents/sarsa.py` & `explainable-rl-0.0.2/explainable_rl/agents/sarsa.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/agents/sarsa_lambda.py` & `explainable-rl-0.0.2/explainable_rl/agents/sarsa_lambda.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/agents/td.py` & `explainable-rl-0.0.2/explainable_rl/agents/td.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/data_handler/data_handler.py` & `explainable-rl-0.0.2/explainable_rl/data_handler/data_handler.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing.py` & `explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing_prediction.py` & `explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing_prediction.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/environments/strategic_pricing_suggestion.py` & `explainable-rl-0.0.2/explainable_rl/environments/strategic_pricing_suggestion.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/evaluation/evaluator.py` & `explainable-rl-0.0.2/explainable_rl/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/explainability/pdp.py` & `explainable-rl-0.0.2/explainable_rl/explainability/pdp.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/explainability/shap_values.py` & `explainable-rl-0.0.2/explainable_rl/explainability/shap_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             action (list): Predicted action.
         """
         Q_state = np.zeros(self.env.bins[-1])
         for a in range(self.env.bins[-1]):
             index = tuple(list(self.binned_sample) + [a])
             current_q = self.Q[index]
             Q_state[a] = current_q
-        binned_action = np.argmax(np.array(current_q))
+        binned_action = np.argmax(np.array(Q_state))
         action = self.get_denorm_actions([binned_action])
         return round(action[0], 4)
 
     def plot_shap_values(
         self, sample, shap_values, predicted_action, fig_name=None, savefig=False
     ):
         """Plot shap values.
```

### Comparing `explainable-rl-0.0.1/explainable_rl/foundation/agent.py` & `explainable-rl-0.0.2/explainable_rl/foundation/agent.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/foundation/engine.py` & `explainable-rl-0.0.2/explainable_rl/foundation/engine.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/foundation/environment.py` & `explainable-rl-0.0.2/explainable_rl/foundation/environment.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/foundation/utils.py` & `explainable-rl-0.0.2/explainable_rl/foundation/utils.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl/performance/performance_evaluator.py` & `explainable-rl-0.0.2/explainable_rl/performance/performance_evaluator.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/explainable_rl.egg-info/PKG-INFO` & `explainable-rl-0.0.2/explainable_rl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: explainable-rl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for explainable tabular reinforcement learning.
 Home-page: https://github.com/gsassatelli/explainable-rl
 Author: Giulia Sassatelli, Ludovico Buizza, Teresa Delgado de las Heras, Mireia Hernandez Caralt, Matteo Gabriel Mecattaf
 Author-email: lcb216@ic.ac.uk
 License: : MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `explainable-rl-0.0.1/explainable_rl.egg-info/SOURCES.txt` & `explainable-rl-0.0.2/explainable_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/setup.cfg` & `explainable-rl-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = explainable-rl
-version = 0.0.1
+version = 0.0.2
 author = Giulia Sassatelli, Ludovico Buizza, Teresa Delgado de las Heras, Mireia Hernandez Caralt, Matteo Gabriel Mecattaf
 author_email = lcb216@ic.ac.uk
 description = A package for explainable tabular reinforcement learning.
 long_description = file: PYPIREADME.md
 long_description_content_type = text/markdown
 url = https://github.com/gsassatelli/explainable-rl
 Bug Tracker = https://github.com/gsassatelli/explainable-rl/issues
@@ -15,22 +15,23 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	ipdb==0.13.11
-	matplotlib==3.7.1
-	numpy==1.23.5
-	pandas==1.5.3
-	scikit_learn==1.2.2
-	seaborn==0.11.1
-	sparse==0.13.0
-	tqdm==4.65.0
+	ipdb>=0.13.11
+	matplotlib>=3.7.1
+	numpy>=1.23.5
+	pandas>=1.5.3
+	scikit_learn>=1.2.2
+	seaborn>=0.11.1
+	sparse>=0.13.0
+	tqdm>=4.65.0
+	pyarrow>=11.0.0
 
 [options.packages.find]
 exclude = 
 	tests/
 	docs/
 	class_diagrams/
 	.github/
```

### Comparing `explainable-rl-0.0.1/tests/test_agents/test_double_q_learner.py` & `explainable-rl-0.0.2/tests/test_agents/test_double_q_learner.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_agents/test_q_learner.py` & `explainable-rl-0.0.2/tests/test_agents/test_q_learner.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_agents/test_sarsa.py` & `explainable-rl-0.0.2/tests/test_agents/test_sarsa.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_agents/test_sarsa_lambda.py` & `explainable-rl-0.0.2/tests/test_agents/test_sarsa_lambda.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_agents/test_td.py` & `explainable-rl-0.0.2/tests/test_agents/test_td.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_data_handler/test_data_handler.py` & `explainable-rl-0.0.2/tests/test_data_handler/test_data_handler.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing.py` & `explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing_prediction.py` & `explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing_prediction.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_environments/test_strategic_pricing_suggestion.py` & `explainable-rl-0.0.2/tests/test_environments/test_strategic_pricing_suggestion.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_explainability/test_pdp.py` & `explainable-rl-0.0.2/tests/test_explainability/test_pdp.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_explainability/test_shap_values.py` & `explainable-rl-0.0.2/tests/test_explainability/test_shap_values.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_foundation/test_engine.py` & `explainable-rl-0.0.2/tests/test_foundation/test_engine.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_foundation/test_utils.py` & `explainable-rl-0.0.2/tests/test_foundation/test_utils.py`

 * *Files identical despite different names*

### Comparing `explainable-rl-0.0.1/tests/test_hyperparams.py` & `explainable-rl-0.0.2/tests/test_hyperparams.py`

 * *Files identical despite different names*

