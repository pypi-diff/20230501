# Comparing `tmp/poetry_polylith_plugin-1.6.0.tar.gz` & `tmp/poetry_polylith_plugin-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_polylith_plugin-1.6.0.tar", max compression
+gzip compressed data, was "poetry_polylith_plugin-1.6.1.tar", max compression
```

## Comparing `poetry_polylith_plugin-1.6.0.tar` & `poetry_polylith_plugin-1.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1475 2023-03-26 20:11:55.858371 poetry_polylith_plugin-1.6.0/README.md
--rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.6.0/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      555 2023-02-17 18:12:11.442075 poetry_polylith_plugin-1.6.0/polylith/bricks/base.py
--rw-r--r--   0        0        0     1045 2023-02-20 14:40:39.599185 poetry_polylith_plugin-1.6.0/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1096 2023-03-13 16:15:02.726313 poetry_polylith_plugin-1.6.0/polylith/bricks/component.py
--rw-r--r--   0        0        0       56 2023-02-13 17:04:54.666249 poetry_polylith_plugin-1.6.0/polylith/check/__init__.py
--rw-r--r--   0        0        0     1051 2023-03-05 09:12:59.774422 poetry_polylith_plugin-1.6.0/polylith/check/grouping.py
--rw-r--r--   0        0        0     1756 2023-04-22 15:22:45.897523 poetry_polylith_plugin-1.6.0/polylith/check/report.py
--rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.6.0/polylith/development/__init__.py
--rw-r--r--   0        0        0      211 2022-12-27 08:11:31.407975 poetry_polylith_plugin-1.6.0/polylith/development/development.py
--rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.6.0/polylith/diff/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-16 08:27:58.640337 poetry_polylith_plugin-1.6.0/polylith/diff/collect.py
--rw-r--r--   0        0        0     2670 2023-04-22 15:22:45.898218 poetry_polylith_plugin-1.6.0/polylith/diff/report.py
--rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.6.0/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.6.0/polylith/dirs/dirs.py
--rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.6.0/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.6.0/polylith/files/files.py
--rw-r--r--   0        0        0      151 2023-04-22 15:22:45.913554 poetry_polylith_plugin-1.6.0/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-22 15:22:45.914360 poetry_polylith_plugin-1.6.0/polylith/imports/parser.py
--rw-r--r--   0        0        0      426 2023-03-26 19:47:00.762194 poetry_polylith_plugin-1.6.0/polylith/info/__init__.py
--rw-r--r--   0        0        0     1692 2023-03-26 19:47:00.762913 poetry_polylith_plugin-1.6.0/polylith/info/collect.py
--rw-r--r--   0        0        0     2216 2023-04-22 15:22:45.914914 poetry_polylith_plugin-1.6.0/polylith/info/report.py
--rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.6.0/polylith/interface/__init__.py
--rw-r--r--   0        0        0      876 2023-02-17 18:12:11.443769 poetry_polylith_plugin-1.6.0/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      201 2023-04-22 15:22:45.915728 poetry_polylith_plugin-1.6.0/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-22 15:22:45.916666 poetry_polylith_plugin-1.6.0/polylith/libs/grouping.py
--rw-r--r--   0        0        0     3677 2023-04-22 15:22:45.917187 poetry_polylith_plugin-1.6.0/polylith/libs/report.py
--rw-r--r--   0        0        0     4156 2023-04-16 08:27:58.676339 poetry_polylith_plugin-1.6.0/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      790 2023-04-22 15:22:45.918035 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/__init__.py
--rw-r--r--   0        0        0     2188 2023-03-26 19:47:00.765011 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/check.py
--rw-r--r--   0        0        0      552 2023-02-17 18:12:11.444317 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create.py
--rw-r--r--   0        0        0      634 2023-02-17 18:12:11.444887 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_base.py
--rw-r--r--   0        0        0      674 2023-03-26 12:16:38.669733 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_component.py
--rw-r--r--   0        0        0      680 2023-02-17 18:12:11.446154 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_project.py
--rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_workspace.py
--rw-r--r--   0        0        0     1744 2023-04-16 08:27:58.696930 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/diff.py
--rw-r--r--   0        0        0      876 2023-03-26 13:11:39.932369 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/info.py
--rw-r--r--   0        0        0     2328 2023-03-26 19:47:00.766358 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/libs.py
--rw-r--r--   0        0        0     1676 2023-04-22 15:22:45.936406 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/sync.py
--rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      959 2023-04-22 15:22:45.896775 poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/plugin.py
--rw-r--r--   0        0        0      331 2023-04-22 15:22:45.947457 poetry_polylith_plugin-1.6.0/polylith/project/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-16 08:27:58.716399 poetry_polylith_plugin-1.6.0/polylith/project/create.py
--rw-r--r--   0        0        0     1433 2023-04-22 15:22:45.948301 poetry_polylith_plugin-1.6.0/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-03-26 19:47:00.767617 poetry_polylith_plugin-1.6.0/polylith/project/parser.py
--rw-r--r--   0        0        0      142 2023-02-17 18:12:11.447324 poetry_polylith_plugin-1.6.0/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-16 08:27:58.749480 poetry_polylith_plugin-1.6.0/polylith/readme/readme.py
--rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.6.0/polylith/repo/__init__.py
--rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.6.0/polylith/repo/repo.py
--rw-r--r--   0        0        0       58 2023-04-22 15:22:45.972545 poetry_polylith_plugin-1.6.0/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      172 2023-04-22 15:22:45.973024 poetry_polylith_plugin-1.6.0/polylith/reporting/theme.py
--rw-r--r--   0        0        0      188 2023-04-22 15:22:45.985436 poetry_polylith_plugin-1.6.0/polylith/sync/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-22 15:22:45.985876 poetry_polylith_plugin-1.6.0/polylith/sync/collect.py
--rw-r--r--   0        0        0      794 2023-04-22 15:22:45.986174 poetry_polylith_plugin-1.6.0/polylith/sync/report.py
--rw-r--r--   0        0        0     1787 2023-04-22 15:22:45.986750 poetry_polylith_plugin-1.6.0/polylith/sync/update.py
--rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.6.0/polylith/test/__init__.py
--rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.6.0/polylith/test/tests.py
--rw-r--r--   0        0        0       94 2023-02-19 21:57:26.720321 poetry_polylith_plugin-1.6.0/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1089 2023-02-17 18:12:11.448456 poetry_polylith_plugin-1.6.0/polylith/workspace/create.py
--rw-r--r--   0        0        0     1789 2023-04-16 09:04:04.273168 poetry_polylith_plugin-1.6.0/polylith/workspace/parser.py
--rw-r--r--   0        0        0      949 2023-02-19 21:57:26.720906 poetry_polylith_plugin-1.6.0/polylith/workspace/paths.py
--rw-r--r--   0        0        0      781 2023-04-22 15:23:18.770242 poetry_polylith_plugin-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-03-26 20:11:55.858371 poetry_polylith_plugin-1.6.1/README.md
+-rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.6.1/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      555 2023-02-17 18:12:11.442075 poetry_polylith_plugin-1.6.1/polylith/bricks/base.py
+-rw-r--r--   0        0        0     1045 2023-02-20 14:40:39.599185 poetry_polylith_plugin-1.6.1/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1096 2023-03-13 16:15:02.726313 poetry_polylith_plugin-1.6.1/polylith/bricks/component.py
+-rw-r--r--   0        0        0       56 2023-02-13 17:04:54.666249 poetry_polylith_plugin-1.6.1/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1051 2023-04-25 15:40:24.585711 poetry_polylith_plugin-1.6.1/polylith/check/grouping.py
+-rw-r--r--   0        0        0     1756 2023-04-22 15:22:45.897523 poetry_polylith_plugin-1.6.1/polylith/check/report.py
+-rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.6.1/polylith/development/__init__.py
+-rw-r--r--   0        0        0      211 2022-12-27 08:11:31.407975 poetry_polylith_plugin-1.6.1/polylith/development/development.py
+-rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.6.1/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-16 08:27:58.640337 poetry_polylith_plugin-1.6.1/polylith/diff/collect.py
+-rw-r--r--   0        0        0     2670 2023-04-22 15:22:45.898218 poetry_polylith_plugin-1.6.1/polylith/diff/report.py
+-rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.6.1/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.6.1/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.6.1/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.6.1/polylith/files/files.py
+-rw-r--r--   0        0        0      151 2023-04-22 15:22:45.913554 poetry_polylith_plugin-1.6.1/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1687 2023-04-22 15:22:45.914360 poetry_polylith_plugin-1.6.1/polylith/imports/parser.py
+-rw-r--r--   0        0        0      426 2023-03-26 19:47:00.762194 poetry_polylith_plugin-1.6.1/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1692 2023-03-26 19:47:00.762913 poetry_polylith_plugin-1.6.1/polylith/info/collect.py
+-rw-r--r--   0        0        0     2216 2023-04-22 15:22:45.914914 poetry_polylith_plugin-1.6.1/polylith/info/report.py
+-rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.6.1/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      876 2023-02-17 18:12:11.443769 poetry_polylith_plugin-1.6.1/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      201 2023-04-22 15:22:45.915728 poetry_polylith_plugin-1.6.1/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-22 15:22:45.916666 poetry_polylith_plugin-1.6.1/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     3677 2023-04-22 15:22:45.917187 poetry_polylith_plugin-1.6.1/polylith/libs/report.py
+-rw-r--r--   0        0        0     4156 2023-04-16 08:27:58.676339 poetry_polylith_plugin-1.6.1/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      790 2023-04-22 15:22:45.918035 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/__init__.py
+-rw-r--r--   0        0        0     2188 2023-03-26 19:47:00.765011 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/check.py
+-rw-r--r--   0        0        0      552 2023-02-17 18:12:11.444317 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create.py
+-rw-r--r--   0        0        0      634 2023-02-17 18:12:11.444887 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_base.py
+-rw-r--r--   0        0        0      674 2023-03-26 12:16:38.669733 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_component.py
+-rw-r--r--   0        0        0      680 2023-02-17 18:12:11.446154 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_project.py
+-rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_workspace.py
+-rw-r--r--   0        0        0     1744 2023-04-16 08:27:58.696930 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/diff.py
+-rw-r--r--   0        0        0      876 2023-03-26 13:11:39.932369 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/info.py
+-rw-r--r--   0        0        0     2328 2023-03-26 19:47:00.766358 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/libs.py
+-rw-r--r--   0        0        0     1676 2023-04-25 18:22:56.129900 poetry_polylith_plugin-1.6.1/polylith/poetry/commands/sync.py
+-rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.6.1/polylith/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-22 15:22:45.896775 poetry_polylith_plugin-1.6.1/polylith/poetry_plugin/plugin.py
+-rw-r--r--   0        0        0      331 2023-04-22 15:22:45.947457 poetry_polylith_plugin-1.6.1/polylith/project/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-16 08:27:58.716399 poetry_polylith_plugin-1.6.1/polylith/project/create.py
+-rw-r--r--   0        0        0     1433 2023-04-22 15:22:45.948301 poetry_polylith_plugin-1.6.1/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-03-26 19:47:00.767617 poetry_polylith_plugin-1.6.1/polylith/project/parser.py
+-rw-r--r--   0        0        0      142 2023-02-17 18:12:11.447324 poetry_polylith_plugin-1.6.1/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1067 2023-04-16 08:27:58.749480 poetry_polylith_plugin-1.6.1/polylith/readme/readme.py
+-rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.6.1/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.6.1/polylith/repo/repo.py
+-rw-r--r--   0        0        0       58 2023-04-22 15:22:45.972545 poetry_polylith_plugin-1.6.1/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-22 15:22:45.973024 poetry_polylith_plugin-1.6.1/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      188 2023-04-22 15:22:45.985436 poetry_polylith_plugin-1.6.1/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     2968 2023-05-01 21:26:13.759489 poetry_polylith_plugin-1.6.1/polylith/sync/collect.py
+-rw-r--r--   0        0        0      794 2023-04-22 15:22:45.986174 poetry_polylith_plugin-1.6.1/polylith/sync/report.py
+-rw-r--r--   0        0        0     1787 2023-04-22 15:22:45.986750 poetry_polylith_plugin-1.6.1/polylith/sync/update.py
+-rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.6.1/polylith/test/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.6.1/polylith/test/tests.py
+-rw-r--r--   0        0        0       94 2023-02-19 21:57:26.720321 poetry_polylith_plugin-1.6.1/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1089 2023-02-17 18:12:11.448456 poetry_polylith_plugin-1.6.1/polylith/workspace/create.py
+-rw-r--r--   0        0        0     1832 2023-05-01 21:26:13.760280 poetry_polylith_plugin-1.6.1/polylith/workspace/parser.py
+-rw-r--r--   0        0        0      949 2023-05-01 20:39:23.499711 poetry_polylith_plugin-1.6.1/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      781 2023-05-01 21:26:35.915271 poetry_polylith_plugin-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.6.1/PKG-INFO
```

### Comparing `poetry_polylith_plugin-1.6.0/README.md` & `poetry_polylith_plugin-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/bricks/base.py` & `poetry_polylith_plugin-1.6.1/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/bricks/brick.py` & `poetry_polylith_plugin-1.6.1/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/bricks/component.py` & `poetry_polylith_plugin-1.6.1/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/check/grouping.py` & `poetry_polylith_plugin-1.6.1/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/check/report.py` & `poetry_polylith_plugin-1.6.1/polylith/check/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/diff/collect.py` & `poetry_polylith_plugin-1.6.1/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/diff/report.py` & `poetry_polylith_plugin-1.6.1/polylith/diff/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/imports/parser.py` & `poetry_polylith_plugin-1.6.1/polylith/imports/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/info/collect.py` & `poetry_polylith_plugin-1.6.1/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/info/report.py` & `poetry_polylith_plugin-1.6.1/polylith/info/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/interface/interfaces.py` & `poetry_polylith_plugin-1.6.1/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/libs/grouping.py` & `poetry_polylith_plugin-1.6.1/polylith/libs/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/libs/report.py` & `poetry_polylith_plugin-1.6.1/polylith/libs/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/libs/stdlib.py` & `poetry_polylith_plugin-1.6.1/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/__init__.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/check.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_base.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_component.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_project.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_workspace.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/create_workspace.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/diff.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/diff.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/info.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/info.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/libs.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/libs.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/sync.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry/commands/sync.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/plugin.py` & `poetry_polylith_plugin-1.6.1/polylith/poetry_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/project/create.py` & `poetry_polylith_plugin-1.6.1/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/project/get.py` & `poetry_polylith_plugin-1.6.1/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/readme/readme.py` & `poetry_polylith_plugin-1.6.1/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/repo/repo.py` & `poetry_polylith_plugin-1.6.1/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/sync/report.py` & `poetry_polylith_plugin-1.6.1/polylith/sync/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/sync/update.py` & `poetry_polylith_plugin-1.6.1/polylith/sync/update.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/test/tests.py` & `poetry_polylith_plugin-1.6.1/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/workspace/create.py` & `poetry_polylith_plugin-1.6.1/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/polylith/workspace/parser.py` & `poetry_polylith_plugin-1.6.1/polylith/workspace/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from functools import lru_cache
 from pathlib import Path
 
 import tomlkit
 from polylith import repo
 
 
+@lru_cache
 def _load_workspace_config(path: Path) -> tomlkit.TOMLDocument:
     fullpath = path / repo.workspace_file
 
     content = fullpath.read_text()
 
     return tomlkit.loads(content)
```

### Comparing `poetry_polylith_plugin-1.6.0/polylith/workspace/paths.py` & `poetry_polylith_plugin-1.6.1/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.0/pyproject.toml` & `poetry_polylith_plugin-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-polylith-plugin"
-version = "1.6.0"
+version = "1.6.1"
 description = "A Poetry plugin that adds tooling support for the Polylith Architecture"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 readme = "README.md"
 packages = [
     {include = "polylith"},
```

### Comparing `poetry_polylith_plugin-1.6.0/PKG-INFO` & `poetry_polylith_plugin-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-polylith-plugin
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Poetry plugin that adds tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

