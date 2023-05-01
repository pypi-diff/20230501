# Comparing `tmp/sweelol-1.1.0.tar.gz` & `tmp/sweelol-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sweelol-1.1.0.tar", last modified: Mon May  1 17:22:11 2023, max compression
+gzip compressed data, was "dist/sweelol-1.1.1.tar", last modified: Mon May  1 17:25:58 2023, max compression
```

## Comparing `sweelol-1.1.0.tar` & `sweelol-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/
--rw-r--r--   0 selorm     (501) staff       (20)     5869 2023-05-01 17:22:11.000000 sweelol-1.1.0/PKG-INFO
--rw-rw-r--   0 selorm     (501) staff       (20)     1086 2023-04-29 21:54:07.000000 sweelol-1.1.0/LICENSE
--rw-rw-r--   0 selorm     (501) staff       (20)       34 2023-04-29 21:54:07.000000 sweelol-1.1.0/MANIFEST.in
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/sweelol.egg-info/
--rw-r--r--   0 selorm     (501) staff       (20)     5869 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/PKG-INFO
--rw-r--r--   0 selorm     (501) staff       (20)        1 2023-04-29 23:13:36.000000 sweelol-1.1.0/sweelol.egg-info/not-zip-safe
--rw-r--r--   0 selorm     (501) staff       (20)      754 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/SOURCES.txt
--rw-r--r--   0 selorm     (501) staff       (20)       40 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/entry_points.txt
--rw-r--r--   0 selorm     (501) staff       (20)       51 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/requires.txt
--rw-r--r--   0 selorm     (501) staff       (20)       22 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/top_level.txt
--rw-r--r--   0 selorm     (501) staff       (20)        1 2023-05-01 17:22:10.000000 sweelol-1.1.0/sweelol.egg-info/dependency_links.txt
--rw-rw-r--   0 selorm     (501) staff       (20)     4458 2023-04-29 22:49:18.000000 sweelol-1.1.0/setup.py
--rw-rw-r--   0 selorm     (501) staff       (20)       38 2023-05-01 17:22:11.000000 sweelol-1.1.0/setup.cfg
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:10.000000 sweelol-1.1.0/django_media_fixtures/
--rw-rw-r--   0 selorm     (501) staff       (20)     6918 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/finders.py
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/django_media_fixtures/tests/
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/django_media_fixtures/tests/testapp/
--rw-rw-r--   0 selorm     (501) staff       (20)      308 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/testapp/models.py
--rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/testapp/__init__.py
--rw-rw-r--   0 selorm     (501) staff       (20)      159 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/testapp/apps.py
--rw-rw-r--   0 selorm     (501) staff       (20)     3452 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/testapp/tests.py
--rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/__init__.py
--rw-rw-r--   0 selorm     (501) staff       (20)     2581 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/tests/settings.py
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/django_media_fixtures/management/
--rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/management/__init__.py
-drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:22:11.000000 sweelol-1.1.0/django_media_fixtures/management/commands/
--rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.0/django_media_fixtures/management/commands/__init__.py
--rw-rw-r--   0 selorm     (501) staff       (20)    13957 2023-05-01 17:19:21.000000 sweelol-1.1.0/django_media_fixtures/management/commands/collectmedia.py
--rw-rw-r--   0 selorm     (501) staff       (20)       22 2023-05-01 17:19:29.000000 sweelol-1.1.0/django_media_fixtures/__init__.py
--rw-rw-r--   0 selorm     (501) staff       (20)     3560 2023-04-29 22:49:18.000000 sweelol-1.1.0/README.rst
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/
+-rw-r--r--   0 selorm     (501) staff       (20)     5869 2023-05-01 17:25:58.000000 sweelol-1.1.1/PKG-INFO
+-rw-rw-r--   0 selorm     (501) staff       (20)     1086 2023-04-29 21:54:07.000000 sweelol-1.1.1/LICENSE
+-rw-rw-r--   0 selorm     (501) staff       (20)       34 2023-04-29 21:54:07.000000 sweelol-1.1.1/MANIFEST.in
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/
+-rw-r--r--   0 selorm     (501) staff       (20)     5869 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/PKG-INFO
+-rw-r--r--   0 selorm     (501) staff       (20)        1 2023-04-29 23:13:36.000000 sweelol-1.1.1/sweelol.egg-info/not-zip-safe
+-rw-r--r--   0 selorm     (501) staff       (20)      754 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/SOURCES.txt
+-rw-r--r--   0 selorm     (501) staff       (20)       40 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/entry_points.txt
+-rw-r--r--   0 selorm     (501) staff       (20)       51 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/requires.txt
+-rw-r--r--   0 selorm     (501) staff       (20)       22 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/top_level.txt
+-rw-r--r--   0 selorm     (501) staff       (20)        1 2023-05-01 17:25:58.000000 sweelol-1.1.1/sweelol.egg-info/dependency_links.txt
+-rw-rw-r--   0 selorm     (501) staff       (20)     4458 2023-04-29 22:49:18.000000 sweelol-1.1.1/setup.py
+-rw-rw-r--   0 selorm     (501) staff       (20)       38 2023-05-01 17:25:58.000000 sweelol-1.1.1/setup.cfg
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/django_media_fixtures/
+-rw-rw-r--   0 selorm     (501) staff       (20)     6918 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/finders.py
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/django_media_fixtures/tests/
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/django_media_fixtures/tests/testapp/
+-rw-rw-r--   0 selorm     (501) staff       (20)      308 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/testapp/models.py
+-rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/testapp/__init__.py
+-rw-rw-r--   0 selorm     (501) staff       (20)      159 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/testapp/apps.py
+-rw-rw-r--   0 selorm     (501) staff       (20)     3452 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/testapp/tests.py
+-rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/__init__.py
+-rw-rw-r--   0 selorm     (501) staff       (20)     2581 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/tests/settings.py
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/django_media_fixtures/management/
+-rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/management/__init__.py
+drwxr-xr-x   0 selorm     (501) staff       (20)        0 2023-05-01 17:25:58.000000 sweelol-1.1.1/django_media_fixtures/management/commands/
+-rw-rw-r--   0 selorm     (501) staff       (20)        0 2023-04-29 21:54:07.000000 sweelol-1.1.1/django_media_fixtures/management/commands/__init__.py
+-rw-rw-r--   0 selorm     (501) staff       (20)    13957 2023-05-01 17:19:21.000000 sweelol-1.1.1/django_media_fixtures/management/commands/collectmedia.py
+-rw-rw-r--   0 selorm     (501) staff       (20)       22 2023-05-01 17:25:42.000000 sweelol-1.1.1/django_media_fixtures/__init__.py
+-rw-rw-r--   0 selorm     (501) staff       (20)     3560 2023-05-01 17:25:42.000000 sweelol-1.1.1/README.rst
```

### Comparing `sweelol-1.1.0/PKG-INFO` & `sweelol-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweelol
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple project to copy media files (intended for fixtures loads), pretty much as Django staticfiles does
 Home-page: https://github.com/pojoba02/django-media-fixtures.git
 Author: Francis I AM
 Author-email: pojoba01@gmail.com
 License: MIT
 Description: |badge1| |badge2| |badge3| |badge4| |badge5|
         
@@ -44,15 +44,15 @@
         
         
         Installation
         ------------
         
         .. code-block:: python
         
-           pip install sweelol==1.0.0
+           pip install sweelol==1.1.1
         
         Then, add the ``django_media_fixtures`` app in your ``settings.INSTALLED_APPS``:
         
         .. code-block:: python
         
             INSTALLED_APPS = [
                 ...,
```

### Comparing `sweelol-1.1.0/LICENSE` & `sweelol-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/sweelol.egg-info/PKG-INFO` & `sweelol-1.1.1/sweelol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweelol
-Version: 1.1.0
+Version: 1.1.1
 Summary: Simple project to copy media files (intended for fixtures loads), pretty much as Django staticfiles does
 Home-page: https://github.com/pojoba02/django-media-fixtures.git
 Author: Francis I AM
 Author-email: pojoba01@gmail.com
 License: MIT
 Description: |badge1| |badge2| |badge3| |badge4| |badge5|
         
@@ -44,15 +44,15 @@
         
         
         Installation
         ------------
         
         .. code-block:: python
         
-           pip install sweelol==1.0.0
+           pip install sweelol==1.1.1
         
         Then, add the ``django_media_fixtures`` app in your ``settings.INSTALLED_APPS``:
         
         .. code-block:: python
         
             INSTALLED_APPS = [
                 ...,
```

### Comparing `sweelol-1.1.0/sweelol.egg-info/SOURCES.txt` & `sweelol-1.1.1/sweelol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/setup.py` & `sweelol-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/django_media_fixtures/finders.py` & `sweelol-1.1.1/django_media_fixtures/finders.py`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/django_media_fixtures/tests/testapp/tests.py` & `sweelol-1.1.1/django_media_fixtures/tests/testapp/tests.py`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/django_media_fixtures/tests/settings.py` & `sweelol-1.1.1/django_media_fixtures/tests/settings.py`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/django_media_fixtures/management/commands/collectmedia.py` & `sweelol-1.1.1/django_media_fixtures/management/commands/collectmedia.py`

 * *Files identical despite different names*

### Comparing `sweelol-1.1.0/README.rst` & `sweelol-1.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 Installation
 ------------
 
 .. code-block:: python
 
-   pip install sweelol==1.0.0
+   pip install sweelol==1.1.1
 
 Then, add the ``django_media_fixtures`` app in your ``settings.INSTALLED_APPS``:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

