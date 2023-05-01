# Comparing `tmp/django-prometheus-2.2.0.dev8.tar.gz` & `tmp/django-prometheus-2.3.0.dev44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-prometheus-2.2.0.dev8.tar", last modified: Wed Dec 30 17:55:28 2020, max compression
+gzip compressed data, was "django-prometheus-2.3.0.dev44.tar", last modified: Mon May  1 19:37:36 2023, max compression
```

## Comparing `django-prometheus-2.2.0.dev8.tar` & `django-prometheus-2.3.0.dev44.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    10598 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7770 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.801124 django-prometheus-2.2.0.dev8/django_prometheus/
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2020-12-30 17:55:07.000000 django-prometheus-2.2.0.dev8/django_prometheus/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      937 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/apps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.801124 django-prometheus-2.2.0.dev8/django_prometheus/cache/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/django_memcached_consul.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      708 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/filebased.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      687 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/locmem.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/memcached.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1160 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/redis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      677 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/cache/metrics.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/conf/
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/conf/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/mysql/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/mysql/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/mysql/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgis/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      705 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgis/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgresql/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgresql/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      824 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgresql/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/sqlite3/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/sqlite3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/backends/sqlite3/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/db/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4766 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/exports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12441 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/middleware.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1911 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/migrations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/django_prometheus/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/tests/test_django_prometheus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1106 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/tests/test_exports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5809 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/tests/test_testutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5909 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/testutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/django_prometheus/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-30 17:55:28.801124 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10598 2020-12-30 17:55:28.000000 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1593 2020-12-30 17:55:28.000000 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-30 17:55:28.000000 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2020-12-30 17:55:28.000000 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-12-30 17:55:28.000000 django-prometheus-2.2.0.dev8/django_prometheus.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-12-30 17:55:28.805124 django-prometheus-2.2.0.dev8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-12-30 17:53:09.000000 django-prometheus-2.2.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:37:36.633759 django-prometheus-2.3.0.dev44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 19:37:26.000000 django-prometheus-2.3.0.dev44/django_prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/django_memcached_consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/filebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/locmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_django_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 19:37:36.633759 django-prometheus-2.3.0.dev44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/setup.py
```

### Comparing `django-prometheus-2.2.0.dev8/LICENSE` & `django-prometheus-2.3.0.dev44/LICENSE`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.2.0.dev8/PKG-INFO` & `django-prometheus-2.3.0.dev44/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,265 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.2.0.dev8
+Version: 2.3.0.dev44
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
-Description: # django-prometheus
-        
-        Export Django monitoring metrics for Prometheus.io
-        
-        [![Join the chat at https://gitter.im/django-prometheus/community](https://badges.gitter.im/django-prometheus/community.svg)](https://gitter.im/django-prometheus/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        
-        [![PyPI version](https://badge.fury.io/py/django-prometheus.svg)](http://badge.fury.io/py/django-prometheus)
-        [![Build Status](https://travis-ci.org/korfuri/django-prometheus.svg?branch=master)](https://travis-ci.org/korfuri/django-prometheus)
-        [![Coverage Status](https://coveralls.io/repos/github/korfuri/django-prometheus/badge.svg?branch=master)](https://coveralls.io/github/korfuri/django-prometheus?branch=master)
-        [![PyPi page link -- Python versions](https://img.shields.io/pypi/pyversions/django-prometheus.svg)](https://pypi.python.org/pypi/django-prometheus)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        ## Features
-        
-        This library provides Prometheus metrics for Django related operations:
-        
-        * Requests & Responses
-        * Database access done via [Django ORM](https://docs.djangoproject.com/en/3.0/topics/db/)
-        * Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.0/topics/cache/)
-        
-        ## Usage
-        
-        ### Requirements
-        
-        * Django >= 2.2
-        
-        ### Installation
-        
-        Install with:
-        
-        ```shell
-        pip install django-prometheus
-        ```
-        
-        Or, if you're using a development version cloned from this repository:
-        
-        ```shell
-        python path-to-where-you-cloned-django-prometheus/setup.py install
-        ```
-        
-        This will install [prometheus_client](https://github.com/prometheus/client_python) as a dependency.
-        
-        ### Quickstart
-        
-        In your settings.py:
-        
-        ```python
-        INSTALLED_APPS = [
-           ...
-           'django_prometheus',
-           ...
-        ]
-        
-        MIDDLEWARE = [
-            'django_prometheus.middleware.PrometheusBeforeMiddleware',
-            # All your other middlewares go here, including the default
-            # middlewares like SessionMiddleware, CommonMiddleware,
-            # CsrfViewmiddleware, SecurityMiddleware, etc.
-            'django_prometheus.middleware.PrometheusAfterMiddleware',
-        ]
-        ```
-        
-        In your urls.py:
-        
-        ```python
-        urlpatterns = [
-            ...
-            url('', include('django_prometheus.urls')),
-        ]
-        ```
-        
-        ### Configuration
-        
-        Prometheus uses Histogram based grouping for monitoring latencies. The default
-        buckets are here: https://github.com/prometheus/client_python/blob/master/prometheus_client/core.py
-        
-        You can define custom buckets for latency, adding more buckets decreases performance but
-        increases accuracy: https://prometheus.io/docs/practices/histograms/
-        
-        ```python
-        PROMETHEUS_LATENCY_BUCKETS = (.1, .2, .5, .6, .8, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.5, 9.0, 12.0, 15.0, 20.0, 30.0, float("inf"))
-        ```
-        
-        ### Monitoring your databases
-        
-        SQLite, MySQL, and PostgreSQL databases can be monitored. Just
-        replace the `ENGINE` property of your database, replacing
-        `django.db.backends` with `django_prometheus.db.backends`.
-        
-        ```python
-        DATABASES = {
-            'default': {
-                'ENGINE': 'django_prometheus.db.backends.sqlite3',
-                'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
-            },
-        }
-        ```
-        
-        ### Monitoring your caches
-        
-        Filebased, memcached, redis caches can be monitored. Just replace
-        the cache backend to use the one provided by django_prometheus
-        `django.core.cache.backends` with `django_prometheus.cache.backends`.
-        
-        ```python
-        CACHES = {
-            'default': {
-                'BACKEND': 'django_prometheus.cache.backends.filebased.FileBasedCache',
-                'LOCATION': '/var/tmp/django_cache',
-            }
-        }
-        ```
-        
-        ### Monitoring your models
-        
-        You may want to monitor the creation/deletion/update rate for your
-        model. This can be done by adding a mixin to them. This is safe to do
-        on existing models (it does not require a migration).
-        
-        If your model is:
-        
-        ```python
-        class Dog(models.Model):
-            name = models.CharField(max_length=100, unique=True)
-            breed = models.CharField(max_length=100, blank=True, null=True)
-            age = models.PositiveIntegerField(blank=True, null=True)
-        ```
-        
-        Just add the `ExportModelOperationsMixin` as such:
-        
-        ```python
-        from django_prometheus.models import ExportModelOperationsMixin
-        
-        class Dog(ExportModelOperationsMixin('dog'), models.Model):
-            name = models.CharField(max_length=100, unique=True)
-            breed = models.CharField(max_length=100, blank=True, null=True)
-            age = models.PositiveIntegerField(blank=True, null=True)
-        ```
-        
-        This will export 3 metrics, `django_model_inserts_total{model="dog"}`,
-        `django_model_updates_total{model="dog"}` and
-        `django_model_deletes_total{model="dog"}`.
-        
-        Note that the exported metrics are counters of creations,
-        modifications and deletions done in the current process. They are not
-        gauges of the number of objects in the model.
-        
-        Starting with Django 1.7, migrations are also monitored. Two gauges
-        are exported, `django_migrations_applied_by_connection` and
-        `django_migrations_unapplied_by_connection`. You may want to alert if
-        there are unapplied migrations.
-        
-        If you want to disable the Django migration metrics, set the
-        `PROMETHEUS_EXPORT_MIGRATIONS` setting to False.
-        
-        ### Monitoring and aggregating the metrics
-        
-        Prometheus is quite easy to set up. An example prometheus.conf to
-        scrape `127.0.0.1:8001` can be found in `examples/prometheus`.
-        
-        Here's an example of a PromDash displaying some of the metrics
-        collected by django-prometheus:
-        
-        ![Example dashboard](https://raw.githubusercontent.com/korfuri/django-prometheus/master/examples/django-promdash.png)
-        
-        ## Adding your own metrics
-        
-        You can add application-level metrics in your code by using
-        [prometheus_client](https://github.com/prometheus/client_python)
-        directly. The exporter is global and will pick up your metrics.
-        
-        To add metrics to the Django internals, the easiest way is to extend
-        django-prometheus' classes. Please consider contributing your metrics,
-        pull requests are welcome. Make sure to read the Prometheus best
-        practices on
-        [instrumentation](http://prometheus.io/docs/practices/instrumentation/)
-        and [naming](http://prometheus.io/docs/practices/naming/).
-        
-        ## Importing Django Prometheus using only local settings
-        
-        If you wish to use Django Prometheus but are not able to change
-        the code base, it's possible to have all the default metrics by
-        modifying only the settings.
-        
-        First step is to inject prometheus' middlewares and to add
-        django_prometheus in INSTALLED_APPS
-        
-        ```python
-        MIDDLEWARE = \
-            ['django_prometheus.middleware.PrometheusBeforeMiddleware'] + \
-            MIDDLEWARE + \
-            ['django_prometheus.middleware.PrometheusAfterMiddleware']
-        
-        INSTALLED_APPS += ['django_prometheus']
-        ```
-        
-        Second step is to create the /metrics end point, for that we need
-        another file (called urls_prometheus_wrapper.py in this example) that
-        will wraps the apps URLs and add one on top:
-        
-        ```python
-        from django.conf.urls import include, url
-        
-        
-        urlpatterns = []
-        
-        urlpatterns.append(url('prometheus/', include('django_prometheus.urls')))
-        urlpatterns.append(url('', include('myapp.urls')))
-        ```
-        
-        This file will add a "/prometheus/metrics" end point to the URLs of django
-        that will export the metrics (replace myapp by your project name).
-        
-        Then we inject the wrapper in settings:
-        
-        ```python
-        ROOT_URLCONF = "graphite.urls_prometheus_wrapper"
-        ```
-        
-        ## Adding custom labels to middleware (request/response) metrics
-        
-        You can add application specific labels to metrics reported by the django-prometheus middleware.
-        This involves extending the classes defined in middleware.py.
-        
-        * Extend the Metrics class and override the `register_metric` method to add the application specific labels.
-        * Extend middleware classes, set the metrics_cls class attribute to the the extended metric class and override the label_metric method to attach custom metrics.
-        
-        See implementation example in [the test app](django_prometheus/tests/end2end/testapp/test_middleware_custom_labels.py#L19-L46)
-        
+Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
+Project-URL: Source, https://github.com/korfuri/django-prometheus
+Project-URL: Tracker, https://github.com/korfuri/django-prometheus/issues
 Keywords: django monitoring prometheus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-prometheus
+
+Export Django monitoring metrics for Prometheus.io
+
+[![Join the chat at https://gitter.im/django-prometheus/community](https://badges.gitter.im/django-prometheus/community.svg)](https://gitter.im/django-prometheus/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+
+[![PyPI version](https://badge.fury.io/py/django-prometheus.svg)](http://badge.fury.io/py/django-prometheus)
+[![Build Status](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/korfuri/django-prometheus/badge.svg?branch=master)](https://coveralls.io/github/korfuri/django-prometheus?branch=master)
+[![PyPi page link -- Python versions](https://img.shields.io/pypi/pyversions/django-prometheus.svg)](https://pypi.python.org/pypi/django-prometheus)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## Features
+
+This library provides Prometheus metrics for Django related operations:
+
+* Requests & Responses
+* Database access done via [Django ORM](https://docs.djangoproject.com/en/3.2/topics/db/)
+* Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.2/topics/cache/)
+
+## Usage
+
+### Requirements
+
+* Django >= 3.2
+* Python 3.7 and above.
+
+### Installation
+
+Install with:
+
+```shell
+pip install django-prometheus
+```
+
+Or, if you're using a development version cloned from this repository:
+
+```shell
+python path-to-where-you-cloned-django-prometheus/setup.py install
+```
+
+This will install [prometheus_client](https://github.com/prometheus/client_python) as a dependency.
+
+### Quickstart
+
+In your settings.py:
+
+```python
+INSTALLED_APPS = [
+   ...
+   'django_prometheus',
+   ...
+]
+
+MIDDLEWARE = [
+    'django_prometheus.middleware.PrometheusBeforeMiddleware',
+    # All your other middlewares go here, including the default
+    # middlewares like SessionMiddleware, CommonMiddleware,
+    # CsrfViewmiddleware, SecurityMiddleware, etc.
+    'django_prometheus.middleware.PrometheusAfterMiddleware',
+]
+```
+
+In your urls.py:
+
+```python
+urlpatterns = [
+    ...
+    path('', include('django_prometheus.urls')),
+]
+```
+
+### Configuration
+
+Prometheus uses Histogram based grouping for monitoring latencies. The default
+buckets are:
+
+```python
+PROMETHEUS_LATENCY_BUCKETS = (0.01, 0.025, 0.05, 0.075, 0.1, 0.25, 0.5, 0.75, 1.0, 2.5, 5.0, 7.5, 10.0, 25.0, 50.0, 75.0, float("inf"),)
+```
+
+You can define custom buckets for latency, adding more buckets decreases performance but
+increases accuracy: <https://prometheus.io/docs/practices/histograms/>
+
+```python
+PROMETHEUS_LATENCY_BUCKETS = (.1, .2, .5, .6, .8, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.5, 9.0, 12.0, 15.0, 20.0, 30.0, float("inf"))
+```
+
+### Monitoring your databases
+
+SQLite, MySQL, and PostgreSQL databases can be monitored. Just
+replace the `ENGINE` property of your database, replacing
+`django.db.backends` with `django_prometheus.db.backends`.
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'django_prometheus.db.backends.sqlite3',
+        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
+    },
+}
+```
+
+### Monitoring your caches
+
+Filebased, memcached, redis caches can be monitored. Just replace
+the cache backend to use the one provided by django_prometheus
+`django.core.cache.backends` with `django_prometheus.cache.backends`.
+
+```python
+CACHES = {
+    'default': {
+        'BACKEND': 'django_prometheus.cache.backends.filebased.FileBasedCache',
+        'LOCATION': '/var/tmp/django_cache',
+    }
+}
+```
+
+### Monitoring your models
+
+You may want to monitor the creation/deletion/update rate for your
+model. This can be done by adding a mixin to them. This is safe to do
+on existing models (it does not require a migration).
+
+If your model is:
+
+```python
+class Dog(models.Model):
+    name = models.CharField(max_length=100, unique=True)
+    breed = models.CharField(max_length=100, blank=True, null=True)
+    age = models.PositiveIntegerField(blank=True, null=True)
+```
+
+Just add the `ExportModelOperationsMixin` as such:
+
+```python
+from django_prometheus.models import ExportModelOperationsMixin
+
+class Dog(ExportModelOperationsMixin('dog'), models.Model):
+    name = models.CharField(max_length=100, unique=True)
+    breed = models.CharField(max_length=100, blank=True, null=True)
+    age = models.PositiveIntegerField(blank=True, null=True)
+```
+
+This will export 3 metrics, `django_model_inserts_total{model="dog"}`,
+`django_model_updates_total{model="dog"}` and
+`django_model_deletes_total{model="dog"}`.
+
+Note that the exported metrics are counters of creations,
+modifications and deletions done in the current process. They are not
+gauges of the number of objects in the model.
+
+Starting with Django 1.7, migrations are also monitored. Two gauges
+are exported, `django_migrations_applied_by_connection` and
+`django_migrations_unapplied_by_connection`. You may want to alert if
+there are unapplied migrations.
+
+If you want to disable the Django migration metrics, set the
+`PROMETHEUS_EXPORT_MIGRATIONS` setting to False.
+
+### Monitoring and aggregating the metrics
+
+Prometheus is quite easy to set up. An example prometheus.conf to
+scrape `127.0.0.1:8001` can be found in `examples/prometheus`.
+
+Here's an example of a PromDash displaying some of the metrics
+collected by django-prometheus:
+
+![Example dashboard](https://raw.githubusercontent.com/korfuri/django-prometheus/master/examples/django-promdash.png)
+
+## Adding your own metrics
+
+You can add application-level metrics in your code by using
+[prometheus_client](https://github.com/prometheus/client_python)
+directly. The exporter is global and will pick up your metrics.
+
+To add metrics to the Django internals, the easiest way is to extend
+django-prometheus' classes. Please consider contributing your metrics,
+pull requests are welcome. Make sure to read the Prometheus best
+practices on
+[instrumentation](http://prometheus.io/docs/practices/instrumentation/)
+and [naming](http://prometheus.io/docs/practices/naming/).
+
+## Importing Django Prometheus using only local settings
+
+If you wish to use Django Prometheus but are not able to change
+the code base, it's possible to have all the default metrics by
+modifying only the settings.
+
+First step is to inject prometheus' middlewares and to add
+django_prometheus in INSTALLED_APPS
+
+```python
+MIDDLEWARE = \
+    ['django_prometheus.middleware.PrometheusBeforeMiddleware'] + \
+    MIDDLEWARE + \
+    ['django_prometheus.middleware.PrometheusAfterMiddleware']
+
+INSTALLED_APPS += ['django_prometheus']
+```
+
+Second step is to create the /metrics end point, for that we need
+another file (called urls_prometheus_wrapper.py in this example) that
+will wraps the apps URLs and add one on top:
+
+```python
+from django.urls import include, path
+
+
+urlpatterns = []
+
+urlpatterns.append(path('prometheus/', include('django_prometheus.urls')))
+urlpatterns.append(path('', include('myapp.urls')))
+```
+
+This file will add a "/prometheus/metrics" end point to the URLs of django
+that will export the metrics (replace myapp by your project name).
+
+Then we inject the wrapper in settings:
+
+```python
+ROOT_URLCONF = "graphite.urls_prometheus_wrapper"
+```
+
+## Adding custom labels to middleware (request/response) metrics
+
+You can add application specific labels to metrics reported by the django-prometheus middleware.
+This involves extending the classes defined in middleware.py.
+
+* Extend the Metrics class and override the `register_metric` method to add the application specific labels.
+* Extend middleware classes, set the metrics_cls class attribute to the the extended metric class and override the label_metric method to attach custom metrics.
+
+See implementation example in [the test app](django_prometheus/tests/end2end/testapp/test_middleware_custom_labels.py#L19-L46)
```

### Comparing `django-prometheus-2.2.0.dev8/README.md` & `django-prometheus-2.3.0.dev44/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # django-prometheus
 
 Export Django monitoring metrics for Prometheus.io
 
 [![Join the chat at https://gitter.im/django-prometheus/community](https://badges.gitter.im/django-prometheus/community.svg)](https://gitter.im/django-prometheus/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [![PyPI version](https://badge.fury.io/py/django-prometheus.svg)](http://badge.fury.io/py/django-prometheus)
-[![Build Status](https://travis-ci.org/korfuri/django-prometheus.svg?branch=master)](https://travis-ci.org/korfuri/django-prometheus)
+[![Build Status](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/korfuri/django-prometheus/badge.svg?branch=master)](https://coveralls.io/github/korfuri/django-prometheus?branch=master)
 [![PyPi page link -- Python versions](https://img.shields.io/pypi/pyversions/django-prometheus.svg)](https://pypi.python.org/pypi/django-prometheus)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Features
 
 This library provides Prometheus metrics for Django related operations:
 
 * Requests & Responses
-* Database access done via [Django ORM](https://docs.djangoproject.com/en/3.0/topics/db/)
-* Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.0/topics/cache/)
+* Database access done via [Django ORM](https://docs.djangoproject.com/en/3.2/topics/db/)
+* Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.2/topics/cache/)
 
 ## Usage
 
 ### Requirements
 
-* Django >= 2.2
+* Django >= 3.2
+* Python 3.7 and above.
 
 ### Installation
 
 Install with:
 
 ```shell
 pip install django-prometheus
@@ -61,25 +62,29 @@
 ```
 
 In your urls.py:
 
 ```python
 urlpatterns = [
     ...
-    url('', include('django_prometheus.urls')),
+    path('', include('django_prometheus.urls')),
 ]
 ```
 
 ### Configuration
 
 Prometheus uses Histogram based grouping for monitoring latencies. The default
-buckets are here: https://github.com/prometheus/client_python/blob/master/prometheus_client/core.py
+buckets are:
+
+```python
+PROMETHEUS_LATENCY_BUCKETS = (0.01, 0.025, 0.05, 0.075, 0.1, 0.25, 0.5, 0.75, 1.0, 2.5, 5.0, 7.5, 10.0, 25.0, 50.0, 75.0, float("inf"),)
+```
 
 You can define custom buckets for latency, adding more buckets decreases performance but
-increases accuracy: https://prometheus.io/docs/practices/histograms/
+increases accuracy: <https://prometheus.io/docs/practices/histograms/>
 
 ```python
 PROMETHEUS_LATENCY_BUCKETS = (.1, .2, .5, .6, .8, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.5, 9.0, 12.0, 15.0, 20.0, 30.0, float("inf"))
 ```
 
 ### Monitoring your databases
 
@@ -195,21 +200,21 @@
 ```
 
 Second step is to create the /metrics end point, for that we need
 another file (called urls_prometheus_wrapper.py in this example) that
 will wraps the apps URLs and add one on top:
 
 ```python
-from django.conf.urls import include, url
+from django.urls import include, path
 
 
 urlpatterns = []
 
-urlpatterns.append(url('prometheus/', include('django_prometheus.urls')))
-urlpatterns.append(url('', include('myapp.urls')))
+urlpatterns.append(path('prometheus/', include('django_prometheus.urls')))
+urlpatterns.append(path('', include('myapp.urls')))
 ```
 
 This file will add a "/prometheus/metrics" end point to the URLs of django
 that will export the metrics (replace myapp by your project name).
 
 Then we inject the wrapper in settings:
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/__init__.py` & `django-prometheus-2.3.0.dev44/django_prometheus/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 # Import all files that define metrics. This has the effect that
 # `import django_prometheus` will always instantiate all metric
 # objects right away.
 from django_prometheus import middleware, models
 
 __all__ = ["middleware", "models", "pip_prometheus"]
 
-__version__ = '2.2.0.dev.8'
+__version__ = "2.3.0.dev44"
+
 
 # Import pip_prometheus to export the pip metrics automatically.
 try:
     import pip_prometheus
 except ImportError:
     # If people don't have pip, don't export anything.
-    pass
-
-default_app_config = "django_prometheus.apps.DjangoPrometheusConfig"
+    pass
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/apps.py` & `django-prometheus-2.3.0.dev44/django_prometheus/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import django_prometheus
 from django.apps import AppConfig
 from django.conf import settings
+
+import django_prometheus
 from django_prometheus.exports import SetupPrometheusExportsFromConfig
 from django_prometheus.migrations import ExportMigrations
 
 
 class DjangoPrometheusConfig(AppConfig):
     name = django_prometheus.__name__
     verbose_name = "Django-Prometheus"
@@ -15,9 +16,9 @@
         Note that this is called even for other management commands
         than `runserver`. As such, it is possible to scrape the
         metrics of a running `manage.py test` or of another command,
         which shouldn't be done for real monitoring (since these jobs
         are usually short-lived), but can be useful for debugging.
         """
         SetupPrometheusExportsFromConfig()
-        if getattr(settings, "PROMETHEUS_EXPORT_MIGRATIONS", True):
+        if getattr(settings, "PROMETHEUS_EXPORT_MIGRATIONS", False):
             ExportMigrations()
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/django_memcached_consul.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/django_memcached_consul.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django_memcached_consul import memcached
+
 from django_prometheus.cache.metrics import (
     django_cache_get_total,
     django_cache_hits_total,
     django_cache_misses_total,
 )
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/filebased.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/locmem.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from django.core.cache.backends import filebased
+from django.core.cache.backends import locmem
+
 from django_prometheus.cache.metrics import (
     django_cache_get_total,
     django_cache_hits_total,
     django_cache_misses_total,
 )
 
 
-class FileBasedCache(filebased.FileBasedCache):
+class LocMemCache(locmem.LocMemCache):
     """Inherit filebased cache to add metrics about hit/miss ratio"""
 
     def get(self, key, default=None, version=None):
-        django_cache_get_total.labels(backend="filebased").inc()
+        django_cache_get_total.labels(backend="locmem").inc()
         cached = super().get(key, default=None, version=version)
         if cached is not None:
-            django_cache_hits_total.labels(backend="filebased").inc()
+            django_cache_hits_total.labels(backend="locmem").inc()
         else:
-            django_cache_misses_total.labels(backend="filebased").inc()
+            django_cache_misses_total.labels(backend="locmem").inc()
         return cached or default
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/locmem.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/memcached.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from django.core.cache.backends import locmem
+from django.core.cache.backends import memcached
+
 from django_prometheus.cache.metrics import (
     django_cache_get_total,
     django_cache_hits_total,
     django_cache_misses_total,
 )
 
 
-class LocMemCache(locmem.LocMemCache):
-    """Inherit filebased cache to add metrics about hit/miss ratio"""
-
+class MemcachedPrometheusCacheMixin:
     def get(self, key, default=None, version=None):
-        django_cache_get_total.labels(backend="locmem").inc()
+        django_cache_get_total.labels(backend="memcached").inc()
         cached = super().get(key, default=None, version=version)
         if cached is not None:
-            django_cache_hits_total.labels(backend="locmem").inc()
+            django_cache_hits_total.labels(backend="memcached").inc()
         else:
-            django_cache_misses_total.labels(backend="locmem").inc()
+            django_cache_misses_total.labels(backend="memcached").inc()
         return cached or default
+
+
+class PyLibMCCache(MemcachedPrometheusCacheMixin, memcached.PyLibMCCache):
+    """Inherit memcached to add metrics about hit/miss ratio"""
+
+    pass
+
+
+class PyMemcacheCache(MemcachedPrometheusCacheMixin, memcached.PyMemcacheCache):
+    """Inherit memcached to add metrics about hit/miss ratio"""
+
+    pass
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/memcached.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/filebased.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from django.core.cache.backends import memcached
+from django.core.cache.backends import filebased
+
 from django_prometheus.cache.metrics import (
     django_cache_get_total,
     django_cache_hits_total,
     django_cache_misses_total,
 )
 
 
-class MemcachedCache(memcached.MemcachedCache):
-    """Inherit memcached to add metrics about hit/miss ratio"""
+class FileBasedCache(filebased.FileBasedCache):
+    """Inherit filebased cache to add metrics about hit/miss ratio"""
 
     def get(self, key, default=None, version=None):
-        django_cache_get_total.labels(backend="memcached").inc()
+        django_cache_get_total.labels(backend="filebased").inc()
         cached = super().get(key, default=None, version=version)
         if cached is not None:
-            django_cache_hits_total.labels(backend="memcached").inc()
+            django_cache_hits_total.labels(backend="filebased").inc()
         else:
-            django_cache_misses_total.labels(backend="memcached").inc()
+            django_cache_misses_total.labels(backend="filebased").inc()
         return cached or default
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/backends/redis.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from django_redis import cache, exceptions
+
 from django_prometheus.cache.metrics import (
     django_cache_get_fail_total,
     django_cache_get_total,
     django_cache_hits_total,
     django_cache_misses_total,
 )
-from django_redis import cache, exceptions
 
 
 class RedisCache(cache.RedisCache):
     """Inherit redis to add metrics about hit/miss/interruption ratio"""
 
     @cache.omit_exception
     def get(self, key, default=None, version=None, client=None):
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/cache/metrics.py` & `django-prometheus-2.3.0.dev44/django_prometheus/cache/metrics.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/db/backends/mysql/base.py` & `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from django.db.backends.mysql import base
+
 from django_prometheus.db.common import DatabaseWrapperMixin, ExportingCursorWrapper
 
 
 class DatabaseFeatures(base.DatabaseFeatures):
     """Our database has the exact same features as the base one."""
 
     pass
 
 
 class DatabaseWrapper(DatabaseWrapperMixin, base.DatabaseWrapper):
     CURSOR_CLASS = base.CursorWrapper
 
     def create_cursor(self, name=None):
         cursor = self.connection.cursor()
-        CursorWrapper = ExportingCursorWrapper(
-            self.CURSOR_CLASS, self.alias, self.vendor
-        )
+        CursorWrapper = ExportingCursorWrapper(self.CURSOR_CLASS, self.alias, self.vendor)
         return CursorWrapper(cursor)
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgis/base.py` & `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import psycopg2.extensions
 from django.contrib.gis.db.backends.postgis import base
+
+from django_prometheus.db.backends.common import get_postgres_cursor_class
 from django_prometheus.db.common import DatabaseWrapperMixin, ExportingCursorWrapper
 
 
 class DatabaseWrapper(DatabaseWrapperMixin, base.DatabaseWrapper):
-    def get_connection_params(self):
-        conn_params = super().get_connection_params()
-        conn_params["cursor_factory"] = ExportingCursorWrapper(
-            psycopg2.extensions.cursor, "postgis", self.vendor
+    def get_new_connection(self, *args, **kwargs):
+        conn = super().get_new_connection(*args, **kwargs)
+        conn.cursor_factory = ExportingCursorWrapper(
+            conn.cursor_factory or get_postgres_cursor_class(), self.alias, self.vendor
         )
-        return conn_params
+        return conn
 
     def create_cursor(self, name=None):
         # cursor_factory is a kwarg to connect() so restore create_cursor()'s
         # default behavior
         return base.DatabaseWrapper.create_cursor(self, name=name)
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/db/backends/postgresql/base.py` & `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import psycopg2.extensions
-from django.db.backends.postgresql import base
-from django_prometheus.db.common import DatabaseWrapperMixin, ExportingCursorWrapper
-
+from django.contrib.gis.db.backends.postgis import base
 
-class DatabaseFeatures(base.DatabaseFeatures):
-    """Our database has the exact same features as the base one."""
-
-    pass
+from django_prometheus.db.backends.common import get_postgres_cursor_class
+from django_prometheus.db.common import DatabaseWrapperMixin, ExportingCursorWrapper
 
 
 class DatabaseWrapper(DatabaseWrapperMixin, base.DatabaseWrapper):
-    def get_connection_params(self):
-        conn_params = super().get_connection_params()
-        conn_params["cursor_factory"] = ExportingCursorWrapper(
-            psycopg2.extensions.cursor, self.alias, self.vendor
+    def get_new_connection(self, *args, **kwargs):
+        conn = super().get_new_connection(*args, **kwargs)
+        conn.cursor_factory = ExportingCursorWrapper(
+            conn.cursor_factory or get_postgres_cursor_class(), "postgis", self.vendor
         )
-        return conn_params
+        return conn
 
     def create_cursor(self, name=None):
         # cursor_factory is a kwarg to connect() so restore create_cursor()'s
         # default behavior
         return base.DatabaseWrapper.create_cursor(self, name=name)
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/db/common.py` & `django-prometheus-2.3.0.dev44/django_prometheus/db/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,38 +44,36 @@
         try:
             return super().get_new_connection(*args, **kwargs)
         except Exception:
             connection_errors_total.labels(self.alias, self.vendor).inc()
             raise
 
     def create_cursor(self, name=None):
-        return self.connection.cursor(
-            factory=ExportingCursorWrapper(self.CURSOR_CLASS, self.alias, self.vendor)
-        )
+        return self.connection.cursor(factory=ExportingCursorWrapper(self.CURSOR_CLASS, self.alias, self.vendor))
 
 
 def ExportingCursorWrapper(cursor_class, alias, vendor):
     """Returns a CursorWrapper class that knows its database's alias and
     vendor name.
     """
 
     labels = {"alias": alias, "vendor": vendor}
 
     class CursorWrapper(cursor_class):
         """Extends the base CursorWrapper to count events."""
 
         def execute(self, *args, **kwargs):
             execute_total.labels(alias, vendor).inc()
-            with query_duration_seconds.labels(**labels).time(), (
-                ExceptionCounterByType(errors_total, extra_labels=labels)
+            with query_duration_seconds.labels(**labels).time(), ExceptionCounterByType(
+                errors_total, extra_labels=labels
             ):
                 return super().execute(*args, **kwargs)
 
         def executemany(self, query, param_list, *args, **kwargs):
             execute_total.labels(alias, vendor).inc(len(param_list))
             execute_many_total.labels(alias, vendor).inc(len(param_list))
-            with query_duration_seconds.labels(**labels).time(), (
-                ExceptionCounterByType(errors_total, extra_labels=labels)
+            with query_duration_seconds.labels(**labels).time(), ExceptionCounterByType(
+                errors_total, extra_labels=labels
             ):
                 return super().executemany(query, param_list, *args, **kwargs)
 
     return CursorWrapper
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/db/metrics.py` & `django-prometheus-2.3.0.dev44/django_prometheus/db/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from prometheus_client import Counter, Histogram
 
-from django_prometheus.conf import NAMESPACE
+from django_prometheus.conf import NAMESPACE, PROMETHEUS_LATENCY_BUCKETS
 
 connections_total = Counter(
     "django_db_new_connections_total",
     "Counter of created connections by database and by vendor.",
     ["alias", "vendor"],
     namespace=NAMESPACE,
 )
@@ -14,18 +14,15 @@
     "Counter of connection failures by database and by vendor.",
     ["alias", "vendor"],
     namespace=NAMESPACE,
 )
 
 execute_total = Counter(
     "django_db_execute_total",
-    (
-        "Counter of executed statements by database and by vendor, including"
-        " bulk executions."
-    ),
+    ("Counter of executed statements by database and by vendor, including" " bulk executions."),
     ["alias", "vendor"],
     namespace=NAMESPACE,
 )
 
 
 execute_many_total = Counter(
     "django_db_execute_many_total",
@@ -42,9 +39,10 @@
     namespace=NAMESPACE,
 )
 
 query_duration_seconds = Histogram(
     "django_db_query_duration_seconds",
     ("Histogram of query duration by database and vendor."),
     ["alias", "vendor"],
+    buckets=PROMETHEUS_LATENCY_BUCKETS,
     namespace=NAMESPACE,
 )
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/exports.py` & `django-prometheus-2.3.0.dev44/django_prometheus/exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import os
 import threading
 
 import prometheus_client
-from prometheus_client import multiprocess
-
 from django.conf import settings
 from django.http import HttpResponse
+from prometheus_client import multiprocess
 
 try:
     # Python 2
     from BaseHTTPServer import HTTPServer
 except ImportError:
     # Python 3
     from http.server import HTTPServer
@@ -90,17 +89,15 @@
             # alias for OSError
             continue  # Try next port
         thread = PrometheusEndpointServer(httpd)
         thread.daemon = True
         thread.start()
         logger.info("Exporting Prometheus /metrics/ on port %s" % port)
         return port  # Stop trying ports at this point
-    logger.warning(
-        "Cannot export Prometheus /metrics/ - " "no available ports in supplied range"
-    )
+    logger.warning("Cannot export Prometheus /metrics/ - " "no available ports in supplied range")
     return None
 
 
 def SetupPrometheusExportsFromConfig():
     """Exports metrics so Prometheus can collect them."""
     port = getattr(settings, "PROMETHEUS_METRICS_EXPORT_PORT", None)
     port_range = getattr(settings, "PROMETHEUS_METRICS_EXPORT_PORT_RANGE", None)
@@ -112,16 +109,14 @@
 
 
 def ExportToDjangoView(request):
     """Exports /metrics as a Django view.
 
     You can use django_prometheus.urls to map /metrics to this view.
     """
-    if "prometheus_multiproc_dir" in os.environ:
+    if "PROMETHEUS_MULTIPROC_DIR" in os.environ or "prometheus_multiproc_dir" in os.environ:
         registry = prometheus_client.CollectorRegistry()
         multiprocess.MultiProcessCollector(registry)
     else:
         registry = prometheus_client.REGISTRY
     metrics_page = prometheus_client.generate_latest(registry)
-    return HttpResponse(
-        metrics_page, content_type=prometheus_client.CONTENT_TYPE_LATEST
-    )
+    return HttpResponse(metrics_page, content_type=prometheus_client.CONTENT_TYPE_LATEST)
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/middleware.py` & `django-prometheus-2.3.0.dev44/django_prometheus/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,13 @@
+from django.utils.deprecation import MiddlewareMixin
 from prometheus_client import Counter, Histogram
 
-from django.conf import settings
-from django.utils.deprecation import MiddlewareMixin
-from django_prometheus.conf import NAMESPACE
+from django_prometheus.conf import NAMESPACE, PROMETHEUS_LATENCY_BUCKETS
 from django_prometheus.utils import PowersOf, Time, TimeSince
 
-DEFAULT_LATENCY_BUCKETS = (
-    0.01,
-    0.025,
-    0.05,
-    0.075,
-    0.1,
-    0.25,
-    0.5,
-    0.75,
-    1.0,
-    2.5,
-    5.0,
-    7.5,
-    10.0,
-    25.0,
-    50.0,
-    75.0,
-    float("inf"),
-)
-
 
 class Metrics:
     _instance = None
 
     @classmethod
     def get_instance(cls):
         if not cls._instance:
@@ -53,18 +32,16 @@
             "django_http_responses_before_middlewares_total",
             "Total count of responses before middlewares run.",
             namespace=NAMESPACE,
         )
         self.requests_latency_before = self.register_metric(
             Histogram,
             "django_http_requests_latency_including_middlewares_seconds",
-            (
-                "Histogram of requests processing time (including middleware "
-                "processing time)."
-            ),
+            ("Histogram of requests processing time (including middleware " "processing time)."),
+            buckets=PROMETHEUS_LATENCY_BUCKETS,
             namespace=NAMESPACE,
         )
         self.requests_unknown_latency_before = self.register_metric(
             Counter,
             "django_http_requests_unknown_latency_including_middlewares_total",
             (
                 "Count of requests for which the latency was unknown (when computing "
@@ -73,17 +50,15 @@
             namespace=NAMESPACE,
         )
         self.requests_latency_by_view_method = self.register_metric(
             Histogram,
             "django_http_requests_latency_seconds_by_view_method",
             "Histogram of request processing time labelled by view.",
             ["view", "method"],
-            buckets=getattr(
-                settings, "PROMETHEUS_LATENCY_BUCKETS", DEFAULT_LATENCY_BUCKETS
-            ),
+            buckets=PROMETHEUS_LATENCY_BUCKETS,
             namespace=NAMESPACE,
         )
         self.requests_unknown_latency = self.register_metric(
             Counter,
             "django_http_requests_unknown_latency_total",
             "Count of requests for which the latency was unknown.",
             namespace=NAMESPACE,
@@ -185,40 +160,38 @@
 
 
 class PrometheusBeforeMiddleware(MiddlewareMixin):
     """Monitoring middleware that should run before other middlewares."""
 
     metrics_cls = Metrics
 
-    def __init__(self, get_response=None):
-        super().__init__(get_response)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.metrics = self.metrics_cls.get_instance()
 
     def process_request(self, request):
         self.metrics.requests_total.inc()
         request.prometheus_before_middleware_event = Time()
 
     def process_response(self, request, response):
         self.metrics.responses_total.inc()
         if hasattr(request, "prometheus_before_middleware_event"):
-            self.metrics.requests_latency_before.observe(
-                TimeSince(request.prometheus_before_middleware_event)
-            )
+            self.metrics.requests_latency_before.observe(TimeSince(request.prometheus_before_middleware_event))
         else:
             self.metrics.requests_unknown_latency_before.inc()
         return response
 
 
 class PrometheusAfterMiddleware(MiddlewareMixin):
     """Monitoring middleware that should run after other middlewares."""
 
     metrics_cls = Metrics
 
-    def __init__(self, get_response=None):
-        super().__init__(get_response)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.metrics = self.metrics_cls.get_instance()
 
     def _transport(self, request):
         return "https" if request.is_secure() else "http"
 
     def _method(self, request):
         m = request.method
@@ -239,26 +212,22 @@
     def label_metric(self, metric, request, response=None, **labels):
         return metric.labels(**labels) if labels else metric
 
     def process_request(self, request):
         transport = self._transport(request)
         method = self._method(request)
         self.label_metric(self.metrics.requests_by_method, request, method=method).inc()
-        self.label_metric(
-            self.metrics.requests_by_transport, request, transport=transport
-        ).inc()
+        self.label_metric(self.metrics.requests_by_transport, request, transport=transport).inc()
 
         # Mimic the behaviour of the deprecated "Request.is_ajax()" method.
         if request.META.get("HTTP_X_REQUESTED_WITH") == "XMLHttpRequest":
             self.label_metric(self.metrics.requests_ajax, request).inc()
 
         content_length = int(request.META.get("CONTENT_LENGTH") or 0)
-        self.label_metric(self.metrics.requests_body_bytes, request).observe(
-            content_length
-        )
+        self.label_metric(self.metrics.requests_body_bytes, request).observe(content_length)
         request.prometheus_after_middleware_event = Time()
 
     def _get_view_name(self, request):
         view_name = "<unnamed view>"
         if hasattr(request, "resolver_match"):
             if request.resolver_match is not None:
                 if request.resolver_match.view_name is not None:
@@ -288,17 +257,15 @@
             ).inc()
         return response
 
     def process_response(self, request, response):
         method = self._method(request)
         name = self._get_view_name(request)
         status = str(response.status_code)
-        self.label_metric(
-            self.metrics.responses_by_status, request, response, status=status
-        ).inc()
+        self.label_metric(self.metrics.responses_by_status, request, response, status=status).inc()
         self.label_metric(
             self.metrics.responses_by_status_view_method,
             request,
             response,
             status=status,
             view=name,
             method=method,
@@ -309,35 +276,29 @@
                 request,
                 response,
                 charset=str(response.charset),
             ).inc()
         if hasattr(response, "streaming") and response.streaming:
             self.label_metric(self.metrics.responses_streaming, request, response).inc()
         if hasattr(response, "content"):
-            self.label_metric(
-                self.metrics.responses_body_bytes, request, response
-            ).observe(len(response.content))
+            self.label_metric(self.metrics.responses_body_bytes, request, response).observe(len(response.content))
         if hasattr(request, "prometheus_after_middleware_event"):
             self.label_metric(
                 self.metrics.requests_latency_by_view_method,
                 request,
                 response,
                 view=self._get_view_name(request),
                 method=request.method,
             ).observe(TimeSince(request.prometheus_after_middleware_event))
         else:
-            self.label_metric(
-                self.metrics.requests_unknown_latency, request, response
-            ).inc()
+            self.label_metric(self.metrics.requests_unknown_latency, request, response).inc()
         return response
 
     def process_exception(self, request, exception):
-        self.label_metric(
-            self.metrics.exceptions_by_type, request, type=type(exception).__name__
-        ).inc()
+        self.label_metric(self.metrics.exceptions_by_type, request, type=type(exception).__name__).inc()
         if hasattr(request, "resolver_match"):
             name = request.resolver_match.view_name or "<unnamed view>"
             self.label_metric(self.metrics.exceptions_by_view, request, view=name).inc()
         if hasattr(request, "prometheus_after_middleware_event"):
             self.label_metric(
                 self.metrics.requests_latency_by_view_method,
                 request,
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/migrations.py` & `django-prometheus-2.3.0.dev44/django_prometheus/migrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from prometheus_client import Gauge
-
 from django.db import connections
 from django.db.backends.dummy.base import DatabaseWrapper
+from prometheus_client import Gauge
+
 from django_prometheus.conf import NAMESPACE
 
 unapplied_migrations = Gauge(
     "django_migrations_unapplied_total",
     "Count of unapplied migrations by database connection",
     ["connection"],
     namespace=NAMESPACE,
@@ -35,17 +35,15 @@
     # Import MigrationExecutor lazily. MigrationExecutor checks at
     # import time that the apps are ready, and they are not when
     # django_prometheus is imported. ExportMigrations() should be
     # called in AppConfig.ready(), which signals that all apps are
     # ready.
     from django.db.migrations.executor import MigrationExecutor
 
-    if "default" in connections and (
-        isinstance(connections["default"], DatabaseWrapper)
-    ):
+    if "default" in connections and (isinstance(connections["default"], DatabaseWrapper)):
         # This is the case where DATABASES = {} in the configuration,
         # i.e. the user is not using any databases. Django "helpfully"
         # adds a dummy database and then throws when you try to
         # actually use it. So we don't do anything, because trying to
         # export stats would crash the app on startup.
         return
     for alias in connections.databases:
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/models.py` & `django-prometheus-2.3.0.dev44/django_prometheus/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,8 +46,9 @@
             model_updates.labels(model_name).inc()
             return super()._do_update(*args, **kwargs)
 
         def delete(self, *args, **kwargs):
             model_deletes.labels(model_name).inc()
             return super().delete(*args, **kwargs)
 
+    Mixin.__qualname__ = f"ExportModelOperationsMixin('{model_name}')"
     return Mixin
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/tests/test_exports.py` & `django-prometheus-2.3.0.dev44/django_prometheus/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus/utils.py` & `django-prometheus-2.3.0.dev44/django_prometheus/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     """
     return default_timer() - t
 
 
 def PowersOf(logbase, count, lower=0, include_zero=True):
     """Returns a list of count powers of logbase (from logbase**lower)."""
     if not include_zero:
-        return [logbase ** i for i in range(lower, count + lower)]
+        return [logbase**i for i in range(lower, count + lower)]
     else:
-        return [0] + [logbase ** i for i in range(lower, count + lower)]
+        return [0] + [logbase**i for i in range(lower, count + lower)]
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus.egg-info/PKG-INFO` & `django-prometheus-2.3.0.dev44/django_prometheus.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,265 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.2.0.dev8
+Version: 2.3.0.dev44
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
-Description: # django-prometheus
-        
-        Export Django monitoring metrics for Prometheus.io
-        
-        [![Join the chat at https://gitter.im/django-prometheus/community](https://badges.gitter.im/django-prometheus/community.svg)](https://gitter.im/django-prometheus/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
-        
-        [![PyPI version](https://badge.fury.io/py/django-prometheus.svg)](http://badge.fury.io/py/django-prometheus)
-        [![Build Status](https://travis-ci.org/korfuri/django-prometheus.svg?branch=master)](https://travis-ci.org/korfuri/django-prometheus)
-        [![Coverage Status](https://coveralls.io/repos/github/korfuri/django-prometheus/badge.svg?branch=master)](https://coveralls.io/github/korfuri/django-prometheus?branch=master)
-        [![PyPi page link -- Python versions](https://img.shields.io/pypi/pyversions/django-prometheus.svg)](https://pypi.python.org/pypi/django-prometheus)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        ## Features
-        
-        This library provides Prometheus metrics for Django related operations:
-        
-        * Requests & Responses
-        * Database access done via [Django ORM](https://docs.djangoproject.com/en/3.0/topics/db/)
-        * Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.0/topics/cache/)
-        
-        ## Usage
-        
-        ### Requirements
-        
-        * Django >= 2.2
-        
-        ### Installation
-        
-        Install with:
-        
-        ```shell
-        pip install django-prometheus
-        ```
-        
-        Or, if you're using a development version cloned from this repository:
-        
-        ```shell
-        python path-to-where-you-cloned-django-prometheus/setup.py install
-        ```
-        
-        This will install [prometheus_client](https://github.com/prometheus/client_python) as a dependency.
-        
-        ### Quickstart
-        
-        In your settings.py:
-        
-        ```python
-        INSTALLED_APPS = [
-           ...
-           'django_prometheus',
-           ...
-        ]
-        
-        MIDDLEWARE = [
-            'django_prometheus.middleware.PrometheusBeforeMiddleware',
-            # All your other middlewares go here, including the default
-            # middlewares like SessionMiddleware, CommonMiddleware,
-            # CsrfViewmiddleware, SecurityMiddleware, etc.
-            'django_prometheus.middleware.PrometheusAfterMiddleware',
-        ]
-        ```
-        
-        In your urls.py:
-        
-        ```python
-        urlpatterns = [
-            ...
-            url('', include('django_prometheus.urls')),
-        ]
-        ```
-        
-        ### Configuration
-        
-        Prometheus uses Histogram based grouping for monitoring latencies. The default
-        buckets are here: https://github.com/prometheus/client_python/blob/master/prometheus_client/core.py
-        
-        You can define custom buckets for latency, adding more buckets decreases performance but
-        increases accuracy: https://prometheus.io/docs/practices/histograms/
-        
-        ```python
-        PROMETHEUS_LATENCY_BUCKETS = (.1, .2, .5, .6, .8, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.5, 9.0, 12.0, 15.0, 20.0, 30.0, float("inf"))
-        ```
-        
-        ### Monitoring your databases
-        
-        SQLite, MySQL, and PostgreSQL databases can be monitored. Just
-        replace the `ENGINE` property of your database, replacing
-        `django.db.backends` with `django_prometheus.db.backends`.
-        
-        ```python
-        DATABASES = {
-            'default': {
-                'ENGINE': 'django_prometheus.db.backends.sqlite3',
-                'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
-            },
-        }
-        ```
-        
-        ### Monitoring your caches
-        
-        Filebased, memcached, redis caches can be monitored. Just replace
-        the cache backend to use the one provided by django_prometheus
-        `django.core.cache.backends` with `django_prometheus.cache.backends`.
-        
-        ```python
-        CACHES = {
-            'default': {
-                'BACKEND': 'django_prometheus.cache.backends.filebased.FileBasedCache',
-                'LOCATION': '/var/tmp/django_cache',
-            }
-        }
-        ```
-        
-        ### Monitoring your models
-        
-        You may want to monitor the creation/deletion/update rate for your
-        model. This can be done by adding a mixin to them. This is safe to do
-        on existing models (it does not require a migration).
-        
-        If your model is:
-        
-        ```python
-        class Dog(models.Model):
-            name = models.CharField(max_length=100, unique=True)
-            breed = models.CharField(max_length=100, blank=True, null=True)
-            age = models.PositiveIntegerField(blank=True, null=True)
-        ```
-        
-        Just add the `ExportModelOperationsMixin` as such:
-        
-        ```python
-        from django_prometheus.models import ExportModelOperationsMixin
-        
-        class Dog(ExportModelOperationsMixin('dog'), models.Model):
-            name = models.CharField(max_length=100, unique=True)
-            breed = models.CharField(max_length=100, blank=True, null=True)
-            age = models.PositiveIntegerField(blank=True, null=True)
-        ```
-        
-        This will export 3 metrics, `django_model_inserts_total{model="dog"}`,
-        `django_model_updates_total{model="dog"}` and
-        `django_model_deletes_total{model="dog"}`.
-        
-        Note that the exported metrics are counters of creations,
-        modifications and deletions done in the current process. They are not
-        gauges of the number of objects in the model.
-        
-        Starting with Django 1.7, migrations are also monitored. Two gauges
-        are exported, `django_migrations_applied_by_connection` and
-        `django_migrations_unapplied_by_connection`. You may want to alert if
-        there are unapplied migrations.
-        
-        If you want to disable the Django migration metrics, set the
-        `PROMETHEUS_EXPORT_MIGRATIONS` setting to False.
-        
-        ### Monitoring and aggregating the metrics
-        
-        Prometheus is quite easy to set up. An example prometheus.conf to
-        scrape `127.0.0.1:8001` can be found in `examples/prometheus`.
-        
-        Here's an example of a PromDash displaying some of the metrics
-        collected by django-prometheus:
-        
-        ![Example dashboard](https://raw.githubusercontent.com/korfuri/django-prometheus/master/examples/django-promdash.png)
-        
-        ## Adding your own metrics
-        
-        You can add application-level metrics in your code by using
-        [prometheus_client](https://github.com/prometheus/client_python)
-        directly. The exporter is global and will pick up your metrics.
-        
-        To add metrics to the Django internals, the easiest way is to extend
-        django-prometheus' classes. Please consider contributing your metrics,
-        pull requests are welcome. Make sure to read the Prometheus best
-        practices on
-        [instrumentation](http://prometheus.io/docs/practices/instrumentation/)
-        and [naming](http://prometheus.io/docs/practices/naming/).
-        
-        ## Importing Django Prometheus using only local settings
-        
-        If you wish to use Django Prometheus but are not able to change
-        the code base, it's possible to have all the default metrics by
-        modifying only the settings.
-        
-        First step is to inject prometheus' middlewares and to add
-        django_prometheus in INSTALLED_APPS
-        
-        ```python
-        MIDDLEWARE = \
-            ['django_prometheus.middleware.PrometheusBeforeMiddleware'] + \
-            MIDDLEWARE + \
-            ['django_prometheus.middleware.PrometheusAfterMiddleware']
-        
-        INSTALLED_APPS += ['django_prometheus']
-        ```
-        
-        Second step is to create the /metrics end point, for that we need
-        another file (called urls_prometheus_wrapper.py in this example) that
-        will wraps the apps URLs and add one on top:
-        
-        ```python
-        from django.conf.urls import include, url
-        
-        
-        urlpatterns = []
-        
-        urlpatterns.append(url('prometheus/', include('django_prometheus.urls')))
-        urlpatterns.append(url('', include('myapp.urls')))
-        ```
-        
-        This file will add a "/prometheus/metrics" end point to the URLs of django
-        that will export the metrics (replace myapp by your project name).
-        
-        Then we inject the wrapper in settings:
-        
-        ```python
-        ROOT_URLCONF = "graphite.urls_prometheus_wrapper"
-        ```
-        
-        ## Adding custom labels to middleware (request/response) metrics
-        
-        You can add application specific labels to metrics reported by the django-prometheus middleware.
-        This involves extending the classes defined in middleware.py.
-        
-        * Extend the Metrics class and override the `register_metric` method to add the application specific labels.
-        * Extend middleware classes, set the metrics_cls class attribute to the the extended metric class and override the label_metric method to attach custom metrics.
-        
-        See implementation example in [the test app](django_prometheus/tests/end2end/testapp/test_middleware_custom_labels.py#L19-L46)
-        
+Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
+Project-URL: Source, https://github.com/korfuri/django-prometheus
+Project-URL: Tracker, https://github.com/korfuri/django-prometheus/issues
 Keywords: django monitoring prometheus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-prometheus
+
+Export Django monitoring metrics for Prometheus.io
+
+[![Join the chat at https://gitter.im/django-prometheus/community](https://badges.gitter.im/django-prometheus/community.svg)](https://gitter.im/django-prometheus/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+
+[![PyPI version](https://badge.fury.io/py/django-prometheus.svg)](http://badge.fury.io/py/django-prometheus)
+[![Build Status](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/korfuri/django-prometheus/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/korfuri/django-prometheus/badge.svg?branch=master)](https://coveralls.io/github/korfuri/django-prometheus?branch=master)
+[![PyPi page link -- Python versions](https://img.shields.io/pypi/pyversions/django-prometheus.svg)](https://pypi.python.org/pypi/django-prometheus)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+## Features
+
+This library provides Prometheus metrics for Django related operations:
+
+* Requests & Responses
+* Database access done via [Django ORM](https://docs.djangoproject.com/en/3.2/topics/db/)
+* Cache access done via [Django Cache framework](https://docs.djangoproject.com/en/3.2/topics/cache/)
+
+## Usage
+
+### Requirements
+
+* Django >= 3.2
+* Python 3.7 and above.
+
+### Installation
+
+Install with:
+
+```shell
+pip install django-prometheus
+```
+
+Or, if you're using a development version cloned from this repository:
+
+```shell
+python path-to-where-you-cloned-django-prometheus/setup.py install
+```
+
+This will install [prometheus_client](https://github.com/prometheus/client_python) as a dependency.
+
+### Quickstart
+
+In your settings.py:
+
+```python
+INSTALLED_APPS = [
+   ...
+   'django_prometheus',
+   ...
+]
+
+MIDDLEWARE = [
+    'django_prometheus.middleware.PrometheusBeforeMiddleware',
+    # All your other middlewares go here, including the default
+    # middlewares like SessionMiddleware, CommonMiddleware,
+    # CsrfViewmiddleware, SecurityMiddleware, etc.
+    'django_prometheus.middleware.PrometheusAfterMiddleware',
+]
+```
+
+In your urls.py:
+
+```python
+urlpatterns = [
+    ...
+    path('', include('django_prometheus.urls')),
+]
+```
+
+### Configuration
+
+Prometheus uses Histogram based grouping for monitoring latencies. The default
+buckets are:
+
+```python
+PROMETHEUS_LATENCY_BUCKETS = (0.01, 0.025, 0.05, 0.075, 0.1, 0.25, 0.5, 0.75, 1.0, 2.5, 5.0, 7.5, 10.0, 25.0, 50.0, 75.0, float("inf"),)
+```
+
+You can define custom buckets for latency, adding more buckets decreases performance but
+increases accuracy: <https://prometheus.io/docs/practices/histograms/>
+
+```python
+PROMETHEUS_LATENCY_BUCKETS = (.1, .2, .5, .6, .8, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.5, 9.0, 12.0, 15.0, 20.0, 30.0, float("inf"))
+```
+
+### Monitoring your databases
+
+SQLite, MySQL, and PostgreSQL databases can be monitored. Just
+replace the `ENGINE` property of your database, replacing
+`django.db.backends` with `django_prometheus.db.backends`.
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'django_prometheus.db.backends.sqlite3',
+        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
+    },
+}
+```
+
+### Monitoring your caches
+
+Filebased, memcached, redis caches can be monitored. Just replace
+the cache backend to use the one provided by django_prometheus
+`django.core.cache.backends` with `django_prometheus.cache.backends`.
+
+```python
+CACHES = {
+    'default': {
+        'BACKEND': 'django_prometheus.cache.backends.filebased.FileBasedCache',
+        'LOCATION': '/var/tmp/django_cache',
+    }
+}
+```
+
+### Monitoring your models
+
+You may want to monitor the creation/deletion/update rate for your
+model. This can be done by adding a mixin to them. This is safe to do
+on existing models (it does not require a migration).
+
+If your model is:
+
+```python
+class Dog(models.Model):
+    name = models.CharField(max_length=100, unique=True)
+    breed = models.CharField(max_length=100, blank=True, null=True)
+    age = models.PositiveIntegerField(blank=True, null=True)
+```
+
+Just add the `ExportModelOperationsMixin` as such:
+
+```python
+from django_prometheus.models import ExportModelOperationsMixin
+
+class Dog(ExportModelOperationsMixin('dog'), models.Model):
+    name = models.CharField(max_length=100, unique=True)
+    breed = models.CharField(max_length=100, blank=True, null=True)
+    age = models.PositiveIntegerField(blank=True, null=True)
+```
+
+This will export 3 metrics, `django_model_inserts_total{model="dog"}`,
+`django_model_updates_total{model="dog"}` and
+`django_model_deletes_total{model="dog"}`.
+
+Note that the exported metrics are counters of creations,
+modifications and deletions done in the current process. They are not
+gauges of the number of objects in the model.
+
+Starting with Django 1.7, migrations are also monitored. Two gauges
+are exported, `django_migrations_applied_by_connection` and
+`django_migrations_unapplied_by_connection`. You may want to alert if
+there are unapplied migrations.
+
+If you want to disable the Django migration metrics, set the
+`PROMETHEUS_EXPORT_MIGRATIONS` setting to False.
+
+### Monitoring and aggregating the metrics
+
+Prometheus is quite easy to set up. An example prometheus.conf to
+scrape `127.0.0.1:8001` can be found in `examples/prometheus`.
+
+Here's an example of a PromDash displaying some of the metrics
+collected by django-prometheus:
+
+![Example dashboard](https://raw.githubusercontent.com/korfuri/django-prometheus/master/examples/django-promdash.png)
+
+## Adding your own metrics
+
+You can add application-level metrics in your code by using
+[prometheus_client](https://github.com/prometheus/client_python)
+directly. The exporter is global and will pick up your metrics.
+
+To add metrics to the Django internals, the easiest way is to extend
+django-prometheus' classes. Please consider contributing your metrics,
+pull requests are welcome. Make sure to read the Prometheus best
+practices on
+[instrumentation](http://prometheus.io/docs/practices/instrumentation/)
+and [naming](http://prometheus.io/docs/practices/naming/).
+
+## Importing Django Prometheus using only local settings
+
+If you wish to use Django Prometheus but are not able to change
+the code base, it's possible to have all the default metrics by
+modifying only the settings.
+
+First step is to inject prometheus' middlewares and to add
+django_prometheus in INSTALLED_APPS
+
+```python
+MIDDLEWARE = \
+    ['django_prometheus.middleware.PrometheusBeforeMiddleware'] + \
+    MIDDLEWARE + \
+    ['django_prometheus.middleware.PrometheusAfterMiddleware']
+
+INSTALLED_APPS += ['django_prometheus']
+```
+
+Second step is to create the /metrics end point, for that we need
+another file (called urls_prometheus_wrapper.py in this example) that
+will wraps the apps URLs and add one on top:
+
+```python
+from django.urls import include, path
+
+
+urlpatterns = []
+
+urlpatterns.append(path('prometheus/', include('django_prometheus.urls')))
+urlpatterns.append(path('', include('myapp.urls')))
+```
+
+This file will add a "/prometheus/metrics" end point to the URLs of django
+that will export the metrics (replace myapp by your project name).
+
+Then we inject the wrapper in settings:
+
+```python
+ROOT_URLCONF = "graphite.urls_prometheus_wrapper"
+```
+
+## Adding custom labels to middleware (request/response) metrics
+
+You can add application specific labels to metrics reported by the django-prometheus middleware.
+This involves extending the classes defined in middleware.py.
+
+* Extend the Metrics class and override the `register_metric` method to add the application specific labels.
+* Extend middleware classes, set the metrics_cls class attribute to the the extended metric class and override the label_metric method to attach custom metrics.
+
+See implementation example in [the test app](django_prometheus/tests/end2end/testapp/test_middleware_custom_labels.py#L19-L46)
```

### Comparing `django-prometheus-2.2.0.dev8/django_prometheus.egg-info/SOURCES.txt` & `django-prometheus-2.3.0.dev44/django_prometheus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 django_prometheus/__init__.py
 django_prometheus/apps.py
 django_prometheus/exports.py
 django_prometheus/middleware.py
 django_prometheus/migrations.py
@@ -26,14 +27,15 @@
 django_prometheus/cache/backends/memcached.py
 django_prometheus/cache/backends/redis.py
 django_prometheus/conf/__init__.py
 django_prometheus/db/__init__.py
 django_prometheus/db/common.py
 django_prometheus/db/metrics.py
 django_prometheus/db/backends/__init__.py
+django_prometheus/db/backends/common.py
 django_prometheus/db/backends/mysql/__init__.py
 django_prometheus/db/backends/mysql/base.py
 django_prometheus/db/backends/postgis/__init__.py
 django_prometheus/db/backends/postgis/base.py
 django_prometheus/db/backends/postgresql/__init__.py
 django_prometheus/db/backends/postgresql/base.py
 django_prometheus/db/backends/sqlite3/__init__.py
```

### Comparing `django-prometheus-2.2.0.dev8/setup.py` & `django-prometheus-2.3.0.dev44/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from setuptools import find_packages, setup
 
 with open("README.md") as fl:
     LONG_DESCRIPTION = fl.read()
 
 
 def get_version():
@@ -20,31 +21,46 @@
     version=get_version(),
     author="Uriel Corfa",
     author_email="uriel@corfa.fr",
     description=("Django middlewares to monitor your application with Prometheus.io."),
     license="Apache",
     keywords="django monitoring prometheus",
     url="http://github.com/korfuri/django-prometheus",
-    packages=find_packages(exclude=["tests",]),
+    project_urls={
+        "Changelog": "https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md",
+        "Documentation": "https://github.com/korfuri/django-prometheus/blob/master/README.md",
+        "Source": "https://github.com/korfuri/django-prometheus",
+        "Tracker": "https://github.com/korfuri/django-prometheus/issues",
+    },
+    packages=find_packages(
+        exclude=[
+            "tests",
+        ]
+    ),
     test_suite="django_prometheus.tests",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     tests_require=["pytest", "pytest-django"],
     setup_requires=["pytest-runner"],
     options={"bdist_wheel": {"universal": "1"}},
-    install_requires=["prometheus-client>=0.7",],
+    install_requires=[
+        "prometheus-client>=0.7",
+    ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Topic :: System :: Monitoring",
         "License :: OSI Approved :: Apache Software License",
     ],
 )
```

