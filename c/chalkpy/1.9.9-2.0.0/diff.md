# Comparing `tmp/chalkpy-1.9.9.tar.gz` & `tmp/chalkpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalkpy-1.9.9.tar", last modified: Tue Nov 22 03:28:53 2022, max compression
+gzip compressed data, was "chalkpy-2.0.0.tar", last modified: Mon May  1 18:58:09 2023, max compression
```

## Comparing `chalkpy-1.9.9.tar` & `chalkpy-2.0.0.tar`

### file list

```diff
@@ -1,953 +1,925 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.642167 chalkpy-1.9.9/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      425 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      861 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (122)      753 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      868 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      794 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-11-22 03:28:40.000000 chalkpy-1.9.9/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2022-11-22 03:28:53.642167 chalkpy-1.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7084 2022-11-22 03:28:40.000000 chalkpy-1.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      495 2022-11-22 03:28:40.000000 chalkpy-1.9.9/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/
--rw-r--r--   0 runner    (1001) docker     (122)     8611 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3260 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/client/
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17134 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/client/client_impl.py
--rw-r--r--   0 runner    (1001) docker     (122)    14428 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/client/client_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/clogging/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/clogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/clogging/chalk_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/config/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/config/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/df/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/df/ChalkDataFrameImpl.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/df/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/
--rw-r--r--   0 runner    (1001) docker     (122)    14204 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_1/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_10/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      598 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_10/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_100/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_100/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_101/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5074 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_101/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_102/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_102/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5125 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_102/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_103/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_103/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5176 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_103/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_104/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_104/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5227 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_104/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_105/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_105/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5278 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_105/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.590167 chalkpy-1.9.9/chalk/feature_n/feature_106/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_106/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5329 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_106/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_107/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_107/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5380 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_107/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_108/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_108/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5431 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_108/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_109/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_109/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_11/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_11/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_110/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5533 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_110/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_111/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_111/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_111/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_112/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_112/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_112/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_113/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_113/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5686 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_113/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_114/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5737 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_114/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_115/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_115/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5788 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_115/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_116/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_116/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5839 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_116/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_117/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5890 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_117/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_118/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_118/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5941 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_118/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_119/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5992 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_119/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_12/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_12/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_120/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_120/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_121/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_121/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6094 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_121/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_122/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_122/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_123/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6196 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_123/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_124/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_124/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6247 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_124/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_125/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_125/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_126/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_126/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6349 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_126/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_127/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_127/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_127/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_128/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_128/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6451 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_128/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.594167 chalkpy-1.9.9/chalk/feature_n/feature_129/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_129/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6502 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_129/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_13/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_13/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_130/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_130/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_131/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6604 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_131/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_132/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6655 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_132/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_133/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_133/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_133/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_134/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_134/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6757 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_134/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_135/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_135/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6808 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_135/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_136/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_136/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6859 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_136/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_137/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_137/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6910 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_137/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_138/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_138/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6961 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_138/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_139/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_139/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7012 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_139/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_14/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_14/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_140/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7063 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_140/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_141/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7114 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_141/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_142/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_142/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7165 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_142/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_143/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_143/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_143/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_144/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_144/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7267 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_144/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_145/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_145/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7318 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_145/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_146/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_146/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7369 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_146/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_147/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_147/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7420 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_147/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_148/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_148/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_148/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_149/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_149/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7522 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_149/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_15/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_15/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_150/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7573 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_150/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.598167 chalkpy-1.9.9/chalk/feature_n/feature_151/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7624 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_151/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_152/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7675 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_152/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_153/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_153/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7726 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_153/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_154/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_154/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7777 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_154/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_155/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_155/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7828 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_155/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_156/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_156/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7879 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_156/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_157/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_157/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7930 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_157/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_158/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_158/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7981 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_158/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_159/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_159/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8032 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_159/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_16/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_16/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_160/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8083 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_160/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_161/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_161/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8134 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_161/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_162/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_162/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8185 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_162/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_163/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_163/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8236 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_163/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_164/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_164/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8287 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_164/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_165/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_165/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8338 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_165/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_166/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8389 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_166/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_167/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_167/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8440 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_167/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_168/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_168/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8491 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_168/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_169/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_169/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8542 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_169/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_17/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_17/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_170/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_170/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8593 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_170/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_171/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_171/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8644 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_171/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_172/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_172/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8695 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_172/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.602167 chalkpy-1.9.9/chalk/feature_n/feature_173/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_173/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8746 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_173/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_174/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_174/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8797 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_174/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_175/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_175/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8848 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_175/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_176/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_176/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8899 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_176/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_177/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_177/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_177/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_178/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_178/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9001 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_178/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_179/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_179/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9052 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_179/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_18/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_18/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_180/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_180/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9103 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_180/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_181/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9154 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_181/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_182/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_182/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9205 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_182/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_183/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_183/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9256 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_183/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_184/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_184/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9307 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_184/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_185/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_185/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9358 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_185/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_186/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_186/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9409 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_186/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_187/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_187/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9460 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_187/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_188/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_188/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9511 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_188/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_189/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_189/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9562 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_189/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_19/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_19/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      888 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_19/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_190/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_190/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9613 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_190/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_191/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_191/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9664 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_191/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_192/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_192/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_192/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_193/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_193/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9766 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_193/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_194/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_194/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9817 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_194/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_195/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_195/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9868 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_195/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.606167 chalkpy-1.9.9/chalk/feature_n/feature_196/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9919 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_196/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_197/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_197/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9970 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_197/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_198/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_198/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10021 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_198/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_199/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_199/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10072 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_199/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_2/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_20/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_20/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_200/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10123 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_200/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_201/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_201/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_201/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_202/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_202/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10225 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_202/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_203/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_203/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10276 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_203/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_204/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_204/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10327 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_204/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_205/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10378 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_205/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_206/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_206/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10429 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_206/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_207/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_207/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10480 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_207/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_208/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_208/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10531 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_208/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_209/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10582 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_209/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_21/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_21/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_210/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10633 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_210/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_211/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_211/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10684 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_211/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_212/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10735 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_212/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_213/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_213/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10786 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_213/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_214/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_214/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10837 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_214/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_215/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_215/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10888 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_215/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_216/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_216/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10939 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_216/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_217/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_217/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10990 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_217/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.610167 chalkpy-1.9.9/chalk/feature_n/feature_218/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_218/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11041 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_218/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_219/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11092 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_219/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_22/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      987 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_22/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_220/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11143 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_220/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_221/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_221/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11194 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_221/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_222/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11245 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_222/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_223/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_223/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11296 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_223/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_224/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_224/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_224/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_225/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11398 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_225/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_226/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_226/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11449 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_226/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_227/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_227/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11500 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_227/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_228/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_228/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_228/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_229/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_229/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11602 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_229/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_23/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_23/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_230/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_230/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11653 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_230/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_231/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11704 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_231/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_232/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_232/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11755 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_232/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_233/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11806 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_233/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_234/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_234/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11857 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_234/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_235/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_235/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11908 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_235/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_236/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_236/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11959 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_236/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_237/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_237/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12010 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_237/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_238/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_238/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12061 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_238/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.614167 chalkpy-1.9.9/chalk/feature_n/feature_239/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_239/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12112 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_239/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_24/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_24/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_240/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12163 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_240/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_241/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_241/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12214 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_241/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_242/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_242/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12265 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_242/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_243/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_243/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12316 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_243/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_244/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_244/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12367 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_244/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_245/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12418 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_245/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_246/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_246/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12469 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_246/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_247/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_247/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12520 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_247/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_248/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_248/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12571 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_248/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_249/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_249/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12622 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_249/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_25/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_25/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_250/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_250/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12673 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_250/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_251/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_251/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12724 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_251/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_252/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_252/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12775 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_252/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_253/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_253/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12826 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_253/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_254/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_254/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12877 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_254/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_255/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_255/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12928 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_255/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_256/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_256/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12979 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_256/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_26/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_26/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_27/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_27/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_28/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_28/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_28/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_29/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_29/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_29/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_3/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.618167 chalkpy-1.9.9/chalk/feature_n/feature_30/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_30/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_30/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_31/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_31/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_32/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1823 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_32/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_33/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1870 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_33/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_34/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_34/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_35/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_35/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1964 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_35/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_36/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_36/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_37/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_37/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_38/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_38/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_39/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_39/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_39/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_4/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_4/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_40/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_40/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_41/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_41/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_41/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_42/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_42/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_43/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_43/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_43/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_44/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_44/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_44/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_45/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_45/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_45/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_46/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_46/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2481 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_46/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_47/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_47/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_48/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_48/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_48/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_49/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_49/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_49/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_5/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_5/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_50/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_50/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_51/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_51/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_51/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_52/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_52/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2763 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_52/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_53/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_53/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_54/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_54/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_54/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.622167 chalkpy-1.9.9/chalk/feature_n/feature_55/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_55/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_55/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_56/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2951 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_56/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_57/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_57/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_58/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_58/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_58/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_59/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_59/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_59/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_6/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      486 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_6/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_60/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_60/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3139 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_60/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_61/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3186 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_61/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_62/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3233 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_62/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_63/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_63/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3280 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_63/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_64/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_64/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_65/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_65/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_65/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_66/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_66/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_66/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_67/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_67/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_67/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_68/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3515 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_68/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_69/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_69/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3562 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_69/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_7/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_7/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_70/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_70/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3609 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_70/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_71/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_71/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_71/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_72/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_72/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_72/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_73/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_73/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_73/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_74/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_74/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_74/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_75/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_75/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_76/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_76/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3891 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_76/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_77/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_77/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_77/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_78/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_78/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3985 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_78/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.626167 chalkpy-1.9.9/chalk/feature_n/feature_79/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_79/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_79/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_8/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      540 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_8/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_80/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4079 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_80/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_81/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_81/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_81/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_82/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_82/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_83/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_83/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_83/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_84/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_84/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4267 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_84/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_85/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_85/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4314 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_85/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_86/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4361 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_86/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_87/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_87/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4408 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_87/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_88/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_88/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_88/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_89/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4502 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_89/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_9/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_9/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_90/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_90/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_90/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_91/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_91/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4596 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_91/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_92/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4643 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_92/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_93/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_93/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_93/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_94/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_94/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4737 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_94/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_95/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_95/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_95/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_96/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_96/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4831 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_96/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_97/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_97/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_97/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_98/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_98/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_98/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.630167 chalkpy-1.9.9/chalk/feature_n/feature_99/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4972 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/feature_n/feature_99/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42343 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)    13124 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/feature_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     5528 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (122)    18782 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/feature_set_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5219 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/feature_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4755 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)      920 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/pseudofeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)    22171 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/features/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/gitignore/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7297 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/gitignore/gitignore_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/integrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      580 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/integrations/named.py
--rw-r--r--   0 runner    (1001) docker     (122)    15643 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/parsed/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3443 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/parsed/duplicate_input_gql.py
--rw-r--r--   0 runner    (1001) docker     (122)     7805 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/parsed/json_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/parsed/user_types_to_json.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/serialization/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     7813 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/serialization/parsed_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/sql/
--rw-r--r--   0 runner    (1001) docker     (122)     5358 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/sql/base/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10395 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/base/protocols.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/base/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     5668 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/base/sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/sql/integrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1919 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7907 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/redshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2314 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (122)     5851 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/sql/integrations/string_chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (122)      732 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/state.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/streams/
--rw-r--r--   0 runner    (1001) docker     (122)      502 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_file_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_internal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_kafka_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      777 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_keyed_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/streams/_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.634167 chalkpy-1.9.9/chalk/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/chalk/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     3915 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/environment_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     6320 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/json_log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/metaprogramming.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (122)    13386 2022-11-22 03:28:40.000000 chalkpy-1.9.9/chalk/utils/stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/chalkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7945 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24200 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      574 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-22 03:28:53.000000 chalkpy-1.9.9/chalkpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      360 2022-11-22 03:28:40.000000 chalkpy-1.9.9/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)     2573 2022-11-22 03:28:40.000000 chalkpy-1.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-22 03:28:40.000000 chalkpy-1.9.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-11-22 03:28:40.000000 chalkpy-1.9.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 03:28:53.642167 chalkpy-1.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2022-11-22 03:28:40.000000 chalkpy-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/_gitignore/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/_gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4908 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/_gitignore/test_gitignore_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/client/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/client/test_client_serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/client/test_expand_features.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/features/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      974 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_chained_feature_time.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_chained_has_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_custom_name.py
--rw-r--r--   0 runner    (1001) docker     (122)    17918 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_df.py
--rw-r--r--   0 runner    (1001) docker     (122)     6373 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_feature_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)     4976 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_features.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_id_assignment.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)      987 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_resolver_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_resolvers_callable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/features/test_ts_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/mypy/mypy_docs_demo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/mypy/mypy_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/mypy/test_mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/parsed/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/parsed/test_user_types_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/serialization/test_codec.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/sql/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/sql/test_implicit_mappings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/sql/test_sql_features.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/sql/test_table_ingest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      767 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/streams/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/streams/test_window.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)      504 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3788 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/test_log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/test_stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.586166 chalkpy-1.9.9/tests/utils/typings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.586166 chalkpy-1.9.9/tests/utils/typings/chalk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/tests/utils/typings/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2022-11-22 03:28:40.000000 chalkpy-1.9.9/tests/utils/typings/chalk/features/feature_set_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.586166 chalkpy-1.9.9/typings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.586166 chalkpy-1.9.9/typings/chalk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 03:28:53.638167 chalkpy-1.9.9/typings/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (122)    48523 2022-11-22 03:28:40.000000 chalkpy-1.9.9/typings/chalk/features/feature_set_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.510142 chalkpy-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 18:57:50.000000 chalkpy-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-01 18:58:09.510142 chalkpy-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-01 18:57:50.000000 chalkpy-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/_autosql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_autosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_autosql/autosql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/charts_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/charts_enums_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/charts_series_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_monitoring/gql_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/_reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_reporting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_reporting/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_validation/feature_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.430141 chalkpy-2.0.0/chalk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    35537 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42271 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/client/client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/client/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24498 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/clogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/clogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/clogging/chalk_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/config/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/config/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/df/ChalkDataFrameImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/df/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_1/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_10/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_100/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_100/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_100/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_101/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_102/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_102/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_102/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_103/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_103/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_103/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_104/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_104/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_104/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_105/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_105/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_105/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_106/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_106/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_106/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.434141 chalkpy-2.0.0/chalk/feature_n/feature_107/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_107/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_107/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_108/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_108/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_108/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_109/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_109/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_11/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_110/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_111/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_111/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_111/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_112/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_112/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_112/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_113/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_113/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_113/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_114/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_115/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_115/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_115/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_116/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_116/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_116/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_117/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_118/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_118/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_118/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_119/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_119/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_12/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_120/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_120/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.438141 chalkpy-2.0.0/chalk/feature_n/feature_121/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_121/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_122/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_123/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_123/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_124/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_124/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_124/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_125/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_126/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_126/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_126/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_127/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_127/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_127/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_128/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_128/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_128/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_129/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_129/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_129/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_13/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_130/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_131/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_131/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_132/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_133/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_133/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_133/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_134/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_134/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.442141 chalkpy-2.0.0/chalk/feature_n/feature_135/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_135/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_135/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_136/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_136/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_136/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_137/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_137/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_137/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_138/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_138/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_138/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_139/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_139/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_139/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_14/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_140/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_141/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_142/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_142/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_142/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_143/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_143/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_143/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_144/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_144/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_144/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_145/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_145/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_145/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_146/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_146/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_146/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_147/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_147/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_147/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_148/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_148/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_148/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_149/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_149/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_15/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.446142 chalkpy-2.0.0/chalk/feature_n/feature_150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_150/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_151/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_152/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_153/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_153/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_153/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_154/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_154/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_154/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_155/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_155/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_155/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_156/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_156/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_156/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_157/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_157/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_157/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_158/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_158/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_158/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_159/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_159/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_159/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_16/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_160/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_161/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_161/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_161/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_162/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_162/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_162/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_163/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_163/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_163/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.450142 chalkpy-2.0.0/chalk/feature_n/feature_164/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_164/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_164/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_165/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_165/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_165/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_166/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_166/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_167/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_167/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_167/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_168/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_168/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_168/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_169/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_169/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_169/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_17/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_170/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_170/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_170/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_171/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_171/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_171/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_172/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_172/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_172/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_173/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_173/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_173/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_174/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_174/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_174/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_175/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_175/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_175/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_176/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_176/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_176/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_177/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_177/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_177/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.454142 chalkpy-2.0.0/chalk/feature_n/feature_178/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_178/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_178/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_179/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_179/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_179/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_18/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_180/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_180/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_180/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_181/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_181/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_182/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_182/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_182/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_183/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_183/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_183/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_184/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_184/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_184/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_185/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_185/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_185/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_186/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_186/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_186/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_187/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_187/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_187/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_188/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_188/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_188/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_189/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_189/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_189/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_19/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_19/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_190/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_190/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_190/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_191/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_191/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_191/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.458142 chalkpy-2.0.0/chalk/feature_n/feature_192/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_192/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_192/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_193/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_193/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_193/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_194/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_194/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_194/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_195/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_195/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_195/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_196/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_196/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_197/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_197/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_198/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_198/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_198/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_199/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_199/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_199/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_2/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_20/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_200/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_200/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_201/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_201/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_201/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_202/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_202/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_202/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_203/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_203/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_203/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_204/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_204/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_204/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.462142 chalkpy-2.0.0/chalk/feature_n/feature_205/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_205/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_206/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_206/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_206/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_207/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_207/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_207/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_208/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_208/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_208/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_209/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_21/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_210/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_211/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_211/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_211/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_212/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_213/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_213/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_213/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_214/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_214/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_214/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_215/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_215/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_215/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_216/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_216/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_216/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_217/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_217/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_217/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_218/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_218/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_218/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_219/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_219/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.466142 chalkpy-2.0.0/chalk/feature_n/feature_22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_22/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_220/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_221/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_221/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_221/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_222/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_222/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_223/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_223/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_223/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_224/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_224/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_224/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_225/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_225/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_226/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_226/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_226/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_227/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_227/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_227/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_228/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_228/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_228/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_229/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_229/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_229/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_23/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_230/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_230/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_230/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_231/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_231/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_232/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_232/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_233/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_233/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_234/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_234/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_234/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.470142 chalkpy-2.0.0/chalk/feature_n/feature_235/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_235/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_235/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_236/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_236/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_236/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_237/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_237/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_237/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_238/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_238/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_238/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_239/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_239/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_239/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_24/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_24/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_240/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_241/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_241/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_241/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_242/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_242/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_242/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_243/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_243/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_243/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_244/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_244/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_244/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_245/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_245/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_245/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_246/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_246/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_246/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_247/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_247/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_247/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_248/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_248/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_248/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_249/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_249/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_249/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_25/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_25/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.474142 chalkpy-2.0.0/chalk/feature_n/feature_250/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_250/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_250/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_251/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_251/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_251/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_252/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_252/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_252/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_253/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_253/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_253/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_254/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_254/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_254/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_255/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_255/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_255/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_256/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_256/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_256/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_26/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_27/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_27/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_28/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_28/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_28/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_29/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_29/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_29/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_3/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_30/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_30/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_30/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_31/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_32/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_33/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.478142 chalkpy-2.0.0/chalk/feature_n/feature_34/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_34/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_35/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_35/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_35/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_36/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_36/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_37/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_37/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_38/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_38/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_39/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_39/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_39/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_4/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.482142 chalkpy-2.0.0/chalk/feature_n/feature_40/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_40/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_41/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_41/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_41/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_42/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_43/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_43/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_43/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_44/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_44/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_44/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_45/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_45/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_45/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_46/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_46/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_46/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_47/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_48/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_48/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_48/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_49/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_49/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_49/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_5/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_50/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_50/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_51/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_51/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_51/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_52/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_52/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_52/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_53/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_53/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_54/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_54/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_54/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_55/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_55/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_55/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_56/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_56/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.486142 chalkpy-2.0.0/chalk/feature_n/feature_57/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_57/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_58/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_58/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_58/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_59/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_59/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_59/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_6/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_60/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_60/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_60/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_61/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_61/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_62/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_62/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_63/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_63/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_63/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_64/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_65/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_65/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_65/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_66/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_66/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_66/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_67/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_67/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_67/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_68/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_69/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_69/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_69/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_7/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_70/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_70/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_70/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_71/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_71/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_71/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.490142 chalkpy-2.0.0/chalk/feature_n/feature_72/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_72/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_72/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_73/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_73/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_73/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_74/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_74/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_74/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_75/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_75/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_76/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_76/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_76/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_77/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_77/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_77/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_78/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_78/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_78/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_79/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_79/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_79/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_8/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_80/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_80/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_81/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_81/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_81/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_82/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_83/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_83/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_83/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_84/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_84/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_84/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_85/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_85/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_85/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_86/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_86/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_87/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_87/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_87/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.494142 chalkpy-2.0.0/chalk/feature_n/feature_88/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_88/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_88/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_89/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_9/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_90/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_90/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_90/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_91/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_91/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_91/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_92/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_92/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_93/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_93/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_93/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_94/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_94/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_94/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_95/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_95/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_95/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_96/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_96/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_96/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_97/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_97/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_97/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_98/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_98/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_98/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.498142 chalkpy-2.0.0/chalk/feature_n/feature_99/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_99/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/feature_n/feature_99/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_chalkop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/features/_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/missing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/_encoding/serialized_dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/features/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/dataframe/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51213 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/dataframe/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/dataframe/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30875 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/feature_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29431 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/feature_set_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/feature_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/feature_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/live_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/pseudofeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/features/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/gitignore/gitignore_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/gitignore/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/integrations/named.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.502142 chalkpy-2.0.0/chalk/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/parsed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/parsed/_graph_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/parsed/duplicate_input_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/parsed/json_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/parsed/user_types_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/serialization/parsed_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sink/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/sql/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/sql/_internal/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/integrations/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/sql_file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/sql_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/_internal/string_chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/finalized_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/sql/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/_kafka_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/streams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.506142 chalkpy-2.0.0/chalk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.510142 chalkpy-2.0.0/chalk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/annotation_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/cached_type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/environment_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/log_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/metaprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/missing_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-05-01 18:57:50.000000 chalkpy-2.0.0/chalk/utils/stubgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:58:09.510142 chalkpy-2.0.0/chalkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-01 18:58:09.000000 chalkpy-2.0.0/chalkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-01 18:57:50.000000 chalkpy-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:58:09.510142 chalkpy-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 18:57:50.000000 chalkpy-2.0.0/setup.py
```

### Comparing `chalkpy-1.9.9/PKG-INFO` & `chalkpy-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: chalkpy
-Version: 1.9.9
+Version: 2.0.0
 Summary: Python SDK for Chalk
-Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
+Project-URL: homepage, https://chalk.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
+Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8.0
+Requires-Python: <3.12,>3.8
 Description-Content-Type: text/markdown
-Provides-Extra: bigquery
+Provides-Extra: base
 Provides-Extra: dev
+Provides-Extra: runtime
+Provides-Extra: sql
+Provides-Extra: bigquery
 Provides-Extra: postgresql
 Provides-Extra: snowflake
 Provides-Extra: sqlite
 Provides-Extra: redshift
 Provides-Extra: mysql
+Provides-Extra: all
+Provides-Extra: polars
 
 # Chalk
 
 Chalk enables innovative machine learning teams to focus on building
 the unique products and models which make their business stand out.
 Behind the scenes Chalk seamlessly handles data infrastructure with
 a best-in-class developer experience. Here’s how it works –
@@ -45,24 +54,24 @@
 To get started, [define your features](/docs/features) with
 [Pydantic](https://pydantic-docs.helpmanual.io/)-inspired Python classes.
 You can define schemas, specify relationships, and add metadata
 to help your team share and re-use work.
 
 ```py
 @features
-class UserFeatures:
+class User:
     id: int
     full_name: str
     nickname: Optional[str]
     email: Optional[str]
     birthday: date
     credit_score: float
     datawarehouse_feature: float
 
-    transactions = has_many(lambda:  TransactionFeature.user_id == UserFeatures.id)
+    transactions = has_many(lambda: Transaction.user_id == User.id)
 ```
 
 ### Resolvers
 
 Next, tell Chalk how to compute your features.
 Chalk ingests data from your existing data stores,
 and lets you use Python to compute features with
@@ -76,19 +85,18 @@
 #### SQL
 
 ```python
 pg = PostgreSQLSource()
 
 @online
 def get_user(uid: User.id) -> Features[User.full_name, User.email]:
-    return (
-        pg.query(User(email=UserSQL.email, full_name=UserSQL.name))
-        .filter_by(id=uid)
-        .first()
-    )
+    return pg.query_string(
+        "select email, full_name from users where id=:id",
+        args=dict(id=uid)
+    ).one()
 ```
 
 #### REST
 
 ```python
 import requests
 
@@ -227,15 +235,15 @@
 
 Data scientists can use Chalk's Jupyter integration to create datasets
 and train models. Datasets are stored and tracked so that they can be
 re-used by other modelers, and so that model provenance is tracked for
 audit and reproducibility.
 
 ```python
-X = ChalkClient.get_training_dataframe(
+X = ChalkClient.offline_query(
     input=labels[[User.uid, timestamp]],
     output=[
         User.returned_transactions_last_60,
         User.user_account_name_match_score,
         User.socure_score,
         User.identity.has_verified_phone,
         User.identity.is_voip_phone,
```

### Comparing `chalkpy-1.9.9/README.md` & `chalkpy-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 To get started, [define your features](/docs/features) with
 [Pydantic](https://pydantic-docs.helpmanual.io/)-inspired Python classes.
 You can define schemas, specify relationships, and add metadata
 to help your team share and re-use work.
 
 ```py
 @features
-class UserFeatures:
+class User:
     id: int
     full_name: str
     nickname: Optional[str]
     email: Optional[str]
     birthday: date
     credit_score: float
     datawarehouse_feature: float
 
-    transactions = has_many(lambda:  TransactionFeature.user_id == UserFeatures.id)
+    transactions = has_many(lambda: Transaction.user_id == User.id)
 ```
 
 ### Resolvers
 
 Next, tell Chalk how to compute your features.
 Chalk ingests data from your existing data stores,
 and lets you use Python to compute features with
@@ -52,19 +52,18 @@
 #### SQL
 
 ```python
 pg = PostgreSQLSource()
 
 @online
 def get_user(uid: User.id) -> Features[User.full_name, User.email]:
-    return (
-        pg.query(User(email=UserSQL.email, full_name=UserSQL.name))
-        .filter_by(id=uid)
-        .first()
-    )
+    return pg.query_string(
+        "select email, full_name from users where id=:id",
+        args=dict(id=uid)
+    ).one()
 ```
 
 #### REST
 
 ```python
 import requests
 
@@ -203,15 +202,15 @@
 
 Data scientists can use Chalk's Jupyter integration to create datasets
 and train models. Datasets are stored and tracked so that they can be
 re-used by other modelers, and so that model provenance is tracked for
 audit and reproducibility.
 
 ```python
-X = ChalkClient.get_training_dataframe(
+X = ChalkClient.offline_query(
     input=labels[[User.uid, timestamp]],
     output=[
         User.returned_transactions_last_60,
         User.user_account_name_match_score,
         User.socure_score,
         User.identity.has_verified_phone,
         User.identity.is_voip_phone,
```

### Comparing `chalkpy-1.9.9/chalk/cli.py` & `chalkpy-2.0.0/chalk/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 import argparse
 import json
-import logging
+import logging as pylogging
 import os
 import sys
 import traceback
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import ValidationError
 
-from chalk import importer
-from chalk.config.project_config import ProjectSettings, load_project_config
+from chalk.config.project_config import load_project_config
+from chalk.importer import import_all_files
 from chalk.parsed.user_types_to_json import get_registered_types_as_json
 from chalk.utils.stubgen import configure_stubgen_argparse, run_stubgen
 
 
-def _get_list_results(directory: Optional[str]):
+def _get_list_results(directory: Optional[str], file_allowlist: Optional[List[str]]):
     scope_to = Path(directory or os.getcwd())
     try:
-        failed = importer.import_all_python_files()
+        failed = import_all_files(file_allowlist=file_allowlist)
         return get_registered_types_as_json(scope_to, failed)
     except Exception:
         ex_type, ex_value, ex_traceback = sys.exc_info()
         assert ex_type is not None
         relevant_traceback = f"""{os.linesep.join(traceback.format_tb(ex_traceback))}
 \n{ex_type.__name__}: {str(ex_value)}
 """
         return json.dumps(dict(failed=[dict(traceback=relevant_traceback)]), indent=2)
 
 
-def dump_cmd(filename: str, directory: Optional[str]):
+def dump_cmd(filename: str, directory: Optional[str], filter_file: Optional[str]):
+    file_allowlist = None
+    if filter_file is not None and os.path.exists(filter_file):
+        with open(filter_file) as f:
+            file_allowlist = [f.strip() for f in f.readlines()]
+
     with open(filename, "w") as f:
-        f.write(_get_list_results(directory))
+        f.write(
+            _get_list_results(
+                directory=directory,
+                file_allowlist=file_allowlist,
+            )
+        )
 
 
 def list_cmd(directory: str):
-    print(_get_list_results(directory))
+    print(_get_list_results(directory=directory, file_allowlist=None))
 
 
 def config_cmd():
     json_response: str
     try:
-        model = load_project_config() or ProjectSettings()
-        json_response = model.json()
+        model = load_project_config()
     except ValidationError as e:
         json_response = json.dumps({"error": str(e)})
+    else:
+        if model is None:
+            print("No `chalk.yaml` configuration file found")
+            return
+        json_response = model.json()
 
     print(json_response)
 
 
 def cli(args_override: Optional[List[str]] = None):
     parser = argparse.ArgumentParser(
         prog="Chalk Python CLI",
@@ -61,36 +75,54 @@
     subparsers = parser.add_subparsers(dest="command")
     subparsers.add_parser("config", help="Print the config for the current project")
     list_parser = subparsers.add_parser("list", help="List the resolvers for the current project and print as json")
     list_parser.add_argument("--directory", help="Scope to this directory", nargs="?")
     dump_parser = subparsers.add_parser("dump", help="Write the resolvers for the current project to the given file")
     dump_parser.add_argument("filename", help="Write to this file")
     dump_parser.add_argument("--directory", help="Scope to this directory", nargs="?")
+    export_parser = subparsers.add_parser(
+        "export", help="Write the resolvers for the current project to the given file"
+    )
+    export_parser.add_argument("filename", help="Write to this file")
+    export_parser.add_argument("--directory", help="Scope to this directory", nargs="?")
+    export_parser.add_argument("--file_filter", help="Path containing only files to consider", nargs="?")
     stubgen_parser = subparsers.add_parser("stubgen", help="Generate type stubs for feature set classes")
+    stubgen_parser.add_argument("--file_filter", help="Path containing only files to consider", nargs="?")
     configure_stubgen_argparse(stubgen_parser)
-    args = parser.parse_args(args_override)
+
+    # Parsing only known args for forwards compatibility.
+    # Changing this to `.parse_args` means once the args are
+    # set for a command, you can never add to them.
+    # Please do not change to `.parse_args`.
+    args, _ = parser.parse_known_args(args_override)
     if args.log_level:
-        level = getattr(logging, args.log_level.upper())
-        logging.basicConfig(
+        level = getattr(pylogging, args.log_level.upper())
+        pylogging.basicConfig(
             format="%(asctime)s %(levelname)s: %(message)s",
             datefmt="%m/%d/%Y %I:%M:%S %p",
             level=level,
         )
 
     if args.command == "list":
         list_cmd(args.directory)
 
     elif args.command == "config":
         config_cmd()
 
     elif args.command == "stubgen":
-        run_stubgen(args)
+        run_stubgen(args, args.file_filter)
+
+    elif args.command == "export":
+        dump_cmd(args.filename, args.directory, args.file_filter)
 
     elif args.command == "dump":
-        dump_cmd(args.filename, args.directory)
+        dump_cmd(args.filename, args.directory, None)
+
     else:
         parser.print_help(sys.stderr)
-        sys.exit(1)
+        return 1
+
+    return 0
 
 
 if __name__ == "__main__":
-    cli()
+    sys.exit(cli())
```

### Comparing `chalkpy-1.9.9/chalk/config/auth_config.py` & `chalkpy-2.0.0/chalk/config/project_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,67 @@
-import logging
+import itertools
 import os
-from functools import lru_cache
 from pathlib import Path
-from typing import Mapping, Optional
+from typing import List, Literal, Mapping, Optional
 
 import yaml
 from pydantic import BaseModel
 
-from chalk.config.project_config import load_project_config
+from chalk._version import __version__
 
-_logger = logging.getLogger(__name__)
 
+class EnvironmentSettings(BaseModel):
+    runtime: Optional[Literal["python310"]]
+    requirements: Optional[str]
+    dockerfile: Optional[str]
 
-class TokenConfig(BaseModel):
-    name: Optional[str]
-    clientId: Optional[str]
-    clientSecret: Optional[str]
-    apiServer: Optional[str]
-    activeEnvironment: Optional[str]
 
+class MetadataSettings(BaseModel):
+    name: str
+    missing: str
 
-class AuthConfig(BaseModel):
-    tokens: Optional[Mapping[str, TokenConfig]]
 
+class FeatureSettings(BaseModel):
+    metadata: Optional[List[MetadataSettings]]
 
-# using lru_cache for 3.8 compat
-@lru_cache(maxsize=None)
-def _load_global_config() -> Optional[AuthConfig]:
-    home = os.getenv("XDG_CONFIG_HOME", os.path.expanduser("~"))
-    path = None
-    for filename in [".chalk.yml"]:
-        p = os.path.join(home, filename)
-        if os.path.exists(p):
-            path = p
 
-    if path is None:
-        return None
+class ValidationSettings(BaseModel):
+    feature: Optional[FeatureSettings]
+
 
-    with open(path, "r") as f:
-        parsed = yaml.safe_load(f)
-        return AuthConfig(**parsed)
+class ProjectSettings(BaseModel):
+    project: str
+    environments: Optional[Mapping[str, EnvironmentSettings]]
+    validation: Optional[ValidationSettings]
+    local_path: str
+    chalkpy: str
 
 
-def _load_config_from_env() -> Optional[TokenConfig]:
-    envvars = dict(
-        clientId=os.getenv("_CHALK_CLIENT_ID"),
-        clientSecret=os.getenv("_CHALK_CLIENT_SECRET"),
-        apiServer=os.getenv("_CHALK_API_SERVER"),
-        activeEnvironment=os.getenv("_CHALK_ACTIVE_ENVIRONMENT"),
-    )
-    if any(v is None for v in envvars.values()):
+def _load_project_config_at_path(filename: Path) -> Optional[ProjectSettings]:
+    has_default_requirements = os.path.exists(filename.parent / "requirements.txt")
+    try:
+        with open(filename, "r") as f:
+            parsed = yaml.safe_load(f)
+            settings = ProjectSettings(
+                **parsed,
+                local_path=str(filename.absolute().resolve()),
+                chalkpy=__version__,
+            )
+            if has_default_requirements and settings.environments is not None:
+                for cfg in settings.environments.values():
+                    if cfg.requirements is None:
+                        cfg.requirements = "requirements.txt"
+            return settings
+    except OSError:
         return None
 
-    return TokenConfig(**envvars)
 
+def load_project_config() -> Optional[ProjectSettings]:
+    base = Path(os.getcwd())
 
-def load_token() -> Optional[TokenConfig]:
-    envvar_config = _load_config_from_env()
-    if envvar_config is not None:
-        return envvar_config
+    for d in itertools.chain([base], base.parents):
+        project = _load_project_config_at_path(d / "chalk.yaml") or _load_project_config_at_path(d / "chalk.yml")
 
-    global_cfg = _load_global_config()
-    if global_cfg is None:
-        return None
+        if project is not None:
+            return project
 
-    absdir = Path(os.getcwd()).absolute().resolve()
-    project_config = load_project_config()
-    if project_config:
-        absdir = Path(project_config.local_path).parent
-    tokens = global_cfg.tokens or {}
-    return tokens.get(str(absdir)) or tokens.get("default")
+    return None
```

### Comparing `chalkpy-1.9.9/chalk/df/ast_parser.py` & `chalkpy-2.0.0/chalk/df/ast_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 from types import FrameType
 from typing import Any, Callable, Dict, Optional, Union
 
 from executing import Source
 
 from chalk.features import Filter
+from chalk.features._chalkop import op
 
 
 class ExecutingException(Exception):
     pass
 
 
 class RetrievingError(ExecutingException):
@@ -20,15 +21,15 @@
     """Get the node by frame, raise errors if possible"""
     exect = Source.executing(frame)
 
     if exect.node:
         # attach the frame for better exception message
         # (i.e. where ImproperUseError happens)
         exect.node.__frame__ = frame  # type: ignore
-        return exect.node  # type: ignore
+        return exect.node
 
     assert isinstance(exect.source, Source)
     if exect.source.text and exect.source.tree and raise_exc:
         raise RetrievingError(
             (
                 "Couldn't retrieve the call node. "
                 "This may happen if you're using some other AST magic at the "
@@ -51,14 +52,31 @@
             # ast.Name would imply something like this:
             # def __getitem__(self, item):
             #    return self.df[item]  # <--- item is of type ast.name. We need to go one frame higher!
             return frame, func_node
     raise RuntimeError("Condition not found in stack")
 
 
+def parse_feature_iter(f):
+    func_frame, func_node = _get_func_frame_and_nodes(lambda node: isinstance(node, ast.Call))
+    if not isinstance(func_node, ast.Call):
+        raise RuntimeError("Could not evaluate function")
+    if not isinstance(func_node.func, ast.Name):
+        raise RuntimeError("Could not evaluate function")
+    func_name = func_node.func.id
+    if func_name == "sum":
+        return op.sum(f)
+    elif func_name == "max":
+        return op.max(f)
+    elif func_name == "min":
+        return op.min(f)
+
+    raise RuntimeError(f"Could not evaluate function {func_name}")
+
+
 def parse_dataframe_getitem():
     func_frame, func_node = _get_func_frame_and_nodes(
         lambda node: isinstance(node, ast.Subscript) and not isinstance(node.slice, ast.Name)
     )
     assert isinstance(func_node, ast.Subscript)
     slc = func_node.slice
     if isinstance(slc, ast.Index):
@@ -66,15 +84,14 @@
         assert isinstance(slc, ast.expr)
     converted_slice = convert_slice(slc)
     return eval_converted_expr(converted_slice, glbs=func_frame.f_globals, lcls=func_frame.f_locals)
 
 
 def parse_when() -> Optional[Filter]:
     func_frame, func_node = _get_func_frame_and_nodes(lambda node: isinstance(node, ast.Call))
-    when_filter = None
     assert isinstance(func_node, ast.Call)
     when = next((k for k in func_node.keywords if k.arg == "when"), None)
     when_filter = convert_slice(when.value) if when else None
     assert isinstance(when_filter, ast.expr)
     return (
         eval_converted_expr(when_filter, glbs=func_frame.f_globals, lcls=func_frame.f_locals) if when_filter else None
     )
```

### Comparing `chalkpy-1.9.9/chalk/feature_n/__init__.py` & `chalkpy-2.0.0/chalk/feature_n/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/codegen.py` & `chalkpy-2.0.0/chalk/feature_n/codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_10/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_10/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_100/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_100/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_101/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_101/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_102/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_102/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_103/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_103/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_104/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_104/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_105/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_105/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_106/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_106/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_107/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_107/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_108/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_108/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_109/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_109/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_11/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_11/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_110/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_110/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_111/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_111/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_112/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_112/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_113/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_113/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_114/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_114/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_115/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_115/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_116/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_116/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_117/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_117/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_118/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_118/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_119/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_119/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_12/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_12/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_120/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_120/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_121/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_121/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_122/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_122/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_123/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_123/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_124/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_124/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_125/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_125/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_126/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_126/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_127/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_127/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_128/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_128/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_129/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_129/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_13/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_13/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_130/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_130/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_131/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_131/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_132/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_132/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_133/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_133/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_134/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_134/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_135/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_135/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_136/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_136/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_137/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_137/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_138/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_138/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_139/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_139/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_14/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_14/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_140/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_140/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_141/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_141/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_142/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_142/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_143/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_143/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_144/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_144/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_145/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_145/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_146/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_146/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_147/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_147/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_148/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_148/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_149/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_149/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_15/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_15/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_150/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_150/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_151/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_151/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_152/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_152/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_153/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_153/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_154/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_154/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_155/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_155/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_156/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_156/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_157/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_157/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_158/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_158/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_159/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_159/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_16/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_16/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_160/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_160/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_161/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_161/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_162/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_162/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_163/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_163/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_164/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_164/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_165/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_165/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_166/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_166/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_167/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_167/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_168/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_168/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_169/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_169/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_17/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_17/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_170/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_170/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_171/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_171/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_172/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_172/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_173/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_173/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_174/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_174/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_175/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_175/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_176/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_176/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_177/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_177/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_178/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_178/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_179/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_179/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_18/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_18/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_180/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_180/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_181/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_181/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_182/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_182/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_183/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_183/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_184/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_184/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_185/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_185/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_186/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_186/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_187/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_187/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_188/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_188/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_189/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_189/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_19/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_19/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_190/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_190/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_191/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_191/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_192/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_192/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_193/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_193/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_194/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_194/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_195/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_195/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_196/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_196/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_197/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_197/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_198/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_198/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_199/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_199/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_20/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_20/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_200/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_200/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_201/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_201/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_202/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_202/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_203/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_203/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_204/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_204/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_205/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_205/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_206/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_206/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_207/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_207/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_208/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_208/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_209/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_209/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_21/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_21/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_210/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_210/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_211/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_211/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_212/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_212/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_213/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_213/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_214/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_214/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_215/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_215/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_216/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_216/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_217/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_217/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_218/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_218/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_219/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_219/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_22/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_22/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_220/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_220/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_221/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_221/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_222/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_222/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_223/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_223/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_224/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_224/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_225/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_225/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_226/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_226/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_227/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_227/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_228/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_228/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_229/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_229/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_23/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_23/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_230/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_230/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_231/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_231/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_232/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_232/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_233/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_233/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_234/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_234/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_235/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_235/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_236/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_236/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_237/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_237/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_238/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_238/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_239/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_239/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_24/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_24/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_240/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_240/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_241/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_241/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_242/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_242/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_243/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_243/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_244/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_244/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_245/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_245/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_246/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_246/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_247/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_247/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_248/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_248/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_249/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_249/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_25/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_25/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_250/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_250/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_251/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_251/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_252/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_252/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_253/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_253/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_254/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_254/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_255/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_255/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_256/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_256/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_26/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_26/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_27/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_27/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_28/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_28/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_29/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_29/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_30/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_30/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_31/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_31/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_32/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_32/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_33/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_33/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_34/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_34/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_35/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_35/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_36/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_36/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_37/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_37/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_38/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_38/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_39/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_39/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_40/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_40/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_41/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_41/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_42/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_42/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_43/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_43/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_44/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_44/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_45/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_45/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_46/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_46/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_47/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_47/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_48/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_48/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_49/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_49/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_50/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_50/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_51/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_51/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_52/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_52/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_53/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_53/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_54/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_54/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_55/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_55/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_56/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_56/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_57/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_57/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_58/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_58/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_59/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_59/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_60/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_60/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_61/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_61/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_62/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_62/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_63/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_63/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_64/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_64/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_65/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_65/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_66/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_66/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_67/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_67/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_68/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_68/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_69/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_69/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_7/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_7/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_70/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_70/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_71/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_71/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_72/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_72/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_73/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_73/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_74/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_74/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_75/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_75/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_76/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_76/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_77/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_77/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_78/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_78/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_79/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_79/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_8/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_8/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_80/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_80/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_81/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_81/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_82/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_82/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_83/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_83/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_84/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_84/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_85/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_85/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_86/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_86/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_87/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_87/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_88/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_88/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_89/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_89/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_9/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_9/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_90/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_90/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_91/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_91/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_92/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_92/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_93/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_93/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_94/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_94/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_95/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_95/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_96/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_96/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_97/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_97/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_98/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_98/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/feature_n/feature_99/feature.py` & `chalkpy-2.0.0/chalk/feature_n/feature_99/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-1.9.9/chalk/features/dataframe.py` & `chalkpy-2.0.0/chalk/features/dataframe/_impl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 from __future__ import annotations
 
+import base64
 import collections.abc
-import datetime
-import enum
-import functools
+import inspect
+import itertools
+import json
 import operator
+import os
 import pathlib
 import warnings
+from datetime import datetime, timezone
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Dict,
     Iterable,
     List,
+    Literal,
+    Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-import polars as pl
+import pyarrow as pa
+from pydantic import BaseModel
 
+from chalk.features._chalkop import Aggregation
+from chalk.features._encoding.missing_value import MissingValueStrategy
+from chalk.features.dataframe._filters import convert_filters_to_pl_expr, filter_data_frame
+from chalk.features.dataframe._validation import validate_df_schema, validate_nulls
 from chalk.features.feature_field import Feature
-from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
-from chalk.features.filter import Filter, TimeDelta
-from chalk.serialization.codec import FEATURE_CODEC
+from chalk.features.feature_wrapper import FeatureWrapper, ensure_feature, unwrap_feature
+from chalk.features.filter import Filter
 from chalk.utils.collections import ensure_tuple, get_unique_item
+from chalk.utils.missing_dependency import missing_dependency_exception
 
 if TYPE_CHECKING:
     import pandas as pd
-    import pyarrow
+    import polars as pl
 
     from chalk.features.feature_set import Features
 
 else:
     try:
         import pandas as pd
     except ImportError:
         pd = None
-    try:
-        import pyarrow
-    except ImportError:
-        pyarrow = None
 
-TDataFrame = TypeVar("TDataFrame", bound="DataFrame")
 
-
-def _polars_data_frames_equal(a: pl.DataFrame, b: pl.DataFrame):
-    return a.frame_equal(b)
+TDataFrame = TypeVar("TDataFrame", bound="DataFrame")
 
 
 class DataFrameMeta(type):
     def __getitem__(cls, item: Any) -> Type[DataFrame]:
         from chalk.features.feature_set import Features
 
         # leaving untyped as we type the individual features as their object type
@@ -81,14 +84,15 @@
         # If doing multiple subscript, then keep the filters, but do not keep the individual columns
         # TODO: Validate that any new columns are a subset of the existing columns
         item = [*item, *cls.filters]
 
         new_filters: List[Filter] = []
         new_references_feature_set: Optional[Type[Features]] = None
         new_columns: List[Feature] = []
+        pydantic_model = None
 
         for a in item:
             if isinstance(a, Filter):
                 new_filters.append(a)
             elif isinstance(a, type) and issubclass(a, Features):
                 if new_references_feature_set is not None:
                     raise ValueError(
@@ -101,14 +105,16 @@
                 new_columns.append(a._chalk_feature)
             elif isinstance(a, bool):
                 # If we encounter a bool, that means we are evaluating the type annotation before
                 # the ResolverAstParser had a chance to extract the source and rewrite the and/or/in operations
                 # into expressions that return filters instead of booleans
                 # This function will be called again for this annotation, so we can ignore it for now.
                 pass
+            elif inspect.isclass(a) and issubclass(a, BaseModel):
+                pydantic_model = a
             else:
                 raise TypeError(f"Invalid type for DataFrame[{a}]: {type(a)}")
 
         if len(new_columns) == 0 and new_references_feature_set is None:
             # This is possible if you have something like
             # Users.transactions[after('60d')]
             # In this case, keep all existing columns
@@ -118,50 +124,68 @@
             new_columns = list(cls.__columns__)
             new_references_feature_set = cls.__references_feature_set__
 
         class SubclassedDataFrame(cls):
             filters = tuple(new_filters)
             __columns__ = tuple(new_columns)
             __references_feature_set__ = new_references_feature_set
+            __pydantic_model__ = pydantic_model
+
+            def __eq__(self, other):
+                if not isinstance(other, SubclassedDataFrame):
+                    return False
+
+                    # This should probably be frozen set
+                return frozenset(self.filters) == frozenset(other.filters) and frozenset(self.columns) == frozenset(
+                    other.columns
+                )
+
+            def __hash__(self):
+                return hash((frozenset(self.filters), frozenset(self.__columns__)))
 
             def __new__(cls: Type[TDataFrame], *args: Any, **kwargs: Any) -> TDataFrame:
                 raise RuntimeError(
                     "A SubclassedDataFrame should never be instantiated. Instead, instantiate a DataFrame(...)."
                 )
 
         return SubclassedDataFrame
 
     def __repr__(cls):
         cls = cast(Type[DataFrame], cls)
         elements = [str(x) for x in (*cls.filters, *cls.columns)]
+        if cls.__pydantic_model__:
+            return f"DataFrame[{', '.join(elements)}], model={cls.__pydantic_model__}"
         return f"DataFrame[{', '.join(elements)}]"
 
     @property
     def columns(cls) -> Tuple[Feature, ...]:
         # Computing the columns lazily as we need to implicitly parse the type annotation
         # to determine if a field is a has-many, and we don't want to do that on the
         # __getitem__ which could happen before forward references can be resolved
         # So, using a property on the metaclass, which acts like an attribute on the class, to
         # provide the dataframe columns
         from chalk.features.feature_field import Feature
 
         cls = cast(Type[DataFrame], cls)
-        columns: Set[Feature] = set()
+        columns: List[Feature] = []
         for x in cls.__columns__:
             assert isinstance(x, Feature)
             # If a feature is directly specified, allow has-ones. But still do not allow has-many features
             assert not x.is_has_many, "Has-many features are not allowed to be specified within a DataFrame"
-            columns.add(x)
+            if x not in columns:
+                columns.append(x)
         if cls.__references_feature_set__ is not None:
             # Only include the first-level feature types
             # Do not recurse has-ones and has-many as that could create an infinite loop
+            # Skipping autogenerated features because if one writes DataFrame[User],
+            # then they definitely did not mean to include a feature they didn't know about
             for x in cls.__references_feature_set__.features:
                 assert isinstance(x, Feature)
-                if not x.is_has_many and not x.is_has_one:
-                    columns.add(x)
+                if not x.is_has_many and not x.is_has_one and x not in columns and not x.is_autogenerated:
+                    columns.append(x)
         return tuple(columns)
 
     @property
     def references_feature_set(cls):
         from chalk.features.feature_set import FeatureSetBase
 
         cls = cast(Type[DataFrame], cls)
@@ -177,45 +201,265 @@
         cls = cast(Type[DataFrame], cls)
         namespaces = [x.path[0].parent.namespace if len(x.path) > 0 else x.namespace for x in cls.columns]
         # Remove the pseudo-columns
         namespaces = [x for x in namespaces if not x.startswith("__chalk__")]
         return get_unique_item(namespaces, f"dataframe {cls.__name__} column namespaces")
 
 
-class DataFrame(metaclass=DataFrameMeta):
+class DataFrameImpl(metaclass=DataFrameMeta):
     filters: ClassVar[Tuple[Filter, ...]] = ()
     columns: Tuple[Feature, ...]  # set via a @property on the metaclass
     __columns__: ClassVar[Tuple[Feature, ...]] = ()
     references_feature_set: Optional[Type[Features]]  # set via a @property on the metaclass
     __references_feature_set__: ClassVar[Optional[Type[Features]]] = None
+    __pydantic_model__: ClassVar[Optional[Type[BaseModel]]] = None
+
+    def join(
+        self,
+        df: DataFrame,
+        on: Any | List[Any],
+        how: Literal["inner", "left", "outer"] = "left",
+    ) -> DataFrame:
+        on = ensure_tuple(on)
+        p = self._underlying.join(
+            df._underlying,
+            on=[str(t) for t in on],
+            how=how,
+        )
+        return DataFrame(p)
+
+    def group_by(
+        self,
+        group: Mapping[Union[Feature, Any], Union[Feature, Any]],
+        agg: Mapping[Any, Any],
+    ) -> DataFrameImpl:
+        """
+        Parameters
+        ----------
+        group
+            A mapping from the desired column name in the resulting `DataFrame`
+            to the name of the column in the source `DataFrame`.
+        agg
+            A mapping from the desired column name in the resulting `DataFrame`
+            to the aggregation operation to perform on the source `DataFrame`.
+
+        Returns
+        -------
+        DataFrameImpl
+            The `DataFrame` with the specified aggregations applied.
+        """
+        import polars as pl
+
+        from chalk.features.feature_set import FeatureSetBase
+
+        group = [pl.col(str(v)).alias(str(k)) for k, v in group.items()]
+        materialized = self._materialize()
+
+        namespaces = {unwrap_feature(a).namespace for a in agg.keys()}
+        namespace = namespaces.pop() if len(namespaces) == 1 else None
+        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
+
+        now = datetime.now(tz=timezone.utc)
+        cols = []
+        operation: Aggregation
+        for alias, operation in agg.items():
+            # if isinstance(operation, int):
+            #     operation = op.count(FeatureWrapper.len_registry[operation])
+            # c = pl.col(str(operation.col))
+            c = operation.col
+            if len(operation.filters) > 0:
+                c = c.filter(
+                    convert_filters_to_pl_expr(
+                        operation.filters,
+                        self._underlying.schema,
+                        timestamp_feature,
+                        now,
+                    )
+                )
+
+            cols.append(operation.fn(c).alias(str(alias)))
+
+        agged = materialized.lazy().groupby(group).agg(cols).collect()
+
+        return DataFrame(
+            agged,
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def vstack(self, other: DataFrame) -> DataFrame:
+        return DataFrame(
+            self._underlying.collect().vstack(other._underlying.collect()).lazy(),
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def rename(self, mapping: Mapping[Any, Any]) -> DataFrame:
+        """Rename columns in the `DataFrame`.
+
+        Parameters
+        ----------
+        mapping
+            A mapping from the current feature for a column to the desired
+            feature for the column.
+
+        Returns
+        -------
+        DataFrame
+            The `DataFrame` with the specified columns renamed.
+
+        Examples
+        --------
+        >>> df = DataFrame([
+        ...     User(id=1, first="Sam", last="Wu"),
+        ...     User(id=2, first="Iris", last="Xi")
+        ... ]).rename({User.last: User.family})
+        """
+        return DataFrame(
+            self._underlying.rename({unwrap_feature(k).fqn: unwrap_feature(v).fqn for k, v in mapping.items()}),
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def with_columns(self, c: Mapping[Any, Any]) -> DataFrame:
+        """Add columns to the `DataFrame`.
+
+        Parameters
+        ----------
+        c
+            A `Mapping` from the desired name of the column
+            in the `DataFrame` to the definition of the new
+            column.
+
+        Examples
+        --------
+        >>> df = DataFrame([
+        ...     User(id=1, first="Sam", last="Wu"),
+        ...     User(id=2, first="Iris", last="Xi")
+        ... ])
+        >>> # Set the fraud score to 0 for all users
+        >>> df.with_columns({User.fraud_score: 0})
+        >>> # Create a full name as the concatenation of first & last
+        >>> df.with_columns({
+        ...     User.full_name: op.concat(User.first, User.last)
+        ... })
+        >>> # Alias a column name
+        >>> df.with_columns({
+        ...     User.first_name: User.first
+        ... })
+
+
+        Returns
+        -------
+        DataFrame
+            A new `DataFrame` with all the existing columns,
+            plus those specified in this function.
+        """
+        import polars as pl
+
+        from chalk.features.feature_set import FeatureSetBase
+
+        namespaces = {unwrap_feature(a).namespace for a in c.keys()}
+        namespace = namespaces.pop() if len(namespaces) == 1 else None
+        timestamp_feature = None if namespace is None else FeatureSetBase.registry[namespace].__chalk_ts__
+
+        now = datetime.now(tz=timezone.utc)
+        cols = []
+        for alias, operation in c.items():
+            # if isinstance(operation, int):
+            #     operation = op.count(FeatureWrapper.len_registry[operation])
+            # c = pl.col(str(operation.col))
+
+            if isinstance(operation, Aggregation):
+                c = operation.col
+                if len(operation.filters) > 0:
+                    c = c.filter(
+                        convert_filters_to_pl_expr(
+                            operation.filters,
+                            self._underlying.schema,
+                            timestamp_feature,
+                            now,
+                        )
+                    )
+
+                cols.append(operation.fn(c).alias(str(alias)))
+            elif isinstance(operation, FeatureWrapper):
+                cols.append(pl.col(str(operation)).alias(str(alias)))
+            else:
+                cols.append(pl.lit(operation).alias(str(alias)))
+
+        agged = self._materialize().lazy().with_columns(cols).collect()
+
+        return DataFrame(
+            agged,
+            convert_dtypes=self._convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
 
     def __init__(
         self,
         data: Union[
-            Dict[Union[str, Feature, FeatureWrapper, Any], Sequence[Features]],
-            Sequence[Any],
+            Dict[Union[str, Feature, Any], Sequence[Any]],
+            Sequence[Union[Features, Any]],
             pl.DataFrame,
             pl.LazyFrame,
             pd.DataFrame,
             Any,  # Polars supports a bunch of other formats for initialization of a DataFrame
         ] = None,
+        # Setting to default_or_allow for backwards compatibility
+        missing_value_strategy: MissingValueStrategy = "default_or_allow",
         pandas_dataframe: Optional[pd.DataFrame] = None,  # For backwards compatibility
-        convert_dtypes: bool = True,  # By default, data should match the dtype of the feature. However, when doing comparisions, data will be converted to bools, in which case it should no longer be validated.
+        # By default, data should match the dtype of the feature.
+        # However, when doing comparisons, data will be converted to bools,
+        # in which case the data types should no longer be converted.
+        # This is an undocumented parameter, so it does not appear in the docstring
+        convert_dtypes: bool = True,
+        pydantic_model: Optional[Type[BaseModel]] = None,
     ):
-        """Construct a Chalk DataFrame
-
-        Args:
-            data: The data. Can be an existing Pandas DataFrame, Polars DataFrame or LazyFrame, a sequence of feature instances,
-                or a dict mapping a feature to a sequence of values.
-            convert_dtypes: Whether to convert the data to match the dtype of the underlying feature.
+        """Construct a Chalk `DataFrame`.
 
+        Parameters
+        ----------
+        data
+            The data. Can be an existing `pandas.DataFrame`,
+            `polars.DataFrame` or `polars.LazyFrame`,
+            a sequence of feature instances, or a `dict` mapping
+            a feature to a sequence of values.
+        missing_value_strategy
+            The strategy to use to handle missing values.
+
+            A feature value is "missing" if it is an ellipsis (`...`),
+            or it is `None` and the feature is not annotated as `Optional[...]`.
+
+            The available strategies are:
+                `'error'`: Raise a `TypeError` if any missing values are found.
+                    Do not attempt to replace missing values with the default
+                    value for the feature.
+                `'default_or_error'`: If the feature has a default value, then
+                    replace missing values with the default value for the feature.
+                    Otherwise, raise a `TypeError`.
+                `'default_or_allow'`:  If the feature has a default value, then
+                    replace missing values with the default value for the feature.
+                    Otherwise, leave it as `None`. This is the default strategy.
+                `'allow'`: Allow missing values to be stored in the `DataFrame`.
+                    This option may result non-nullable features being assigned
+                    `None` values.
         """
         from chalk.features.feature_set import Features, FeatureSetBase
 
-        # Typing the keys of ``data`` as Any, as {FeatureCls.item: x} would be typed as the underlying annotation of the features cls
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+
+        self._pydantic_model = pydantic_model
+        self._convert_dtypes = convert_dtypes
+
+        # Typing the keys of ``data`` as Any, as {FeatureCls.item: x} would be typed as the underlying annotation
+        # of the features cls
         if pandas_dataframe is not None:
             warnings.warn(
                 DeprecationWarning("ChalkDataFrameImpl(pandas_dataframe=...) has been renamed to DataFrame(data=...)")
             )
             data = pandas_dataframe
         if pd is not None and isinstance(data, pd.DataFrame):
             # Convert the columns to root fqn strings
@@ -261,116 +505,93 @@
                             raise ValueError("DataFrames within DataFrames are not supported")
                         if x.root_fqn not in new_data:
                             raise ValueError(f"Feature {x.root_fqn} is not defined in all feature sets.")
                         new_data[x.root_fqn].append(feature_val)
                 data = new_data
             if isinstance(data, dict):
                 # Convert the columns to root fqn strings
-                # str(Feature) and str(FeatureWrapper) return the root fqns
-                new_data_dict: Dict[str, Sequence[Any] | pl.Series] = {}
-                for (k, v) in data.items():
-                    v = [_preprocess_element(x) for x in v]
-
-                    if convert_dtypes:
-                        polars_dtype = FEATURE_CODEC.get_polars_dtype(str(k))
-                        elements_as_series = _generate_empty_series_for_dtype(str(k), polars_dtype, 0)
-                        null_element = _generate_empty_series_for_dtype(str(k), polars_dtype, 1)
-                        for i, element in enumerate(v):
-                            if element is None or isinstance(element, (list, tuple)) and len(element) == 0:
-                                elements_as_series.append(null_element)
-                            else:
-                                element_as_series = pl.Series(name=str(k), values=[element])
-                                if element_as_series.dtype != polars_dtype:
-
-                                    if _polars_dtype_contains_struct(polars_dtype):
-                                        # Cannot cast to a struct type. Instead, will error, so the user can ensure the underlying
-                                        # dictionaries / dataclasses are of the correct type
-                                        raise TypeError(
-                                            (
-                                                f"Expected field `{str(k)}` to have dtype `{str(polars_dtype)}`; got dtype `{str(element_as_series.dtype)}`"
-                                                f" for element {element} at index {i}"
-                                            )
-                                        )
-                                    else:
-                                        try:
-                                            if element_as_series.dtype == pl.Utf8 and polars_dtype == pl.Datetime:
-                                                element_as_series = element_as_series.str.strptime(
-                                                    pl.Datetime, fmt="+", strict=False
-                                                ).cast(polars_dtype)
-                                            else:
-                                                element_as_series = element_as_series.cast(polars_dtype)
-                                        except pl.ComputeError as e:
-                                            # If operating on a lazy frame, we won't get the exception until we call .compute()
-                                            raise TypeError(
-                                                f"Feature `{str(k)}` at index {i} with value '{element}' could not be converted to dtype `{polars_dtype.string_repr()}`"
-                                            ) from e
-                                elements_as_series.append(element_as_series)
-                        elements_as_series = elements_as_series.rechunk(True)
+                new_data_dict: Dict[str, Union[Sequence[Any], pl.Series]] = {}
+                for k, v in data.items():
+                    str_k = str(k)
+                    feature = Feature.from_root_fqn(str_k)
+
+                    if feature.is_has_one or feature.is_has_many:
+                        name = "has-one" if feature.is_has_one else "has-many"
+                        warnings.warn(
+                            DeprecationWarning(
+                                (
+                                    f"Feature '{feature}' is a {name} feature. Its values will not be validated, "
+                                    f"nor can this column be used for filtering. Support for passing {name} features "
+                                    "into a Chalk DataFrame will be removed. Instead, specify each feature of the "
+                                    "nested feature class as an individual column."
+                                )
+                            )
+                        )
+                        series = pl.Series(v, dtype=pl.Object)
                     else:
-                        elements_as_series = pl.Series(name=str(k), values=v)
-                    # # Otherwise, we can let polars infer the dtype. We will cast it later if convert_dtypes is True
-                    # # We do not want to specify it now, as otherwise polars will drop values instead of cast
-                    new_data_dict[str(k)] = elements_as_series
+                        if convert_dtypes:
+                            try:
+                                pa_array = feature.converter.from_rich_to_pyarrow(
+                                    v,
+                                    missing_value_strategy=missing_value_strategy,
+                                )
+                            except (TypeError, ValueError) as e:
+                                if len(v) > 0:
+                                    type_error = f" The first value that could not be loaded has type '{type(v[0])}'."
+                                else:
+                                    type_error = ""
+
+                                raise TypeError(
+                                    (
+                                        f"The values for feature `{k}` could not be loaded into a DataFrame column "
+                                        f"of type `{feature.converter.pyarrow_dtype}`." + type_error
+                                    )
+                                ) from e
+                            series = pl.from_arrow(pa_array)
+                            assert isinstance(series, pl.Series)
+                        else:
+                            series = v
+                    new_data_dict[str_k] = series
+
                 data = new_data_dict
             data = pl.DataFrame(data)
         if isinstance(data, (pl.LazyFrame, pl.DataFrame)):
             underlying = data
         else:
             raise ValueError(f"Unable to convert data of type {type(data).__name__} into a DataFrame")
         # Rename / validate that all column names are root fqns
-        # It is possible that a feature name is a
-        self.columns = tuple(Feature.from_root_fqn(str(c)) for c in underlying.columns)
-        underlying = underlying.rename(
-            {original_c: new_c.root_fqn for (original_c, new_c) in zip(underlying.columns, self.columns)}
-        )
-        namespaces = [x.path[0].parent.namespace if len(x.path) > 0 else x.namespace for x in self.columns]
+        if self._pydantic_model is None:
+            self.columns = tuple(Feature.from_root_fqn(str(c)) for c in underlying.columns)
+            # n.b. the goal here is to normalize "feature" and "str" columns to "str" columns
+            if any(not isinstance(c, str) for c in underlying.columns):
+                underlying = underlying.rename(
+                    {original_c: new_c.root_fqn for (original_c, new_c) in zip(underlying.columns, self.columns)}
+                )
+        else:
+            self.columns = ()
 
         # Convert columns to the correct dtype to match the fqn
-        if convert_dtypes:
-            for root_fqn in underlying.columns:
-                expected_dtype = FEATURE_CODEC.get_polars_dtype(root_fqn)
-                actual_dtype = underlying.schema[root_fqn]
-                if actual_dtype != expected_dtype:
-                    if _polars_dtype_contains_struct(expected_dtype):
-                        # Cannot cast to a struct type. Instead, will error, so the user can ensure the underlying
-                        # dictionaries / dataclasses are of the correct type
-                        raise TypeError(
-                            f"Expected field `{root_fqn}` to have dtype `{expected_dtype}`; got dtype `{actual_dtype}`"
-                        )
-                    else:
-                        try:
-                            if expected_dtype == pl.Datetime and actual_dtype == pl.Utf8:
-                                underlying = underlying.with_columns(
-                                    [
-                                        pl.col(root_fqn)
-                                        .str.strptime(pl.Datetime, fmt="+", strict=False)
-                                        .cast(expected_dtype)
-                                    ]
-                                )
-                            else:
-                                underlying = underlying.with_columns([pl.col(root_fqn).cast(expected_dtype)])
-                        except pl.ComputeError as e:
-                            # If operating on a lazy frame, we won't get the exception until we call .compute()
-                            raise TypeError(
-                                f"Values for feature `{root_fqn}` could not be converted to dtype `{expected_dtype.string_repr()}`. Found type {actual_dtype}, instead."
-                            ) from e
+        if self._pydantic_model is None and convert_dtypes:
+            underlying = validate_df_schema(underlying)
+            underlying = validate_nulls(underlying, missing_value_strategy=missing_value_strategy)
 
         if isinstance(underlying, pl.DataFrame):
             underlying = underlying.lazy()
-        self._underlying: pl.LazyFrame = underlying
+        self._underlying = underlying
 
         # Remove the pseudo-features when determining the namespace
+        namespaces = (x.path[0].parent.namespace if len(x.path) > 0 else x.namespace for x in self.columns)
         namespaces_set = set(x for x in namespaces if not x.startswith("__chalk__"))
-        if len(namespaces_set) != 1:
+        if len(namespaces_set) == 1:
+            self.namespace = get_unique_item(namespaces_set, f"dataframe column namespaces")
+            self.references_feature_set = FeatureSetBase.registry[self.namespace]
+        else:
             # Allow empty dataframes or dataframes with multiple namespaces
             self.namespace = None
             self.references_feature_set = None
-        else:
-            self.namespace = get_unique_item(namespaces_set, f"dataframe column namespaces")
-            self.references_feature_set = FeatureSetBase.registry[self.namespace]
 
     ##############
     # Classmethods
     ##############
 
     @classmethod
     def from_dict(
@@ -404,94 +625,284 @@
         else:
             data = cast("Tuple[Features]", data)
             features_seq = data
         df = cls(features_seq)
         return df
 
     @classmethod
+    def _get_storage_options(cls) -> Optional[Dict[str, Any]]:
+        if os.getenv("GCP_INTEGRATION_CREDENTIALS_B64") is not None:
+            try:
+                from google.oauth2 import service_account
+            except ImportError:
+                raise missing_dependency_exception("google-auth")
+            token = service_account.Credentials.from_service_account_info(
+                json.loads(base64.b64decode(os.getenv("GCP_INTEGRATION_CREDENTIALS_B64"))),
+                scopes=[
+                    "https://www.googleapis.com/auth/cloud-platform",
+                    "https://www.googleapis.com/auth/userinfo.email",
+                ],
+            )
+            return {"token": token}
+        else:
+            return None
+
+    @classmethod
+    def read_delta(
+        cls: Type[TDataFrame],
+        table_uri: str,
+        version: Optional[int] = None,
+        columns: Optional[
+            Union[
+                Dict[str, Union[str, Feature, Any]],
+                Dict[int, Union[str, Feature, Any]],
+            ]
+        ] = None,
+        delta_table_options: Optional[Dict[str, Any]] = None,
+        pyarrow_options: Optional[Dict[str, Any]] = None,
+    ) -> TDataFrame:
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+
+        if columns is None:
+            cols_to_select, _, new_columns = None, None, None
+        else:
+            cols_to_select, _, new_columns = cls._parse_columns(columns)
+
+        data = pl.read_delta(
+            table_uri=table_uri,
+            version=version,
+            columns=cols_to_select,
+            storage_options=DataFrame._get_storage_options(),
+            delta_table_options=delta_table_options,
+            pyarrow_options=pyarrow_options,
+        )
+        if new_columns is not None:
+            data = data.rename({c: new_columns[i] for i, c in enumerate(data.columns)})
+        return cls(data)
+
+    @classmethod
     def read_parquet(
         cls: Type[TDataFrame],
         path: Union[str, pathlib.Path],
-        columns: Optional[Union[List[int], List[str], Dict[str, Union[str, Feature, FeatureWrapper, Any]]]] = None,
+        columns: Optional[
+            Union[
+                Dict[str, Union[str, Feature, Any]],
+                Dict[int, Union[str, Feature, Any]],
+            ]
+        ] = None,
+        use_pyarrow: bool = False,
     ) -> TDataFrame:
-        if isinstance(columns, dict):
-            columns_to_read = list(columns.keys())
-            column_map = {k: str(v) for (k, v) in columns.items()}
-        else:
-            columns_to_read = columns
-            column_map = None
-        data = pl.read_parquet(path, columns_to_read)
-        if column_map is not None:
-            data = data.rename(column_map)
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+
+        if columns is None:
+            cols_to_select, _, new_columns = None, None, None
+        else:
+            cols_to_select, _, new_columns = cls._parse_columns(columns)
+
+        data = pl.read_parquet(
+            source=path,
+            columns=cols_to_select,
+            storage_options=DataFrame._get_storage_options(),
+            use_pyarrow=use_pyarrow,
+        )
+        if new_columns is not None:
+            data = data.rename({c: new_columns[i] for i, c in enumerate(data.columns)})
         return cls(data)
 
     @classmethod
+    def _parse_columns(
+        cls,
+        col_mapping: Union[
+            Dict[str, Union[str, Feature, FeatureWrapper, Any]],
+            Dict[int, Union[str, Feature, FeatureWrapper, Any]],
+        ],
+    ) -> Tuple[Union[List[str], List[int]], List[Type[pl.DataType]], List[str]]:
+        if not isinstance(col_mapping, dict):
+            raise ValueError(f"Invalid column mapping. Received '{type(col_mapping).__name__}'; expected dict")
+        columns = []
+        dtypes = []
+        new_cols: List[str] = []
+        for k, v in col_mapping.items():
+            columns.append(k)
+            new_cols.append(str(v))
+            dtypes.append(ensure_feature(v).converter.polars_dtype)
+        return columns, dtypes, new_cols
+
+    @classmethod
     def read_csv(
         cls: Type[TDataFrame],
         path: Union[str, pathlib.Path],
-        has_header: bool,
-        columns: Optional[Union[List[int], List[str], Dict[str, Union[str, Feature, FeatureWrapper, Any]]]] = None,
+        has_header: bool = True,
+        columns: Optional[
+            Union[
+                Dict[str, Union[str, Feature, Any]],
+                Dict[int, Union[str, Feature, Any]],
+            ]
+        ] = None,
+    ) -> TDataFrame:
+        """Read a .csv file as a `DataFrame`.
+
+        Parameters
+        ----------
+        path
+            The path to the .csv file. This may be a S3 or GCS
+            storage url.
+        has_header
+            Whether the .csv file has a header row as the first row.
+        columns
+            A mapping of index to feature name.
+
+        Returns
+        -------
+        TDataFrame
+            A `DataFrame` with the contents of the file loaded as features.
+
+        Examples
+        --------
+        >>> values = DataFrame.read_csv(
+        ...     "s3://...",
+        ...     columns={0: MyFeatures.id, 1: MyFeatures.name},
+        ...     has_header=False,
+        ... )
+        """
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+
+        if columns is None:
+            cols_to_select, dtypes, new_columns = None, None, None
+        else:
+            cols_to_select, dtypes, new_columns = cls._parse_columns(columns)
+
+        data = pl.read_csv(
+            source=path,
+            has_header=has_header,
+            columns=cols_to_select,
+            dtypes=dtypes,
+            new_columns=new_columns,
+            storage_options=DataFrame._get_storage_options(),
+        )
+        return cls(data)
+
+    @classmethod
+    def read_avro(
+        cls: Type[TDataFrame],
+        path: Union[str, pathlib.Path],
     ) -> TDataFrame:
-        if isinstance(columns, dict):
-            columns_to_read = list(columns.keys())
-            column_map = {k: str(v) for (k, v) in columns.items()}
-        else:
-            columns_to_read = columns
-            column_map = None
-        data = pl.read_csv(path, has_header, columns_to_read)
-        if column_map is not None:
-            data = data.rename(column_map)
+        """Read a .avro file as a `DataFrame`.
+
+        Parameters
+        ----------
+        path
+            The path to the `.avro` file. This may be a S3 or GCS
+            storage url.
+
+        Returns
+        -------
+        TDataFrame
+            A `DataFrame` with the contents of the file loaded as features.
+
+        Examples
+        --------
+        >>> values = DataFrame.read_avro(
+        ...     "s3://...",
+        ... )
+        """
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+
+        data = None
+        if isinstance(path, str) and path.startswith("s3://"):
+            try:
+                import fsspec
+            except ImportError:
+                raise missing_dependency_exception("fsspec")
+            try:
+                import s3fs
+            except ImportError:
+                raise missing_dependency_exception("s3fs")
+            try:
+                import io
+            except ImportError:
+                raise missing_dependency_exception("io")
+            with fsspec.open(path, "rb") as f:
+                buffer = io.BytesIO(initial_bytes=f.read())
+                data = pl.read_avro(buffer)
+        else:
+            data = pl.read_avro(source=path)
         return cls(data)
 
     #############
     # Aggregation
     #############
 
     def max(self):
-        return DataFrame(self._underlying.max(), convert_dtypes=False)
+        return DataFrame(self._underlying.max(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def mean(self):
-        return DataFrame(self._underlying.mean(), convert_dtypes=False)
+        return DataFrame(self._underlying.mean(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def median(self):
-        return DataFrame(self._underlying.median(), convert_dtypes=False)
+        return DataFrame(self._underlying.median(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def min(self):
-        return DataFrame(self._underlying.min(), convert_dtypes=False)
+        return DataFrame(self._underlying.min(), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def std(self, ddof: int = 1):
-        return DataFrame(self._underlying.std(ddof), convert_dtypes=False)
+        return DataFrame(self._underlying.std(ddof), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     def sum(self):
         # Treat missing sums as zero
-        return DataFrame(self._underlying.sum().fill_null(0), convert_dtypes=False)
+        return DataFrame(
+            self._underlying.sum().fill_null(0),
+            convert_dtypes=False,
+            pydantic_model=self._pydantic_model,
+        )
 
     def var(self, ddof: int = 1):
-        return DataFrame(self._underlying.var(ddof), convert_dtypes=False)
+        return DataFrame(self._underlying.var(ddof), convert_dtypes=False, pydantic_model=self._pydantic_model)
 
     ####################
     # Summary Operations
     ####################
 
     # These ops require us to materialize the dataframe.
 
     def _materialize(self) -> pl.DataFrame:
         materialized = self._underlying.collect()
         self._underlying = materialized.lazy()
         return materialized
 
     def any(self):
-        """Returns whether any of the values in the dataframe are truthy. Requires the dataframe to only contain boolean values."""
+        """Returns whether any of the values in the dataframe are truthy.
+        Requires the dataframe to only contain boolean values."""
+        import polars as pl
+
+        if len(self) == 0:
+            return False
         if not all(isinstance(x, type) and issubclass(x, pl.Boolean) for x in self._underlying.dtypes):
             raise TypeError("DataFrame.any() is not defined on a dataframe that contains non-boolean columns.")
         materialized = self._materialize()
         return any(col.any() for col in materialized.get_columns())
 
     def all(self):
         """Returns whether all of the values in the dataframe are truthy. Requires the dataframe to only contain boolean values."""
+        import polars as pl
+
+        if len(self) == 0:
+            return True
         if not all(isinstance(x, type) and issubclass(x, pl.Boolean) for x in self._underlying.dtypes):
             raise TypeError("DataFrame.any() is not defined on a dataframe that contains non-boolean columns.")
         materialized = self._materialize()
         return all(col.all() for col in materialized.get_columns())
 
     def __len__(self):
         materialized = self._materialize()
@@ -507,14 +918,65 @@
         materialized = self._materialize()
         if materialized.shape == (1, 1):
             return materialized.rows()[0][0]
         raise ValueError(
             "The dataframe contains multiple items. DataFrame.item() can only be used if the dataframe has a single element."
         )
 
+    def sort(
+        self,
+        by: Union[str, Feature, Any, Iterable[str, Feature, Any]],
+        *more_by: Union[str, Feature, Any],
+        descending: Union[bool, Sequence[bool]] = False,
+        nulls_last: bool = False,
+    ) -> DataFrame:
+        """
+        Sort the dataframe by the given columns.
+
+        Parameters
+        ----------
+        by
+            Feature(s) to sort by. Strings are parsed as feature names.
+        more_by
+            Additional columns to sort by, specified as positional arguments.
+        descending
+            Sort in descending order. When sorting by multiple columns,
+            can be specified per feature by passing a sequence of booleans.
+        nulls_last
+            Place null values last.
+
+        Returns
+        -------
+        DataFrame
+            A new dataframe with the rows sorted.
+
+        Examples
+        --------
+        >>> df = DataFrame({
+        ...     User.a: [1, 2, 3],
+        ...     User.b: [3, 2, 1],
+        ... })
+        >>> df.sort(User.a)
+              a  b
+        -----------
+        0     1  3
+        1     2  2
+        2     3  1
+        """
+        by = tuple(str(x) for x in itertools.chain(ensure_tuple(by), more_by))
+        return DataFrame(
+            self._underlying.sort(
+                by=by,
+                descending=descending,
+                nulls_last=nulls_last,
+            ),
+            convert_dtypes=False,
+            pydantic_model=self._pydantic_model,
+        )
+
     def __bool__(self):
         if self.shape == (1, 1):
             # It's a dataframe of 1 item. self.any() and self.all() would return the same thing
             return self.all()
         raise ValueError("__bool__ is ambiguous on a DataFrame. Instead, use DataFrame.any() or DataFrame.all().")
 
     def __str__(self):
@@ -535,44 +997,131 @@
     # Arithmetic and Comparisons
     ############################
 
     # These ops require us to materialize the dataframe.
 
     def _perform_op(
         self,
-        op: Callable[[Any, Any], Any],
+        op: Union[str, Callable[[Any, Any], Any]],
         other: Union[DataFrame, pl.DataFrame, pd.DataFrame, Any],
         convert_dtypes: bool,
     ):
+        import polars as pl
+
         materialized = self._materialize()
         if isinstance(other, DataFrame):
             other = other.to_polars()
         if isinstance(other, pl.LazyFrame):
             other = other.collect()
-        if isinstance(other, pd.DataFrame):
+        if pd is not None and isinstance(other, pd.DataFrame):
             other = pl.from_pandas(other)
-        return DataFrame(op(materialized, other), convert_dtypes=convert_dtypes)
+        if op in ("eq", "ne", "lt", "le", "ge", "gt"):
+            if isinstance(other, pl.DataFrame):
+                return self._perform_comp_df(op, other, convert_dtypes=convert_dtypes)
+            else:
+                return DataFrame(
+                    getattr(operator, op)(materialized, other),
+                    convert_dtypes=convert_dtypes,
+                    pydantic_model=self._pydantic_model,
+                )
+        assert callable(op)
+        return DataFrame(
+            op(materialized, other),
+            convert_dtypes=convert_dtypes,
+            pydantic_model=self._pydantic_model,
+        )
+
+    def _perform_comp_df(
+        self,
+        op: str,
+        other: pl.DataFrame,
+        convert_dtypes: bool,
+    ):
+        # There's a bug in the default polars implementation for comparisons -- see
+        # https://github.com/pola-rs/polars/issues/5870
+        import polars as pl
+
+        materialized = self._materialize()
+        if set(materialized.columns) != set(other.columns):
+            raise ValueError(f"DataFrame columns do not match. {materialized.columns} != {other.columns}")
+        # Put the columns in the same order
+        other = other.select(materialized.columns)
+        if materialized.shape != other.shape:
+            raise ValueError("DataFrame dimensions do not match")
+
+        suffix = "__POLARS_CMP_OTHER"
+        other_renamed = other.select(pl.all().suffix(suffix))
+        combined = pl.concat([materialized, other_renamed], how="horizontal")
+
+        if op == "eq":
+            expr = [
+                (
+                    pl.when(pl.col(n).is_null() & pl.col(f"{n}{suffix}").is_null())
+                    .then(pl.lit(True))
+                    .otherwise(pl.col(n) == pl.col(f"{n}{suffix}"))
+                    .alias(n)
+                )
+                for n in materialized.columns
+            ]
+        elif op == "ne":
+            expr = [
+                (
+                    pl.when(pl.col(n).is_null() & pl.col(f"{n}{suffix}").is_null())
+                    .then(pl.lit(False))
+                    .otherwise(pl.col(n) != pl.col(f"{n}{suffix}"))
+                    .alias(n)
+                )
+                for n in materialized.columns
+            ]
+        elif op == "gt":
+            expr = [pl.col(n) > pl.col(f"{n}{suffix}") for n in materialized.columns]
+        elif op == "lt":
+            expr = [pl.col(n) < pl.col(f"{n}{suffix}") for n in materialized.columns]
+        elif op == "ge":
+            expr = [
+                (
+                    pl.when(pl.col(n).is_null() & pl.col(f"{n}{suffix}").is_null())
+                    .then(pl.lit(True))
+                    .otherwise(pl.col(n) >= pl.col(f"{n}{suffix}"))
+                    .alias(n)
+                )
+                for n in materialized.columns
+            ]
+        elif op == "le":
+            expr = [
+                (
+                    pl.when(pl.col(n).is_null() & pl.col(f"{n}{suffix}").is_null())
+                    .then(pl.lit(True))
+                    .otherwise(pl.col(n) <= pl.col(f"{n}{suffix}"))
+                    .alias(n)
+                )
+                for n in materialized.columns
+            ]
+        else:
+            raise ValueError(f"got unexpected comparison operator: {op}")
+
+        return DataFrame(combined.select(expr), convert_dtypes=convert_dtypes, pydantic_model=self._pydantic_model)
 
     def __eq__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):  # type: ignore
-        return self._perform_op(operator.eq, other, convert_dtypes=False)
+        return self._perform_op("eq", other, convert_dtypes=False)
 
     def __ne__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):  # type: ignore
-        return self._perform_op(operator.ne, other, convert_dtypes=False)
+        return self._perform_op("ne", other, convert_dtypes=False)
 
     def __gt__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):
-        return self._perform_op(operator.gt, other, convert_dtypes=False)
+        return self._perform_op("gt", other, convert_dtypes=False)
 
     def __lt__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):
-        return self._perform_op(operator.lt, other, convert_dtypes=False)
+        return self._perform_op("lt", other, convert_dtypes=False)
 
     def __ge__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):
-        return self._perform_op(operator.ge, other, convert_dtypes=False)
+        return self._perform_op("ge", other, convert_dtypes=False)
 
     def __le__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]):
-        return self._perform_op(operator.le, other, convert_dtypes=False)
+        return self._perform_op("le", other, convert_dtypes=False)
 
     def __add__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]) -> DataFrame:
         return self._perform_op(operator.add, other, convert_dtypes=True)
 
     def __sub__(self, other: Union[DataFrame, pl.DataFrame, pl.LazyFrame, pd.DataFrame, Any]) -> DataFrame:
         return self._perform_op(operator.sub, other, convert_dtypes=True)
 
@@ -591,359 +1140,153 @@
     def __pow__(self, other: Union[int, float]) -> DataFrame:
         return self._perform_op(operator.pow, other, convert_dtypes=True)
 
     ############
     # Conversion
     ############
     def to_polars(self) -> pl.LazyFrame:
-        """Get the underlying dataframe as a Polars LazyFrame."""
-        # Implementing to_polars() to return the LazyFrame, rather than the DataFrame, to encourage customers to use
-        # lazy operations if possible. They can manually call .collect() if needed
+        """Get the underlying `DataFrame` as a `polars.LazyFrame`."""
         return self._underlying
 
+    def to_pyarrow(self) -> pa.Table:
+        materialized = self._materialize()
+        pa_table = materialized.to_arrow()
+        if self._convert_dtypes:
+            pa_schema = pa.schema({k: Feature.from_root_fqn(k).converter.pyarrow_dtype for k in pa_table.column_names})
+            pa_table = pa_table.cast(pa_schema)
+        return pa_table
+
     def to_pandas(self) -> pd.DataFrame:
-        """Get the underlying dataframe as a Pandas DataFrame."""
-        # For pandas, the columns should be the Features, not the root fqns
-        def types_mapper(dtype: pyarrow.DataType):
-            if dtype in (pyarrow.utf8(), pyarrow.large_utf8()):
-                return pd.StringDtype()
+        """Get the underlying dataframe as a `pandas.DataFrame`."""
+        if pd is None:
+            raise missing_dependency_exception("chalkpy[pandas]")
+
+        def types_mapper(dtype: pa.DataType):
+            if dtype in (pa.utf8(), pa.large_utf8()):
+                return pd.StringDtype("python")
             return None
 
-        pd_dataframe = self._underlying.collect().to_pandas(types_mapper=types_mapper)
+        pd_dataframe = self._materialize().to_pandas(types_mapper=types_mapper)
+        # For pandas, the columns should be the Features, not the root fqns
+        # So, convert the columns to object types, and then set them to the features
         pd_dataframe.columns = pd_dataframe.columns.astype("object")
         pd_dataframe = pd_dataframe.rename(columns={x.root_fqn: x for x in self.columns})
         return pd_dataframe
 
+    def to_features(self) -> Sequence[Features]:
+        """Get values in the dataframe as `Features` instances."""
+        from chalk.features.feature_set import FeatureSetBase
+
+        if self.namespace is None:
+            raise ValueError("This method is not supported if the DataFrame spans multiple namespaces")
+        ans: List[Features] = []
+        for row in self.to_pyarrow().to_pylist():
+            rooted_prefix_to_values: Dict[str, Dict[str, Any]] = {}
+
+            for k, v in row.items():
+                rooted_prefix_split = k.split(".")[:-1]
+                for i in range(1, len(rooted_prefix_split) + 1):
+                    rooted_prefix = ".".join(rooted_prefix_split[:i])
+                    if rooted_prefix not in rooted_prefix_to_values:
+                        rooted_prefix_to_values[rooted_prefix] = {}
+                rooted_prefix_to_values[".".join(rooted_prefix_split)][k] = v
+            # Sorting in reverse to construct the innermost features first
+            sorted_sub_features = sorted(rooted_prefix_to_values.keys(), key=lambda x: len(x), reverse=True)
+
+            for rooted_prefix in sorted_sub_features:
+                values = rooted_prefix_to_values[rooted_prefix]
+                sub_kwargs: Dict[str, Any] = {}
+                for k, v in values.items():
+                    feature = Feature.from_root_fqn(k)
+                    assert not feature.is_has_many, "has-many features are not supported recursively within a dataframe"
+                    if feature.is_has_one:
+                        sub_kwargs[feature.attribute_name] = v
+                    else:
+                        sub_kwargs[feature.attribute_name] = feature.converter.from_primitive_to_rich(v)
+                if rooted_prefix == self.namespace:
+                    features_cls = FeatureSetBase.registry[self.namespace]
+                    ans.append(features_cls(**sub_kwargs))
+                else:
+                    rooted_prefix_split = rooted_prefix.split(".")
+                    features_cls = Feature.from_root_fqn(rooted_prefix).joined_class
+                    assert features_cls is not None
+                    parent_rooted_prefix, feature_name = ".".join(rooted_prefix_split[:-1]), rooted_prefix_split[-1]
+                    del feature_name  # unused
+                    rooted_prefix_to_values[parent_rooted_prefix][rooted_prefix] = features_cls(**sub_kwargs)
+        return ans
+
     #######################
     # Filtering / Selecting
     #######################
-    def __getitem__(self, item: Any):
-        from chalk.features.feature_set import FeatureSetBase
+    def __getitem__(self, item: Any) -> DataFrame:
+        """Filter by rows or by columns.
+
+        Parameters
+        ----------
+        item
+
+        Returns
+        -------
+
+        """
+        if isinstance(item, int) and not isinstance(item, bool):
+            if item >= 0:
+                l = len(self)
+                if item >= l:
+                    raise IndexError(f"Index {item} out of range (length {l})")
+                underlying = self._underlying.head(item + 1).tail(1)
+            else:
+                underlying = self._underlying.tail(-item).head(1)
+
+            df = DataFrame(
+                underlying,
+                convert_dtypes=False,
+                pydantic_model=self._pydantic_model,
+            )
+            return list(df.to_features())[0]
 
         has_bool_or_filter_value = any(isinstance(x, (bool, Filter)) for x in ensure_tuple(item))
         if has_bool_or_filter_value:
             # If we have a boolean or Filter value, then that means we need to ast-parse the caller since
             # python has already evaluated AND, OR, and IN operations into literal booleans or Filters
             # Skipping the parsing unless if we have need to for efficiency and to eliminate conflicts
             # with pytest
             from chalk.df.ast_parser import parse_dataframe_getitem
 
             item = parse_dataframe_getitem()
         if any(isinstance(x, (FeatureWrapper, Feature, Filter)) for x in ensure_tuple(item)):
-            # Use the Chalk projection / selection syntax, where we support our Filter objects and
-            # selection by column name
-            projections: list[str] = []
-            filters: List[Filter] = []
-            for x in ensure_tuple(item):
-                if isinstance(x, (FeatureWrapper, Feature, str)):
-                    projections.append(str(x))
-
-                elif isinstance(x, Filter):
-                    filters.append(x)
-                else:
-                    raise TypeError(
-                        "When indexing by Filters or Features, it is not simultaneously possible to perform other indexing operations."
-                    )
-
-            now = datetime.datetime.now(tz=datetime.timezone.utc)
-            timestamp_feature = None if self.namespace is None else FeatureSetBase.registry[self.namespace].__chalk_ts__
-            pl_expr = convert_filters_to_pl_expr(filters, self._underlying.schema, timestamp_feature, now)
-            df = self._underlying
-            if pl_expr is not None:
-                df = df.filter(pl_expr)
-            # Do the projection
-            if len(projections) > 0:
-                df = df.select(projections)
-            return DataFrame(df)
+            return DataFrame(
+                filter_data_frame(item, namespace=self.namespace, underlying=self._underlying),
+                pydantic_model=self._pydantic_model,
+            )
         else:
             # Otherwise, use the standard polars selection format
             # Must materialize the dataframe to use __getitem__
             materialized = self._materialize()
             df = materialized[item]
-            return DataFrame(df)
+            return DataFrame(df, pydantic_model=self._pydantic_model)
 
+    def slice(self, offset: int = 0, length: Optional[int] = None) -> DataFrame:
+        """Slice the `DataFrame`.
 
-def _feature_type_or_value(e: Union[Feature, FeatureWrapper]):
-    if isinstance(e, FeatureWrapper):
-        e = unwrap_feature(e)
-    return e
-
-
-def _polars_dtype_contains_struct(dtype: pl.DataType | Type[pl.DataType]):
-    """Returns whether the dtype contains a (potentially nested) struct"""
-    if isinstance(dtype, pl.Struct) or (isinstance(dtype, type) and issubclass(dtype, pl.Struct)):
-        return True
-    if isinstance(dtype, pl.List):
-        assert dtype.inner is not None
-        return _polars_dtype_contains_struct(dtype.inner)
-    return False
-
-
-def _maybe_replace_timestamp_feature(f: Union[Feature, Any], observed_at_feature: Optional[Feature]):
-    """Replace the ``CHALK_TS`` pseudo-feature with the actual timestamp column."""
-    if not isinstance(f, Feature) or f.fqn != "__chalk__.CHALK_TS":
-        return f
-    if observed_at_feature is not None:
-        return observed_at_feature
-    raise ValueError("No Timestamp Feature Found")
-
-
-def _maybe_convert_timedelta_to_timestamp(
-    f: Union[TimeDelta, datetime.timedelta, Any], now: Optional[datetime.datetime]
-):
-    """Convert timedeltas relative to ``now`` into absolute datetimes."""
-    if isinstance(f, TimeDelta):
-        f = f.to_std()
-    if isinstance(f, datetime.timedelta):
-        if now is None:
-            raise ValueError(
-                "The filter contains a relative timestamp. The current datetime must be provided to evaluate this filter."
-            )
-        return now + f
-    return f
+        Parameters
+        ----------
+        offset
+            The offset to start at.
+        length
+            The number of rows in the slice. If None (the default), include all rows from `offset`
+            to the end of the `DataFrame`.
+
+        Returns
+        -------
+        DataFrame
+            The dataframe with the slice applied.
+        """
+        return DataFrame(self._underlying.slice(offset, length))
 
 
-def _parse_feature_or_value(
-    f: Union[Feature, Any], timestamp_feature: Optional[Feature], now: Optional[datetime.datetime]
-):
-    """Parse a feature or value into the correct type that can be used for filtering."""
-    f = _feature_type_or_value(f)
-    f = _maybe_convert_timedelta_to_timestamp(f, now)
-    f = _maybe_replace_timestamp_feature(f, timestamp_feature)
-    if isinstance(f, enum.Enum):
-        f = f.value
-    return f
-
-
-def _polars_is_eq(
-    lhs: Any,
-    rhs: Any,
-    lhs_dtype: Optional[Union[Type[pl.DataType], pl.DataType]],
-    rhs_dtype: Optional[Union[Type[pl.DataType], pl.DataType]],
-):
-    """Compare a column with another column or literal value, including possibly a struct.
-    Polars does not permit equality comparisons on structs directly. Instead, must compare field by field, potentially recursively.
-    """
-    if rhs_dtype is not None:
-        if lhs_dtype is None:
-            # Swap the columns
-            return _polars_is_eq(rhs, lhs, rhs_dtype, lhs_dtype)
-        else:
-            # Comparing two columns
-            assert isinstance(lhs, pl.Expr)
-            assert isinstance(rhs, pl.Expr)
-            if isinstance(lhs_dtype, pl.Struct):
-                assert isinstance(rhs_dtype, pl.Struct)
-                # Assert equality field by field
-                filters = []
-                for field in lhs_dtype.fields:
-                    field_name = field.name
-                    new_lhs = lhs.struct.field(field_name)
-                    new_lhs_dtype = field.dtype
-                    new_rhs = rhs.struct.field(field_name)
-                    new_rhs_dtype = field.dtype
-                    filters.append(_polars_is_eq(new_lhs, new_rhs, new_lhs_dtype, new_rhs_dtype))
-                assert len(filters) > 0, "structs with 0 fields are unsupported"
-                return functools.reduce(lambda a, b: a & b, filters)
-            return lhs == rhs
-    # rhs is literal
-    # lhs is a column
-    assert lhs_dtype is not None, "one side must be a column"
-    assert isinstance(lhs, pl.Expr)
-    if isinstance(lhs_dtype, pl.Struct):
-        # Assert equality field by field
-        filters = []
-        for field in lhs_dtype.fields:
-            field_name = field.name
-            new_lhs = lhs.struct.field(field_name)
-            new_lhs_dtype = field.dtype
-            # Assuming that struct-like objects make their members accessible by attribute name or __getitem__
-            try:
-                new_rhs = getattr(rhs, field_name)
-            except AttributeError:
-                new_rhs = rhs[field_name]
-            new_rhs_dtype = None  # literal values do not have dtypes
-            filters.append(_polars_is_eq(new_lhs, new_rhs, new_lhs_dtype, new_rhs_dtype))
-        assert len(filters) > 0, "structs with 0 fields are unsupported"
-        return functools.reduce(lambda a, b: a & b, filters)
-    if not isinstance(lhs_dtype, type):
-        lhs_dtype = type(lhs_dtype)
-    return lhs == pl.lit(rhs, dtype=lhs_dtype, allow_object=True)
-
-
-def _polars_is_in(lhs: pl.Expr, rhs: Iterable, lhs_dtype: Union[Type[pl.DataType], pl.DataType]):
-    """Filter for where the lhs is in the RHS. The RHS must be a literal collection."""
-    if isinstance(lhs_dtype, pl.Struct):
-        # Assert equality field by field
-        filters = []
-        rhs_by_fields: Dict[str, List[Any]] = {}
-        for item in rhs:
-            for field in lhs_dtype.fields:
-                if field.name not in rhs_by_fields:
-                    rhs_by_fields[field.name] = []
-                # Assuming that struct-like objects make their members accessible by attribute name or __getitem__
-                try:
-                    rhs_vector = getattr(item, field.name)
-                except AttributeError:
-                    rhs_vector = item[field.name]
-                rhs_by_fields[field.name].append(rhs_vector)
-        for field in lhs_dtype.fields:
-            field_name = field.name
-            new_lhs = lhs.struct.field(field_name)
-            new_lhs_dtype = field.dtype
-            new_rhs = rhs_by_fields[field_name]
-            filters.append(_polars_is_in(new_lhs, new_rhs, new_lhs_dtype))
-        assert len(filters) > 0, "structs with 0 fields are unsupported"
-        return functools.reduce(lambda a, b: a & b, filters)
-    if not isinstance(lhs_dtype, type):
-        lhs_dtype = type(lhs_dtype)
-    return lhs.is_in(pl.lit(pl.Series(values=rhs, dtype=lhs_dtype), allow_object=True))
-
-
-def _coerce_value_to_dtype(val: Any, dtype: Union[pl.DataType, Type[pl.DataType]]):
-    # For the most part, we don't need to do any manual coercion -- polars will handle that for us.
-    # Only need to pay attention to enums, which could be stored as the underlying type, or as an object
-    if isinstance(val, collections.abc.Iterable) and not isinstance(val, str):
-        return [_coerce_value_to_dtype(x, dtype) for x in val]
-    if isinstance(val, enum.Enum) and dtype != pl.Object:
-        return val.value
-    return val
-
-
-def _convert_filter_to_pl_expr(
-    f: Filter,
-    df_schema: dict[str, pl.PolarsDataType],
-    timestamp_feature: Optional[Feature] = None,
-    now: Optional[datetime.datetime] = None,
-) -> pl.Expr:
-    """Convert filters to a polars expression
-
-    Args:
-        f: The filter
-        df_schema: The DataFrame schema.
-        timestamp_feature: The feature corresponding to the observation time
-        now: The datetime to use for the current timestamp. Used to resolve relative
-            timestamps in filters to absolute datetimes.
-
-    Returns:
-        A series of boolean values that can be used to select the rows where the filter is truthy
-    """
-    # Passing `now` in explicitly instead of using datetime.datetime.now() so that multiple filters
-    # relying on relative timestamps (e.g. before, after) will have the same "now" time.
-    if f.operation == "not":
-        assert f.rhs is None, "not has just one side"
-        assert isinstance(f.lhs, Filter), "lhs must be a filter"
-        return ~_convert_filter_to_pl_expr(f.lhs, df_schema, timestamp_feature, now)
-    elif f.operation == "and":
-        assert isinstance(f.rhs, Filter), "rhs must be a filter"
-        assert isinstance(f.lhs, Filter), "lhs must be a filter"
-        return _convert_filter_to_pl_expr(f.lhs, df_schema, timestamp_feature, now) & _convert_filter_to_pl_expr(
-            f.rhs, df_schema, timestamp_feature, now
-        )
-    elif f.operation == "or":
-        assert isinstance(f.rhs, Filter), "rhs must be a filter"
-        assert isinstance(f.lhs, Filter), "lhs must be a filter"
-        return _convert_filter_to_pl_expr(f.lhs, df_schema, timestamp_feature, now) | _convert_filter_to_pl_expr(
-            f.rhs, df_schema, timestamp_feature, now
-        )
-
-    lhs = _parse_feature_or_value(f.lhs, timestamp_feature, now)
-    rhs = _parse_feature_or_value(f.rhs, timestamp_feature, now)
-
-    lhs_dtype = None
-    if isinstance(lhs, Feature):
-        lhs_dtype = df_schema[str(lhs)]
-        lhs = pl.col(str(lhs))
-
-    rhs_dtype = None
-    if isinstance(rhs, Feature):
-        rhs_dtype = df_schema[str(rhs)]
-        rhs = pl.col(str(rhs))
-
-    if lhs_dtype is None:
-        # LHS is literal. Encode it into the rhs_dtype
-        assert rhs_dtype is not None
-        lhs = _coerce_value_to_dtype(lhs, rhs_dtype)
-    if rhs_dtype is None:
-        # RHS is literal. Encode it into the lhs_dtype
-        assert lhs_dtype is not None
-        rhs = _coerce_value_to_dtype(rhs, lhs_dtype)
-
-    if rhs is None:
-        assert isinstance(lhs, pl.Expr)
-        if f.operation == "==":
-            return lhs.is_null()
-
-        elif f.operation == "!=":
-            return lhs.is_not_null()
-
-    if f.operation in ("in", "not in"):
-        assert lhs_dtype is not None
-        assert isinstance(lhs, pl.Expr)
-        assert isinstance(rhs, collections.abc.Iterable)
-        ret = _polars_is_in(lhs, rhs, lhs_dtype)
-        if f.operation == "not in":
-            ret = ~ret
-    elif f.operation in ("==", "!="):
-        ret = _polars_is_eq(lhs, rhs, lhs_dtype, rhs_dtype)
-        if f.operation == "!=":
-            ret = ~ret
-    elif f.operation == "!=":
-        ret = lhs != rhs
-    elif f.operation == ">=":
-        ret = lhs >= rhs  # type: ignore
-    elif f.operation == ">":
-        ret = lhs > rhs  # type: ignore
-    elif f.operation == "<":
-        ret = lhs < rhs  # type: ignore
-    elif f.operation == "<=":
-        ret = lhs <= rhs  # type: ignore
-    else:
-        raise ValueError(f'Unknown operation "{f.operation}"')
-    assert isinstance(ret, pl.Expr)
-    return ret
-
-
-def convert_filters_to_pl_expr(
-    filters: Sequence[Filter],
-    df_schema: dict[str, pl.PolarsDataType],
-    timestamp_feature: Optional[Feature] = None,
-    now: Optional[datetime.datetime] = None,
-):
-    if len(filters) == 0:
-        return None
-    polars_filters = (_convert_filter_to_pl_expr(f, df_schema, timestamp_feature, now) for f in filters)
-    return functools.reduce(lambda a, b: a & b, polars_filters)
-
-
-def _generate_empty_series_for_dtype(name: str, dtype: Union[Type[pl.DataType], pl.DataType], length: int) -> pl.Series:
-    """Safely generate a series of all null values for the specified datatype.
-
-    Unlike the ``pl.Series`` constructor, this function can handle struct dtypes.
-    """
-    if isinstance(dtype, pl.Struct):
-        # Struct dtypes cannot be specified in the pl.Series constructor.
-        # Instead, create a dataframe, then call .to_struct() on it
-        # If recursing within a struct, it should have a length of zero
-        data = {f.name: _generate_empty_series_for_dtype(f.name, f.dtype, length) for f in dtype.fields}
-        temp_df = pl.DataFrame(data)
-        return temp_df.to_struct(name)
-    if isinstance(dtype, pl.List):
-        assert dtype.inner is not None
-        data = {name: _generate_empty_series_for_dtype(name, dtype.inner, 0)}
-        temp_df = pl.DataFrame(data)
-        list_of_struct_series = temp_df.select(pl.col(name).reshape((length, -1))).get_column(name)
-        return list_of_struct_series
-    return pl.Series(name, dtype=dtype, values=([None] * length))
-
-
-# list [[], [None, None]]
-
-
-def _preprocess_element(element: Any):
-    if isinstance(element, enum.Enum):
-        element = element.value
-    # Polars has trouble with third-party timezone libraries,
-    # So convert it to python's internal timezone library
-    if isinstance(element, datetime.datetime) and element.tzinfo is not None:
-        element = element.astimezone(datetime.timezone.utc)
-    return element
+# Hack to get VSCode/Pylance/Pyright to type DataFrame as Type[DataFrameImpl]
+# but IntelliJ to type it as Type[Any]
+# Vscode can parse through literal dicts; IntelliJ can't
+_dummy_dict = {"0": DataFrameImpl}
+
+DataFrame = _dummy_dict["0"]
```

### Comparing `chalkpy-1.9.9/chalk/features/feature_field.py` & `chalkpy-2.0.0/chalk/streams/_windows.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,374 +1,347 @@
 from __future__ import annotations
 
-import copy
-import dataclasses
-import functools
-import itertools
-from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, TypeVar, Union, cast
+from datetime import timedelta
+from typing import TYPE_CHECKING, Any, Generic, List, Mapping, Optional, Set, Type, TypeVar, Union, cast
 
-import polars as pl
-from sqlalchemy.types import TypeEngine
-
-from chalk.features.tag import Tags
-from chalk.serialization.parsed_annotation import ParsedAnnotation
+from chalk._validation.feature_validation import FeatureValidation
+from chalk._validation.validation import Validation
+from chalk.features._encoding.primitive import TPrimitive
 from chalk.utils.collections import ensure_tuple
-from chalk.utils.duration import Duration, timedelta_to_duration
-
-if TYPE_CHECKING:
-    from chalk.features.feature_set import Features
-    from chalk.features.filter import Filter
-
-T = TypeVar("T")
-U = TypeVar("U")
-JsonValue = TypeVar("JsonValue")
+from chalk.utils.duration import Duration, parse_chalk_duration
 
-__all__ = ["Feature", "feature", "feature_time", "has_one", "has_many"]
+TPrim = TypeVar("TPrim", bound=TPrimitive)
+TRich = TypeVar("TRich")
 
+if TYPE_CHECKING:
+    import pyarrow as pa
 
-@dataclasses.dataclass
-class HasOnePathObj:
-    parent: Feature
-    child: Feature
-    parent_to_child_attribute_name: str
+    from chalk.features._encoding.converter import TDecoder, TEncoder
 
 
-@dataclasses.dataclass
-class FeatureValidation:
-    min: Optional[T]
-    max: Optional[T]
-    min_length: Optional[int]
-    max_length: Optional[int]
-    contains: Optional[T]
+class WindowedInstance(Generic[TRich]):
+    def __init__(self, values: Mapping[str, TRich]):
+        self.values = values
+
+    def __call__(self, period: str):
+        return self.values[period]
+
+
+class WindowedMeta(type, Generic[TRich]):
+    def __getitem__(cls, underlying: Type[TRich]) -> Windowed[TRich]:
+        return Windowed(
+            kind=underlying,
+            buckets=[],
+            description=None,
+            owner=None,
+            tags=None,
+            name=None,
+            default=...,
+            max_staleness=None,
+            version=None,
+            etl_offline_to_online=None,
+            encoder=None,
+            decoder=None,
+            min=None,
+            max=None,
+            min_length=None,
+            max_length=None,
+            contains=None,
+            strict=False,
+            dtype=None,
+            validations=None,
+            offline_ttl=None,
+        )  # noqa
+
+
+JsonValue = Any
+
+
+def get_duration_secs(duration: Union[str, int, timedelta]) -> int:
+    if isinstance(duration, str):
+        duration = parse_chalk_duration(duration)
+    if isinstance(duration, timedelta):
+        duration_secs_float = duration.total_seconds()
+        duration_secs_int = int(duration_secs_float)
+        if duration_secs_float != duration_secs_int:
+            raise ValueError("Windows that are fractions of seconds are not yet supported")
+        duration = duration_secs_int
+    return duration
+
+
+def get_name_with_duration(name_or_fqn: str, duration: Union[str, int, timedelta]) -> str:
+    duration_secs = get_duration_secs(duration)
+    return f"{name_or_fqn}__{duration_secs}__"
 
 
-class Feature:
-    def __init__(
-        self,
-        name: Optional[str] = None,
-        attribute_name: Optional[str] = None,
-        namespace: Optional[str] = None,
-        features_cls: Optional[Type[Features]] = None,
-        typ: Optional[Union[ParsedAnnotation, type]] = None,
-        version: Optional[int] = None,
-        description: Optional[str] = None,
-        owner: Optional[str] = None,
-        tags: Optional[List[str]] = None,
-        primary: bool = False,
-        max_staleness: Optional[Duration] = ...,
-        etl_offline_to_online: Optional[bool] = None,
-        encoder: Optional[Callable[[Any], JsonValue]] = None,
-        decoder: Optional[Callable[[JsonValue], Any]] = None,
-        polars_dtype: Optional[Union[Type[pl.DataType], pl.DataType]] = None,
-        sqlalchemy_dtype: Optional[Union[TypeEngine, Type[TypeEngine]]] = None,
-        join: Optional[Union[Callable[[], Filter], Filter]] = None,
-        path: Tuple[HasOnePathObj, ...] = (),
-        is_feature_time: bool = False,
-        is_autogenerated: bool = False,
-        validations: Optional[FeatureValidation] = None,
-    ):
-        self.typ = ParsedAnnotation(underlying=typ) if isinstance(typ, type) else typ
-        self.features_cls = features_cls
-        self._name = name
-        # the attribute name for the feature in the @features class (in case if the name is specified differently)
-        self._attribute_name = attribute_name
-        self._namespace = namespace
-        self.path = path
-        self.version = version
-        self.description = description
-        self.owner = owner
-        self.tags = tags
-        self.primary = primary
-        self.max_staleness = max_staleness
-        self.etl_offline_to_online = etl_offline_to_online
-        self.encoder = encoder
-        self.decoder = decoder
-        self.polars_dtype = polars_dtype
-        self.sqlalchemy_dtype = sqlalchemy_dtype
-        self.is_feature_time = is_feature_time
-        self.is_autogenerated = is_autogenerated
-        self._join = join
-        self._validations = validations
-
-    def __str__(self):
-        return self.root_fqn
-
-    @property
-    def attribute_name(self):
-        if self._attribute_name is None:
-            raise RuntimeError(
-                "Feature.attribute_name is not yet defined. Is the feature being constructed outside of a Features class?"
-            )
-        return self._attribute_name
-
-    @attribute_name.setter
-    def attribute_name(self, attribute_name: str):
-        self._attribute_name = attribute_name
-        if self._name is None:
-            # If there is no name, also set the name to the attribute name
-            self._name = attribute_name
+if TYPE_CHECKING:
+    _WINDOWED_METACLASS = type
+else:
+    _WINDOWED_METACLASS = WindowedMeta
 
-    @property
-    def name(self):
-        if self._name is None:
-            raise RuntimeError(
-                "Feature.name is not yet defined. Is the feature being constructed outside of a Features class?"
-            )
-        return self._name
 
-    @name.setter
-    def name(self, name: str):
-        self._name = name
+class Windowed(Generic[TRich], metaclass=_WINDOWED_METACLASS):
+    """Declare a windowed feature.
 
-    @property
-    def namespace(self):
-        if self._namespace is None:
-            raise RuntimeError(
-                "Feature.namespace is not yet defined. Is the feature being constructed outside of a Features class?"
-            )
-        return self._namespace
-
-    @namespace.setter
-    def namespace(self, namespace: str):
-        self._namespace = namespace
-
-    @classmethod
-    @functools.lru_cache(1024)
-    def from_root_fqn(cls, root_fqn: str) -> Feature:
-        """Convert a Root FQN into a feature.
-
-        Args:
-            root_fqn: The root fqn of the feature
-
-        Returns:
-            The feature for that root_fqn.
-        """
-        from chalk.features.feature_set import Features, FeatureSetBase
-        from chalk.features.pseudofeatures import PSEUDOFEATURES
-
-        for x in PSEUDOFEATURES:
-            if root_fqn == x.root_fqn or root_fqn == x.name:
-                return x
-        split_fqn = root_fqn.split(".")
-        root_ns = split_fqn[0]
-        split_fqn = split_fqn[1:]
-        features_cls = FeatureSetBase.registry[root_ns]
-
-        # FQNs are by name, so must lookup the feature in features_cls.features instead of using getattr
-        feat: Optional[Feature] = None
-
-        while len(split_fqn) > 0:
-            feature_name = split_fqn[0]
-            split_fqn = split_fqn[1:]
-
-            found_feature = False
-
-            for x in features_cls.features:
-                assert isinstance(x, Feature)
-                if x.name == feature_name:
-                    assert x.attribute_name is not None
-                    found_feature = True
-                    feat = x if feat is None else feat.copy_with_path(x)
-                    if len(split_fqn) > 0:
-                        # Going to recurse, so validate that the feature is something that we can recurse on.
-                        if not x.is_has_one:
-                            raise TypeError(
-                                (
-                                    f"Feature {features_cls.__chalk_namespace__}.{feature_name}.{'.'.join(split_fqn)} "
-                                    f"does not exist as {features_cls.__chalk_namespace__}.{feature_name} "
-                                    f"is not a has-one"
-                                )
-                            )
-                        assert x.typ is not None
-                        assert issubclass(x.typ.underlying, Features)
-                        features_cls = x.typ.underlying
-                    break
-            if not found_feature:
-                raise ValueError(
-                    f"Did not find feature named '{feature_name}' in features cls {features_cls.__chalk_namespace__}"
-                )
-        assert feat is not None
-        return feat
+    Examples
+    --------
+    >>> @features
+    ... class User:
+    ...     failed_logins: Windowed[int] = windowed("10m", "24h")
+    """
 
     @property
-    def root_namespace(self) -> str:
-        if len(self.path) > 0:
-            assert self.path[0].parent.namespace is not None, "parent namespace is None"
-            return self.path[0].parent.namespace
-        assert self.namespace is not None, "namespace is None"
-        return self.namespace
+    def buckets_seconds(self) -> Set[int]:
+        return set(int(parse_chalk_duration(bucket).total_seconds()) for bucket in self._buckets)
 
     @property
-    def root_fqn(self):
-        assert self.name is not None, "Missing name on feature"
-        if len(self.path) > 0:
-            return ".".join(
-                itertools.chain(
-                    (self.root_namespace,),
-                    (x.parent.name for x in self.path),
-                    (self.name,),
-                )
-            )
-        return f"{self.namespace}.{self.name}"
+    def kind(self) -> Type[TRich]:
+        if self._kind is None:
+            raise RuntimeError("Window type has not yet been parsed")
+        return self._kind
 
-    def __hash__(self) -> int:
-        return hash(self.root_fqn)
+    @kind.setter
+    def kind(self, kind: Type[TRich]) -> None:
+        assert self._kind is None, "Window type cannot be set twice"
+        self._kind = kind
 
-    def __eq__(self, other: object):
-        if self.is_has_many:
-            # For equality checks on a has-many, we would also need to compare the columns and types
-            # For now, ignoring.
-            return NotImplemented
-        if isinstance(other, Feature):
-            other = other.root_fqn
-        if isinstance(other, str):
-            return self.root_fqn == other
-        return NotImplemented
+    def _to_feature(self, bucket: Optional[Union[int, str]]):
+        from chalk.features import Feature
 
-    def __repr__(self):
-        return f"Feature(fqn={self.namespace}.{self.name}, typ={self.typ})"
+        assert self._name is not None
 
-    @property
-    def fqn(self) -> str:
-        return f"{self.namespace}.{self.name}"
-
-    @property
-    def is_has_one(self):
-        # A feature is a has-one relationship if the type is
-        # another singleton features cls and there is a join condition
-        assert self.typ is not None
-        # Need to short-circuit if it is a dataframe, as DataFrames
-        # might not have an underlying
-        return not self.typ.is_dataframe and self.join is not None
+        if bucket is None:
+            name = self._name
+        else:
+            if get_duration_secs(bucket) not in self.buckets_seconds:
+                raise ValueError(f"Bucket {bucket} is not in the list of specified buckets")
+            name = get_name_with_duration(self._name, bucket)
 
-    @property
-    def is_has_many(self):
-        assert self.typ is not None
-        return self.typ.is_dataframe and self.join is not None
-
-    @property
-    def is_scalar(self):
-        return not self.is_has_many and not self.is_has_one and not self.is_feature_time
-
-    @property
-    def has_resolved_join(self):
-        return self._join is not None
+        return Feature(
+            name=name,
+            version=self._version,
+            owner=self._owner,
+            tags=None if self._tags is None else list(ensure_tuple(self._tags)),
+            description=self._description,
+            primary=False,
+            default=self._default,
+            max_staleness=self._max_staleness,
+            offline_ttl=self._offline_ttl,
+            etl_offline_to_online=self._etl_offline_to_online,
+            encoder=self._encoder,
+            decoder=self._decoder,
+            pyarrow_dtype=self._dtype,
+            validations=FeatureValidation(
+                min=self._min,
+                max=self._max,
+                min_length=self._min_length,
+                max_length=self._max_length,
+                contains=self._contains,
+                strict=self._strict,
+            ),
+            all_validations=None
+            if self._validations is None
+            else [
+                FeatureValidation(
+                    min=v.min,
+                    max=v.max,
+                    min_length=v.min_length,
+                    max_length=v.max_length,
+                    contains=None,
+                    strict=v.strict,
+                )
+                for v in self._validations
+            ],
+            # Only the root feature should have all the durations
+            # The pseudofeatures, which are bound to a duration, should not have the durations
+            # of the other buckets
+            window_durations=tuple(self.buckets_seconds) if bucket is None else tuple(),
+            window_duration=None if bucket is None else get_duration_secs(bucket),
+        )
 
-    @property
-    def join(self) -> Optional[Filter]:
-        from chalk.features.feature_set import Features
+    def __init__(
+        self,
+        buckets: List[str],
+        description: Optional[str],
+        owner: Optional[str],
+        tags: Optional[Any],
+        name: Optional[str],
+        default: Union[TRich, ellipsis],
+        max_staleness: Optional[Union[Duration, ellipsis]],
+        version: Optional[int],
+        etl_offline_to_online: Optional[bool],
+        encoder: Optional[TEncoder[TPrim, TRich]],
+        decoder: Optional[TDecoder[TPrim, TRich]],
+        min: Optional[TRich],
+        max: Optional[TRich],
+        min_length: Optional[int],
+        max_length: Optional[int],
+        contains: Optional[TRich],
+        strict: bool,
+        validations: Optional[List[Validation]],
+        dtype: Optional[pa.DataType],
+        kind: Optional[Type[TRich]],
+        offline_ttl: Optional[Union[Duration, ellipsis]],
+    ):
+        self._kind = kind
+        self._name: Optional[str] = None
+        self._buckets = buckets
+        self._description = description
+        self._owner = owner
+        self._tags = tags
+        self._name = name
+        self._default = default
+        self._max_staleness = max_staleness
+        self._offline_ttl = offline_ttl
+        self._description = description
+        self._version = version
+        self._etl_offline_to_online = etl_offline_to_online
+        self._encoder = encoder
+        self._decoder = decoder
+        self._min = min
+        self._max = max
+        self._min_length = min_length
+        self._max_length = max_length
+        self._contains = contains
+        self._strict = strict
+        self._validations = validations
+        self._dtype = dtype
 
-        if self._join is not None:
-            # Join was explicitly specified
-            return self._join() if callable(self._join) else self._join
-        # Attempt to extract the join condition from the foreign feature
-        assert self.typ is not None
-        foreign_features = self.typ.underlying
-        if not issubclass(foreign_features, Features):
-            return None
-        assert self.features_cls is not None
-        joins: List[Tuple[str, Filter]] = []  # Tuple of (name, Join)
-        for f in foreign_features.features:
-            assert isinstance(f, Feature)
-            assert f.typ is not None
-            if f.typ.underlying is self.features_cls and f.has_resolved_join:
-                assert f.join is not None
-                assert f.name is not None
-                join = f.join() if callable(f.join) else f.join
-                joins.append((f.name, join))
-        if len(joins) == 0:
-            # It's a nested feature
-            return None
-        # TODO(Ravi): Enable this check. But let's see if we can be smarter about which join to automatically use, if there are multiple
-        # if len(joins) > 1:
-        #     assert self.features_cls is not None
-        #     raise ValueError(
-        #         f"Multiple join conditions exist for {self.features_cls.__name__} and {foreign_features.__name__} on keys: "
-        #         + f", ".join(f'{foreign_features.__name__}.{name}' for (name, _) in joins)
-        #     )
-        join = joins[0][1]
-        if callable(join):
-            join = join()
-        self._join = join
-        return join
 
-    @property
-    def joined_class(self) -> Optional[Type[Features]]:
-        j = self.join
-        if j is None:
-            return None
-        if j.lhs is not None and j.rhs is not None and isinstance(j.lhs, Feature) and isinstance(j.rhs, Feature):
-            if j.lhs.namespace != self.namespace:
-                return j.lhs.features_cls
-            return j.rhs.features_cls
-        return None
-
-    def copy_with_path(self, child: Feature) -> Feature:
-        child_copy = copy.copy(child)
-        assert child.attribute_name is not None
-        child_copy.path = tuple(
-            (
-                *self.path,
-                HasOnePathObj(
-                    parent=self,
-                    child=child,
-                    parent_to_child_attribute_name=child.attribute_name,
-                ),
-            )
-        )
-        return child_copy
+class SelectedWindow:
+    def __init__(self, kind: Windowed, selected: str):
+        self.windowed = kind
+        self.selected = selected
 
 
-def feature(
+def windowed(
+    *buckets: str,
     description: Optional[str] = None,
     owner: Optional[str] = None,
-    tags: Optional[Tags] = None,
+    tags: Optional[Any] = None,
     name: Optional[str] = None,
+    default: Union[TRich, ellipsis] = ...,
+    max_staleness: Optional[Union[Duration, ellipsis]] = ...,
+    offline_ttl: Optional[Union[Duration, ellipsis]] = ...,
     version: Optional[int] = None,
-    primary: bool = False,
-    max_staleness: Optional[Duration] = ...,
     etl_offline_to_online: Optional[bool] = None,
-    encoder: Optional[Callable[[T], JsonValue]] = None,
-    decoder: Optional[Callable[[JsonValue], T]] = None,
-    min: Optional[T] = None,
-    max: Optional[T] = None,
+    encoder: Optional[TEncoder[TPrim, TRich]] = None,
+    decoder: Optional[TDecoder[TPrim, TRich]] = None,
+    min: Optional[TRich] = None,
+    max: Optional[TRich] = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
-    contains: Optional[T] = None,
-) -> T:
-    return cast(
-        T,
-        Feature(
-            name=name,
-            version=version,
-            owner=owner,
-            tags=None if tags is None else list(ensure_tuple(tags)),
-            description=description,
-            primary=primary,
-            max_staleness=timedelta_to_duration(max_staleness)
-            if isinstance(max_staleness, timedelta)
-            else max_staleness,
-            etl_offline_to_online=etl_offline_to_online,
-            encoder=encoder,
-            decoder=decoder,
-            validations=FeatureValidation(
-                min=min,
-                max=max,
-                min_length=min_length,
-                max_length=max_length,
-                contains=contains,
-            ),
-        ),
+    strict: bool = False,
+    validations: Optional[List[Validation]] = None,
+    dtype: Optional[pa.DataType] = None,
+) -> Windowed[TRich]:
+    """Create a windowed feature.
+
+    See more at https://docs.chalk.ai/docs/aggregations#windowed-features
+
+    Parameters
+    ----------
+    buckets
+        The size of the buckets for the window function.
+    default
+        The default value of the feature if it otherwise can't be computed.
+    owner
+        You may also specify which person or group is responsible for a feature.
+        The owner tag will be available in Chalk's web portal.
+        Alerts that do not otherwise have an owner will be assigned
+        to the owner of the monitored feature.
+    tags
+        Add metadata to a feature for use in filtering, aggregations,
+        and visualizations. For example, you can use tags to assign
+        features to a team and find all features for a given team.
+    max_staleness
+        When a feature is expensive or slow to compute, you may wish to cache its value.
+        Chalk uses the terminology "maximum staleness" to describe how recently a feature
+        value needs to have been computed to be returned without re-running a resolver.
+
+        Read more at https://docs.chalk.ai/docs/feature-caching
+    version
+        Feature versions allow you to manage a feature as its
+        definition changes over time.
+
+        The `version` keyword argument allows you to specify the
+        maximum number of versions available for this feature.
+
+        See more at https://docs.chalk.ai/docs/feature-versions
+    etl_offline_to_online
+        When `True`, Chalk copies this feature into the online environment
+        when it is computed in offline resolvers.
+
+        Read more at https://docs.chalk.ai/docs/reverse-etl
+    min
+        If specified, when this feature is computed, Chalk will check that `x >= min`.
+    max
+        If specified, when this feature is computed, Chalk will check that `x <= max`.
+    min_length
+        If specified, when this feature is computed, Chalk will check that `len(x) >= min_length`.
+    max_length
+        If specified, when this feature is computed, Chalk will check that `len(x) <= max_length`.
+    strict
+        If `True`, if this feature does not meet the validation criteria, Chalk will not persist
+        the feature value and will treat it as failed.
+    validations
+    offline_ttl
+
+    Other Parameters
+    ----------------
+    name
+        The name for the feature. By default, the name of a feature is
+        the name of the attribute on the class, prefixed with
+        the camel-cased name of the class. Note that if you provide an
+        explicit name, the namespace, determined by the feature class,
+        will still be prepended. See `features` for more details.
+    description
+        Descriptions are typically provided as comments preceding
+        the feature definition. For example, you can document a
+        `email_count` feature with information about the values
+        as follows::
+        >>> @features
+        ... class User:
+        ...     # Count of emails sent
+        ...     email_count: Windowed[int] = windowed("10m", "30m")
+
+        You can also specify the description directly with this parameter.
+        >>> @features
+        ... class User:
+        ...     email_count: Windowed[int] = windowed(
+        ...         "10m", "30m"
+        ...         description="Count of emails sent",
+        ...     )
+    encoder
+    decoder
+    dtype
+
+    Returns
+    -------
+    Windowed[TPrim, TRich]
+        Metadata for the windowed feature, parameterized by
+        `TPrim` (the primitive type of the feature) and
+        `TRich` (the decoded type of the feature, if `decoder` is provided).
+    """
+    return Windowed(
+        list(buckets),
+        description=description,
+        owner=owner,
+        tags=tags,
+        name=name,
+        default=default,
+        max_staleness=max_staleness,
+        version=version,
+        etl_offline_to_online=etl_offline_to_online,
+        encoder=cast("TEncoder", encoder),
+        decoder=decoder,
+        min=min,
+        max=max,
+        min_length=min_length,
+        max_length=max_length,
+        contains=None,
+        strict=strict,
+        dtype=dtype,
+        kind=None,
+        validations=validations,
+        offline_ttl=offline_ttl,
     )
-
-
-def feature_time() -> Any:
-    return Feature(typ=datetime, is_feature_time=True)
-
-
-def has_one(f: Callable[[], Any]) -> Any:
-    return Feature(join=f)
-
-
-def has_many(f: Callable[[], Any]) -> Any:
-    return Feature(join=f)
```

### Comparing `chalkpy-1.9.9/chalk/features/feature_set.py` & `chalkpy-2.0.0/chalk/features/feature_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
+from datetime import timedelta
 from typing import Any, Callable, ClassVar, Dict, Iterator, List, Optional, Tuple, Type, cast
 
-from typing_extensions import TypeAlias, TypeGuard
+from typing_extensions import TypeGuard
 
 from chalk.features.feature_field import Feature
-from chalk.features.feature_wrapper import FeatureWrapper
+from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
+from chalk.features.live_updates import register_live_updates_if_in_notebook
 from chalk.utils.collections import ensure_tuple, get_unique_item
-from chalk.utils.duration import Duration
 
 __all__ = ["Features", "FeaturesMeta", "FeatureSetBase", "is_features_cls"]
 
 
 class FeaturesMeta(type):
     """Metaclass for classes decorated with ``@features``.
 
@@ -37,17 +38,17 @@
         # Annotating the return type as Type[Any] as instances of @features classes are
         # not recognized as being subclasses of Features by the type checker (even though at runtime they would be)
         from chalk.features.dataframe import DataFrame
 
         # Typing the `__getitem__` as any, since the @features members are typed as the underlying data structure
         # But, they should always be features or a tuple of features
         if isinstance(item, type) and issubclass(item, Features):
-            item = [f for f in item.features if isinstance(f, (Feature, FeatureWrapper))]
+            item = [f for f in item.features if not f.is_autogenerated]
         item = ensure_tuple(item)
-        item = tuple(x._chalk_feature if isinstance(x, FeatureWrapper) else x for x in item)
+        item = tuple(unwrap_feature(x) if isinstance(x, FeatureWrapper) else x for x in item)
         for x in item:
             if isinstance(x, str):
                 raise TypeError(
                     f'String features like {cls.__name__}["{x}"] are unsupported. Instead, replace with "{cls.__name__}[{x}]"'
                 )
             if isinstance(x, Feature) or (isinstance(x, type) and issubclass(x, DataFrame)):
                 continue
@@ -63,14 +64,17 @@
 
         return SubFeatures
 
     def __repr__(cls) -> str:
         cls = cast(Type[Features], cls)
         return f"Features[{', '.join(str(f) for f in cls.features)}]"
 
+    def __call__(cls, *args: object, **kwargs: object):
+        raise RuntimeError("Instances features cls should never be directly created. Instead, use Features[User.id]")
+
     @property
     def namespace(cls):
         cls = cast(Type[Features], cls)
         namespaces = [x.namespace for x in cls.features]
         return get_unique_item(namespaces, name=f"{cls.__name__} feature namespaces")
 
 
@@ -79,21 +83,18 @@
 
     This class is never instantiated or directly inherited. However, classes
     annotated with @features can be thought of as inheriting from this class.
     It can be used with ``isinstance`` and ``issubclass`` checks, as well as for
     typing.
     """
 
-    def __new__(cls, *args: object, **kwargs: object):
-        raise RuntimeError("Instances features cls should never be directly created. Instead, use Features[User.id]")
-
     # Internally, the Features class is instantiated when results come through, and
     # results are bound to instances of this class via attributes
     __chalk_etl_offline_to_online__: ClassVar[bool]
-    __chalk_max_staleness__: ClassVar[Optional[Duration]]
+    __chalk_max_staleness__: ClassVar[timedelta]
     __chalk_namespace__: ClassVar[str]
     __chalk_primary__: ClassVar[Optional[Feature]]  # The primary key feature
     __chalk_owner__: ClassVar[Optional[str]]
     __chalk_tags__: ClassVar[List[str]]
     __chalk_ts__: ClassVar[Optional[Feature]]  # The timestamp feature
     features: ClassVar[Tuple[Feature, ...]] = ()
     __is_features__: ClassVar[bool] = True
@@ -104,28 +105,35 @@
         """Iterating over features yields tuples of (fqn, value) for all scalarish feature values."""
         raise NotImplementedError
 
     def __len__(self) -> int:
         """The number of features that are set."""
         raise NotImplementedError
 
+    def items(self) -> Iterator[Tuple[str, Any]]:
+        """Iterating over features yields tuples of (fqn, value) for all feature values."""
+        raise NotImplementedError
 
-# Hack to get intellij to not complain about Features[...] when used as a return annotation
-# Intellij ignores the __getitem__ on the metaclass, causing it to want all return values
-# to be Features instances, when we accept literal values or tuples
-# This hack is compatible with VSCode/Pylance
-Features: TypeAlias = (lambda: FeaturesImpl)()
+
+# Hack to get VSCode/Pylance/Pyright to type Features as Type[FeatureImpl]
+# but IntelliJ to type it as Type[Any]
+# Vscode can parse through literal dicts; IntelliJ can't
+_dummy_dict = {"0": FeaturesImpl}
+
+Features = _dummy_dict["0"]
 
 
 class FeatureSetBase:
     """Registry containing all @features classes."""
 
-    registry: Dict[str, Type[Features]] = {}  # mapping of fqn to Features cls
-    root_fqn_to_feature: Dict[str, Feature] = {}  # mapping of root fqn to the Feature instance
-    hook: "ClassVar[Optional[Callable[[Features], None]]]" = None
+    registry: ClassVar[Dict[str, Type[Features]]] = {}  # mapping of fqn to Features cls
+    hook: ClassVar[Optional[Callable[[Features], None]]] = None
 
     def __init__(self) -> None:
         raise RuntimeError("FeatureSetBase should never be instantiated")
 
 
-def is_features_cls(maybe_features: Any) -> TypeGuard[Type[Features]]:
+register_live_updates_if_in_notebook(FeatureSetBase)
+
+
+def is_features_cls(maybe_features: Any) -> TypeGuard[Type[FeaturesImpl]]:
     return isinstance(maybe_features, type) and issubclass(maybe_features, Features)
```

### Comparing `chalkpy-1.9.9/chalk/features/feature_set_decorator.py` & `chalkpy-2.0.0/chalk/features/feature_set_decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,49 @@
+from __future__ import annotations
+
 import ast
+import copy
 import functools
 import inspect
 import re
 import sys
 import textwrap
 import threading
 import types
 from datetime import datetime, timedelta
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Mapping,
-    MutableMapping,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+from itertools import islice
+from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Type, TypeVar, Union, cast, overload
 
-from chalk.features.feature_field import Feature, feature_time
+from chalk.features._class_property import classproperty, classproperty_support
+from chalk.features.feature_field import Feature, _VersionInfo
 from chalk.features.feature_set import Features, FeatureSetBase
-from chalk.features.feature_wrapper import FeatureWrapper
+from chalk.features.feature_time import feature_time
+from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
 from chalk.features.tag import Tags
 from chalk.serialization.parsed_annotation import ParsedAnnotation
+from chalk.streams import Windowed
 from chalk.utils.collections import ensure_tuple
-from chalk.utils.duration import Duration, timedelta_to_duration
+from chalk.utils.duration import Duration, parse_chalk_duration
 from chalk.utils.metaprogramming import MISSING, create_fn, field_assign, set_new_attribute
 from chalk.utils.string import removeprefix, to_snake_case
 
 T = TypeVar("T")
 
 __all__ = ["features"]
 
+GENERATED_OBSERVED_AT_NAME = "__chalk_observed_at__"
+
 
 @overload
 def features(
     *,
     owner: Optional[str] = None,
     tags: Optional[Tags] = None,
-    etl_offline_to_online: bool = ...,
-    max_staleness: Optional[Duration] = ...,
+    etl_offline_to_online: bool = False,
+    max_staleness: Optional[Duration] = None,
     name: Optional[str] = None,
 ) -> Callable[[Type[T]], Type[T]]:
     ...
 
 
 @overload
 def features(cls: Type[T]) -> Type[T]:
@@ -56,157 +51,215 @@
 
 
 def features(
     cls: Optional[Type[T]] = None,
     *,
     owner: Optional[str] = None,
     tags: Optional[Tags] = None,
-    etl_offline_to_online: Optional[bool] = None,
-    max_staleness: Optional[Duration] = ...,
+    etl_offline_to_online: bool = False,
+    max_staleness: Optional[Duration] = None,
     name: Optional[str] = None,
 ) -> Union[Callable[[Type[T]], Type[T]], Type[T]]:
-    """Returns the same class as was passed in, with dunder methods
-    added based on the fields defined in the class.
+    """Chalk lets you spell out your features directly in Python.
 
-    Examines PEP 526 __annotations__ to determine fields.
+    Features are namespaced to a `FeatureSet`.
+    To create a new `FeatureSet`, apply the `@features`
+    decorator to a Python class with typed attributes.
+    A `FeatureSet` is constructed and functions much like
+    Python's own `dataclass`.
+
+    Parameters
+    ----------
+    owner
+        The individual or team responsible for these features.
+        The Chalk Dashboard will display this field, and alerts
+        can be routed to owners.
+    tags
+        Added metadata for features for use in filtering, aggregations,
+        and visualizations. For example, you can use tags to assign
+        features to a team and find all features for a given team.
+    etl_offline_to_online
+        When `True`, Chalk copies this feature into the online environment
+        when it is computed in offline resolvers.
+        Setting `etl_offline_to_online` on a feature class assigns it to all features on the
+        class which do not explicitly specify `etl_offline_to_online`.
+    max_staleness
+        When a feature is expensive or slow to compute, you may wish to cache its value.
+        Chalk uses the terminology "maximum staleness" to describe how recently a feature
+        value needs to have been computed to be returned without re-running a resolver.
+        Assigning a `max_staleness` to the feature class assigns it to all features on the
+        class which do not explicitly specify a `max_staleness` value of their own.
+
+    Other Parameters
+    ----------------
+    cls
+        The decorated class. You shouldn't need to pass this argument.
+    name
+        The name for the feature set. By default, the name of a feature is
+        taken from the name of the attribute on the class, prefixed with
+        the camel-cased name of the class.
+
+    Examples
+    --------
+    >>> @features(
+    ...     owner="andy@chalk.ai",
+    ...     max_staleness="30m",
+    ...     etl_offline_to_online=True,
+    ...     tags="user-group",
+    ... )
+    ... class User:
+    ...     id: str
+    ...     name: str | None
+    ...     location: LatLng
     """
 
     def wrap(c: Type[T]) -> Type[T]:
+        nonlocal max_staleness
         namespace = name or to_snake_case(c.__name__)
         if name is not None and re.sub(r"[^a-z_0-9]", "", namespace) != namespace:
             raise ValueError(
                 (
                     f"Namespace must be composed of lower-case alpha-numeric characters and '_'. Provided namespace "
                     f"'{namespace}' for class '{c.__name__}' contains invalid characters."
                 )
             )
         if name is not None and len(namespace) == 0:
             raise ValueError(f"Namespace cannot be an empty string, but is for the class '{c.__name__}'.")
+        if max_staleness is None:
+            max_staleness = timedelta(0)
+        if isinstance(max_staleness, str):
+            max_staleness = parse_chalk_duration(max_staleness)
         updated_class = _process_class(
             cls=c,
             owner=owner,
             tags=ensure_tuple(tags),
             etl_offline_to_online=etl_offline_to_online,
-            max_staleness=timedelta_to_duration(max_staleness)
-            if isinstance(max_staleness, timedelta)
-            else max_staleness,
+            max_staleness=max_staleness,
             namespace=namespace,
         )
-        set_new_attribute(
-            cls=updated_class,
-            name="namespace",
-            value=namespace,
-        )
         assert issubclass(updated_class, Features)
         FeatureSetBase.registry[updated_class.__chalk_namespace__] = updated_class
-
-        primary_feature = _discover_feature(
-            updated_class,
-            "primary",
-            lambda f: f.primary,
-            lambda f: f.name == "id" and not f.has_resolved_join and not f.is_feature_time,
-        )
-        if primary_feature is not None:
-            primary_feature.primary = True
-
-        timestamp_feature = _discover_feature(
-            updated_class,
-            "feature time",
-            lambda f: f.is_feature_time,
-        )
-        set_new_attribute(cls=updated_class, name="__chalk_primary__", value=primary_feature)
-        set_new_attribute(cls=updated_class, name="__chalk_ts__", value=timestamp_feature)
-        FeatureSetBase.hook and FeatureSetBase.hook(cast(Features, updated_class))
+        if FeatureSetBase.hook is not None:
+            FeatureSetBase.hook(cast(Features, updated_class))
 
         return cast(Type[T], updated_class)
 
     # See if we're being called as @features or @features().
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as @features without parens.
     return wrap(cls)
 
 
-def _discover_feature(cls: Type[Features], name: str, *conditions: Callable[[Feature], bool]):
+def _discover_feature(
+    features: Sequence[Feature], name: str, *conditions: Callable[[Feature], bool]
+) -> Optional[Feature]:
     for cond in conditions:
-        features = [c for c in cls.features if cond(c)]
-        if len(features) == 1:
-            return features[0]
-        if len(features) > 1:
+        filtered_features = [c for c in features if cond(c)]
+        if len(filtered_features) == 1:
+            return filtered_features[0]
+        if len(filtered_features) > 1:
+            assert filtered_features[0].features_cls is not None
+            feature_cls_name = filtered_features[0].features_cls.__name__
             raise ValueError(
-                f"Multiple {name} features are not supported in {cls.__name__}: "
-                + ", ".join(f"{cls.__name__}.{x.name}" for x in features)
+                f"Multiple {name} features are not supported in {feature_cls_name}: "
+                + ", ".join(f"{feature_cls_name}.{x.name}" for x in filtered_features)
             )
     return None
 
 
-def _init_param(f: Feature):
+def _init_param(name: str, annotation: Any, _locals: Dict[str, Any]):
     # Return the __init__ parameter string for this field.  For
     # example, the equivalent of 'x:int=3' (except instead of 'int',
     # reference a variable set to int, and instead of '3', reference a
     # variable set to 3).
-    return f"{f.attribute_name}:_type_{f.attribute_name}=MISSING"
+    annotation_name = f"_type_{name}"
+    _locals[annotation_name] = annotation
+    return f"{name}:{annotation_name}=MISSING"
+
+
+def _setattr_fn(bidirectional_alias: Dict[str, str], _globals: Dict[str, Any]):
+    return create_fn(
+        name="__setattr__",
+        args=["self", "key", "value"],
+        body=[
+            f"alias = {bidirectional_alias}",
+            "if key in alias:",
+            "    super(self.__class__, self).__setattr__(alias[key], value)",
+            "return super(self.__class__, self).__setattr__(key, value)",
+        ],
+        _globals=_globals,
+        _locals={},
+        return_type=None,
+    )
 
 
 def _getattribute_fn(_globals: Dict[str, Any]):
-    # If calling getattr() on an instance for a feature name, do NOT return a class-level FeatureWrapper
+    # If calling getattr() on an instance for a feature name,
+    # do NOT return a class-level FeatureWrapper.
     # Instead, raise an attribute error
+
     return create_fn(
         name="__getattribute__",
         args=["self", "attribute_name"],
         body=[
             "o = object.__getattribute__(self, attribute_name)",
             "if isinstance(o, FeatureWrapper):",
-            "    raise AttributeError(f'Feature {attribute_name} is not defined on this instance of class {type(self).__name__}')",
+            "    raise AttributeError(f'Feature \\'{attribute_name}\\' is not defined on this instance of class \\'{type(self).__name__}\\'')",
             "return o",
         ],
         _globals=_globals,
         _locals={
             "FeatureWrapper": FeatureWrapper,
         },
         return_type=Any,
     )
 
 
-def _init_fn(fields: List[Feature], self_name: str, _globals: Dict[str, Any]):
-    # fields contains both real fields and InitVar pseudo-fields.
+def _init_fn(
+    feature_names_and_annotations: List[Tuple[str, Any]],
+    alias_from_to: Mapping[str, str],
+    _globals: Dict[str, Any],
+):
+    _locals = {
+        "MISSING": MISSING,
+    }
+    _init_params = [_init_param(name, annotation, _locals) for (name, annotation) in feature_names_and_annotations]
+    _init_params.append(_init_param(GENERATED_OBSERVED_AT_NAME, datetime, _locals))
+
+    # Not using "self" for the self name in case if there is a feature called "self"
+    self_name = "__chalk_self__"
+    body_lines: List[str] = []
+    for from_, to in alias_from_to.items():
+        body_lines.extend(
+            [
+                f"if {from_} is not MISSING and {to} is not MISSING:",
+                f"    raise ValueError('The features \\'{from_}\\' and \\'{to}\\' are aliases of each other. Only one can be specified, but both were given.')",
+                f"{from_} = {to} if {from_} is MISSING else {from_}",
+            ]
+        )
+    body_lines.extend([field_assign(name, name, self_name) for (name, _) in feature_names_and_annotations])
 
-    # Make sure we don't have fields without defaults following fields
-    # with defaults.  This actually would be caught when exec-ing the
-    # function source code, but catching it here gives a better error
-    # message, and future-proofs us in case we build up the function
-    # using ast.
-
-    _locals: MutableMapping[str, Any] = {f"_type_{f.attribute_name}": f.typ and f.typ.annotation for f in fields}
-    _locals.update(
-        {
-            "MISSING": MISSING,
-            # '_HAS_DEFAULT_FACTORY': _HAS_DEFAULT_FACTORY,
-        }
+    # Check to see whether the GENERATED_OBSERVED_AT_NAME is the name of the timestamp feature
+    # We must include GENERATED_OBSERVED_AT_NAME in the __init__ signature, even if there is a timestamp
+    # feature defined and named, because we cannot parse the class annotations until after the module is fully
+    # loaded (otherwise we'll get circular errors when trying to resolve forward reference annotations)
+    # So, we ALWAYS include the GENERATED_OBSERVED_AT_NAME as part of the signature, and then error if
+    # that is not the name of the timestamp feature
+    error_msg = f"{self_name}.__class__.__name__ + \".__init__() got unexpected value for argument '{GENERATED_OBSERVED_AT_NAME}'\""
+    has_explicit_ts_feature = f"{self_name}.__chalk_ts__.attribute_name != '{GENERATED_OBSERVED_AT_NAME}'"
+    specified_val_for_generated_observed_at = f"{GENERATED_OBSERVED_AT_NAME} is not MISSING"
+    # Raising a TypeError to be consistent with an unexpected argument message
+    body_lines.append(
+        f"if {specified_val_for_generated_observed_at} and {has_explicit_ts_feature}: raise TypeError({error_msg})"
     )
+    body_lines.append(field_assign(GENERATED_OBSERVED_AT_NAME, GENERATED_OBSERVED_AT_NAME, self_name))
 
-    body_lines = []
-    for f in fields:
-        assert f.attribute_name is not None
-        line = field_assign(f.attribute_name, f.attribute_name, self_name)
-        # line is None means that this field doesn't require
-        # initialization (it's a pseudo-field).  Just skip it.
-        if line:
-            body_lines.append(line)
-
-    # If no body lines, use 'pass'.
-    if not body_lines:
-        body_lines = ["pass"]
-
-    # Add the keyword-only args.  Because the * can only be added if
-    # there's at least one keyword-only arg, there needs to be a test here
-    # (instead of just concatenting the lists together).
-    _init_params = [_init_param(f) for f in fields]
     return create_fn(
         name="__init__",
         args=[self_name] + _init_params,
         body=body_lines,
         _locals=_locals,
         _globals=_globals,
         return_type=None,
@@ -221,52 +274,71 @@
 
 def _get_field(
     cls: Type,
     annotation_name: str,
     comments: Mapping[str, str],
     class_owner: Optional[str],
     class_tags: Optional[Tuple[str, ...]],
-    class_etl_offline_to_online: Optional[bool],
-    class_max_staleness: Optional[Duration],
+    class_etl_offline_to_online: bool,
+    class_max_staleness: timedelta,
     namespace: str,
-):
+) -> Feature:
     # Return a Field object for this field name and type.  ClassVars and
     # InitVars are also returned, but marked as such (see f._field_type).
     # default_kw_only is the value of kw_only to use if there isn't a field()
     # that defines it.
 
     # If the default value isn't derived from Field, then it's only a
     # normal default value.  Convert it to a Field().
-    default = getattr(cls, annotation_name, MISSING)
+    default = getattr(cls, annotation_name, ...)
 
     if isinstance(default, Feature):
+        # The feature was set like x: int = Feature(...)
         f = default
+        if f.version is not None:
+            f.version.base_name = f._name or annotation_name
+            f.name = f.version.name_for_version(f.version.default)
+        if f.is_name_set():
+            if "." in f.name:
+                raise ValueError(
+                    f"Custom feature names cannot contain a dot, but the feature '{f.name}' on the class '{cls.__name__}' includes a dot. You might consider using a has-one feature instead."
+                )
+            elif " " in f.name:
+                raise ValueError(
+                    f"Custom feature names cannot contain spaces, but the feature '{f.name}' on the class '{cls.__name__}' includes a space."
+                )
+    elif isinstance(default, Windowed):
+        # The feature was set like x: Windowed[int] = windowed()
+        # Convert it to a Feature
+        f = default._to_feature(bucket=None)
     else:
+        # The feature was not set explicitly
         if isinstance(default, types.MemberDescriptorType):
             # This is a field in __slots__, so it has no default value.
-            default = MISSING
-        f = Feature(name=annotation_name, namespace=namespace)
+            default = ...
+        f = Feature(name=annotation_name, namespace=namespace, default=default)
 
     # Only at this point do we know the name and the type.  Set them.
     f.namespace = namespace
     f.typ = ParsedAnnotation(cls, annotation_name)
+
     f.features_cls = cls
     f.attribute_name = annotation_name
     _process_field(f, comments, class_owner, class_tags, class_etl_offline_to_online, class_max_staleness)
     return f
 
 
 def _process_field(
     f: Feature,
     comments: Mapping[str, str],
     class_owner: Optional[str],
     class_tags: Optional[Tuple[str, ...]],
-    class_etl_offline_to_online: Optional[bool],
-    class_max_staleness: Optional[Duration],
-):
+    class_etl_offline_to_online: bool,
+    class_max_staleness: timedelta,
+) -> Feature:
     comment_for_feature = comments.get(f.attribute_name)
     comment_based_description = None
     comment_based_owner = None
     comment_based_tags = None
 
     if comment_for_feature is not None:
         comment_lines = []
@@ -307,19 +379,21 @@
                 f"Owner for {f.namespace}.{f.name} specified both on the feature and in the comment. "
                 f"Please use only one of these two."
             )
         )
     elif f.owner is None:
         f.owner = comment_based_owner or class_owner
 
-    if f.max_staleness is Ellipsis:
-        f.max_staleness = class_max_staleness if class_max_staleness is not Ellipsis else None
-
-    if f.etl_offline_to_online is None:
-        f.etl_offline_to_online = False if class_etl_offline_to_online is None else class_etl_offline_to_online
+    # Using the private variable because the max_staleness is a read-only property
+    if f._max_staleness is ...:
+        f._max_staleness = class_max_staleness
+
+    # Using the private variable because the etl_offline_to_online is a read-only property
+    if f._etl_offline_to_online is None:
+        f._etl_offline_to_online = False if class_etl_offline_to_online is None else class_etl_offline_to_online
     return f
 
 
 def _recursive_repr(user_function: Callable[[T], str]) -> Callable[[T], str]:
     # Decorator to make a repr function return "..." for a recursive
     # call.
     repr_running = set()
@@ -335,72 +409,84 @@
         finally:
             repr_running.discard(key)
         return result
 
     return wrapper
 
 
-def _repr_fn(fields: List[Feature], _globals: Dict[str, Any]):
-    tuples = ",".join(f"('{f.attribute_name}', getattr(self, '{f.attribute_name}', MISSING))" for f in fields)
+def _repr_fn(_globals: Dict[str, Any]):
+    tuples = "((f.attribute_name, getattr(self, f.attribute_name, MISSING)) for f in self.features)"
     fn = create_fn(
         name="__repr__",
         args=["self"],
         body=[
             'return f"{self.__class__.__qualname__}(" + '
-            + f"', '.join(f'{{x[0]}}={{x[1]}}' for x in [{tuples}] if x[1] != MISSING)"
+            + f"', '.join(f'{{x[0]}}={{x[1]}}' for x in {tuples} if x[1] != MISSING)"
             + '+ ")"'
         ],
         _globals=_globals,
         _locals={"MISSING": MISSING},
     )
     return _recursive_repr(fn)
 
 
-def _eq_fn(fields: List[Feature], _globals: Dict[str, Any]):
-    cmp_str = " and ".join(
-        f"(getattr(self, '{f.attribute_name}', MISSING) == getattr(other, '{f.attribute_name}', MISSING))"
-        for f in fields
-    )
-    if not cmp_str:
-        # if there are no features in this class
-        cmp_str = "True"
+def _eq_fn(_globals: Dict[str, Any]):
+    cmp_str = "all(getattr(self, f.attribute_name, MISSING) == getattr(__chalk_other__, f.attribute_name, MISSING) for f in self.features)"
     return create_fn(
         name="__eq__",
-        args=["self", "other"],
-        body=["if not isinstance(other, type(self)):", "    return NotImplemented", f"return {cmp_str}"],
+        args=["self", "__chalk_other__"],
+        body=[
+            "if not isinstance(__chalk_other__, type(self)):",
+            "    return NotImplemented",
+            f"return {cmp_str}",
+        ],
         _globals=_globals,
         _locals={
             "MISSING": MISSING,
         },
     )
 
 
 def _len_fn(_globals: Dict[str, Any]):
     return create_fn(
         name="__len__",
         args=["self"],
         body=[
-            "count = 0",
-            f"for f in self.features:",
-            "    if hasattr(self, f.attribute_name):",
-            "        count += 1",
-            "return count",
+            "__chalk_count__ = 0",
+            f"for __chalk_f__ in self.features:",
+            "    if not __chalk_f__.no_display and hasattr(self, __chalk_f__.attribute_name):",
+            "        __chalk_count__ += 1",
+            "return __chalk_count__",
+        ],
+        _globals=_globals,
+        _locals={},
+    )
+
+
+def _items_fn(_globals: Dict[str, Any]):
+    return create_fn(
+        name="items",
+        args=["self"],
+        body=[
+            f"for __chalk_f__ in self.features:",
+            "    if not __chalk_f__.no_display and hasattr(self, __chalk_f__.attribute_name):",
+            "        yield __chalk_f__.fqn, getattr(self, __chalk_f__.attribute_name)",
         ],
         _globals=_globals,
         _locals={},
     )
 
 
-def _iter_fn(fields: List[Feature], _globals: Mapping[str, Any]):
+def _iter_fn(_globals: Mapping[str, Any]):
     return create_fn(
         "__iter__",
         args=["self"],
         body=[
             f"for __chalk_f__ in self.features:",
-            f"    if hasattr(self, __chalk_f__.attribute_name) and type(__chalk_f__).__name__ == 'Feature' and not __chalk_f__.is_has_one and not __chalk_f__.is_has_many:",
+            f"    if hasattr(self, __chalk_f__.attribute_name) and type(__chalk_f__).__name__ == 'Feature' and not __chalk_f__.is_has_one and not __chalk_f__.is_has_many and not __chalk_f__.no_display:",
             f"        yield __chalk_f__.fqn, getattr(self, __chalk_f__.attribute_name)",
         ],
     )
 
 
 def _parse_annotation_comments(cls: Type) -> Mapping[str, str]:
     source = textwrap.dedent(inspect.getsource(cls))
@@ -428,112 +514,243 @@
     return comments_for_annotations
 
 
 def _process_class(
     cls: Type[T],
     owner: Optional[str],
     tags: Tuple[str, ...],
-    etl_offline_to_online: Optional[bool],
-    max_staleness: Optional[Duration],
+    etl_offline_to_online: bool,
+    max_staleness: timedelta,
     namespace: str,
 ) -> Type[T]:
-    cls_annotations = cls.__dict__.get("__annotations__", {})
+    raw_cls_annotations = cls.__dict__.get("__annotations__", {})
+
+    cls_annotations: Dict[str, Any] = {}
+    for name, annotation in raw_cls_annotations.items():
+        if isinstance(annotation, Windowed):
+            # NOTE: For Windowed resolvers, both the Annotation and the value are instances of Windowed,
+            # unlike normal features whose annotation is the underlying type, and the value is an instance
+            # of FeatureWrapper. So both `annotation` and `wind` should be instances of Windowed
+            # In the future, we should use a subclass of Windowed, rather than an instance, for the type annotation,
+            # similar to what we do for Features
+            wind = getattr(cls, name, None)
+            if wind is None or not isinstance(wind, Windowed):
+                assert annotation._kind is not None
+                raise TypeError(
+                    (
+                        f"Windowed feature '{namespace}.{name}' is missing windows. "
+                        f"To create a windowed feature, use "
+                        f"'{name}: Windowed[{annotation._kind.__name__}] = windowed('10m', '30m')."
+                    )
+                )
+            wind.kind = annotation.kind
+            wind._name = name
+            annotation._buckets = wind._buckets
+            for bucket in wind._buckets:
+                # Make pseudofeatures for each bucket of the window
+                feat = wind._to_feature(bucket=bucket)
+                setattr(cls, feat.name, feat)
+                # For the psuedofeatures, which track an individual bucket, the correct annotation is the
+                # underlying annotation, not Windowed[underlying], since it's only one value
+                cls_annotations[feat.name] = wind.kind
+
+        cls_annotations[name] = annotation
 
     if cls.__module__ in sys.modules:
         _globals = sys.modules[cls.__module__].__dict__
     else:
         _globals = {}
 
     # Find feature times that weren't annotated.
-    for (name, member) in inspect.getmembers(cls):
+    for name, member in inspect.getmembers(cls):
+        if name not in cls_annotations and isinstance(member, Windowed):
+            raise TypeError(f"Windowed feature '{namespace}.{name}' is missing an annotation, like 'Windowed[str]'")
         if name not in cls_annotations and isinstance(member, Feature):
             # All feature types need annotations, except for datetimes, which we can automatically infer
-            if member.typ is not None and member.typ.is_parsed and issubclass(member.typ.underlying, datetime):
-                cls_annotations[name] = datetime
-            else:
-                raise TypeError(f"Member {name} is missing an annotation")
+            if not member.is_typ_set() or not member.typ.is_parsed:
+                raise TypeError(
+                    f"Feature '{namespace}.{name}' is missing an annotation. Please add one, like '{name}: str = ...'"
+                )
+            cls_annotations[name] = member.typ.annotation
+
+    cls.__annotations__ = cls_annotations
 
     # If we pass this function something that isn't a class, it could raise
     try:
         comments = _parse_annotation_comments(cls)
     except:
         comments = {}
 
-    cls_fields = [
-        _get_field(
-            cls=cls,
-            annotation_name=name,
-            comments=comments,
-            class_owner=owner,
-            class_tags=tags,
-            class_etl_offline_to_online=etl_offline_to_online,
-            class_max_staleness=max_staleness,
-            namespace=namespace,
+    cls_fields: List[Feature] = []
+
+    def __chalk_primary__(cls: Type[Features]):
+        return _discover_feature(
+            cls_fields,
+            "primary",
+            lambda f: f._primary is True,
+            lambda f: f.typ.is_primary,
+            lambda f: (
+                f.name == "id" and not f.has_resolved_join and not f._is_feature_time and not f.typ.is_feature_time
+            ),
+        )
+
+    set_new_attribute(cls, "__chalk_primary__", value=classproperty(__chalk_primary__, cached=True))
+
+    def __chalk_ts__(cls: Type[Features]) -> Feature:
+        # Not using `f.is_feature_time` as that would create an infinite recursion, since
+        # `.is_feature_time` accesses `__chalk_ts__`
+        ts_feature: Optional[Feature] = _discover_feature(
+            cls_fields,
+            "feature time",
+            lambda f: f._is_feature_time is True,
+            lambda f: f.typ.is_feature_time,
+            lambda f: f.name == "ts" and not f.has_resolved_join and not f._primary and not f.typ.is_primary,
+        )
+        if ts_feature is None:
+            return unwrap_feature(getattr(cls, GENERATED_OBSERVED_AT_NAME))
+        return ts_feature
+
+    set_new_attribute(cls=cls, name="__chalk_ts__", value=classproperty(__chalk_ts__, cached=True))
+
+    def __chalk_observed_at__(cls: Type[Features]) -> FeatureWrapper:
+        ts_feature: Optional[Feature] = _discover_feature(
+            cls_fields,
+            "feature time",
+            # Not using `f.is_feature_time` as that would create an infinite recursion, since
+            # `.is_feature_time` accesses `__chalk_ts__` which can access this function
+            lambda f: f._is_feature_time is True,
+            lambda f: f.typ.is_feature_time,
+            lambda f: f.name == "ts" and not f.has_resolved_join and not f._primary and not f.typ.is_primary,
         )
-        for name in cls_annotations
-    ]
-    # If there is no timestamp feature, synthesize one
-    ts_feature: Optional[Feature] = next((x for x in cls_fields if x.is_feature_time), None)
-    if ts_feature is None:
-        # Alternatively check if there is a feature called `ts` that is a datetime
-        ts_feature = next((x for x in cls_fields if x.name == "ts" and not x.has_resolved_join), None)
         if ts_feature is not None:
-            ts_feature.is_feature_time = True
-    if ts_feature is None:
-        # If the timestamp feature is still none, then synthesize one
+            if ts_feature.attribute_name != GENERATED_OBSERVED_AT_NAME:
+                raise AttributeError(f"Object {cls.__name__} has no attribute '{GENERATED_OBSERVED_AT_NAME}")
+        # If the timestamp feature is still none, then synthesize one on first use
         ts_feature = feature_time()
         assert ts_feature is not None
-        ts_feature.name = "__chalk_observed_at__"
-        ts_feature.attribute_name = "__chalk_observed_at__"
-        ts_feature.namespace = namespace
-        ts_feature.typ = ParsedAnnotation(underlying=datetime)
-        ts_feature.features_cls = cls  # type: ignore
+        ts_feature.name = GENERATED_OBSERVED_AT_NAME
+        ts_feature.attribute_name = GENERATED_OBSERVED_AT_NAME
+        ts_feature.namespace = cls.__chalk_namespace__
+        ts_feature.features_cls = cls
         ts_feature.is_autogenerated = True
+        cls.__annotations__[GENERATED_OBSERVED_AT_NAME] = datetime
         _process_field(
             ts_feature,
-            comments=comments,
-            class_owner=owner,
-            class_tags=tags,
-            class_etl_offline_to_online=etl_offline_to_online,
-            class_max_staleness=max_staleness,
+            comments={},
+            class_owner=cls.__chalk_owner__,
+            class_tags=tuple(cls.__chalk_tags__),
+            class_etl_offline_to_online=cls.__chalk_etl_offline_to_online__,
+            class_max_staleness=cls.__chalk_max_staleness__,
         )
-        cls_fields.append(ts_feature)
+
+        return FeatureWrapper(ts_feature)
+
     set_new_attribute(
         cls=cls,
-        name="__init__",
-        value=_init_fn(
-            fields=cls_fields,
-            # The name to use for the "self"
-            # param in __init__.  Use "self"
-            # if possible.
-            self_name="self",
-            _globals=_globals,
-        ),
+        name=GENERATED_OBSERVED_AT_NAME,
+        value=classproperty(__chalk_observed_at__, cached=True, bind_to_instances=False),
     )
 
-    set_new_attribute(cls=cls, name="__repr__", value=_repr_fn(fields=cls_fields, _globals=_globals))
-    set_new_attribute(cls=cls, name="__eq__", value=_eq_fn(fields=cls_fields, _globals=_globals))
+    def __features__(cls: Features) -> List[Feature]:
+        features = list(cls_fields)
+        if cls.__chalk_ts__ not in features:
+            assert cls.__chalk_ts__ is not None
+            features.append(cls.__chalk_ts__)
+        return features
+
+    set_new_attribute(cls=cls, name="features", value=classproperty(__features__, cached=True))
+    set_new_attribute(cls=cls, name="__repr__", value=_repr_fn(_globals=_globals))
+    set_new_attribute(cls=cls, name="__eq__", value=_eq_fn(_globals=_globals))
     set_new_attribute(cls=cls, name="__hash__", value=None)
-    set_new_attribute(cls=cls, name="__iter__", value=_iter_fn(fields=cls_fields, _globals=_globals))
+    set_new_attribute(cls=cls, name="__iter__", value=_iter_fn(_globals=_globals))
+    set_new_attribute(cls=cls, name="items", value=_items_fn(_globals=_globals))
 
+    set_new_attribute(cls=cls, name="namespace", value=namespace)
     set_new_attribute(cls=cls, name="__chalk_namespace__", value=namespace)
     set_new_attribute(cls=cls, name="__chalk_owner__", value=owner)
     set_new_attribute(cls=cls, name="__chalk_tags__", value=list(tags))
-    set_new_attribute(
-        cls=cls, name="__chalk_max_staleness__", value=max_staleness if max_staleness is not Ellipsis else None
-    )
+    set_new_attribute(cls=cls, name="__chalk_max_staleness__", value=max_staleness)
     set_new_attribute(
         cls=cls,
         name="__chalk_etl_offline_to_online__",
-        value=etl_offline_to_online if etl_offline_to_online is not Ellipsis else False,
+        value=etl_offline_to_online,
     )
-    set_new_attribute(cls=cls, name="features", value=cls_fields)
     set_new_attribute(cls=cls, name="__is_features__", value=True)
     set_new_attribute(cls=cls, name="__len__", value=_len_fn(_globals=_globals))
     set_new_attribute(cls=cls, name="__getattribute__", value=_getattribute_fn(_globals=_globals))
+    # Moving this line lower causes all kinds of problems.
+    cls = classproperty_support(cls)
+
+    # Parse the fields after we have the correct `cls` set
+    cls_fields.extend(
+        _get_field(
+            cls=cls,
+            annotation_name=name,
+            comments=comments,
+            class_owner=owner,
+            class_tags=tags,
+            class_etl_offline_to_online=etl_offline_to_online,
+            class_max_staleness=max_staleness,
+            namespace=namespace,
+        )
+        for name in cls_annotations
+    )
+
+    alias_from_to: Dict[str, str] = {}
+
+    # We're appending to this list
+    for f in islice(cls_fields, len(cls_fields)):
+        if f.version is None:
+            continue
+        alias_from_to[f.attribute_name] = f"{f.attribute_name}_v{f.version.default}"
+
+        for i in range(1, f.version.maximum + 1):
+            f_i = copy.copy(f)
+            f_i.name = f.version.name_for_version(i)
+            f_i.attribute_name = f"{f.attribute_name}_v{i}"
+            f_i.version = _VersionInfo(
+                version=i,
+                maximum=f.version.maximum,
+                default=f.version.default,
+                reference=f.version.reference,
+            )
+            f.version.reference[i] = f_i
+            cls_fields.append(f_i)
+
+            # The default feature already exists.
+            f_i.no_display = i == f.version.default
+
+            if f_i.attribute_name in cls_annotations:
+                assert f_i.features_cls is not None
+                raise ValueError(
+                    (
+                        f"The class '{f_i.features_cls.__name__}' "
+                        f"has an existing annotation '{f_i.attribute_name}' "
+                        "that collides with a versioned feature. Please remove the existing "
+                        "annotation, or lower the version."
+                    )
+                )
+
+    set_new_attribute(
+        cls=cls,
+        name="__setattr__",
+        value=_setattr_fn(
+            bidirectional_alias=dict({v: k for k, v in alias_from_to.items()}, **alias_from_to),
+            _globals=_globals,
+        ),
+    )
+    set_new_attribute(
+        cls=cls,
+        name="__init__",
+        value=_init_fn(
+            feature_names_and_annotations=[(x.attribute_name, x.typ.annotation) for x in cls_fields],
+            alias_from_to=alias_from_to,
+            _globals=_globals,
+        ),
+    )
 
     for f in cls_fields:
         assert f.attribute_name is not None
         # Wrap all class features with FeatureWrapper
         setattr(cls, f.attribute_name, FeatureWrapper(f))
 
     return cls
```

### Comparing `chalkpy-1.9.9/chalk/features/hooks.py` & `chalkpy-2.0.0/chalk/features/hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 import logging
-from typing import Callable, Iterable, List, Optional, Set, TypeVar, Union, overload
+from typing import Any, Callable, Iterable, Optional, Set, Tuple, Union, overload
 
-T = TypeVar("T")
+from typing_extensions import TypeAlias
 
+from chalk.features.tag import Environments
+from chalk.utils.collections import ensure_tuple
 
-HookFn = Callable[[], T]
-EnvironmentFilter = Optional[Union[List[str], str]]
+HookFn: TypeAlias = Callable[[], Any]
 
 
 def _run_all_hooks(environment: str, hooks: Iterable["Hook"]) -> None:
     for hook in hooks:
         if hook.environment is None or environment in hook.environment:
             try:
                 hook()
@@ -20,31 +21,25 @@
 
 
 class Hook:
     # Registry
     before_all: Set["Hook"] = set()
     after_all: Set["Hook"] = set()
 
-    environment: Optional[List[str]]
+    environment: Optional[Tuple[str, ...]]
     fn: HookFn
     filename: str
 
-    def __init__(self, fn: HookFn, filename: str, environment: Optional[EnvironmentFilter] = None):
+    def __init__(self, fn: HookFn, filename: str, environment: Optional[Environments] = None):
         self.fn = fn
         self.filename = filename
-        self.environment = (
-            [
-                environment,
-            ]
-            if isinstance(environment, str)
-            else environment
-        )
+        self.environment = None if environment is None else ensure_tuple(environment)
 
-    def __call__(self, *args, **kwargs):
-        return self.fn(*args, **kwargs)
+    def __call__(self):
+        return self.fn()
 
     def __repr__(self):
         return f'Hook(filename={self.filename}, fn={self.fn.__name__}", environment={str(self.environment)})'
 
     @classmethod
     def run_all_before_all(cls, environment: str) -> None:
         return _run_all_hooks(environment, cls.before_all)
@@ -56,45 +51,45 @@
 
 @overload
 def before_all(fn: HookFn, /) -> Hook:
     ...
 
 
 @overload
-def before_all(fn: None = None, /, environment: EnvironmentFilter = None) -> Callable[[HookFn], Hook]:
+def before_all(fn: None = None, /, environment: Optional[Environments] = None) -> Callable[[HookFn], Hook]:
     ...
 
 
 def before_all(
-    fn: Optional[HookFn] = None, /, environment: EnvironmentFilter = None
+    fn: Optional[HookFn] = None, /, environment: Optional[Environments] = None
 ) -> Union[Hook, Callable[[HookFn], Hook]]:
     caller_filename = inspect.stack()[1].filename
 
-    def decorator(f, cf=caller_filename):
-        hook = Hook(fn=f, filename=cf, environment=environment)
+    def decorator(f: HookFn):
+        hook = Hook(fn=f, filename=caller_filename, environment=environment)
         Hook.before_all.add(hook)
         return hook
 
     return decorator(fn) if fn else decorator
 
 
 @overload
-def after_all(fn: HookFn, /, environment: EnvironmentFilter = None) -> Hook:
+def after_all(fn: HookFn, /, environment: Optional[Environments] = None) -> Hook:
     ...
 
 
 @overload
-def after_all(fn: None = None, /, environment: EnvironmentFilter = None) -> Callable[[HookFn], Hook]:
+def after_all(fn: None = None, /, environment: Optional[Environments] = None) -> Callable[[HookFn], Hook]:
     ...
 
 
 def after_all(
-    fn: Optional[HookFn] = None, /, environment: EnvironmentFilter = None
+    fn: Optional[HookFn] = None, /, environment: Optional[Environments] = None
 ) -> Union[Hook, Callable[[HookFn], Hook]]:
     caller_filename = inspect.stack()[1].filename
 
-    def decorator(f, cf=caller_filename):
-        hook = Hook(fn=f, filename=cf, environment=environment)
+    def decorator(f: HookFn):
+        hook = Hook(fn=f, filename=caller_filename, environment=environment)
         Hook.after_all.add(hook)
         return hook
 
     return decorator(fn) if fn else decorator
```

### Comparing `chalkpy-1.9.9/chalk/features/pseudofeatures.py` & `chalkpy-2.0.0/chalk/features/pseudofeatures.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 from datetime import datetime
+from typing import List
 
 from chalk.features.feature_field import Feature
 
 __all__ = [
     "CHALK_TS_FEATURE",
     "ID_FEATURE",
     "OBSERVED_AT_FEATURE",
     "REPLACED_OBSERVED_AT_FEATURE",
     "PSEUDOFEATURES",
+    "PSEUDONAMESPACE",
 ]
 
+PSEUDONAMESPACE = "__chalk__"
 CHALK_TS_FEATURE = Feature(
     name="CHALK_TS",
-    namespace="__chalk__",
+    namespace=PSEUDONAMESPACE,
     typ=datetime,
     max_staleness=None,
     etl_offline_to_online=False,
 )
-ID_FEATURE = Feature(name="__id__", namespace="__chalk__", typ=str, max_staleness=None, etl_offline_to_online=False)
+ID_FEATURE = Feature(
+    name="__id__",
+    namespace=PSEUDONAMESPACE,
+    typ=str,
+    max_staleness=None,
+    etl_offline_to_online=False,
+)
 OBSERVED_AT_FEATURE = Feature(
-    name="__observed_at__", namespace="__chalk__", typ=datetime, max_staleness=None, etl_offline_to_online=False
+    name="__observed_at__",
+    namespace=PSEUDONAMESPACE,
+    typ=datetime,
+    max_staleness=None,
+    etl_offline_to_online=False,
 )
 REPLACED_OBSERVED_AT_FEATURE = Feature(
     name="__replaced_observed_at__",
-    namespace="__chalk__",
+    namespace=PSEUDONAMESPACE,
     typ=datetime,
     max_staleness=None,
     etl_offline_to_online=False,
 )
 
-PSEUDOFEATURES = [CHALK_TS_FEATURE, ID_FEATURE, OBSERVED_AT_FEATURE, REPLACED_OBSERVED_AT_FEATURE]
+PSEUDOFEATURES: List[Feature] = [CHALK_TS_FEATURE, ID_FEATURE, OBSERVED_AT_FEATURE, REPLACED_OBSERVED_AT_FEATURE]
```

### Comparing `chalkpy-1.9.9/chalk/features/resolver.py` & `chalkpy-2.0.0/chalk/sql/_internal/sql_file_resolver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,690 +1,665 @@
-import ast
+from __future__ import annotations
+
 import dataclasses
 import inspect
-import textwrap
-from dataclasses import dataclass
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    Generic,
-    List,
-    Optional,
-    Protocol,
-    Sequence,
-    Type,
-    TypeVar,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-    overload,
-)
-
-from pydantic import BaseModel
-from typing_extensions import ParamSpec
-
-from chalk.df.ast_parser import convert_slice, eval_converted_expr
-from chalk.features.dataframe import DataFrame
-from chalk.features.feature_field import Feature
-from chalk.features.feature_set import Features
-from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
-from chalk.features.filter import Filter
-from chalk.features.tag import Environments, Tags
-from chalk.sql.base.protocols import BaseSQLSourceProtocol
-from chalk.state import StateWrapper
-from chalk.utils.collection_type import GenericAlias
-from chalk.utils.collections import ensure_tuple
-from chalk.utils.duration import Duration, ScheduleOptions
-from chalk.utils.environment_parsing import env_var_bool
-
-MachineType = str
-T = TypeVar("T")
-P = ParamSpec("P")
-
-
-@dataclasses.dataclass(frozen=True)
-class ResolverArgErrorHandler:
-    default_value: Any
-
+import json
+import os
+import re
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Literal, Optional, Sequence, Type, Union, cast
+
+import yaml
+from pydantic import BaseModel, ValidationError, validator
+
+from chalk import OfflineResolver, OnlineResolver
+from chalk.features import DataFrame, Feature, Features, FeatureSetBase
+from chalk.features.resolver import ResolverArgErrorHandler, StreamResolver
+from chalk.sql._internal.integrations.bigquery import BigQuerySourceImpl
+from chalk.sql._internal.integrations.cloudsql import CloudSQLSourceImpl
+from chalk.sql._internal.integrations.mysql import MySQLSourceImpl
+from chalk.sql._internal.integrations.postgres import PostgreSQLSourceImpl
+from chalk.sql._internal.integrations.redshift import RedshiftSourceImpl
+from chalk.sql._internal.integrations.snowflake import SnowflakeSourceImpl
+from chalk.sql._internal.integrations.sqlite import SQLiteSourceImpl
+from chalk.sql._internal.sql_source import BaseSQLSource
+from chalk.streams import KafkaSource
+from chalk.streams.base import StreamSource
+from chalk.streams.types import StreamResolverSignature
+from chalk.utils.duration import parse_chalk_duration
+from chalk.utils.missing_dependency import missing_dependency_exception
+from chalk.utils.string import to_camel_case
+
+if TYPE_CHECKING:
+    from sqlglot.expressions import Expression
+
+_SOURCES = {
+    "snowflake": SnowflakeSourceImpl,
+    "postgres": PostgreSQLSourceImpl,
+    "postgresql": PostgreSQLSourceImpl,
+    "mysql": MySQLSourceImpl,
+    "bigquery": BigQuerySourceImpl,
+    "cloudsql": CloudSQLSourceImpl,
+    "redshift": RedshiftSourceImpl,
+    "sqlite": SQLiteSourceImpl,
+    "kafka": KafkaSource,
+}
+
+_DIALECTS_SQLGLOT: Dict[Type[BaseSQLSource], str] = {
+    SnowflakeSourceImpl: "snowflake",
+    PostgreSQLSourceImpl: "postgres",
+    MySQLSourceImpl: "mysql",
+    BigQuerySourceImpl: "bigquery",
+    RedshiftSourceImpl: "redshift",
+    SQLiteSourceImpl: "sqlite",
+}
+
+_RESOLVER_TYPES = {
+    "offline": OfflineResolver,
+    "batch": OfflineResolver,
+    "online": OnlineResolver,
+    "realtime": OnlineResolver,
+    "stream": StreamResolver,
+    "streaming": StreamResolver,
+}
+
+
+class IncrementalSettings(BaseModel):
+    incremental_column: Optional[str]
+    lookback_period: Optional[str]
+    mode: Literal["row", "group", "parameter"]
+    incremental_timestamp: Literal["feature_time", "resolver_execution_time"]
+
+    @validator("lookback_period")
+    @classmethod
+    def validate_lookback_period(cls, value: Optional[str]):
+        if value is None:
+            return None
+        try:
+            parse_chalk_duration(value)
+        except Exception as e:
+            raise ValueError(f"Could not parse value '{value}' as timedelta, {e}")
+        return value
 
-@dataclass
-class StateDescriptor(Generic[T]):
-    kwarg: str
-    pos: int
-    initial: T
-    typ: Type[T]
+    @validator("mode")
+    @classmethod
+    def validate_mode(cls, mode: Literal["row", "group", "parameter"], values: Dict[str, Any]):
+        if mode in ["row", "group"] and not values["incremental_column"]:
+            raise ValueError(f"'incremental_column' must be set if mode is 'row' or 'group'.")
+        return mode
 
 
-class FilterFunction(Protocol):
-    def __call__(self, *args: Feature) -> bool:
-        ...
+class CommentDict(BaseModel):
+    source: str
+    resolves: str
+    incremental: Optional[IncrementalSettings]
+    tags: Optional[List[str]]
+    environment: Optional[List[str]]
+    count: Optional[Literal[1, "one", "one_or_none"]]
+    cron: Optional[str]
+    machine_type: Optional[str]
+    max_staleness: Optional[str]
+    message: Optional[str]
+    owner: Optional[str]
+    type: Optional[str]
+    timeout: Optional[str]
+
+    @validator("tags", "environment", pre=True)
+    @classmethod
+    def validate_list_inputs(cls, value: Union[str, List[str], None]):
+        if isinstance(value, list):
+            return value
+        if isinstance(value, str):
+            return [value]
+        raise ValueError(f"Value {value} must be a string or a list of strings.")
+
+    @validator("max_staleness", "timeout")
+    @classmethod
+    def validate_timedelta(cls, string: Optional[str]):
+        if string is None:
+            return None
+        try:
+            parse_chalk_duration(string)
+        except Exception as e:
+            raise ValueError(f"Could not parse value '{string}' as timedelta, {e}")
+        return string
 
+    @validator("type")
+    @classmethod
+    def validate_type(cls, resolver_type: str):
+        if resolver_type not in _RESOLVER_TYPES:
+            raise ValueError(
+                (
+                    f"Resolver type '{resolver_type}' not supported. "
+                    f"'online', 'offline' and 'streaming' are supported options"
+                )
+            )
+        return resolver_type
 
-class SampleFunction(Protocol):
-    def __call__(self) -> DataFrame:
-        ...
 
+@dataclasses.dataclass(frozen=True)
+class ResolverError:
+    """Generic class for returning errors at any point during resolution process"""
 
-@dataclass
-class Cron:
-    schedule: Optional[ScheduleOptions] = None
-    filter: Optional[FilterFunction] = None
-    sample: Optional[SampleFunction] = None
-    trigger_downstream: Optional[bool] = True
+    display: str
+    path: str
+    parameter: Optional[str]
 
 
-def _get_expected_features_list(output: Type[Features]) -> Sequence[Feature]:
-    if issubclass(output, Features):
-        output = output.features
+@dataclasses.dataclass(frozen=True)
+class ResolverResult:
+    """Chief return class with resolver we actually use"""
 
-    if len(output) == 1 and issubclass(output[0], DataFrame):
-        return output[0].columns
-    else:
-        return output
+    resolver: Optional[Union[OnlineResolver, OfflineResolver, StreamResolver]]
+    errors: List[ResolverError]
+    db: Optional[Union[BaseSQLSource, StreamSource]]
+    fields: Optional[Dict[str, str]]
+    args: Optional[Dict[str, str]]
 
 
-class Resolver(Protocol):
-    function_definition: str
-    fqn: str
-    filename: str
-    inputs: List[Feature]
-    output: Type[Features]
-    fn: Callable
-    environment: Optional[List[str]]
-    tags: Optional[List[str]]
-    max_staleness: Optional[Duration]
-    machine_type: Optional[MachineType]
-    state: Optional[StateDescriptor]
-    default_args: List[Optional[ResolverArgErrorHandler]]
-
-    registry: "ClassVar[List[Resolver]]" = []
-    hook: "ClassVar[Optional[Callable[[Resolver], None]]]" = None
-
-    def __hash__(self):
-        return hash(self.fqn)
-
-
-def _process_call(result, *, declared_output: Any):
-    from chalk.sql import StringChalkQuery
-    from chalk.sql.integrations.chalk_query import ChalkQuery
-
-    if isinstance(result, (ChalkQuery, StringChalkQuery)):
-        return result.execute_internal(expected_features=_get_expected_features_list(declared_output))
-
-    return result
-
-
-class SinkResolver:
-    registry: "List[SinkResolver]" = []
-
-    def __eq__(self, other):
-        return isinstance(other, SinkResolver) and self.fqn == other.fqn
-
-    def __hash__(self):
-        return hash(self.fqn)
-
-    def __call__(self, *args, **kwargs):
-        return _process_call(self.fn(*args, **kwargs), declared_output=None)
-
-    def __init__(
-        self,
-        function_definition: str,
-        fqn: str,
-        filename: str,
-        doc: Optional[str],
-        inputs: List[Feature],
-        output: Type[Features],
-        fn: Callable,
-        environment: Optional[List[str]],
-        tags: Optional[List[str]],
-        machine_type: Optional[MachineType],
-        buffer_size: Optional[int],
-        debounce: Optional[Duration],
-        max_delay: Optional[Duration],
-        upsert: Optional[bool],
-        integration: Optional[BaseSQLSourceProtocol] = None,
-    ):
-        self.function_definition = function_definition
-        self.fqn = fqn
-        self.filename = filename
-        self.inputs = inputs
-        self.output = output
-        self.fn = fn
-        self.environment = environment
-        self.tags = tags
-        self.doc = doc
-        self.machine_type = machine_type
-        self.buffer_size = buffer_size
-        self.debounce = debounce
-        self.max_delay = max_delay
-        self.upsert = upsert
-        self.integration = integration
-
-    def __repr__(self):
-        return f"SinkResolver(name={self.fqn})"
-
-
-class OnlineResolver(Resolver):
-    cron: Union[ScheduleOptions, Cron]
-
-    def __eq__(self, other):
-        return isinstance(other, OnlineResolver) and self.fqn == other.fqn
-
-    def __hash__(self):
-        return hash(self.fqn)
-
-    def __call__(self, *args, **kwargs):
-        return _process_call(self.fn(*args, **kwargs), declared_output=self.output)
-
-    @property
-    def __name__(self):
-        return self.fn.__name__
-
-    @property
-    def __module__(self):
-        return self.fn.__module__
-
-    def __init__(
-        self,
-        function_definition: str,
-        fqn: str,
-        filename: str,
-        doc: Optional[str],
-        inputs: List[Feature],
-        output: Type[Features],
-        fn: Callable,
-        environment: Optional[List[str]],
-        tags: Optional[List[str]],
-        max_staleness: Optional[Duration],
-        cron: Optional[Union[ScheduleOptions, Cron]],
-        machine_type: Optional[MachineType],
-        when: Optional[Filter],
-        state: Optional[StateDescriptor],
-        default_args: List[Optional[ResolverArgErrorHandler]],
-    ):
-        self.function_definition = function_definition
-        self.fqn = fqn
-        self.filename = filename
-        self.inputs = inputs
-        self.output = output
-        self.fn = fn
-        self.environment = environment
-        self.tags = tags
-        self.max_staleness = max_staleness
-        self.cron = cron
-        self.doc = doc
-        self.machine_type = machine_type
-        self.when = when
-        self.state = state
-        self.default_args = default_args
-
-    def __repr__(self):
-        return f"OnlineResolver(name={self.fqn})"
-
-
-class OfflineResolver(Resolver):
-    def __eq__(self, other):
-        return isinstance(other, OfflineResolver) and self.fqn == other.fqn
-
-    def __hash__(self):
-        return hash(self.fqn)
-
-    def __call__(self, *args, **kwargs):
-        return _process_call(self.fn(*args, **kwargs), declared_output=self.output)
-
-    @property
-    def __name__(self):
-        return self.fn.__name__
-
-    @property
-    def __module__(self):
-        return self.fn.__module__
-
-    def __init__(
-        self,
-        function_definition: str,
-        fqn: str,
-        filename: str,
-        doc: Optional[str],
-        inputs: List[Feature],
-        output: Type[Features],
-        fn: Callable,
-        environment: Optional[List[str]],
-        tags: Optional[List[str]],
-        max_staleness: Optional[Duration],
-        cron: Union[ScheduleOptions, Cron],
-        machine_type: Optional[MachineType],
-        state: Optional[StateDescriptor],
-        when: Optional[Filter],
-        default_args: List[Optional[ResolverArgErrorHandler]],
-    ):
-        self.when = when
-        self.function_definition = function_definition
-        self.fqn = fqn
-        self.filename = filename
-        self.doc = doc
-        self.inputs = inputs
-        self.output = output
-        self.fn = fn
-        self.environment = environment
-        self.tags = tags
-        self.max_staleness = max_staleness
-        self.cron = cron
-        self.machine_type = machine_type
-        self.state = state
-        self.default_args = default_args
+@dataclasses.dataclass(frozen=True)
+class SQLStringResult:
+    """Class for getting the sql string from the file"""
 
-    def __repr__(self):
-        return f"OfflineResolver(name={self.fqn})"
+    path: str
+    sql_string: Optional[str]
+    error: Optional[ResolverError]
+
+    @classmethod
+    def fail(cls, display_error: str, path: str) -> "SQLStringResult":
+        return cls(path=path, sql_string=None, error=ResolverError(display=display_error, path=path, parameter=None))
 
 
 @dataclasses.dataclass(frozen=True)
-class ResolverParseResult:
-    fqn: str
-    inputs: List[Feature]
-    state: Optional[StateDescriptor]
-    output: Optional[Type[Features]]
-    function_definition: str
-    function: Callable
-    doc: Optional[str]
-    default_args: List[Optional[ResolverArgErrorHandler]]
-
-
-class ResolverAnnotationParser:
-    def __init__(self, resolver: Callable, glbs: Optional[Dict[str, Any]], lcls: Optional[Dict[str, Any]]):
-        self.resolver = resolver
-        self.glbs = glbs
-        self.lcls = lcls
-
-        self._args = {arg.arg: arg for arg in self._get_resolver_args()}
-
-    def _get_resolver_args(self):
-        source = inspect.getsource(self.resolver)
-        parsed_source = ast.parse(textwrap.dedent(source))
-        assert len(parsed_source.body) == 1
-        function_def = parsed_source.body[0]
-        assert isinstance(function_def, ast.FunctionDef)
-        args = function_def.args
-        all_args = [*args.posonlyargs, *args.args, *args.kwonlyargs]
-        return all_args
-
-    def parse_annotation(self, name: str):
-        arg = self._args[name]
-        annotation = arg.annotation
-        assert annotation is not None
-        if isinstance(annotation, ast.Constant):
-            val = annotation.value
-            assert isinstance(val, str), "if a literal annotation, it must be a string"
-            # string of type annotation
-            val = ast.parse(val, mode="eval")
-            assert isinstance(val, ast.Module)
-            annotation = val.body
-        if isinstance(annotation, ast.Subscript):
-            # All fancy ast parsing would appear within the subscript of a df __getitem__
-            annotation = ast.Subscript(
-                value=annotation.value,
-                slice=convert_slice(annotation.slice),
-                ctx=annotation.ctx,
-            )
-        return eval_converted_expr(annotation, self.glbs, self.lcls)
+class GlotResult:
+    """Class for editing the sql string, and using sqlglot on sql string"""
 
+    sql_string: str
+    glot: Optional[Expression]
+    args: Dict[str, str]
+    default_args: List[Optional[str]]
+    comment_dict: Optional[CommentDict]
+    docstring: Optional[str]
+    errors: List[ResolverError]
 
-def get_resolver_fqn(function: Callable):
-    return f"{function.__module__}.{function.__name__}"
 
+@dataclasses.dataclass(frozen=True)
+class ParseResult:
+    """Class for important info gathered from glot"""
 
-def get_state_default_value(
-    state_typ: Type[Any],
-    declared_default: Any,
-    parameter_name_for_errors: str,
-    resolver_fqn_for_errors: str,
-) -> Any:
-    if not issubclass(state_typ, BaseModel) and not dataclasses.is_dataclass(state_typ):
-        raise ValueError(
-            f"State value must be a pydantic model or dataclass, "
-            f"but argument '{parameter_name_for_errors}' has type '{type(state_typ).__name__}'"
+    sql_string: str
+    comment_dict: CommentDict
+    fields: Dict[str, str]
+    namespace: str
+    source: Union[BaseSQLSource, StreamSource, None]
+    docstring: Optional[str]
+    errors: List[ResolverError]
+
+
+def get_sql_file_resolvers(
+    sql_file_resolve_location: Path,
+    sources: Sequence[BaseSQLSource],
+) -> Iterable[ResolverResult]:
+    """Iterate through all `.chalk.sql` filepaths, gather the sql strings, and get a resolver hopefully for each."""
+    for dp, dn, fn in os.walk(os.path.expanduser(sql_file_resolve_location)):
+        del dn  # unused
+        for f in fn:
+            filepath = os.path.join(dp, f)
+            if not filepath.endswith(".chalk.sql"):
+                continue
+            sql_string_result = _get_sql_string(filepath)
+            yield get_sql_file_resolver(sources, sql_string_result)
+
+
+def get_sql_file_resolvers_from_paths(
+    sources: Sequence[BaseSQLSource],
+    paths: List[str],
+) -> List[ResolverResult]:
+    return [
+        get_sql_file_resolver(
+            sources=sources,
+            sql_string_result=_get_sql_string(p),
         )
+        for p in paths
+    ]
 
-    default = declared_default
-    if default is inspect.Signature.empty:
+
+def get_sql_file_resolver(sources: Iterable[BaseSQLSource], sql_string_result: SQLStringResult) -> ResolverResult:
+    """Parse the sql strings and get a ResolverResult from each"""
+    if sql_string_result.error:
+        return ResolverResult(resolver=None, errors=[sql_string_result.error], db=None, fields=None, args=None)
+    assert sql_string_result.sql_string is not None
+    path = sql_string_result.path
+
+    errors: List[ResolverError] = []
+    glot_result = _get_sql_glot(sql_string=sql_string_result.sql_string, path=path, sources=sources)
+    if glot_result.errors:
+        return ResolverResult(resolver=None, errors=glot_result.errors, db=None, fields=None, args=None)
+
+    parsed = _parse_glot(glot_result, path, sources)
+    if parsed.errors:
+        return ResolverResult(resolver=None, errors=parsed.errors, db=parsed.source, fields=None, args=None)
+
+    # validate inputs and outputs as real features in graph
+    inputs: List[Feature] = []
+    for arg in glot_result.args.values():
         try:
-            default = state_typ()
+            inputs.append(Feature.from_root_fqn(arg))
         except Exception as e:
-            cls_name = state_typ.__name__
-            raise ValueError(
-                (
-                    "State parameter must have a default value, or be able to be instantiated "
-                    f"with no arguments. For resolver '{resolver_fqn_for_errors}', no default found, and default "
-                    f"construction failed with '{str(e)}'. Assign a default in the resolver's "
-                    f"signature ({parameter_name_for_errors}: {cls_name} = {cls_name}(...)), or assign a default"
-                    f" to each of the fields of '{cls_name}'."
+            errors.append(
+                ResolverError(
+                    display=f"The file '{path}' references an input feature '{arg}' which does not exist",
+                    path=path,
+                    parameter=arg,
+                )
+            )
+    outputs: List[Feature] = []
+    for output in parsed.fields.values():
+        if output.endswith("*"):
+            features = FeatureSetBase.registry[parsed.namespace].features
+            for feature in features:
+                if feature.is_scalar:
+                    outputs.append(feature)
+            continue
+        try:
+            outputs.append(Feature.from_root_fqn(output))
+        except Exception as e:
+            errors.append(
+                ResolverError(
+                    display=f"The file '{path}' references an output feature '{output}' which does not exist",
+                    path=path,
+                    parameter=output,
                 )
             )
 
-    if not isinstance(default, state_typ):
-        raise ValueError(
-            f"Expected type '{state_typ.__name__}' for '{parameter_name_for_errors}', but default has type '{type(default).__name__}'"
-        )
+    resolver_type_str = parsed.comment_dict.type if parsed.comment_dict.type else "online"
+    resolver_type = _RESOLVER_TYPES[resolver_type_str]
 
-    return default
+    if resolver_type == StreamResolver:
+        return _get_stream_resolver(path, glot_result, parsed, outputs)
 
+    incremental_dict = parsed.comment_dict.incremental.dict() if parsed.comment_dict.incremental else None
+    return_one = parsed.comment_dict.count
+    source = parsed.source
+    assert isinstance(source, BaseSQLSource)
+
+    # function for online resolver to process
+    def fn(
+        *input_values: Any,
+        database: BaseSQLSource = source,
+        sql_query: str = parsed.sql_string,
+        field_dict: Dict[str, str] = parsed.fields,
+        args_dict: Dict[str, str] = glot_result.args,
+        incremental: Optional[Dict[str, Any]] = incremental_dict,
+    ):
+        arg_dict = {arg: input_value for input_value, arg in zip(input_values, args_dict.keys())}
+        func = database.query_string(
+            query=sql_query,
+            fields=field_dict,
+            args=arg_dict,
+        )
+        if incremental:
+            func = func.incremental(**incremental)
+        elif return_one in [1, "one"]:
+            func = func.one()
+        elif return_one == "one_or_none":
+            func = func.one_or_none()
+        return func
+
+    if errors:
+        return ResolverResult(
+            resolver=None, errors=errors, db=parsed.source, fields=parsed.fields, args=glot_result.args
+        )
 
-def parse_function(
-    fn: Callable,
-    glbs: Optional[Dict[str, Any]],
-    lcls: Optional[Dict[str, Any]],
-    ignore_return: bool = False,
-) -> ResolverParseResult:
-    fqn = get_resolver_fqn(function=fn)
-    sig = inspect.signature(fn)
-    annotation_parser = ResolverAnnotationParser(fn, glbs, lcls)
+    if return_one:
+        output = Features[tuple(outputs)]
+    else:
+        output = Features[DataFrame[tuple(outputs)]]
 
-    function_definition = inspect.getsource(fn)
-    return_annotation = get_type_hints(fn)["return"]
+    default_args: List[Optional[ResolverArgErrorHandler]] = [
+        ResolverArgErrorHandler(default_value) for default_value in glot_result.default_args
+    ]
+
+    filename = os.path.basename(path)
+    # attempt to instantiate the resolver
+    try:
+        assert resolver_type in (OnlineResolver, OfflineResolver)
+        resolver = resolver_type(
+            filename=path,
+            function_definition=_remove_comments(sql_string_result.sql_string),
+            fqn=filename.replace(".chalk.sql", ""),
+            doc=parsed.docstring,
+            inputs=inputs,
+            output=output,
+            fn=fn,
+            environment=parsed.comment_dict.environment,
+            tags=parsed.comment_dict.tags,
+            max_staleness=parsed.comment_dict.max_staleness,
+            cron=parsed.comment_dict.cron,
+            machine_type=parsed.comment_dict.machine_type,
+            when=None,
+            state=None,
+            default_args=default_args,
+            owner=parsed.comment_dict.owner,
+            timeout=parsed.comment_dict.timeout,
+        )
+    except Exception as e:
+        errors.append(
+            ResolverError(
+                display=f"{resolver_type_str.capitalize()} resolver could not be instantiated, {e}",
+                path=path,
+                parameter=None,
+            )
+        )
+        return ResolverResult(
+            resolver=None, errors=errors, db=parsed.source, fields=parsed.fields, args=glot_result.args
+        )
 
-    ret_val = None
+    return ResolverResult(
+        resolver=resolver, errors=errors, db=parsed.source, fields=parsed.fields, args=glot_result.args
+    )
 
-    if isinstance(return_annotation, FeatureWrapper):
-        return_annotation = return_annotation._chalk_feature
 
-    if isinstance(return_annotation, Feature):
-        assert return_annotation.typ is not None
+def _get_sql_string(path: str) -> SQLStringResult:
+    """Attempt to get a sql string from a filepath and gracefully exit if unable to"""
 
-        if return_annotation.is_has_many:
-            assert issubclass(return_annotation.typ.parsed_annotation, DataFrame)
-            ret_val = Features[return_annotation.typ.parsed_annotation.columns]
-        elif return_annotation.is_has_one:
-            assert issubclass(return_annotation.typ.underlying, Features)
-            ret_val = Features[return_annotation.typ.underlying.features]
+    if not path.endswith(".chalk.sql"):
+        return SQLStringResult.fail(display_error=f"sql resolver file '{path}' must end in '.chalk.sql'", path=path)
+    sql_string = None
+    if os.path.isfile(path):
+        with open(path) as f:
+            sql_string = f.read()
+    else:
+        caller_filename = inspect.stack()[1].filename
+        dir_path = os.path.dirname(os.path.realpath(caller_filename))
+        if isinstance(path, bytes):
+            path = path.decode("utf-8")
+        relative_path = os.path.join(dir_path, path)
+        if os.path.isfile(relative_path):
+            with open(relative_path) as f:
+                sql_string = f.read()
+    if sql_string is None:
+        return SQLStringResult.fail(display_error=f"Cannot find file '{path}'", path=path)
+    return SQLStringResult(path=path, sql_string=sql_string, error=None)
+
+
+def _get_sql_glot(sql_string: str, path: str, sources: Iterable[BaseSQLSource]) -> GlotResult:
+    """Get sqlglot from sql string and gracefully exit if unable to"""
+    try:
+        import sqlglot
+        import sqlglot.expressions
+    except ImportError:
+        raise missing_dependency_exception("chalkpy[runtime]")
+    args = {}  # sql string -> input feature string
+    variables = set(re.findall("\\${.*?\\}", sql_string))
+    errors: List[ResolverError] = []
+    default_args: List[Optional[str]] = []
+    # replace ?{variable_name} with :variable_name for sqlalchemy, and keep track of input args necessary
+    for variable_pattern in variables:
+        has_default_arg = False
+        variable = variable_pattern[2:-1]  # cut off ${ and }
+        for split_var in ["|", " or "]:  # default argument
+            # TODO cannot parse something like {Transaction.category or "Waffles or Pancakes"} yet
+            if split_var in variable:
+                split = variable.split(split_var)
+                if len(split) != 2:
+                    errors.append(
+                        ResolverError(
+                            display=(
+                                f"If character '|' is used, both variable name and default value must be "
+                                f'specified in ({variable}) like \'?{{variable_name | "default_value"}}'
+                            ),
+                            path=path,
+                            parameter=None,
+                        )
+                    )
+                else:  # has default argument
+                    variable = split[0].strip()
+                    default_arg = split[1].strip()
+                    default_arg = json.loads(default_arg)
+                    f = Feature.from_root_fqn(variable)
+                    default_arg = f.converter.from_json_to_rich(default_arg)
+                    default_args.append(default_arg)
+                    has_default_arg = True
+        if not has_default_arg:
+            # TODO default value of None should be refactored since None is a legitimate default value
+            default_args.append(None)
+        period_replaced = variable.replace(".", "_")
+        sql_safe_str = f"__chalk_{period_replaced}__"
+        sql_string = sql_string.replace(variable_pattern, f":{sql_safe_str}")
+        args[sql_safe_str] = variable
+    comments = ""
+    docstring = ""
+    for comment in sql_string.splitlines():
+        if comment.strip().startswith("--"):
+            comment = comment.strip().replace("--", "")
+            if comment.strip().startswith("-"):
+                comments += f"{comment}\n"
+            else:
+                split = comment.split(":")
+                if len(split) != 2:
+                    docstring += f"{comment.strip()}\n"
+                else:
+                    comments += f"{comment}\n"
         else:
-            # function annotated like def get_account_id(user_id: User.id) -> User.account_id
-            ret_val = Features[return_annotation]
+            break
 
-    if ret_val is None:
-        if not isinstance(return_annotation, type):
-            raise TypeError(f"return_annotation {return_annotation} of type {type(return_annotation)} is not a type")
-        if issubclass(return_annotation, Features):
-            # function annotated like def get_account_id(user_id: User.id) -> Features[User.account_id]
-            # or def get_account_id(user_id: User.id) -> User:
-            ret_val = return_annotation
-        elif issubclass(return_annotation, DataFrame):
-            # function annotated like def get_transactions(account_id: Account.id) -> DataFrame[Transaction]
-            ret_val = Features[return_annotation]
-
-    if ret_val is None and not ignore_return:
-        raise ValueError(f"Resolver {fqn} did not have a valid return type")
-
-    inputs = [annotation_parser.parse_annotation(p) for p in sig.parameters.keys()]
-
-    # Unwrap anything that is wrapped with FeatureWrapper
-    inputs = [unwrap_feature(p) if isinstance(p, FeatureWrapper) else p for p in inputs]
-
-    state = None
-    default_args: List[Optional[ResolverArgErrorHandler]] = [None for _ in range(len(inputs))]
-
-    for i, (arg_name, parameter) in enumerate(sig.parameters.items()):
-        bad_input = lambda: ValueError(
-            f"Resolver inputs must be Features or State. Received {str(inputs[i])} for argument '{arg_name}'."
-        )
-        arg = inputs[i]
-
-        if isinstance(arg, GenericAlias) and get_origin(arg) == Union:
-            args = get_args(arg)
-            if len(args) != 2:
-                raise bad_input()
-            if type(None) not in args:
-                raise bad_input()
-            real_arg = next((a for a in args if a is not type(None)), None)
-            if real_arg is None:
-                raise bad_input()
-            default_args[i] = ResolverArgErrorHandler(None)
-            arg = unwrap_feature(real_arg)
-            inputs[i] = arg
-
-        if parameter.empty != parameter.default:
-            default_args[i] = ResolverArgErrorHandler(parameter.default)
+    try:
+        comment_dict: Dict[str, Any] = yaml.safe_load(comments)
+    except Exception as e:
+        errors.append(
+            ResolverError(
+                display=f"Comments key-values '{comments}' must be of YAML form, {e}",
+                path=path,
+                parameter=comments,
+            )
+        )
+        return GlotResult(
+            sql_string=sql_string,
+            glot=None,
+            args=args,
+            default_args=default_args,
+            comment_dict=None,
+            docstring=docstring,
+            errors=errors,
+        )
+    try:
+        comment_dict_object = CommentDict.parse_obj(comment_dict)
+    except ValidationError as e:
+        for error in e.errors():
+            errors.append(
+                ResolverError(
+                    display=f"Could not parse comment(s) '{'.'.join(str(x) for x in error['loc'])}': {error['msg']}",
+                    path=path,
+                    parameter=json.dumps(comment_dict),
+                )
+            )
+        return GlotResult(
+            sql_string=sql_string,
+            glot=None,
+            args=args,
+            default_args=default_args,
+            comment_dict=None,
+            docstring=docstring,
+            errors=errors,
+        )
+    docstring = docstring.strip()
 
-        if not isinstance(arg, (StateWrapper, Feature)):
-            raise bad_input()
+    source_comment = comment_dict_object.source
+    source_type = None
+    if source_comment not in _SOURCES:  # actual name of source
+        for possible_source in sources:
+            if possible_source.name == source_comment:
+                source_type = _DIALECTS_SQLGLOT.get(type(possible_source))  # dialect may be unsupported
+    else:
+        if source_comment in _DIALECTS_SQLGLOT.values():  # source type, if supported
+            source_type = source_comment
+    try:
+        glot = sqlglot.parse_one(sql=sql_string, read=source_type)
+    except Exception as e:
+        errors.append(ResolverError(display=f"Cannot SQL parse {sql_string}, {e}", path=path, parameter=None))
+        return GlotResult(
+            sql_string=sql_string,
+            glot=None,
+            args=args,
+            default_args=default_args,
+            comment_dict=comment_dict_object,
+            docstring=docstring,
+            errors=errors,
+        )
+    if not isinstance(glot, sqlglot.expressions.Select):
+        errors.append(
+            ResolverError(display=f"SQL query {sql_string} should be of 'SELECT' type", path=path, parameter=None)
+        )
+    return GlotResult(
+        sql_string=sql_string,
+        glot=glot,
+        args=args,
+        default_args=default_args,
+        comment_dict=comment_dict_object,
+        docstring=docstring,
+        errors=errors,
+    )
 
-        if not isinstance(arg, StateWrapper):
-            continue
 
-        typ = arg.typ
-        if state is not None:
-            raise ValueError(
-                f"Only one state argument is allowed. Two provided to '{fqn}': '{state.kwarg}' and '{arg_name}'"
+def _parse_glot(glot_result: GlotResult, path: str, sources: Iterable[BaseSQLSource]) -> ParseResult:
+    """Parse useful info from sqlglot and gracefully exit if unable to"""
+    # define a source SQL database. Can either specify name or kind if only one of the kind is present.
+    comment_dict = glot_result.comment_dict
+    assert comment_dict is not None
+    docstring = glot_result.docstring
+    source_name = comment_dict.source
+    source = None
+    errors: List[ResolverError] = []
+    if source_name not in _SOURCES:  # actual name of source
+        for possible_source in sources:
+            if possible_source.name == source_name:
+                source = possible_source
+    else:
+        for possible_source in sources:
+            if isinstance(possible_source, _SOURCES[source_name]):
+                if source:
+                    errors.append(
+                        ResolverError(
+                            display=(
+                                f"More than one {source_name} source exists. Instead, refer to the integration by "
+                                f"name among ({[source.name for source in sources]})."
+                            ),
+                            path=path,
+                            parameter=source_name,
+                        )
+                    )
+                source = possible_source
+    if not source:
+        errors.append(ResolverError(display=f"Source '{source_name}' not found", path=path, parameter=source_name))
+    # get resolver fields: which columns selected will match to which chalk feature?
+    namespace = comment_dict.resolves
+    if namespace not in FeatureSetBase.registry:
+        camelcase_namespace = to_camel_case(namespace)
+        if camelcase_namespace in FeatureSetBase.registry:
+            namespace = camelcase_namespace
+        else:
+            errors.append(
+                ResolverError(
+                    display=f"No @features class with the name '{namespace}'", path=path, parameter=source_name
+                )
             )
+    if errors:
+        return ParseResult(
+            sql_string=glot_result.sql_string,
+            comment_dict=comment_dict,
+            fields={},
+            namespace=namespace,
+            source=source,
+            docstring=docstring,
+            errors=errors,
+        )
 
-        arg_name = parameter.name
-        arg = inputs[i]
-
-        state = StateDescriptor(
-            kwarg=arg_name,
-            pos=i,
-            initial=get_state_default_value(
-                state_typ=arg.typ,
-                resolver_fqn_for_errors=fqn,
-                parameter_name_for_errors=arg_name,
-                declared_default=parameter.default,
-            ),
-            typ=typ,
-        )
-
-    assert ret_val is None or issubclass(ret_val, Features)
-
-    state_index = state.pos if state is not None else None
-    return ResolverParseResult(
-        fqn=fqn,
-        inputs=[v for i, v in enumerate(inputs) if i != state_index],
-        output=ret_val,
-        function_definition=function_definition,
-        function=fn,
-        doc=fn.__doc__,
-        state=state,
-        default_args=default_args,
+    fields: Dict[str, str] = {}  # sql string -> output feature string
+    assert glot_result.glot is not None
+    for column_name in glot_result.glot.named_selects:
+        fields[column_name] = f"{namespace}.{column_name}"
+
+    return ParseResult(
+        sql_string=glot_result.sql_string,
+        comment_dict=comment_dict,
+        fields=fields,
+        namespace=namespace,
+        source=source,
+        docstring=docstring,
+        errors=errors,
     )
 
 
-@overload
-def online(
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    cron: Optional[Union[ScheduleOptions, Cron]] = None,
-    machine_type: Optional[MachineType] = None,
-    when: Optional[Any] = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
-
-
-@overload
-def online(
-    fn: Callable[P, T],
-    /,
-) -> Callable[P, T]:
-    ...
-
-
-def online(
-    fn: Optional[Callable[P, T]] = None,
-    /,
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    cron: Optional[Union[ScheduleOptions, Cron]] = None,
-    machine_type: Optional[MachineType] = None,
-    when: Optional[Any] = None,
-) -> Union[Callable[[Callable[P, T]], Callable[P, T]], Callable[P, T]]:
-    caller_frame = inspect.stack()[1]
-    caller_filename = caller_frame.filename
-    caller_globals = caller_frame.frame.f_globals
-    caller_locals = caller_frame.frame.f_locals
-
-    def decorator(fn: Callable[P, T], cf: str = caller_filename):
-        parsed = parse_function(fn, caller_globals, caller_locals)
-        if not env_var_bool("CHALK_ALLOW_REGISTRY_UPDATES") and parsed.fqn in {s.fqn for s in Resolver.registry}:
-            raise ValueError(f"Duplicate resolver {parsed.fqn}")
-        if parsed.output is None:
-            raise ValueError(f"Online resolvers must return features; '{parsed.fqn}' returns None")
-
-        resolver = OnlineResolver(
-            filename=cf,
-            function_definition=parsed.function_definition,
-            fqn=parsed.fqn,
-            doc=parsed.doc,
-            inputs=parsed.inputs,
-            output=parsed.output,
-            fn=parsed.function,
-            environment=None if environment is None else list(ensure_tuple(environment)),
-            tags=None if tags is None else list(ensure_tuple(tags)),
-            max_staleness=None,
-            cron=cron,
-            machine_type=machine_type,
-            when=when,
-            state=parsed.state,
-            default_args=parsed.default_args,
-        )
-
-        Resolver.registry.append(resolver)
-        Resolver.hook and resolver.hook(resolver)
-
-        # Return the decorated resolver, which notably implements __call__() so it acts the same as
-        # the underlying function if called directly, e.g. from test code
-        return resolver
-
-    return decorator(fn) if fn else decorator
-
-
-@overload
-def offline(
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    cron: Optional[Union[ScheduleOptions, Cron]] = None,
-    machine_type: Optional[MachineType] = None,
-    when: Optional[Any] = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
-
-
-@overload
-def offline(
-    fn: Callable[P, T],
-    /,
-) -> Callable[P, T]:
-    ...
-
-
-def offline(
-    fn: Optional[Callable[P, T]] = None,
-    /,
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    cron: Union[ScheduleOptions, Cron] = None,
-    machine_type: Optional[MachineType] = None,
-    when: Optional[Any] = None,
-) -> Union[Callable[[Callable[P, T]], Callable[P, T]], Callable[P, T]]:
-    caller_frame = inspect.stack()[1]
-    caller_filename = caller_frame.filename
-    caller_globals = caller_frame.frame.f_globals
-    caller_locals = caller_frame.frame.f_locals
-
-    def decorator(fn: Callable[P, T], cf: str = caller_filename):
-        parsed = parse_function(fn, caller_globals, caller_locals)
-        if not env_var_bool("CHALK_ALLOW_REGISTRY_UPDATES") and parsed.fqn in {s.fqn for s in Resolver.registry}:
-            raise ValueError(f"Duplicate resolver {parsed.fqn}")
-        if parsed.output is None:
-            raise ValueError(f"Offline resolvers must return features; '{parsed.fqn}' returns None")
-        resolver = OfflineResolver(
-            filename=cf,
-            function_definition=parsed.function_definition,
-            fqn=parsed.fqn,
-            doc=parsed.doc,
-            inputs=parsed.inputs,
-            output=parsed.output,
-            fn=parsed.function,
-            environment=None if environment is None else list(ensure_tuple(environment)),
-            tags=None if tags is None else list(ensure_tuple(tags)),
-            max_staleness=None,
-            cron=cron,
-            machine_type=machine_type,
-            state=parsed.state,
-            when=when,
-            default_args=parsed.default_args,
-        )
-        Resolver.registry.append(resolver)
-        Resolver.hook and resolver.hook(resolver)
-        return fn
-
-    return decorator(fn) if fn else decorator
-
-
-@overload
-def sink(
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    machine_type: Optional[MachineType] = None,
-    buffer_size: Optional[int] = None,
-    debounce: Optional[Duration] = None,
-    max_delay: Optional[Duration] = None,
-    upsert: Optional[bool] = None,
-    integration: Optional[BaseSQLSourceProtocol] = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
-
-
-@overload
-def sink(
-    fn: Callable[P, T],
-    /,
-) -> Callable[P, T]:
-    ...
-
-
-def sink(
-    fn: Optional[Callable[P, T]] = None,
-    /,
-    *,
-    environment: Optional[Environments] = None,
-    tags: Optional[Tags] = None,
-    machine_type: Optional[MachineType] = None,
-    buffer_size: Optional[int] = None,
-    debounce: Optional[Duration] = None,
-    max_delay: Optional[Duration] = None,
-    upsert: Optional[bool] = None,
-    integration: Optional[BaseSQLSourceProtocol] = None,
-) -> Union[Callable[[Callable[P, T]], Callable[P, T]], Callable[P, T]]:
-    caller_frame = inspect.stack()[1]
-    caller_filename = caller_frame.filename
-    caller_globals = caller_frame.frame.f_globals
-    caller_locals = caller_frame.frame.f_locals
-
-    def decorator(fn: Callable[P, T], cf: str = caller_filename):
-        parsed = parse_function(fn, caller_globals, caller_locals, ignore_return=True)
-        SinkResolver.registry.append(
-            SinkResolver(
-                filename=cf,
-                function_definition=parsed.function_definition,
-                fqn=parsed.fqn,
-                doc=parsed.doc,
-                inputs=parsed.inputs,
-                output=parsed.output,
-                fn=parsed.function,
-                environment=None if environment is None else list(ensure_tuple(environment)),
-                tags=None if tags is None else list(ensure_tuple(tags)),
-                machine_type=machine_type,
-                buffer_size=buffer_size,
-                debounce=debounce,
-                max_delay=max_delay,
-                upsert=upsert,
-                integration=integration,
+def _get_stream_resolver(
+    path: str, glot_result: GlotResult, parsed: ParseResult, outputs: List[Feature]
+) -> ResolverResult:
+    errors = []
+    output_features = Features[DataFrame[tuple(outputs)]]
+
+    if isinstance(output_features.features[0], type) and issubclass(output_features.features[0], DataFrame):
+        output_feature_fqns = set(f.fqn for f in cast(Type[DataFrame], output_features.features[0]).columns)
+    else:
+        output_feature_fqns = set(f.fqn for f in output_features.features)
+
+    signature = StreamResolverSignature(
+        params=[],
+        output_feature_fqns=output_feature_fqns,
+    )
+
+    sql_query: str = _remove_comments(parsed.sql_string)
+    filename = os.path.basename(path)
+    assert isinstance(parsed.source, StreamSource)
+
+    try:
+
+        def fn():
+            return sql_query
+
+        # attempt to instantiate the resolver
+        resolver = StreamResolver(
+            function_definition=sql_query,
+            fqn=filename.replace(".chalk.sql", ""),
+            filename=path,
+            source=parsed.source,
+            fn=fn,
+            environment=parsed.comment_dict.environment,
+            doc=parsed.docstring,
+            module=filename.replace(".chalk.sql", ""),
+            mode=None,
+            machine_type=parsed.comment_dict.machine_type,
+            message=parsed.comment_dict.message,
+            output=output_features,
+            signature=signature,
+            state=None,
+            sql_query=sql_query,
+            owner=parsed.comment_dict.owner,
+            parse=None,
+            keys=None,  # TODO implement parse and keys for sql file resolvers?
+            timestamp=None,
+        )
+    except Exception as e:
+        errors.append(
+            ResolverError(
+                display=f"Streaming resolver could not be instantiated, {e}",
+                path=path,
+                parameter=None,
             )
         )
-        return fn
+        return ResolverResult(resolver=None, errors=errors, db=parsed.source, fields=None, args=None)
+
+    return ResolverResult(
+        resolver=resolver, errors=errors, db=parsed.source, fields=parsed.fields, args=glot_result.args
+    )
+
 
-    return decorator(fn) if fn else decorator
+def _remove_comments(sql_string: str) -> str:
+    sql_string = re.sub(
+        re.compile("/\\*.*?\\*/", re.DOTALL), "", sql_string
+    )  # remove all occurrences streamed comments (/*COMMENT */) from string
+    sql_string = re.sub(
+        re.compile("//.*?\n"), "", sql_string
+    )  # remove all occurrence single-line comments (//COMMENT\n ) from string
+    sql_string = re.sub(
+        re.compile("--.*?\n"), "", sql_string
+    )  # remove all occurrence single-line comments (//COMMENT\n ) from string
+    return sql_string.strip()
```

### Comparing `chalkpy-1.9.9/chalk/gitignore/gitignore_parser.py` & `chalkpy-2.0.0/chalk/gitignore/gitignore_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from __future__ import annotations
 
 # Inlined from https://github.com/mherrmann/gitignore_parser/blob/master/gitignore_parser.py
 import os
 import re
 from os.path import dirname
 from pathlib import Path
-from typing import Callable, List, NamedTuple, Optional, Tuple
+from typing import Callable, List, NamedTuple, Optional, Tuple, Union
 
 
-def _handle_negation(file_path: str, rules: List[IgnoreRule]):
-    matched = False
-    for rule in rules:
-        if rule.match(file_path):
+def _handle_negation(file_path: Union[str, Path], rules: List[IgnoreRule]):
+    for rule in reversed(rules):
+        if rule.match(str(file_path)):
             if rule.negation:
-                matched = False
+                return False
             else:
-                matched = True
-    return matched
+                return True
+    return False
 
 
-def parse_gitignore(full_path: str, base_dir: Optional[str] = None) -> Callable[[str], bool]:
+def parse_gitignore(
+    full_path: Union[str, Path], base_dir: Optional[str] = None
+) -> Tuple[Callable[[Union[str, Path]], bool], bool]:
     if base_dir is None:
         base_dir = dirname(full_path)
-    rules = []
+    rules: List[IgnoreRule] = []
     with open(full_path) as ignore_file:
         counter = 0
         for line in ignore_file:
             counter += 1
             line = line.rstrip("\n")
-            rule = _rule_from_pattern(line, base_path=Path(base_dir).resolve(), source=(full_path, counter))
+            rule = _rule_from_pattern(line, base_path=Path(base_dir).resolve(), source=(str(full_path), counter))
             if rule:
                 rules.append(rule)
-    if not any(r.negation for r in rules):
-        return lambda file_path: any(r.match(file_path) for r in rules)
-    else:
+
+    has_negation = any(r.negation for r in rules)
+    if has_negation:
         # We have negation rules. We can't use a simple "any" to evaluate them.
         # Later rules override earlier rules.
-        return lambda file_path: _handle_negation(file_path, rules)
+        return lambda file_path: _handle_negation(file_path, rules), has_negation
+    else:
+        return lambda file_path: any(r.match(str(file_path)) for r in rules), has_negation
 
 
 def _rule_from_pattern(pattern: str, base_path: Optional[Path] = None, source: Optional[Tuple[str, int]] = None):
     """
     Take a .gitignore match pattern, such as "*.py[cod]" or "**/*.bak",
     and return an IgnoreRule suitable for matching against files and
     directories. Patterns which do not match files, such as comments
@@ -106,15 +109,16 @@
             striptrailingspaces = False
         else:
             if striptrailingspaces:
                 pattern = pattern[:i]
         i = i - 1
     regex = _fnmatch_pathname_to_regex(pattern, directory_only)
     if anchored:
-        regex = "".join(["^", regex])
+        regex = f"^{regex}"
+    regex = f"(?ms){regex}"
     return IgnoreRule(
         pattern=orig_pattern,
         regex=regex,
         negation=negation,
         directory_only=directory_only,
         anchored=anchored,
         base_path=Path(base_path) if base_path else None,
@@ -204,11 +208,13 @@
                 if stuff[0] == "!":
                     stuff = "".join(["^", stuff[1:]])
                 elif stuff[0] == "^":
                     stuff = "".join("\\" + stuff)
                 res.append("[{}]".format(stuff))
         else:
             res.append(re.escape(c))
-    res.insert(0, "(?ms)")
-    if not directory_only:
-        res.append("$")
+    if directory_only:
+        res.append(r"/.*$")
+    else:
+        res.append("(/.*|[^/]*)$")
+
     return "".join(res)
```

### Comparing `chalkpy-1.9.9/chalk/mypy_plugin.py` & `chalkpy-2.0.0/chalk/mypy_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import re
 from typing import Any, Callable, Dict, List, Mapping, Optional, Set, Tuple, Union
 
+from mypy.lookup import lookup_fully_qualified
 from mypy.nodes import (
     ARG_NAMED_OPT,
     ARG_OPT,
     ARG_POS,
     GDEF,
     Argument,
     AssignmentStmt,
     Block,
     CallExpr,
     ClassDef,
     Expression,
     JsonDict,
+    MypyFile,
     NameExpr,
     PlaceholderNode,
     RefExpr,
     SymbolTable,
     SymbolTableNode,
     TypeInfo,
     Var,
 )
 from mypy.plugin import (
     AnalyzeTypeContext,
     ClassDefContext,
     DynamicClassDefContext,
     FunctionContext,
     MethodContext,
-    MypyFile,
     Plugin,
     SemanticAnalyzerPluginInterface,
-    lookup_fully_qualified,
 )
 from mypy.plugins.common import add_method, deserialize_and_fixup_type
 from mypy.types import Instance, NoneType, Type, UnboundType
 
 from chalk.features import DataFrame, Features, feature, features
 from chalk.features.dataframe import DataFrameMeta
 
@@ -266,17 +266,18 @@
         class_name = attr.feature_name.replace(".", "__")
         class_def = ClassDef(class_name, Block([]))
         fullname = ctx.api.qualified_name(class_name)
         class_def.fullname = fullname
 
         attr_info = TypeInfo(SymbolTable(), class_def, ctx.api.cur_mod_id)
         class_def.info = attr_info
-        if not hasattr(attr.type, "type"):
+        attr_type_type = getattr(attr.type, "type", None)
+        if attr_type_type is None:
             continue
-        attr_info.mro = [attr_info, attr.type.type]
+        attr_info.mro = [attr_info, attr_type_type]
         # meta = ctx.api.named_type('chalk.features.FeatureComparisonMeta')
         # attr_info.declared_metaclass = meta
         attr.info = attr_info
         if getattrs(attr, "type.type.declared_metaclass.type.fullname") == PluginKeywords.dataframe_meta:
             PluginKeywords.set_dataframe_cols_metadata(
                 obj=attr_info,
                 cols=[
```

### Comparing `chalkpy-1.9.9/chalk/parsed/user_types_to_json.py` & `chalkpy-2.0.0/chalk/parsed/user_types_to_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,122 @@
 import dataclasses
 import json
 import os
 import re
 import sys
 from pathlib import Path
-from typing import Any, List, Optional
-
-from pydantic import BaseModel
+from typing import List, Optional
 
+from chalk._monitoring.Chart import Chart
+from chalk._monitoring.gql_conversion import convert_chart
 from chalk._version import __version__
-from chalk.config.project_config import ValidationSettings, load_project_config
+from chalk.config.project_config import ProjectSettings, load_project_config
 from chalk.features import FeatureSetBase
-from chalk.features.resolver import Resolver, SinkResolver
+from chalk.features.resolver import Resolver, SinkResolver, StreamResolver
 from chalk.importer import FailedImport
+from chalk.parsed._graph_validation import validate_graph
+from chalk.parsed.duplicate_input_gql import (
+    ChalkPYInfo,
+    EnvironmentSettingsGQL,
+    FeatureSettings,
+    MetadataSettings,
+    ProjectSettingsGQL,
+    UpsertGraphGQL,
+    ValidationSettings,
+)
 from chalk.parsed.json_conversions import convert_type_to_gql
-from chalk.streams._internal import StreamResolver
 from chalk.utils import paths
 
 
 def _is_relative_to(x: Path, other: Path) -> bool:
     try:
         x.relative_to(other)
         return True
     except ValueError:
         return False
 
 
-def _convert_type_to_dict(t: Any) -> dict:
-    return dataclasses.asdict(convert_type_to_gql(t))
+def project_settings_to_gql(config: ProjectSettings) -> ProjectSettingsGQL:
+    def read_packages(filename: str) -> Optional[List[str]]:
+        reqs = list()
+        try:
+            with open(filename) as f:
+                for r in f.readlines():
+                    cleaned = re.sub("#.*", "", r).rstrip("\n").strip()
+                    if cleaned != "":
+                        reqs.append(cleaned)
+            return reqs
+        except OSError:
+            return None
+
+    return ProjectSettingsGQL(
+        project=config.project,
+        environments=None
+        if config.environments is None
+        else [
+            EnvironmentSettingsGQL(
+                id=i,
+                runtime=e.runtime,
+                requirements=e.requirements,
+                dockerfile=e.dockerfile,
+                requiresPackages=None
+                if e.requirements is None
+                else read_packages(
+                    os.path.join(
+                        os.path.dirname(config.local_path),
+                        e.requirements,
+                    )
+                ),
+            )
+            for i, e in config.environments.items()
+        ],
+        validation=ValidationSettings(
+            feature=FeatureSettings(
+                metadata=[MetadataSettings(name=m.name, missing=m.missing) for m in config.validation.feature.metadata]
+                if config.validation.feature.metadata
+                else None
+            )
+            if config.validation.feature
+            else None
+        )
+        if config.validation
+        else None,
+    )
 
 
 def get_registered_types_as_json(scope_to: Path, failed: List[FailedImport], indent: int = 2) -> str:
     features = [
-        _convert_type_to_dict(feature)
+        convert_type_to_gql(feature)
         for x in FeatureSetBase.registry.values()
         if x.__module__ in sys.modules and _is_relative_to(paths.get_classpath(x), scope_to)
         for feature in x.features
-        if not feature.is_autogenerated
+        if not feature.is_autogenerated and not feature.no_display
     ]
     stream_resolvers = [
-        _convert_type_to_dict(t) for t in StreamResolver.registry if _is_relative_to(Path(t.filename), scope_to)
+        convert_type_to_gql(t) for t in StreamResolver.registry if _is_relative_to(Path(t.filename), scope_to)
     ]
-    resolvers = [_convert_type_to_dict(t) for t in Resolver.registry if _is_relative_to(Path(t.filename), scope_to)]
+    resolvers = [convert_type_to_gql(t) for t in Resolver.registry if _is_relative_to(Path(t.filename), scope_to)]
     sink_resolvers = [
-        _convert_type_to_dict(t) for t in SinkResolver.registry if _is_relative_to(Path(t.filename), scope_to)
+        convert_type_to_gql(t) for t in SinkResolver.registry if _is_relative_to(Path(t.filename), scope_to)
     ]
-
-    class EnvironmentSettings(BaseModel):
-        id: str
-        runtime: Optional[str]
-        requirements: Optional[str]
-        requires_packages: Optional[List[str]]
-        dockerfile: Optional[str]
-
-    class ProjectSettings(BaseModel):
-        project: str
-        environments: Optional[List[EnvironmentSettings]]
-        validation: Optional[ValidationSettings]
-
-    def read_packages(filename: str) -> Optional[List[str]]:
-        reqs = list()
-        try:
-            with open(filename) as f:
-                for r in f.readlines():
-                    cleaned = re.sub("#.*", "", r).rstrip("\n").strip()
-                    if cleaned != "":
-                        reqs.append(cleaned)
-            return reqs
-        except OSError:
-            return None
+    charts = [convert_chart(chart) for chart in Chart._registry]
 
     config = load_project_config()
     if config is not None:
-        config = ProjectSettings(
-            project=config.project,
-            environments=config.environments
-            and [
-                EnvironmentSettings(
-                    id=i,
-                    runtime=e.runtime,
-                    requirements=e.requirements,
-                    dockerfile=e.dockerfile,
-                    requires_packages=None
-                    if e.requirements is None
-                    else read_packages(
-                        os.path.join(
-                            os.path.dirname(config.local_path),
-                            e.requirements,
-                        )
-                    ),
-                )
-                for i, e in config.environments.items()
-            ],
-            validation=config.validation,
-        ).dict()
+        config = project_settings_to_gql(config)
 
+    graph = UpsertGraphGQL(
+        streams=stream_resolvers,
+        sinks=sink_resolvers,
+        features=features,
+        config=config,
+        failed=failed,
+        resolvers=resolvers,
+        charts=charts,
+        chalkpy=ChalkPYInfo(version=__version__),
+    )
+    errors = validate_graph(graph)
+    graph.errors = errors
     return json.dumps(
-        dict(
-            streams=stream_resolvers,
-            sinks=sink_resolvers,
-            resolvers=resolvers,
-            features=features,
-            config=config,
-            failed=[d.dict() for d in failed],
-            chalkpy={"version": __version__},
-        ),
+        dataclasses.asdict(graph),
         indent=indent,
     )
```

### Comparing `chalkpy-1.9.9/chalk/serialization/parsed_annotation.py` & `chalkpy-2.0.0/chalk/serialization/parsed_annotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 from __future__ import annotations
 
 import types
-from typing import TYPE_CHECKING, List, Optional, Set, Type, TypeVar, Union, cast, get_args, get_origin, get_type_hints
+import warnings
+from typing import TYPE_CHECKING, FrozenSet, List, Optional, Set, Tuple, Type, TypeVar, Union, cast
 
+from typing_extensions import Annotated, get_args, get_origin
+
+from chalk.utils.cached_type_hints import cached_get_type_hints
 from chalk.utils.collection_type import GenericAlias
 
 if TYPE_CHECKING:
     from chalk.features import Features
+    from chalk.streams import Windowed
 
 T = TypeVar("T")
 U = TypeVar("U")
 JsonValue = TypeVar("JsonValue")
 
 
 class ParsedAnnotation:
     def __init__(
         self,
         features_cls: Optional[Type[Features]] = None,
         attribute_name: Optional[str] = None,
         *,
-        underlying: Optional[type] = None,
+        underlying: Optional[Union[type, Annotated, Windowed]] = None,
     ) -> None:
         # Either pass in the underlying -- if it is already parsed -- or pass in the feature cls and attribute name
         self._features_cls = features_cls
         self._attribute_name = attribute_name
         self._is_nullable: Optional[bool] = None
         self._is_dataframe: Optional[bool] = None
         self._collection_type: Optional[GenericAlias] = None
         self._is_scalar: Optional[bool] = None
+        self._is_feature_time: Optional[bool] = None
+        self._is_primary: Optional[bool] = None
         self._underlying = None
         self._parsed_annotation = None
         if underlying is not None:
             if features_cls is not None and attribute_name is not None:
                 raise ValueError("If specifying the underlying, do not specify (features_cls, attribute_name)")
             self._parse_type(underlying)
         elif features_cls is None or attribute_name is None:
             raise ValueError(
                 "If not specifying the underlying, then both the (features_cls, attribute_name) must be provided"
             )
-        # Store the class and attribute name so we can later use typing.get_type_hints to
+        # Store the class and attribute name to later use typing.get_type_hints to
         # resolve any forward references in the type annotations
         # Resolution happens lazily -- after everything is imported -- to avoid circular imports
 
     @property
     def is_parsed(self) -> bool:
         return self._underlying is not None
 
     @property
-    def annotation(self) -> Union[str, type]:
+    def annotation(self) -> Union[str, type, Windowed, Annotated]:
         """Return the type annotation, without parsing the underlying type if it is not yet already parsed."""
         if self._parsed_annotation is not None:
             # It is already parsed. Return it.
             return self._parsed_annotation
         assert self._features_cls is not None
         assert self._attribute_name is not None
         return self._features_cls.__annotations__[self._attribute_name]
 
     @property
-    def parsed_annotation(self) -> type:
+    def parsed_annotation(self) -> Union[type, Windowed]:
         """The parsed type annotation. It will be parsed if needed.
 
-        Unlike :attr:`underlying`, parsed annotation contains any container or optional types, such as
+        Unlike `.underlying`, parsed annotation contains any container or optional types, such as
         list, dataframe, or Optional.
         """
         if self._parsed_annotation is None:
             self._parse_annotation()
         assert self._parsed_annotation is not None
         return self._parsed_annotation
 
@@ -72,50 +79,84 @@
         if isinstance(self.annotation, type):
             return self.annotation.__name__
         return str(self.annotation)
 
     def _parse_annotation(self):
         assert self._features_cls is not None
         assert self._attribute_name is not None
-        hints = get_type_hints(self._features_cls)
+        hints = cached_get_type_hints(self._features_cls, include_extras=True)
         parsed_annotation = hints[self._attribute_name]
         self._parse_type(parsed_annotation)
 
-    def _parse_type(self, annotation: Optional[type]):
+    def _parse_type(self, annotation: Optional[Union[type, Windowed, Annotated]]):
         from chalk.features import DataFrame, Features
 
         assert self._parsed_annotation is None, "The annotation was already parsed"
         self._parsed_annotation = annotation
-        origin = get_origin(annotation)
+        self._is_document = False
+        self._document_class = None
         self._is_nullable = False
+        self._is_primary = False
+        self._is_feature_time = False
         if self._features_cls is not None and self._attribute_name is not None:
             # Return a more helpful error message, since we have context
             error_ctx = f" {self._features_cls.__name__}.{self._attribute_name}"
         else:
             error_ctx = ""
+        origin = get_origin(annotation)
+        if origin is Annotated:
+            args = get_args(annotation)
+            if "__chalk_ts__" in args:
+                self._is_feature_time = True
+            if "__chalk_primary__" in args:
+                self._is_primary = True
+            if "__chalk_document__" in args:
+                self._is_document = True
+                self._document_class = args[0]
+            annotation = args[0]
+            origin = get_origin(annotation)
+
         if origin in (
             Union,
             getattr(types, "UnionType", Union),
         ):  # using getattr as UnionType was introduced in python 3.10
             args = get_args(annotation)
             # If it's a union, then the only supported union is for nullable features. Validate this
             if len(args) != 2 or (None not in args and type(None) not in args):
                 raise TypeError(
                     f"Invalid annotation for feature{error_ctx}: Unions with non-None types are not allowed"
                 )
             annotation = args[0] if args[1] in (None, type(None)) else args[1]
+            origin = get_origin(annotation)
+            doc_args = get_args(annotation)
+            if self._is_document:
+                self._document_class = annotation
+            if "__chalk_document__" in doc_args:
+                self._is_document = True
+                annotation = doc_args[0]
+                self._document_class = annotation
+                origin = get_origin(annotation)
             self._is_nullable = True
 
         # The only allowed collections here are Set, List, or DataFrame
         if origin in (set, Set):
             args = get_args(annotation)
             assert len(args) == 1, "typing.Set takes just one arg"
             annotation = args[0]
             self._collection_type = Set[cast(Type, annotation)]
-
+        if origin in (frozenset, FrozenSet):
+            args = get_args(annotation)
+            assert len(args) == 1, "typing.FrozenSet takes just one arg"
+            annotation = args[0]
+            self._collection_type = FrozenSet[cast(Type, annotation)]
+        if origin in (tuple, Tuple):
+            args = get_args(annotation)
+            assert len(args) == 2 and args[1] is ..., "typing.Tuple is only supported if it is homogenous"
+            annotation = args[0]
+            self._collection_type = FrozenSet[cast(Type, annotation)]
         if origin in (list, List):
             args = get_args(annotation)
             assert len(args) == 1, "typing.List takes just one arg"
             annotation = args[0]
             self._collection_type = List[cast(Type, annotation)]
 
         self._is_dataframe = False
@@ -145,48 +186,116 @@
             raise TypeError(
                 f"Invalid type annotation for feature{error_ctx}: Dataframes must be of Features types, not {self._parsed_annotation}"
             )
 
         self._underlying = annotation
 
     @property
+    def is_document(self) -> bool:
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._is_document is not None
+        return self._is_document
+
+    @property
+    def document_class(self) -> type:
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        return self._document_class
+
+    @property
     def is_nullable(self) -> bool:
         """Whether the type annotation is nullable."""
         if self._parsed_annotation is None:
             self._parse_annotation()
         assert self._is_nullable is not None
         return self._is_nullable
 
     @property
-    def underlying(self) -> type:
+    def underlying(self) -> Union[type, Windowed]:
         """The underlying type annotation from the annotation."""
+        warnings.warn(
+            DeprecationWarning(
+                "`feature.typ.underlying` is deprecated. For scalar features, use `feature.converter.rich_type`. "
+                "For has-one features, use `feature.joined_class`."
+            )
+        )
         if self.parsed_annotation is None:
             self._parse_annotation()
         if self._underlying is None:
             raise TypeError("There is no underlying type")
         return self._underlying
 
     @underlying.setter
     def underlying(self, underlying: Optional[type]):
         self._underlying = underlying
 
     @property
+    def is_windowed(self) -> bool:
+        from chalk.streams import Windowed
+
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._underlying is not None
+        return isinstance(self._underlying, Windowed)
+
+    @property
+    def is_features_cls(self) -> bool:
+        from chalk.features import Features
+
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._underlying is not None
+        return isinstance(self._underlying, type) and issubclass(self._underlying, Features)
+
+    @property
+    def as_features_cls(self) -> Type[Features]:
+        from chalk.features import Features
+
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._underlying is not None
+        if not (isinstance(self._underlying, type) and issubclass(self._underlying, Features)):
+            raise RuntimeError("The underlying is not a features class")
+        return self._underlying
+
+    @property
     def is_dataframe(self) -> bool:
         """Whether the type annotation is a dataframe."""
         if self._parsed_annotation is None:
             self._parse_annotation()
         assert self._is_dataframe is not None
         return self._is_dataframe
 
     @property
     def collection_type(self) -> Optional[GenericAlias]:
+        warnings.warn(
+            DeprecationWarning(
+                "`feature.typ.collection_type` is deprecated. "
+                "Instead, convert to rich types via `feature.converter.from_XXX_to_rich` is a list"
+            )
+        )
         if self._parsed_annotation is None:
             self._parse_annotation()
         return self._collection_type
 
     @property
     def is_scalar(self) -> bool:
         """Whether the type annotation is a scalar type (i.e. not a Features type)."""
         if self._parsed_annotation is None:
             self._parse_annotation()
         assert self._is_scalar is not None
         return self._is_scalar
+
+    @property
+    def is_primary(self) -> bool:
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._is_primary is not None
+        return self._is_primary
+
+    @property
+    def is_feature_time(self) -> bool:
+        if self._parsed_annotation is None:
+            self._parse_annotation()
+        assert self._is_feature_time is not None
+        return self._is_feature_time
```

### Comparing `chalkpy-1.9.9/chalk/sql/integrations/cloudsql.py` & `chalkpy-2.0.0/chalk/sql/_internal/integrations/cloudsql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,64 @@
+from __future__ import annotations
+
 import os
-from typing import Any, Mapping, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
-from sqlalchemy.engine.url import URL
+from chalk.sql._internal.sql_source import BaseSQLSource
+from chalk.utils.missing_dependency import missing_dependency_exception
 
-from chalk.sql.base.sql_source import BaseSQLSource
+if TYPE_CHECKING:
+    from sqlalchemy.engine.url import URL
 
 
 class CloudSQLSourceImpl(BaseSQLSource):
     def __init__(
         self,
         *,
         instance_name: Optional[str] = None,
         db: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         name: Optional[str] = None,
+        engine_args: Optional[Dict[str, Any]] = None,
     ):
+        try:
+            import psycopg2
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[postgresql]")
+        del psycopg2  # unused
         prefix = name + "_" if name else ""
         self.instance_name = instance_name or os.getenv(prefix + "CLOUDSQL_INSTANCE_NAME")
         self.db = db or os.getenv(prefix + "CLOUDSQL_DATABASE")
         self.user = user or os.getenv(prefix + "CLOUDSQL_USER")
         self.password = password or os.getenv(prefix + "CLOUDSQL_PASSWORD")
-
-        super(CloudSQLSourceImpl, self).__init__()
-
-    def engine_args(self) -> Mapping[str, Any]:
-        return dict(
-            pool_size=20,
-            max_overflow=60,
-            # Trying to fix mysterious dead connection issue
-            connect_args={
+        if engine_args is None:
+            engine_args = {}
+        engine_args.setdefault("pool_size", 20)
+        engine_args.setdefault("max_overflow", 60)
+        engine_args.setdefault(
+            "connect_args",
+            {
                 "keepalives": 1,
                 "keepalives_idle": 30,
                 "keepalives_interval": 10,
                 "keepalives_count": 5,
             },
         )
+        # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
+        # transactions are not needed
+        # Setting the isolation level on the engine, instead of the connection, avoids
+        # a DBAPI statement to reset the transactional level back to the default before returning the
+        # connection to the pool
+        engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+
+    def local_engine_url(self) -> URL:
+        from sqlalchemy.engine.url import URL
 
-    def local_engine_url(self) -> Union[str, URL]:
         return URL.create(
             drivername="postgresql",
             username=self.user,
             password=self.password,
             host="",
             query={"host": "{}/{}/.s.PGSQL.5432".format("/cloudsql", self.instance_name)},
             database=self.db,
```

### Comparing `chalkpy-1.9.9/chalk/sql/integrations/postgres.py` & `chalkpy-2.0.0/chalk/sql/_internal/integrations/mysql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,64 @@
-from typing import Any, Dict, Mapping, Optional, TypeVar, Union
+from __future__ import annotations
 
-from sqlalchemy.engine.url import URL
+import os
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from chalk.integrations.named import load_integration_variable
-from chalk.sql.base.sql_source import BaseSQLSource, TableIngestMixIn
+from chalk.sql._internal.sql_source import BaseSQLSource, TableIngestMixIn
+from chalk.sql.protocols import SQLSourceWithTableIngestProtocol
+from chalk.utils.missing_dependency import missing_dependency_exception
 
-T = TypeVar("T")
+if TYPE_CHECKING:
+    from sqlalchemy.engine.url import URL
 
 
-class PostgreSQLSourceImpl(BaseSQLSource, TableIngestMixIn):
+class MySQLSourceImpl(BaseSQLSource, TableIngestMixIn, SQLSourceWithTableIngestProtocol):
     def __init__(
         self,
         host: Optional[str] = None,
-        port: Optional[str] = None,
+        port: Optional[Union[int, str]] = None,
         db: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         name: Optional[str] = None,
+        engine_args: Optional[Dict[str, Any]] = None,
     ):
-        self.host = host or load_integration_variable(integration_name=name, name="PGHOST")
-        self.port = port or load_integration_variable(integration_name=name, name="PGPORT")
-        self.db = db or load_integration_variable(integration_name=name, name="PGDATABASE")
-        self.user = user or load_integration_variable(integration_name=name, name="PGUSER")
-        self.password = password or load_integration_variable(integration_name=name, name="PGPASSWORD")
+        try:
+            import pymysql
+        except ModuleNotFoundError:
+            raise missing_dependency_exception("chalkpy[mysql]")
+        del pymysql
+        self.name = name
+        self.host = host or load_integration_variable(name="MYSQL_HOST", integration_name=name)
+        self.port = (
+            int(port)
+            if port is not None
+            else load_integration_variable(name="MYSQL_TCP_PORT", integration_name=name, parser=int)
+        )
+        self.db = db or load_integration_variable(name="MYSQL_DATABASE", integration_name=name)
+        self.user = user or load_integration_variable(name="MYSQL_USER", integration_name=name)
+        self.password = password or load_integration_variable(name="MYSQL_PWD", integration_name=name)
         self.ingested_tables: Dict[str, Any] = {}
-        super(PostgreSQLSourceImpl, self).__init__()
+        if engine_args is None:
+            engine_args = {}
+        engine_args.setdefault("pool_size", 20)
+        engine_args.setdefault("max_overflow", 60)
+        # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
+        # transactions are not needed
+        # Setting the isolation level on the engine, instead of the connection, avoids
+        # a DBAPI statement to reset the transactional level back to the default before returning the
+        # connection to the pool
+        engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
 
-    def engine_args(self) -> Mapping[str, Any]:
-        return dict(
-            pool_size=20,
-            max_overflow=60,
-            # Trying to fix mysterious dead connection issue
-            connect_args={
-                "keepalives": 1,
-                "keepalives_idle": 30,
-                "keepalives_interval": 10,
-                "keepalives_count": 5,
-            },
-        )
+    def local_engine_url(self) -> URL:
+        from sqlalchemy.engine.url import URL
 
-    def local_engine_url(self) -> Union[str, URL]:
         return URL.create(
-            drivername="postgresql",
+            drivername="mysql+pymysql",
             username=self.user,
             password=self.password,
             host=self.host,
             port=self.port,
             database=self.db,
         )
```

### Comparing `chalkpy-1.9.9/chalk/streams/_keyed_state.py` & `chalkpy-2.0.0/chalk/state.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Any, Generic, Type, TypeVar, cast
-
-from typing_extensions import TypeAlias
+from typing import Generic, TypeVar, cast
 
 T = TypeVar("T")
-TState = TypeVar("TState", bound="StateImpl")
 
 
-class KeyedStateWrapper(Generic[T]):
-    typ: Type[T]
+class StateWrapper(Generic[T]):
+    typ: T
 
-    def __init__(self, typ: Type[T]):
+    def __init__(self, typ: T):
         self.typ = typ
 
 
-class KeyedStateMeta(type):
-    def __getitem__(cls, item: Type[T]) -> Type[T]:
-        return cast(Type[T], KeyedStateWrapper(item))  # noqa
-
-
-class KeyedStateImpl(metaclass=KeyedStateMeta):
-    def __new__(cls: Type[TState], *args: Any, **kwargs: Any) -> TState:
-        raise RuntimeError("KeyedState should never be instantiated")
-
-
-# Hack to get intellij to not complain about the type of KeyedState[...]
-# This hack is compatible with vscode
-KeyedState: TypeAlias = (lambda: KeyedStateImpl)()
+class StateMeta(type):
+    def __getitem__(cls, item: T) -> T:
+        return cast(T, StateWrapper(item))
+
+
+# We're using this mechanism very intentionally
+# instead of using __getitem__ on a metaclass
+# to allow the editor to auto-complete the
+# members of T. IntelliJ doesn't auto-complete
+# on the return types of metaclass methods.
+# Please check that editors are happy before
+# changing this pattern.
+State = StateMeta("State", (object,), {})
+"""
+Read more at https://docs.chalk.ai/docs/state
+"""
+KeyedState = State
```

### Comparing `chalkpy-1.9.9/chalk/utils/collections.py` & `chalkpy-2.0.0/chalk/utils/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,47 @@
 import collections.abc
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Tuple, TypeVar, Union, cast, overload
 
+from typing_extensions import Annotated, get_args, get_origin
+
+try:
+    from types import UnionType
+except ImportError:
+    UnionType = Union
+
+_NoneType = type(None)
+_AnnotatedType = type(Annotated[int, ""])
+
 T = TypeVar("T")
 
 
+def unwrap_annotated_if_needed(typ: Any):
+    args = get_args(typ)
+    if type(typ) is _AnnotatedType and hasattr(typ, "__metadata__"):
+        return args[0]
+    return typ
+
+
+def unwrap_optional_and_annotated_if_needed(typ: Any):
+    origin = get_origin(typ)
+    args = get_args(typ)
+    typ = unwrap_annotated_if_needed(typ)
+
+    if origin in (Union, UnionType) and len(args) == 2 and any(d == _NoneType for d in args):
+        return next(m for m in get_args(typ) if m != _NoneType)
+
+    return typ
+
+
+def is_namedtuple(value: Any) -> bool:
+    """Infer whether value is a NamedTuple."""
+    # From https://github.com/pola-rs/polars/blob/5f3e332fb2a653064f083b02949c527e0ec0afda/py-polars/polars/internals/construction.py#L78
+    return all(hasattr(value, attr) for attr in ("_fields", "_field_defaults", "_replace"))
+
+
 def flatten(v: Sequence[Union[T, Sequence[Union[T, Sequence[T]]]]]) -> List[T]:
     ret = []
     for x in v:
         if isinstance(x, collections.abc.Sequence) and not isinstance(x, (str, bytes, bytearray)):
             ret.extend(flatten(x))
         else:
             ret.append(x)
@@ -36,19 +70,23 @@
 
 def chunks(lst: Iterable[T], n: int) -> Iterable[Iterable[T]]:
     """Yield successive n-sized chunks from ``lst``, potentially lazily.
 
     Chunks are generated up-front if ``lst`` is a list, tuple, or set. In this case,
     the result will be an iterator of n-sized chunks of the underlying collection type.
 
-    Otherwise, the chunks and the contents of each chunk are generated lazily, where at most one sample from ``lst`` is read in advance.
+    Otherwise, the chunks and the contents of each chunk are generated lazily,
+    where at most one sample from ``lst`` is read in advance.
 
-    Args:
-        lst: The collection
-        n: The chunk size. If <=0, then everything will be yielded back as one chunk.
+    Parameters
+    ----------
+    lst
+        The collection
+    n
+        The chunk size. If <=0, then everything will be yielded back as one chunk.
     """
     if n <= 0:
         yield lst
 
     iterator = iter(lst)
 
     # Greedily loading the next sample to detect if we exhausted the iterable, so we don't yield an empty chunk at the end
@@ -88,36 +126,54 @@
 def ensure_tuple(x: Union[T, Sequence[T], Dict[Any, T], None]) -> Tuple[T, ...]:
     """Converts ``x`` into a tuple.
     * If ``x`` is ``None``, then ``tuple()`` is returned.
     * If ``x`` is a tuple, then ``x`` is returned as-is.
     * If ``x`` is a list, then ``tuple(x)`` is returned.
     * If ``x`` is a dict, then ``tuple(v for v in x.values())`` is returned.
     Otherwise, a single element tuple of ``(x,)`` is returned.
-    Args:
-        x (Any): The input to convert into a tuple.
-    Returns:
-        tuple: A tuple of ``x``.
+
+    Parameters
+    ----------
+    x
+        The input to convert into a tuple.
+
+    Returns
+    -------
+    tuple
+        A tuple of ``x``.
     """
     # From https://github.com/mosaicml/composer/blob/020ca02e3848ee8fb6b7fff0c8123f597b05be8a/composer/utils/iter_helpers.py#L40
     if x is None:
         return ()
     if isinstance(x, (str, bytes, bytearray)):
         return (cast(T, x),)
     if isinstance(x, collections.abc.Sequence):
         return tuple(x)
     if isinstance(x, dict):
         return tuple(x.values())
     return (x,)
 
 
-def get_unique_item(collection: Iterable[Optional[T]], name: str) -> T:
+def get_unique_item(collection: Iterable[Optional[T]], name: Optional[str] = None) -> T:
     item = None
+    in_name = f" in `{name}`" if name is not None else ""
     for x in collection:
         if x is None:
-            raise ValueError(f"Item in {name} is None")
+            raise ValueError(f"Item{in_name} None")
         if item is not None:
             if x != item:
-                raise ValueError(f"Multiple values in {name} are not permitted. Found {x}, {item}")
+                raise ValueError(f"Multiple values{in_name} are not permitted. Found {x}, {item}")
         item = x
     if item is None:
-        raise ValueError(f"There should be at least one item in {name}")
+        raise ValueError(f"There should be at least one item{in_name}")
+    return item
+
+
+def get_unique_item_or_none(iterable: Iterable[Optional[T]]) -> Optional[T]:
+    item = None
+    for x in iterable:
+        if x is None:
+            continue
+        if item is not None:
+            raise ValueError(f"Multiple values not permitted. Found {item}, {x}")
+        item = x
     return item
```

### Comparing `chalkpy-1.9.9/chalk/utils/enum.py` & `chalkpy-2.0.0/chalk/utils/enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import enum
+import functools
 from typing import Type
 
 
+@functools.lru_cache(None)  # Cache all calls to this function
 def get_enum_value_type(enum_cls: Type[enum.Enum]) -> type:
-    """Get the type of the enum value. Requires that all enum member values have the same
-    type; otherwise raises a TypeError.
-    Returns ``None`` if the enum has no members.
+    """Get the type of the enum value.
+    Requires that all enum member values have the same type;
+    otherwise raises a TypeError.
+    Returns `None` if the enum has no members.
 
     Note: if an enum contains both float and int members, then this function will return `float`.
 
-    Args:
-        enum_cls (Type[Enum]): The enum class
-
-    Returns:
+    Parameters
+    ----------
+    enum_cls
+        The enum class
+
+    Returns
+    -------
+    type
         The type of the enum member values.
 
-    Raises:
-        ValueError: If ``enum_cls`` has no members.
-        TypeError: If ``enum_cls`` has members of heterogeneous types, then a TypeError is raised.
+    Raises
+    ------
+    ValueError
+        If `enum_cls` has no members.
+    TypeError
+        If `enum_cls` has members of heterogeneous types, then a TypeError is raised.
     """
     typ = None
     for x in enum_cls:
         if typ is None:
             typ = type(x.value)
             continue
         if issubclass(type(x.value), typ):
```

### Comparing `chalkpy-1.9.9/chalk/utils/metaprogramming.py` & `chalkpy-2.0.0/chalk/utils/metaprogramming.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import builtins
 import types
-from typing import Any, Dict, List, Mapping, Optional, Type
+from typing import Any, Dict, List, Mapping, Optional, Tuple, Type, Union
 
 
 # A sentinel object to detect if a parameter is supplied or not.
 # Use a class to give it a better repr.
 class _MISSING_TYPE:
     def __repr__(self):
         return "<MISSING>"
@@ -42,22 +42,20 @@
     txt = f"def __create_fn__({local_vars}):\n{txt}\n return {name}"
     ns: Mapping[str, Any] = {}
     exec(txt, _globals, ns)
     return ns["__create_fn__"](**_locals)
 
 
 def set_new_attribute(cls: Type, name: str, value: Any):
-    # Never overwrites an existing attribute.  Returns True if the
-    # attribute already exists.
+    # Set an attribute, or raise a ValueError if the attribute is already set
     if name in cls.__dict__:
-        return True
+        raise ValueError(f"Attribute '{name}' is already set")
     if isinstance(value, types.FunctionType):
         value.__qualname__ = f"{cls.__qualname__}.{value.__name__}"
     setattr(cls, name, value)
-    return False
 
 
 def field_assign(name: str, value: str, self_name: str):
     # self_name is what "self" is called in this function: don't
     # hard-code "self", since that might be a field name.
     # Only assigning values that are not "MISSING" so attempting to access
     # a missing value will immediately raise an AttributeError rather than return MISSING
```

### Comparing `chalkpy-1.9.9/chalkpy.egg-info/SOURCES.txt` & `chalkpy-2.0.0/chalkpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-.gitignore
-.pre-commit-config.yaml
-.pre-commit-hooks.yaml
+MANIFEST.in
 README.md
-SECURITY.md
-mypy.ini
 pyproject.toml
-requirements-dev.txt
-requirements.txt
 setup.py
-.github/CODEOWNERS
-.github/dependabot.yml
-.github/ISSUE_TEMPLATE/bug_report.md
-.github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/integration-tests.yml
-.github/workflows/lint.yml
-.github/workflows/release.yml
-.github/workflows/test.yml
 chalk/__init__.py
 chalk/_version.py
 chalk/cli.py
 chalk/importer.py
 chalk/mypy_plugin.py
 chalk/py.typed
 chalk/state.py
+chalk/_autosql/__init__.py
+chalk/_autosql/autosql.py
+chalk/_monitoring/Chart.py
+chalk/_monitoring/__init__.py
+chalk/_monitoring/charts_codegen.py
+chalk/_monitoring/charts_enums_codegen.py
+chalk/_monitoring/charts_series_base.py
+chalk/_monitoring/gql_conversion.py
+chalk/_reporting/__init__.py
+chalk/_reporting/models.py
+chalk/_reporting/progress.py
+chalk/_validation/__init__.py
+chalk/_validation/feature_validation.py
+chalk/_validation/validation.py
 chalk/client/__init__.py
 chalk/client/client_impl.py
-chalk/client/client_protocol.py
+chalk/client/dataset.py
+chalk/client/exc.py
+chalk/client/models.py
 chalk/clogging/__init__.py
 chalk/clogging/chalk_logger.py
 chalk/config/__init__.py
 chalk/config/auth_config.py
 chalk/config/project_config.py
 chalk/df/ChalkDataFrameImpl.py
 chalk/df/__init__.py
@@ -545,113 +547,92 @@
 chalk/feature_n/feature_97/__init__.py
 chalk/feature_n/feature_97/feature.py
 chalk/feature_n/feature_98/__init__.py
 chalk/feature_n/feature_98/feature.py
 chalk/feature_n/feature_99/__init__.py
 chalk/feature_n/feature_99/feature.py
 chalk/features/__init__.py
-chalk/features/dataframe.py
+chalk/features/_chalkop.py
+chalk/features/_class_property.py
+chalk/features/_document.py
 chalk/features/feature_field.py
 chalk/features/feature_set.py
 chalk/features/feature_set_decorator.py
+chalk/features/feature_time.py
 chalk/features/feature_wrapper.py
 chalk/features/filter.py
 chalk/features/hooks.py
+chalk/features/live_updates.py
+chalk/features/primary.py
 chalk/features/pseudofeatures.py
 chalk/features/resolver.py
 chalk/features/tag.py
+chalk/features/_encoding/__init__.py
+chalk/features/_encoding/converter.py
+chalk/features/_encoding/inputs.py
+chalk/features/_encoding/json.py
+chalk/features/_encoding/missing_value.py
+chalk/features/_encoding/primitive.py
+chalk/features/_encoding/pyarrow.py
+chalk/features/_encoding/rich.py
+chalk/features/_encoding/serialized_dtype.py
+chalk/features/dataframe/__init__.py
+chalk/features/dataframe/_filters.py
+chalk/features/dataframe/_impl.py
+chalk/features/dataframe/_validation.py
 chalk/gitignore/__init__.py
 chalk/gitignore/gitignore_parser.py
+chalk/gitignore/helper.py
 chalk/integrations/__init__.py
 chalk/integrations/named.py
+chalk/logging/__init__.py
+chalk/monitoring/__init__.py
 chalk/parsed/__init__.py
+chalk/parsed/_graph_validation.py
 chalk/parsed/duplicate_input_gql.py
 chalk/parsed/json_conversions.py
 chalk/parsed/user_types_to_json.py
 chalk/serialization/__init__.py
-chalk/serialization/codec.py
 chalk/serialization/parsed_annotation.py
+chalk/sink/__init__.py
+chalk/sink/_models.py
 chalk/sql/__init__.py
-chalk/sql/base/__init__.py
-chalk/sql/base/protocols.py
-chalk/sql/base/session.py
-chalk/sql/base/sql_source.py
-chalk/sql/integrations/__init__.py
-chalk/sql/integrations/bigquery.py
-chalk/sql/integrations/chalk_query.py
-chalk/sql/integrations/cloudsql.py
-chalk/sql/integrations/mysql.py
-chalk/sql/integrations/postgres.py
-chalk/sql/integrations/redshift.py
-chalk/sql/integrations/snowflake.py
-chalk/sql/integrations/sqlite.py
-chalk/sql/integrations/string_chalk_query.py
+chalk/sql/finalized_query.py
+chalk/sql/protocols.py
+chalk/sql/_internal/__init__.py
+chalk/sql/_internal/chalk_query.py
+chalk/sql/_internal/incremental.py
+chalk/sql/_internal/sql_file_resolver.py
+chalk/sql/_internal/sql_source.py
+chalk/sql/_internal/string_chalk_query.py
+chalk/sql/_internal/integrations/__init__.py
+chalk/sql/_internal/integrations/bigquery.py
+chalk/sql/_internal/integrations/cloudsql.py
+chalk/sql/_internal/integrations/mysql.py
+chalk/sql/_internal/integrations/postgres.py
+chalk/sql/_internal/integrations/redshift.py
+chalk/sql/_internal/integrations/snowflake.py
+chalk/sql/_internal/integrations/sqlite.py
 chalk/streams/__init__.py
 chalk/streams/_file_source.py
-chalk/streams/_internal.py
 chalk/streams/_kafka_source.py
-chalk/streams/_keyed_state.py
-chalk/streams/_stream.py
-chalk/streams/_types.py
 chalk/streams/_windows.py
+chalk/streams/base.py
+chalk/streams/types.py
 chalk/testing/__init__.py
 chalk/utils/__init__.py
+chalk/utils/annotation_parsing.py
+chalk/utils/cached_type_hints.py
 chalk/utils/collection_type.py
 chalk/utils/collections.py
+chalk/utils/constants.py
 chalk/utils/duration.py
 chalk/utils/enum.py
 chalk/utils/environment_parsing.py
-chalk/utils/json_log_formatter.py
+chalk/utils/json.py
 chalk/utils/log_with_context.py
 chalk/utils/metaprogramming.py
+chalk/utils/missing_dependency.py
+chalk/utils/notebook.py
 chalk/utils/paths.py
-chalk/utils/sqlalchemy.py
 chalk/utils/string.py
-chalk/utils/stubgen.py
-chalkpy.egg-info/PKG-INFO
-chalkpy.egg-info/SOURCES.txt
-chalkpy.egg-info/dependency_links.txt
-chalkpy.egg-info/entry_points.txt
-chalkpy.egg-info/requires.txt
-chalkpy.egg-info/top_level.txt
-tests/__init__.py
-tests/_gitignore/__init__.py
-tests/_gitignore/test_gitignore_parser.py
-tests/client/__init__.py
-tests/client/test_client_serialization.py
-tests/client/test_expand_features.py
-tests/features/__init__.py
-tests/features/test_chained_feature_time.py
-tests/features/test_chained_has_one.py
-tests/features/test_custom_name.py
-tests/features/test_df.py
-tests/features/test_feature_discovery.py
-tests/features/test_features.py
-tests/features/test_hooks.py
-tests/features/test_id_assignment.py
-tests/features/test_iter.py
-tests/features/test_resolver_state.py
-tests/features/test_resolvers_callable.py
-tests/features/test_ts_feature.py
-tests/mypy/__init__.py
-tests/mypy/mypy_docs_demo.py
-tests/mypy/mypy_test.py
-tests/mypy/test_mypy_plugin.py
-tests/parsed/__init__.py
-tests/parsed/test_user_types_to_json.py
-tests/serialization/__init__.py
-tests/serialization/test_codec.py
-tests/sql/__init__.py
-tests/sql/test_implicit_mappings.py
-tests/sql/test_sql_features.py
-tests/sql/test_table_ingest.py
-tests/streams/__init__.py
-tests/streams/test_stream.py
-tests/streams/test_window.py
-tests/utils/__init__.py
-tests/utils/test_collections.py
-tests/utils/test_duration.py
-tests/utils/test_enum.py
-tests/utils/test_log_with_context.py
-tests/utils/test_stubgen.py
-tests/utils/typings/chalk/features/feature_set_decorator.pyi
-typings/chalk/features/feature_set_decorator.pyi
+chalk/utils/stubgen.py
```

