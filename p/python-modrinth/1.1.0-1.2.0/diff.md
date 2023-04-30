# Comparing `tmp/python-modrinth-1.1.0.tar.gz` & `tmp/python-modrinth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-modrinth-1.1.0.tar", last modified: Mon Mar 27 23:14:07 2023, max compression
+gzip compressed data, was "python-modrinth-1.2.0.tar", last modified: Sun Apr 30 22:10:50 2023, max compression
```

## Comparing `python-modrinth-1.1.0.tar` & `python-modrinth-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 23:14:07.039289 python-modrinth-1.1.0/
--rw-rw-rw-   0        0        0    11525 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4204 2023-03-27 23:14:07.039289 python-modrinth-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3636 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/README.md
--rw-rw-rw-   0        0        0      124 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      703 2023-03-27 23:14:07.040289 python-modrinth-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-27 23:14:07.019154 python-modrinth-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 23:14:07.033609 python-modrinth-1.1.0/src/pyrinth/
--rw-rw-rw-   0        0        0      160 2023-03-20 20:49:28.000000 python-modrinth-1.1.0/src/pyrinth/__init__.py
--rw-rw-rw-   0        0        0    10932 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/src/pyrinth/models.py
--rw-rw-rw-   0        0        0     6215 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/src/pyrinth/modrinth.py
--rw-rw-rw-   0        0        0    28526 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/src/pyrinth/projects.py
--rw-rw-rw-   0        0        0     8889 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/src/pyrinth/users.py
--rw-rw-rw-   0        0        0     1145 2023-03-27 22:52:06.000000 python-modrinth-1.1.0/src/pyrinth/util.py
-drwxrwxrwx   0        0        0        0 2023-03-27 23:14:07.038284 python-modrinth-1.1.0/src/python_modrinth.egg-info/
--rw-rw-rw-   0        0        0     4204 2023-03-27 23:14:07.000000 python-modrinth-1.1.0/src/python_modrinth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-03-27 23:14:07.000000 python-modrinth-1.1.0/src/python_modrinth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 23:14:07.000000 python-modrinth-1.1.0/src/python_modrinth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-27 23:14:07.000000 python-modrinth-1.1.0/src/python_modrinth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.668475 python-modrinth-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/src/pyrinth/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/modrinth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50360 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/src/python_modrinth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/top_level.txt
```

