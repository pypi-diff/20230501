# Comparing `tmp/django-addresses-0.1.tar.gz` & `tmp/django-addresses-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-addresses-0.1.tar", last modified: Mon Jun 24 15:20:01 2013, max compression
+gzip compressed data, was "dist/django-addresses-0.2.0b1.tar", last modified: Mon May  1 17:14:41 2023, max compression
```

## Comparing `django-addresses-0.1.tar` & `django-addresses-0.2.0b1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/
--rw-r--r--   0 simon     (1000) simon     (1000)      621 2013-06-24 15:20:00.000000 django-addresses-0.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      936 2013-06-24 15:19:19.000000 django-addresses-0.1/setup.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1390 2013-06-24 15:17:13.000000 django-addresses-0.1/LICENCE
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/
--rw-r--r--   0 simon     (1000) simon     (1000)      172 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/forms.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/fixtures/
--rw-r--r--   0 simon     (1000) simon     (1000)    45970 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/fixtures/initial_data.xml
--rw-r--r--   0 simon     (1000) simon     (1000)       23 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     2242 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/tests.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3216 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/models.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/
--rw-r--r--   0 simon     (1000) simon     (1000)        0 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/conf/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en_GB/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 simon     (1000) simon     (1000)     1148 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/conf/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en/LC_MESSAGES/
--rw-r--r--   0 simon     (1000) simon     (1000)     1148 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/conf/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en_US/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2013-06-24 15:20:00.000000 django-addresses-0.1/addressbook/conf/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 simon     (1000) simon     (1000)     1142 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/conf/locale/en_US/LC_MESSAGES/django.po
--rw-r--r--   0 simon     (1000) simon     (1000)      104 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/conf/settings.py
--rw-r--r--   0 simon     (1000) simon     (1000)      438 2013-06-20 07:36:25.000000 django-addresses-0.1/addressbook/admin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/
+-rw-r--r--   0 simon      (501) staff       (20)      625 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/PKG-INFO
+-rwxr-xr-x   0 simon      (501) staff       (20)      813 2023-05-01 16:43:05.000000 django-addresses-0.2.0b1/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/migrations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-19 14:46:01.000000 django-addresses-0.2.0b1/addressbook/migrations/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1811 2023-04-27 09:44:44.000000 django-addresses-0.2.0b1/addressbook/migrations/0002_auto_20230427_1033.py
+-rw-r--r--   0 simon      (501) staff       (20)     3515 2023-04-27 09:48:04.000000 django-addresses-0.2.0b1/addressbook/migrations/0001_initial.py
+-rw-r--r--   0 simon      (501) staff       (20)     3344 2023-05-01 16:46:15.000000 django-addresses-0.2.0b1/addressbook/models.py
+-rw-r--r--   0 simon      (501) staff       (20)       20 2023-05-01 16:46:54.000000 django-addresses-0.2.0b1/addressbook/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      147 2023-04-27 12:53:46.000000 django-addresses-0.2.0b1/addressbook/apps.py
+-rw-r--r--   0 simon      (501) staff       (20)      176 2023-05-01 16:43:05.000000 django-addresses-0.2.0b1/addressbook/forms.py
+-rw-r--r--   0 simon      (501) staff       (20)      371 2023-05-01 16:43:05.000000 django-addresses-0.2.0b1/addressbook/admin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/fixtures/
+-rw-r--r--   0 simon      (501) staff       (20)    28911 2023-04-27 04:59:03.000000 django-addresses-0.2.0b1/addressbook/fixtures/initial_data.json
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_US/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 simon      (501) staff       (20)     1142 2023-04-19 12:49:14.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_US/LC_MESSAGES/django.po
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_GB/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2023-04-19 12:49:14.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-01 17:14:41.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en/LC_MESSAGES/
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2023-04-19 12:49:14.000000 django-addresses-0.2.0b1/addressbook/conf/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-19 12:49:14.000000 django-addresses-0.2.0b1/addressbook/conf/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      105 2023-05-01 16:43:05.000000 django-addresses-0.2.0b1/addressbook/conf/settings.py
+-rw-r--r--   0 simon      (501) staff       (20)     1390 2023-04-19 12:49:14.000000 django-addresses-0.2.0b1/LICENCE
```

### Comparing `django-addresses-0.1/PKG-INFO` & `django-addresses-0.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-addresses
-Version: 0.1
+Version: 0.2.0b1
 Summary: Some forms around a few models to manage addresses
 Home-page: https://github.com/simonluijk/django-addresses
 Author: Simon Luijk
 Author-email: simon@simonluijk.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-addresses-0.1/LICENCE` & `django-addresses-0.2.0b1/LICENCE`

 * *Files identical despite different names*

### Comparing `django-addresses-0.1/addressbook/conf/locale/en_GB/LC_MESSAGES/django.po` & `django-addresses-0.2.0b1/addressbook/conf/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-addresses-0.1/addressbook/conf/locale/en/LC_MESSAGES/django.po` & `django-addresses-0.2.0b1/addressbook/conf/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-addresses-0.1/addressbook/conf/locale/en_US/LC_MESSAGES/django.po` & `django-addresses-0.2.0b1/addressbook/conf/locale/en_US/LC_MESSAGES/django.po`

 * *Files identical despite different names*

