# Comparing `tmp/django-ical-1.9.0.tar.gz` & `tmp/django-ical-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ical-1.9.0.tar", last modified: Tue Apr  4 19:19:18 2023, max compression
+gzip compressed data, was "django-ical-1.9.1.tar", last modified: Mon May  1 08:19:54 2023, max compression
```

## Comparing `django-ical-1.9.0.tar` & `django-ical-1.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.541408 django-ical-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 19:19:03.000000 django-ical-1.9.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.517408 django-ical-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.529408 django-ical-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-04 19:19:03.000000 django-ical-1.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-04 19:19:03.000000 django-ical-1.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 19:19:03.000000 django-ical-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 19:19:03.000000 django-ical-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-04 19:19:03.000000 django-ical-1.9.0/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-04 19:19:03.000000 django-ical-1.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-04 19:19:03.000000 django-ical-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-04 19:19:03.000000 django-ical-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-04 19:19:03.000000 django-ical-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 19:19:03.000000 django-ical-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-04 19:19:18.537408 django-ical-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-04 19:19:03.000000 django-ical-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.529408 django-ical-1.9.0/django_ical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/feedgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.533408 django-ical-1.9.0/django_ical/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19424 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/tests/test_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/tests/test_recurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-04 19:19:03.000000 django-ical-1.9.0/django_ical/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.533408 django-ical-1.9.0/django_ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-04 19:19:18.000000 django-ical-1.9.0/django_ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-04 19:19:18.000000 django-ical-1.9.0/django_ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:19:18.000000 django-ical-1.9.0/django_ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-04 19:19:18.000000 django-ical-1.9.0/django_ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 19:19:18.000000 django-ical-1.9.0/django_ical.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.533408 django-ical-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.537408 django-ical-1.9.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/django_ical.feedgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:19:18.537408 django-ical-1.9.0/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/reference/django_ical.feedgenerator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/reference/django_ical.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/reference/django_ical.views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-04-04 19:19:03.000000 django-ical-1.9.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-04 19:19:03.000000 django-ical-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:19:18.541408 django-ical-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-04 19:19:03.000000 django-ical-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-04 19:19:03.000000 django-ical-1.9.0/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-04 19:19:03.000000 django-ical-1.9.0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-04 19:19:03.000000 django-ical-1.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 08:19:34.000000 django-ical-1.9.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.136628 django-ical-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 08:19:34.000000 django-ical-1.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-01 08:19:34.000000 django-ical-1.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 08:19:34.000000 django-ical-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 08:19:34.000000 django-ical-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 08:19:34.000000 django-ical-1.9.1/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-01 08:19:34.000000 django-ical-1.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-01 08:19:34.000000 django-ical-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-01 08:19:34.000000 django-ical-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 08:19:34.000000 django-ical-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 08:19:34.000000 django-ical-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-01 08:19:54.144627 django-ical-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-01 08:19:34.000000 django-ical-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/feedgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/test_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/test_recurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/django_ical.feedgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.feedgenerator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 08:19:34.000000 django-ical-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:19:54.144627 django-ical-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-01 08:19:34.000000 django-ical-1.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 08:19:34.000000 django-ical-1.9.1/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-01 08:19:34.000000 django-ical-1.9.1/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-01 08:19:34.000000 django-ical-1.9.1/tox.ini
```

### Comparing `django-ical-1.9.0/.github/workflows/release.yml` & `django-ical-1.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/.github/workflows/test.yml` & `django-ical-1.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/CHANGES.rst` & `django-ical-1.9.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 
 Changes
 =======
 
 
+1.9.1 (2023-05-01)
+------------------
+
+- Fix multiple CATEGORIES and add tests
+  [mjfinney]
+
+
 1.9.0 (2023-04-04)
 ------------------
 
 - Support for iCalendar VTODO elements
   [wetneb]
```

### Comparing `django-ical-1.9.0/CODE_OF_CONDUCT.md` & `django-ical-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/LICENSE` & `django-ical-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/PKG-INFO` & `django-ical-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ical
-Version: 1.9.0
+Version: 1.9.1
 Summary: iCal feeds for Django based on Django's syndication feed framework.
 Home-page: https://github.com/jazzband/django-ical
 Author: Ian Lewis
 Author-email: security@jazzband.com
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.com
 License: MIT License
@@ -82,14 +82,21 @@
    :alt: Jazzband
 
 
 Changes
 =======
 
 
+1.9.1 (2023-05-01)
+------------------
+
+- Fix multiple CATEGORIES and add tests
+  [mjfinney]
+
+
 1.9.0 (2023-04-04)
 ------------------
 
 - Support for iCalendar VTODO elements
   [wetneb]
```

### Comparing `django-ical-1.9.0/README.rst` & `django-ical-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/django_ical/feedgenerator.py` & `django-ical-1.9.1/django_ical/feedgenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 ...     link="http://www.example.com/events.ical",
 ...     description="A iCalendar feed of my events.",
 ...     language="en",
 ... )
 >>> feed.add_item(
 ...     title="Hello",
 ...     link="http://www.example.com/test/",
-...     description="Testing."
+...     description="Testing.",
 ...     start_datetime=datetime(2012, 5, 6, 10, 00),
 ...     end_datetime=datetime(2012, 5, 6, 12, 00),
 ... )
->>> fp = open('test.ical', 'w')
+>>> fp = open('test.ical', 'wb')
 >>> feed.write(fp, 'utf-8')
 >>> fp.close()
 
 For definitions of the iCalendar format see:
 http://www.ietf.org/rfc/rfc2445.txt
 """
 
@@ -70,15 +70,14 @@
     ("valarm", None),
     # additional properties supported by the Todo class (VTODO calendar component).
     # see https://icalendar.readthedocs.io/en/latest/_modules/icalendar/cal.html#Todo
     ("completed", "completed"),
     ("percent_complete", "percent-complete"),
     ("priority", "priority"),
     ("due", "due"),
-    ("categories", "categories"),
 )
 
 class ICal20Feed(SyndicationFeed):
     """
     iCalendar 2.0 Feed implementation.
     """
```

### Comparing `django-ical-1.9.0/django_ical/tests/test_feed.py` & `django-ical-1.9.1/django_ical/tests/test_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
                 "geolocation": (37.386013, -122.082932),
                 "modified": datetime(2012, 5, 7, 10, 0),
                 "organizer": {
                     "cn": "John Doe",
                     "email": "john.doe@example.com",
                     "role": "CHAIR",
                 },
+                "categories": ['Cat1', 'Cat2'],
                 "alarms": [
                     {
                         "trigger": timedelta(minutes=-30),
                         "action": "DISPLAY",
                         "description": "Alarm2a",
                     },
                     {
@@ -372,14 +373,17 @@
         self.assertEqual(
             calendar.subcomponents[1]["LAST-MODIFIED"].to_ical(), b"20120507T100000Z"
         )
         self.assertEqual(
             calendar.subcomponents[1]["ORGANIZER"].to_ical(),
             b"MAILTO:john.doe@example.com",
         )
+        self.assertEqual(
+            calendar.subcomponents[1]["CATEGORIES"].to_ical(), b"Cat1,Cat2"
+        )
         self.assertIn(
             b"BEGIN:VALARM\r\nACTION:DISPLAY\r\nDESCRIPTION:Alarm2a\r\nTRIGGER:-PT30M\r\nEND:VALARM\r\n",
             [comp.to_ical() for comp in calendar.subcomponents[1].subcomponents],
         )
         self.assertIn(
             b"BEGIN:VALARM\r\nACTION:DISPLAY\r\nDESCRIPTION:Alarm2b\r\nTRIGGER:-P1D\r\nEND:VALARM\r\n",
             [comp.to_ical() for comp in calendar.subcomponents[1].subcomponents],
@@ -403,15 +407,15 @@
             calendar.subcomponents[2]["ORGANIZER"].to_ical(),
             b"MAILTO:bossy.martin@example.com",
         )
         self.assertEqual(
             calendar.subcomponents[2]["PRIORITY"].to_ical(), b"1"
         )
         self.assertEqual(
-            calendar.subcomponents[2]["CATEGORIES"][0].to_ical(), b"CLEANING"
+            calendar.subcomponents[2]["CATEGORIES"].to_ical(), b"CLEANING"
         )
         self.assertEqual(
             calendar.subcomponents[2]["PERCENT-COMPLETE"].to_ical(), b"89"
         )
 
     def test_wr_timezone(self):
         """
```

### Comparing `django-ical-1.9.0/django_ical/tests/test_recurrence.py` & `django-ical-1.9.1/django_ical/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/django_ical/utils.py` & `django-ical-1.9.1/django_ical/utils.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/django_ical/views.py` & `django-ical-1.9.1/django_ical/views.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/django_ical.egg-info/PKG-INFO` & `django-ical-1.9.1/django_ical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ical
-Version: 1.9.0
+Version: 1.9.1
 Summary: iCal feeds for Django based on Django's syndication feed framework.
 Home-page: https://github.com/jazzband/django-ical
 Author: Ian Lewis
 Author-email: security@jazzband.com
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.com
 License: MIT License
@@ -82,14 +82,21 @@
    :alt: Jazzband
 
 
 Changes
 =======
 
 
+1.9.1 (2023-05-01)
+------------------
+
+- Fix multiple CATEGORIES and add tests
+  [mjfinney]
+
+
 1.9.0 (2023-04-04)
 ------------------
 
 - Support for iCalendar VTODO elements
   [wetneb]
```

### Comparing `django-ical-1.9.0/django_ical.egg-info/SOURCES.txt` & `django-ical-1.9.1/django_ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/docs/Makefile` & `django-ical-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/docs/make.bat` & `django-ical-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/docs/source/conf.py` & `django-ical-1.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/docs/source/index.rst` & `django-ical-1.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/docs/source/usage.rst` & `django-ical-1.9.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/setup.py` & `django-ical-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/tests.py` & `django-ical-1.9.1/tests.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.0/tox.ini` & `django-ical-1.9.1/tox.ini`

 * *Files identical despite different names*

