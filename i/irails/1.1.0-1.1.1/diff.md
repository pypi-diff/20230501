# Comparing `tmp/irails-1.1.0.tar.gz` & `tmp/irails-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.0.tar", last modified: Sun Apr 30 10:11:35 2023, max compression
+gzip compressed data, was "irails-1.1.1.tar", last modified: Mon May  1 07:13:47 2023, max compression
```

## Comparing `irails-1.1.0.tar` & `irails-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.805205 irails-1.1.0/
--rw-rw-rw-   0        0        0       39 2023-04-30 09:03:04.000000 irails-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6906 2023-04-30 10:11:35.804212 irails-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6125 2023-04-30 10:11:35.000000 irails-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.759327 irails-1.1.0/irails/
--rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 irails-1.1.0/irails/__init__.py
--rw-rw-rw-   0        0        0      926 2023-04-26 08:44:44.000000 irails-1.1.0/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.0/irails/_utils.py
--rw-rw-rw-   0        0        0    10334 2023-04-23 10:09:38.000000 irails-1.1.0/irails/auth.py
--rw-rw-rw-   0        0        0    10558 2023-04-29 11:22:58.000000 irails-1.1.0/irails/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.0/irails/cbv.py
--rw-rw-rw-   0        0        0     5436 2023-04-30 09:03:04.000000 irails-1.1.0/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.0/irails/controller.py
--rw-rw-rw-   0        0        0    12619 2023-04-27 14:24:00.000000 irails-1.1.0/irails/controller_utils.py
--rw-rw-rw-   0        0        0    13502 2023-04-29 10:39:45.000000 irails-1.1.0/irails/core.py
--rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 irails-1.1.0/irails/database.py
--rw-rw-rw-   0        0        0     6896 2023-04-30 10:10:22.000000 irails-1.1.0/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.0/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.0/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.775284 irails-1.1.0/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.0/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     8345 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6545 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2283 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/_project.py
--rw-rw-rw-   0        0        0      591 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1535 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.736398 irails-1.1.0/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.786256 irails-1.1.0/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.0/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.0/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 irails-1.1.0/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.0/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.0/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.0/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       19 2023-04-28 05:57:01.000000 irails-1.1.0/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.789248 irails-1.1.0/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.0/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.790245 irails-1.1.0/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.0/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.799222 irails-1.1.0/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.0/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.0/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.0/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.0/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.0/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 irails-1.1.0/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.0/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.0/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.803211 irails-1.1.0/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 irails-1.1.0/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 irails-1.1.0/irails/scripts/tpls/project/public/error_500.html
--rw-rw-rw-   0        0        0     1645 2023-04-24 14:18:26.000000 irails-1.1.0/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:35.768311 irails-1.1.0/irails.egg-info/
--rw-rw-rw-   0        0        0     6906 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      767 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-30 10:11:35.000000 irails-1.1.0/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 10:11:35.805205 irails-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2921 2023-04-30 09:03:04.000000 irails-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.186154 irails-1.1.1/
+-rw-rw-rw-   0        0        0       39 2023-04-30 09:03:04.000000 irails-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6901 2023-05-01 07:13:47.185159 irails-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6120 2023-05-01 07:13:46.000000 irails-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.131298 irails-1.1.1/irails/
+-rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 irails-1.1.1/irails/__init__.py
+-rw-rw-rw-   0        0        0     1507 2023-04-30 11:36:07.000000 irails-1.1.1/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.1/irails/_utils.py
+-rw-rw-rw-   0        0        0    11003 2023-04-30 14:40:36.000000 irails-1.1.1/irails/auth.py
+-rw-rw-rw-   0        0        0    10558 2023-05-01 06:23:44.000000 irails-1.1.1/irails/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.1/irails/cbv.py
+-rw-rw-rw-   0        0        0     6367 2023-05-01 04:02:40.000000 irails-1.1.1/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.1/irails/controller.py
+-rw-rw-rw-   0        0        0    12619 2023-04-27 14:24:00.000000 irails-1.1.1/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14294 2023-05-01 04:41:56.000000 irails-1.1.1/irails/core.py
+-rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.1/irails/database.py
+-rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.1/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.1/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.1/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.145260 irails-1.1.1/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.1/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8345 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6545 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2283 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0      591 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1535 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.105585 irails-1.1.1/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.155233 irails-1.1.1/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.1/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.1/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 irails-1.1.1/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.1/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.1/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.1/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       19 2023-04-28 05:57:01.000000 irails-1.1.1/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.157229 irails-1.1.1/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.1/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.158225 irails-1.1.1/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.1/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.167203 irails-1.1.1/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.1/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.1/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.1/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.1/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 irails-1.1.1/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.1/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.172187 irails-1.1.1/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 irails-1.1.1/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 irails-1.1.1/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.174184 irails-1.1.1/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.110572 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.177182 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.180168 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.110572 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.182162 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2073 2023-05-01 07:10:19.000000 irails-1.1.1/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.139277 irails-1.1.1/irails.egg-info/
+-rw-rw-rw-   0        0        0     6901 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2023-05-01 07:13:47.000000 irails-1.1.1/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      767 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:13:47.187148 irails-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2921 2023-05-01 07:13:37.000000 irails-1.1.1/setup.py
```

### Comparing `irails-1.1.0/PKG-INFO` & `irails-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -210,27 +210,27 @@
     <header style="text-align:left;display: flex;">
         <h1>Python</h1>
         <h4>on FastApi</h4>
 
     </header>
     <nav>
         {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
-                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
+        <a href="${routers_map[item]['path']}">${routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+        <a href="/user/logout"><b>${request.session['user']['username']}</b>
                 Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
-        <p>here is the `text` variable in class method:{{text}}</p>
-        <p style="color:red"><b>{{flash}}</b></p>
+        <p>here is the `text` variable in class method:${text}</p>
+        <p style="color:red"><b>${flash}</b></p>
     </section>
     <footer>
         <p>&copy; 2023 My Website</p>
     </footer>
 </body>
 
 </html>
```

### Comparing `irails-1.1.0/README.md` & `irails-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -190,27 +190,27 @@
     <header style="text-align:left;display: flex;">
         <h1>Python</h1>
         <h4>on FastApi</h4>
 
     </header>
     <nav>
         {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
-                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
+        <a href="${routers_map[item]['path']}">${routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+        <a href="/user/logout"><b>${request.session['user']['username']}</b>
                 Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
-        <p>here is the `text` variable in class method:{{text}}</p>
-        <p style="color:red"><b>{{flash}}</b></p>
+        <p>here is the `text` variable in class method:${text}</p>
+        <p style="color:red"><b>${flash}</b></p>
     </section>
     <footer>
         <p>&copy; 2023 My Website</p>
     </footer>
 </body>
 
 </html>
```

### Comparing `irails-1.1.0/irails/_utils.py` & `irails-1.1.1/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/auth.py` & `irails-1.1.1/irails/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import base64
 import binascii
+import importlib
+import os
 
 import casbin
 from casbin.enforcer import Enforcer
  
 from fastapi import FastAPI,Request,Response
 from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials,BaseUser
 from starlette.middleware.authentication import AuthenticationMiddleware
@@ -11,15 +13,15 @@
 from casbin.persist.adapters import FileAdapter
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
  
 from .config import config,_log
 import jwt
 from datetime import datetime, timedelta
-from typing import Optional, Tuple, Union,Dict
+from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 AUTH_EXPIRED='[EXPIRED]!'
 
 _session_name:str = ""
 class AuthenticationBackend_(AuthenticationBackend):
     def create_access_token(self,**kwargs):
         raise NotImplementedError()
@@ -215,33 +217,49 @@
         access_token = jwt.encode(userObj, self.secret_key ,self.algorithm )
         userObj.update({"token":access_token})
         request.session[_session_name] = userObj
         return access_token
     
 _casbin_auth:CasbinAuth = None
 
-def init(app:FastAPI,backend:AuthenticationBackend,adapter:Adapter=None,**kwagrs)->AuthenticationBackend:
+def init(app:FastAPI,backend:AuthenticationBackend,adapter_class:Type=None,**kwagrs)->AuthenticationBackend:
     """
         kwargs:secret_key=KEY
     """
     __session_name = config.get("auth").get("session_name",'user')
     global _casbin_auth
     cfg = config.get("auth")
+    adapter_uri = kwagrs.get('adapter_uri',None)
+    del kwagrs['adapter_uri']
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
-    if not adapter:
-        adapter_file = cfg.get("auth_adapter",'./configs/casbin-adapter.csv') 
-        adapter = FileAdapter(adapter_file)   
+    adapter = adapter_class(adapter_uri)
     enforcer = casbin.Enforcer(model_file, adapter)
     _casbin_auth = CasbinAuth(enforcer=enforcer,session_name=__session_name)
-     
+    
     return backend(**kwagrs) 
 def reload_adapter(app:FastAPI,adapter:Adapter=None):
     cfg = config.get("auth")
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
     if not adapter:
         adapter_file = cfg.get("auth_adapter",'./configs/casbin-adapter.csv')    
         adapter = FileAdapter(adapter_file)   
     enforcer = casbin.Enforcer(model_file, adapter) 
     app.router.current_casbin_instance = enforcer
 
-_auth_types = {'basic':BasicAuth,'jwt':JWTAuthenticationBackend}
-_adapters = {'file':FileAdapter,}
+def get_auth_backend(name:str)->AuthenticationBackend: 
+    _auth_types = {'basic':BasicAuth,'jwt':JWTAuthenticationBackend}
+    return _auth_types[name] if name in  _auth_types else None
+
+def get_adapter_module(name:str)->Adapter:
+    from ._loader import load_module
+    if name.lower()=='file':
+        return FileAdapter
+    module_name= f"{name}_adapter"
+    module_dir = os.path.dirname(__file__)
+    module_dir = os.path.join(module_dir,'casbin_adapters')
+    module_path = os.path.join(module_dir, module_name + '.py') 
+    module = load_module(module_name,module_path)
+    if module and hasattr(module,'Adapter'):
+        return getattr(module,'Adapter')   
+    else:
+        raise RuntimeError("Can't load module:{module_path}")
+
```

### Comparing `irails-1.1.0/irails/base_controller.py` & `irails-1.1.1/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/cbv.py` & `irails-1.1.1/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/config.py` & `irails-1.1.1/irails/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 # from fastapi.logger import logger
 
 import re
  
 
 def is_in_irails(directory):
     """
-    check exists configs dir, apps dir, main.py and configs/general.yaml 
+    check exists configs dir,   main.py and configs/general.yaml 
     """
     
     configs_dir = os.path.join(directory, 'configs')
-    apps_dir = os.path.join(directory, 'apps')
     main_file = os.path.join(directory, 'main.py')
 
-    if not os.path.exists(configs_dir) or not os.path.exists(apps_dir) or not os.path.exists(main_file):
+    if not os.path.exists(configs_dir) or not os.path.exists(main_file):
         return False  
     general_file = os.path.join(configs_dir, 'general.yaml')
 
     if not os.path.exists(general_file):
         return False
     
     return True
@@ -40,26 +39,30 @@
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
         return None
 
 class YamlConfig:
+    _raw_config = {}
     def __init__(self, filename:str="",config:Dict={}):
         self.filename = filename
         self.config = config
         self.load()
     def __getitem__(self,key):
         return self.get(key)
     def load(self):
         if os.path.isfile(self.filename):
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
+                YamlConfig._raw_config = self.config
+
         elif os.path.isdir(self.filename):
             self.config = self._merge_yaml_files(self.filename)
+            YamlConfig._raw_config = self.config
         elif self.config:
             return True
         else:
             if is_cli_mode():
                 pass
             else:
                 raise Exception(f"{self.filename} is not a file or directory")
@@ -69,24 +72,42 @@
     def save(self):
         if not self.filename:
             return False
         with open(self.filename, "w") as f:
             yaml.safe_dump(self.config, f)
         return True
     def get(self, key:str, default=None): 
+        
+        
         value = self.config.get(key, default)
         if isinstance(value,str) and value.find("{")>-1:
-            while value.find("{")>-1 and value.find("}")>-1:
+            while value.find("{")>-1 and value.find("}")>0:
                 name = _extract_name(value)
                 if name:
                     if name==key:
-                        raise RuntimeError(f"circular reference `{name}`")
+                        raise RuntimeError(f"configure file error circular reference `{name}`")
+                    
+                    if name.find(".")>0:
+                        paris = name.split(".")
+                        _root_value = self._raw_config[paris.pop(0)]
+                        _value = _root_value
+                        while paris:
+                            _value = _value[paris.pop(0)]
+                            while _value.find("{")>-1 and value.find("}")>0:
+                                _name = _extract_name(_value)
+                                if _name:
+                                    _expr = _root_value.get(_name,"")
+                                    _x = f"{_name}"
+                                    _value = _value.replace('{'+_x+'}',_expr)
+                        return _value
+                        pass
+                    
                     expr = self.config.get(name,"")
-                    x = f"{name}"
-                    value = value.replace('{'+x+'}',expr)
+                x = f"{name}"
+                value = value.replace('{'+x+'}',expr)
         elif isinstance(value,dict):
             return YamlConfig(filename="",config=value)
         return value
     
     def set(self, key, value):
         self.config[key] = value
 
@@ -123,14 +144,15 @@
 def __init_log(__logCfg):
     if not __logCfg:
         return None
     from fastapi.logger import logger
     __log_level = __logCfg['level'] or 'DEBUG'
     __log_file = __logCfg['file'] or None 
     __isdebug = config.get("debug") or False
+    logger.name = __logCfg.get("name",'iRails')
     if __log_file:
         __log_file = os.path.abspath(__log_file)
     log_format="%(asctime)s %(name)s:%(levelname)s:%(message)s"
     datefmt="%Y-%M-%d %H:%M:%S" 
     if __log_file:
         if __isdebug:
             try:
@@ -143,14 +165,15 @@
         
     else:
         import sys
         handler = logging.StreamHandler(sys.stdout)  
     handler.setLevel(logging._nameToLevel[__log_level]) 
     handler.setFormatter(logging.Formatter(fmt= log_format,datefmt=datefmt)) 
     logger.addHandler(handler)
+    
     logger.setLevel(logging._nameToLevel[__log_level]) 
     return logger
     # return logging.getLogger(__logCfg['name'] or 'FastapiMvcFramework')
 
 config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
 
 _log = __init_log(config.get("log"))
```

### Comparing `irails-1.1.0/irails/controller.py` & `irails-1.1.1/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/controller_utils.py` & `irails-1.1.1/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/core.py` & `irails-1.1.1/irails/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,28 +77,27 @@
     db_uri:str = db_cfg.get("uri")
     alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
     if db_uri:
         if db_uri.startswith('sqlite'):
             db_directory = os.path.dirname(db_uri.split(':///')[1])
             os.makedirs(db_directory, exist_ok=True) 
         application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini,cfg=db_cfg)
+    return db_cfg
 
-def __init_auth(app,auth_type:str):
-    __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
-    casbin_adapter =  auth._adapters[__type_casbin_adapter] if __type_casbin_adapter in auth._adapters else None
-    if not casbin_adapter:
-        raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
+def __init_auth(app,auth_type:str,casbin_adapter_class,__adapter_uri):
     
-    auth_class = auth._auth_types[auth_type] if auth_type in auth._auth_types else None
+    
+    auth_class = auth.get_auth_backend(auth_type)
     if not auth_class:
         raise f"{auth_type} auth type not support"
-    __adapter_uri = config.get("auth").get("adapter_uri",'./configs/casbin-adapter.csv') 
+    
+    
     secret_key = config.get("auth").get(f"{auth_type}_key","")
-    kwargs = {'secret_key':secret_key} 
-    return auth.init(app=app, backend = auth_class,**kwargs)
+    kwargs = {'secret_key':secret_key,'adapter_uri':__adapter_uri} 
+    return auth.init(app=app, backend = auth_class,adapter_class=casbin_adapter_class, **kwargs)
 
 
 def api_router(path:str="", version:str="",**allargs):  
     '''
     :param path :special path format ,ex. '/{controller}/{version}'
     :param version :str like 'v1.0' ,'2.0'..
     '''
@@ -251,24 +250,16 @@
 
 
 def get_wrapped_endpoint(func):
     ret = func
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
-
-def generate_mvc_app( ):
+def _register_controllers():
     global __is_debug
-    _log.disabled = False
-    from ._loader import _load_apps
-    _load_apps()
-    if __is_debug:
-        _log.info("\n\n=================================generating mvc app===========================================")
-    if not len(__all_controller__)>0:
-        raise "must use @api_route to define a controller class"
     all_routers = []
     all_routers_map = {}
     for ctrl in __all_controller__:
         all_routers.append(register_controllers_to_app(application, ctrl))
     for router in all_routers:
         for r in router.routes:
             funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
@@ -276,27 +267,63 @@
             auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
             if __is_debug:  
-                _log.info('{:20}-->{:50}-->{}'.format(str(methods),r.path,funcname) )
+                _log.info((str(methods),r.path,funcname) )
             all_routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
     application.routers_map = all_routers_map  
-    midware.init(app=application,debug=__is_debug)
+def generate_mvc_app( ):
+    global __is_debug
+    _log.disabled = False
+    from ._loader import _load_apps
+    
+    _log.info("\n\init mvc app...")
+    loaded,unloaded=_load_apps(debug=__is_debug) 
+    _log.info(f'Load Apps Completed,{loaded} loaded,{unloaded} unloaded')  
+    if not len(__all_controller__)>0:
+        raise RuntimeError("must use @api_route to define a controller class")
     
+    _register_controllers()
+
+    _log.info("static files mouting...")
+    midware.init(app=application,debug=__is_debug)
+
+    if __is_debug:
+        _log.info("checking database configure...")
+    db_cfg = __init_database()
     auth_type = config.get("auth",None)
+    _casbin_adapter_class=None
+    _adapter_uri:str=None
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
-            application.authObj = __init_auth(application,auth_type)
-    __init_database()
-    if __is_debug:
-        _log.info("=================================generating mvc app end===========================================")
+            __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
+            _casbin_adapter_class =  auth.get_adapter_module(__type_casbin_adapter)
+            _adapter_uri = config.get("auth").get("adapter_uri") 
+            if not _casbin_adapter_class:
+                raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
+            
+    
+    if __is_debug and db_cfg:
+        _log.info("checking database migrations....")
+        try:
+             
+            alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
+            uri = db_cfg.get("uri")
+            database.check_migration(application.data_engine,uri,alembic_ini)
+        except Exception as e:
+            _log.disabled = False
+            _log.error(e.args)
+    if _casbin_adapter_class and _adapter_uri:
+        _log.info("init casbin auth system...")
+        application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
+    _log.info("init mvc app end.")
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug
     host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
     port = "port" in kwargs  and kwargs["port"] or 8000
```

### Comparing `irails-1.1.0/irails/database.py` & `irails-1.1.1/irails/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 def sanitize_path(path):
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
     return sanitized_path
 
-def __check_migration(engine:Engine,uri,alembic_ini): 
+def check_migration(engine:Engine,uri,alembic_ini): 
     def _update_uri_to_ini(): 
         #auto update alembic.ini sqlalchemy.url section 
         config = configparser.ConfigParser() 
         # read ini config
         config.read(alembic_ini)
         config.set('alembic','sqlalchemy.url',uri)
         # save modified ini file
@@ -100,51 +100,46 @@
         reversions_dir = config.get("alembic",'script_location')
         reversions_dir = os.path.join(reversions_dir,"versions")
         if not os.path.exists(reversions_dir):
             os.makedirs(reversions_dir,exist_ok=True)
     Base.metadata.create_all(bind=engine)
     _update_uri_to_ini()
     #  
-    alembic_cfg = Config(alembic_ini)   
-    #  
-    
+    alembic_cfg = Config(alembic_ini)    
     try:
         command.check(config=alembic_cfg)
     except Exception as e: 
         msg = sanitize_path(str(e.args)) 
         command.revision(alembic_cfg, autogenerate=True, message=msg) 
         # upgrade the db
         command.upgrade(alembic_cfg, "head") 
-
+def get_engine():
+    global engine
+    return engine
 def init_database( uri:str,debug:bool=False,alembic_ini:str="",cfg=None):
     '''
     params :uri sqlalchemy connection string
     :params debug mode of debug 
     :params alembic_ini alembic config file path,when debug=True will auto migrate the changes 
     '''
-    global DataMap,mapped_base 
+    global DataMap,mapped_base ,engine
     dbencode = cfg.get('dbencode')
     dbdecode = cfg.get('dbdecode')
-    if ismongo_cloud(uri=uri):
-        from pymongo import MongoClient
-        client = MongoClient(uri)
-        database = client.get_database("<DATABASE>")
-        collection = database.get_collection("<COLLECTION>")
+    # if ismongo_cloud(uri=uri):
+    #     from pymongo import MongoClient
+    #     client = MongoClient(uri)
+    #     database = client.get_database("<DATABASE>")
+    #     collection = database.get_collection("<COLLECTION>")
 
     engine = create_engine(uri,  echo=debug)
     dbfirst = cfg.get("dbfirst")
     maptables = cfg.get("maptables")
     
-    if not dbfirst and debug and alembic_ini:
-        try:
-            #Base.metadata.create_all(engine)
-            __check_migration(engine,uri,alembic_ini)
-        except Exception as e:
-            _log.disabled = False
-            _log.error(e.args)
+    if not dbfirst :
+        pass
     elif dbfirst: 
         def convert_varchar(s): 
             try:
                 return s.encode(dbencode).decode(dbdecode)
             except:
                 return s
```

### Comparing `irails-1.1.0/irails/midware.py` & `irails-1.1.1/irails/midware.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,21 +13,54 @@
 import traceback
 
 from starlette.staticfiles import PathLike
 from .config import _log,config
 from .midware_session import (SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES)
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.types import   Scope 
-from .view import _View
+from .view import _View,env_configs,static_format
 from .config import config
 
 from fastapi.middleware import Middleware
 from starlette.middleware import Middleware as StarletteMiddleware
 from starlette.types import Receive, Scope, Send
- 
+import jinja2
+import chardet
+class MvcStaticFiles(StaticFiles):
+    
+    def file_response(
+        self,
+        full_path: PathLike,
+        stat_result: os.stat_result,
+        scope: Scope,
+        status_code: int = 200,
+    ) -> Response:
+        ext = full_path.split(".")[-1] if full_path.find(".")>-1 else ""
+        if ext and ext in static_format: 
+             
+            context = {"request":Request(scope)}
+            with open(full_path, 'rb') as f:
+                bstr = f.read()
+                result = chardet.detect(bstr) 
+                content = bstr.decode(result['encoding'])
+                 
+            tmp = jinja2.Template(source = content,**env_configs)
+            txt =  tmp.render(context)
+            return Response(txt)
+        else:
+            return super().file_response(
+                full_path,
+                stat_result,
+                scope,
+                status_code=status_code,
+                 
+            )
+
+         
+
 def mount_statics(app,static_paths={},debug=False):
     __roots = {}
     if not static_paths:
         static_paths = app._app_views_dirs
     for _dir  in  static_paths: 
         
         _url:str = static_paths[_dir] 
@@ -37,33 +70,33 @@
         if _url=='/':
             __roots[_dir] = _url
         else:
             if not _url.endswith("/"):_url+="/"
             _url = _url.lower()
             if debug:
                 _log.info(f"StaticDir:{_dir} mounted: {_url}")
-            app.mount(_url,StaticFiles(directory=_dir),name=_dir)       
+            app.mount(_url,MvcStaticFiles(directory=_dir),name=_dir)       
     #mount public resources
     public_dir =  os.path.abspath(config.get("public_dir"))
     if not os.path.exists(public_dir):
         os.makedirs(public_dir) 
-    app.mount('/public/',  StaticFiles(directory=public_dir), name='public') 
+    app.mount('/public/',  MvcStaticFiles(directory=public_dir), name='public') 
     
     if config.get("upload"):
             updir = config.get("upload")['dir'] or "uploads"
     else:
         updir = 'uploads'
 
     if os.path.exists(updir):
         app.mount('/uploads/',  StaticFiles(directory=updir), name='uploads') 
     #root mount must the last
     for _dir in __roots:
         if debug:
             _log.info(f"StaticDir:{_dir} mounted: {__roots[_dir]}")
-        app.mount(__roots[_dir],StaticFiles(directory=_dir),name=_dir)
+        app.mount(__roots[_dir],MvcStaticFiles(directory=_dir),name=_dir)
 def init(app :FastAPI,debug:bool = False): 
     cors_cfg = config.get("cors")
     if cors_cfg:
         app.add_middleware(
         CORSMiddleware,
         allow_origins=cors_cfg.get('allow_origins'),
         allow_credentials=cors_cfg.get("allow_credentials"),
```

### Comparing `irails-1.1.0/irails/midware_casbin.py` & `irails-1.1.1/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/midware_session.py` & `irails-1.1.1/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/_app.py` & `irails-1.1.1/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/_controller.py` & `irails-1.1.1/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/_project.py` & `irails-1.1.1/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/_run.py` & `irails-1.1.1/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/main.py` & `irails-1.1.1/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/app/controller.tpl` & `irails-1.1.1/irails/scripts/tpls/app/controller.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.1/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/app/home.tpl` & `irails-1.1.1/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.1/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.1/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.1/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.1/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.1/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/irails/view.py` & `irails-1.1.1/irails/view.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 import os
 from typing import Any, Mapping
 from fastapi import BackgroundTasks, Request,Response
 from fastapi.templating import Jinja2Templates
 from fastapi.exceptions import HTTPException
 import jinja2 
-from .config import ROOT_PATH
  
+from .config import ROOT_PATH,config
+
+env_configs = {} 
+static_format = []
+def __get_view_configure():
+    global static_format,env_configs
+    env_options = config.get("view")# {'variable_start_string':'${','variable_end_string':'}'}
+    if env_options:
+        static_format = env_options.get('static_format',[])
+        env_options = env_options.get("jinja2")
+        env_configs = env_options.config
+     
+
+__get_view_configure()
+
 class _View(object):
     def __init__(self,request,response=None, tmpl_path:str=f"{os.path.abspath('')}/app/views"):
         self._views_directory = tmpl_path
-        self._templates = Jinja2Templates(directory=self.views_directory)
+        
+        self._templates = Jinja2Templates(directory=self.views_directory,**env_configs)
         self.request = request
         self.response = response
        
     @property
     def templates(self):
         return self._templates
```

### Comparing `irails-1.1.0/irails.egg-info/PKG-INFO` & `irails-1.1.1/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -210,27 +210,27 @@
     <header style="text-align:left;display: flex;">
         <h1>Python</h1>
         <h4>on FastApi</h4>
 
     </header>
     <nav>
         {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
-                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
+        <a href="${routers_map[item]['path']}">${routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+        <a href="/user/logout"><b>${request.session['user']['username']}</b>
                 Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
-        <p>here is the `text` variable in class method:{{text}}</p>
-        <p style="color:red"><b>{{flash}}</b></p>
+        <p>here is the `text` variable in class method:${text}</p>
+        <p style="color:red"><b>${flash}</b></p>
     </section>
     <footer>
         <p>&copy; 2023 My Website</p>
     </footer>
 </body>
 
 </html>
```

### Comparing `irails-1.1.0/irails.egg-info/SOURCES.txt` & `irails-1.1.1/irails.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,8 +44,13 @@
 irails/scripts/tpls/project/configs/cache.yaml
 irails/scripts/tpls/project/configs/casbin-adapter.csv
 irails/scripts/tpls/project/configs/casbin-model.conf
 irails/scripts/tpls/project/configs/database.yaml
 irails/scripts/tpls/project/configs/general.yaml
 irails/scripts/tpls/project/configs/session.yaml
 irails/scripts/tpls/project/public/error_404.html
-irails/scripts/tpls/project/public/error_500.html
+irails/scripts/tpls/project/public/error_500.html
+irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
```

### Comparing `irails-1.1.0/irails.egg-info/requires.txt` & `irails-1.1.1/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.0/setup.py` & `irails-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 import chardet
 
-version = "1.1.0"
+version = "1.1.1"
 def update_readme(source,spec,content=""):
     assert source or content
 
     if not content:
         with open(source, 'r') as file:
             content = file.read()
     with open('README.md', 'r') as file:
```

