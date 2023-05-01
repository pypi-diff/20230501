# Comparing `tmp/broker-0.3.0.tar.gz` & `tmp/broker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broker-0.3.0.tar", last modified: Mon Apr 10 19:38:44 2023, max compression
+gzip compressed data, was "broker-0.3.1.tar", last modified: Mon May  1 19:33:11 2023, max compression
```

## Comparing `broker-0.3.0.tar` & `broker-0.3.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.150156 broker-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-10 19:38:30.000000 broker-0.3.0/.github/workflows/update_broker_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-10 19:38:30.000000 broker-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-10 19:38:30.000000 broker-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-10 19:38:30.000000 broker-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 19:38:30.000000 broker-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-10 19:38:44.162156 broker-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-10 19:38:30.000000 broker-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:38:30.000000 broker-0.3.0/broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker/binds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:30.000000 broker-0.3.0/broker/binds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-04-10 19:38:30.000000 broker-0.3.0/broker/binds/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-10 19:38:30.000000 broker-0.3.0/broker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-10 19:38:30.000000 broker-0.3.0/broker/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-10 19:38:30.000000 broker-0.3.0/broker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-10 19:38:30.000000 broker-0.3.0/broker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-10 19:38:30.000000 broker-0.3.0/broker/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-10 19:38:30.000000 broker-0.3.0/broker/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/broker/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28625 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-10 19:38:30.000000 broker-0.3.0/broker/providers/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-04-10 19:38:30.000000 broker-0.3.0/broker/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 19:38:30.000000 broker-0.3.0/broker/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.154156 broker-0.3.0/broker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:38:43.000000 broker-0.3.0/broker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 19:38:44.000000 broker-0.3.0/broker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-10 19:38:30.000000 broker-0.3.0/broker_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-10 19:38:30.000000 broker-0.3.0/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 19:38:30.000000 broker-0.3.0/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 19:38:30.000000 broker-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 19:38:44.162156 broker-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 19:38:30.000000 broker-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-10 19:38:30.000000 broker-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/ansible_tower/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_children.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_jobs.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/ansible_tower/fake_workflows.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/args_file.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/args_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/broker_args.json
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/broker_args.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.150156 broker-0.3.0/tests/data/cli_scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/cli_scenarios/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.158156 broker-0.3.0/tests/data/cli_scenarios/satlab/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/data/container/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/container/fake_containers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/container/fake_images.json
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-10 19:38:30.000000 broker-0.3.0/tests/data/fake_inventory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-10 19:38:30.000000 broker-0.3.0/tests/functional/test_satlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:38:44.162156 broker-0.3.0/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-10 19:38:30.000000 broker-0.3.0/tests/providers/test_ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-10 19:38:30.000000 broker-0.3.0/tests/providers/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-10 19:38:30.000000 broker-0.3.0/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.634777 broker-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.638778 broker-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/update_broker_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-01 19:32:51.000000 broker-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-01 19:32:51.000000 broker-0.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-01 19:32:51.000000 broker-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 19:32:51.000000 broker-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-01 19:33:11.646777 broker-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-01 19:32:51.000000 broker-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 19:32:51.000000 broker-0.3.1/broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/binds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:32:51.000000 broker-0.3.1/broker/binds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-01 19:32:51.000000 broker-0.3.1/broker/binds/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-01 19:32:51.000000 broker-0.3.1/broker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-01 19:32:51.000000 broker-0.3.1/broker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-01 19:32:51.000000 broker-0.3.1/broker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-01 19:32:51.000000 broker-0.3.1/broker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-01 19:32:51.000000 broker-0.3.1/broker/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-01 19:32:51.000000 broker-0.3.1/broker/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-01 19:32:51.000000 broker-0.3.1/broker/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-05-01 19:32:51.000000 broker-0.3.1/broker/providers/ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-01 19:32:52.000000 broker-0.3.1/broker/providers/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-01 19:32:52.000000 broker-0.3.1/broker/providers/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-01 19:32:52.000000 broker-0.3.1/broker/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-01 19:32:52.000000 broker-0.3.1/broker/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:32:59.000000 broker-0.3.1/broker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-01 19:32:52.000000 broker-0.3.1/broker_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-01 19:32:52.000000 broker-0.3.1/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 19:32:52.000000 broker-0.3.1/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 19:32:52.000000 broker-0.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 19:33:11.650778 broker-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 19:32:52.000000 broker-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-01 19:32:52.000000 broker-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/ansible_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_children.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/args_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/args_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/broker_args.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/broker_args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.638778 broker-0.3.1/tests/data/cli_scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/cli_scenarios/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/cli_scenarios/satlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/container/fake_containers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/container/fake_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/fake_inventory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/test_satlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-01 19:32:52.000000 broker-0.3.1/tests/providers/test_ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 19:32:52.000000 broker-0.3.1/tests/providers/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_settings.py
```

### Comparing `broker-0.3.0/.github/workflows/codeql-analysis.yml` & `broker-0.3.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/.github/workflows/python-publish.yml` & `broker-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/.github/workflows/update_broker_image.yml` & `broker-0.3.1/.github/workflows/update_broker_image.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/.gitignore` & `broker-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/LICENSE` & `broker-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/PKG-INFO` & `broker-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.0
+Version: 0.3.1
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.0/README.md` & `broker-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/binds/containers.py` & `broker-0.3.1/broker/binds/containers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/broker.py` & `broker-0.3.1/broker/broker.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/commands.py` & `broker-0.3.1/broker/commands.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/exceptions.py` & `broker-0.3.1/broker/exceptions.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/helpers.py` & `broker-0.3.1/broker/helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/hosts.py` & `broker-0.3.1/broker/hosts.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,20 @@
     def __init__(self, hostname=None, name=None, from_dict=False, **kwargs):
         # Allow the class to construct itself from kwargs
         if from_dict:
             self.__dict__.update(kwargs)
         else:
             self.hostname = hostname or kwargs.get("ip", None)
             if not self.hostname:
-                raise HostError("Host must be constructed with a hostname or ip")
+                # check to see if we're being reconstructued, likely for checkin
+                import inspect
+                if any(f.function == "reconstruct_host" for f in inspect.stack()):
+                    logger.debug("Ignoring missing hostname and ip for checkin reconstruction.")
+                else:
+                    raise HostError("Host must be constructed with a hostname or ip")
             self.name = name
         self.username = kwargs.get("username", settings.HOST_USERNAME)
         self.password = kwargs.get("password", settings.HOST_PASSWORD)
         self.timeout = kwargs.get(
             "connection_timeout", settings.HOST_CONNECTION_TIMEOUT
         )
         self.port = kwargs.get("port", settings.HOST_SSH_PORT)
```

### Comparing `broker-0.3.0/broker/logger.py` & `broker-0.3.1/broker/logger.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/providers/__init__.py` & `broker-0.3.1/broker/providers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,17 @@
                     instance = candidate
             self.instance, *_ = instance  # store the instance name on the provider
             fresh_settings.update((inst_vals := instance.values()[0]))
             settings[section_name] = fresh_settings
             if not inst_vals.get("override_envars"):
                 # if a provider instance doesn't want to override envars, load them
                 settings.execute_loaders(loaders=[dynaconf.loaders.env_loader])
-
-        settings.validators.extend([v for v in self._validators if v not in settings.validators])
+        new_validators = [v for v in self._validators if v not in settings.validators]
+        logger.debug(f"Adding new validators: {[v.names[0] for v in new_validators]}")
+        settings.validators.extend(new_validators)
         # use selective validation to only validate the instance settings
         try:
             settings.validators.validate(only=section_name)
         except dynaconf.ValidationError as err:
             raise exceptions.ConfigurationError(err)
 
     def _set_attributes(self, obj, attrs):
```

### Comparing `broker-0.3.0/broker/providers/ansible_tower.py` & `broker-0.3.1/broker/providers/ansible_tower.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,28 +201,39 @@
             if inventory_info := self.v2.inventory.get(id=inventory):
                 return inventory_info.results[0].name
             else:
                 raise exceptions.ProviderError(
                     provider="AnsibleTower",
                     message=f"Unknown AnsibleTower inventory by id {inventory}",
                 )
-        if inventory_info := self.v2.inventory.get(search=inventory):
-            if inventory_info.count > 1:
-                raise exceptions.ProviderError(
-                    provider="AnsibleTower",
-                    message=f"Ambigious AnsibleTower inventory name {inventory}",
-                )
-            elif inventory_info.count == 1:
-                inv_struct = inventory_info.results.pop()
-                return inv_struct.id
-            else:
-                raise exceptions.ProviderError(
-                    provider="AnsibleTower",
-                    message=f"Unknown AnsibleTower inventory {inventory}",
-                )
+        elif isinstance(inventory, str):
+            if inventory_info := self.v2.inventory.get(search=inventory):
+                if inventory_info.count > 1:
+                    raise exceptions.ProviderError(
+                        provider="AnsibleTower",
+                        message=f"Ambigious AnsibleTower inventory name {inventory}",
+                    )
+                elif inventory_info.count == 1:
+                    inv_struct = inventory_info.results.pop()
+                    return inv_struct.id
+                else:
+                    raise exceptions.ProviderError(
+                        provider="AnsibleTower",
+                        message=f"Unknown AnsibleTower inventory {inventory}",
+                    )
+        elif inv_id := getattr(inventory, "id", None):
+            return inv_id
+        elif inv_name := getattr(inventory, "name", None):
+            return inv_name
+        else:
+            caller_context = inspect.stack()[1][0].f_locals
+            raise exceptions.ProviderError(
+                provider="AnsibleTower",
+                message=f"Ambiguous AnsibleTower inventory {inventory} passed from {caller_context}",
+            )
 
     def _merge_artifacts(self, at_object, strategy="last", artifacts=None):
         """Gather and merge all artifacts associated with an object and its children
 
         :param at_object: object you want to merge
 
         :param strategy:
@@ -545,15 +556,17 @@
             for inv in self.v2.inventory.get(page_size=100).results
             if user in inv.name or user == "@ll"
         ]
         hosts = []
         for inv in invs:
             inv_hosts = inv.get_related("hosts", page_size=200).results
             hosts.extend(inv_hosts)
-        return [self._compile_host_info(host) for host in hosts]
+        with click.progressbar(hosts, label='Compiling host information') as hosts_bar:
+            compiled_host_info = [self._compile_host_info(host) for host in hosts_bar]
+        return compiled_host_info
 
     def extend(self, target_vm, new_expire_time=None):
         """Run the extend workflow with defaults args
 
         :param target_vm: This should be a host object
         """
         # check if an inventory was specified. if so overwrite the current inventory
```

### Comparing `broker-0.3.0/broker/providers/container.py` & `broker-0.3.1/broker/providers/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             **{**kwargs, "hostname": hostname, "name": name}
         )
         self._set_attributes(host_inst, broker_args=kwargs, cont_inst=cont_inst)
         return host_inst
 
     def nick_help(self, **kwargs):
         """Useful information about container images"""
-        results_limit = kwargs.get("results_limit", settings.CONTAINER.results_limit)
+        results_limit = kwargs.get("results_limit", settings.container.results_limit)
         if image := kwargs.get("container_host"):
             logger.info(
                 f"Information for {image} container-host:\n"
                 f"{helpers.yaml_format(self.runtime.image_info(image))}"
             )
         elif kwargs.get("container_hosts"):
             images = [
```

### Comparing `broker-0.3.0/broker/providers/test_provider.py` & `broker-0.3.1/broker/providers/test_provider.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/session.py` & `broker-0.3.1/broker/session.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker/settings.py` & `broker-0.3.1/broker/settings.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker.egg-info/PKG-INFO` & `broker-0.3.1/broker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.0
+Version: 0.3.1
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.0/broker.egg-info/SOURCES.txt` & `broker-0.3.1/broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/broker_settings.yaml.example` & `broker-0.3.1/broker_settings.yaml.example`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # Broker settings
 # different log levels for file and stdout
 logging:
     console_level: info
     file_level: debug
 # Host Settings
 # These can be left alone if you're not using Broker as a library
-host_username: "root"
+host_username: root
 host_password: "<password>"
-host_ssh_port: "<port>"
+host_ssh_port: 22
 host_ssh_key_filename: "</path/to/the/ssh-key>"
 # Provider settings
 AnsibleTower:
-    instances:
-        - production:
-            base_url: "https://<ansible tower host>/"
-            # Username AND password, OR an OAUTH token can be used for authentication
-            username: "<username>"
-            password: "<plain text password>"
-            # token: "<AT personal access token>"
-            inventory: "inventory name"
-            default: True
-        - testing:
-            base_url: "https://<ansible tower host>/"
-            # Username AND password, OR an OAUTH token can be used for authentication
-            username: "<username>"
-            password: "<plain text password>"
-            # token: "<AT personal access token>"
-            inventory: "inventory name"
+    base_url: "https://<ansible tower host>/"
+    # Username is required for both token and password-based authentication
+    username: "<username>"
+    # token is the preferred authentication method
+    token: "<AT personal access token>"
+    # password: "<plain text password>"
+    inventory: "inventory name"
     release_workflow: "remove-vm"
     extend_workflow: "extend-vm"
     new_expire_time: "+172800"
     workflow_timeout: 3600
     results_limit: 50
 Container:
     instances:
```

### Comparing `broker-0.3.0/setup.cfg` & `broker-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/data/ansible_tower/fake_children.json` & `broker-0.3.1/tests/data/ansible_tower/fake_children.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/data/ansible_tower/fake_jobs.json` & `broker-0.3.1/tests/data/ansible_tower/fake_jobs.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/data/container/fake_containers.json` & `broker-0.3.1/tests/data/container/fake_containers.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/data/container/fake_images.json` & `broker-0.3.1/tests/data/container/fake_images.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/data/fake_inventory.yaml` & `broker-0.3.1/tests/data/fake_inventory.yaml`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/functional/README.md` & `broker-0.3.1/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/functional/test_containers.py` & `broker-0.3.1/tests/functional/test_containers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/functional/test_satlab.py` & `broker-0.3.1/tests/functional/test_satlab.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/providers/test_ansible_tower.py` & `broker-0.3.1/tests/providers/test_ansible_tower.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/providers/test_container.py` & `broker-0.3.1/tests/providers/test_container.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/test_broker.py` & `broker-0.3.1/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/test_helpers.py` & `broker-0.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.0/tests/test_settings.py` & `broker-0.3.1/tests/test_settings.py`

 * *Files identical despite different names*

