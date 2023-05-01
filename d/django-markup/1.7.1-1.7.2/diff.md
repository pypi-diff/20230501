# Comparing `tmp/django-markup-1.7.1.tar.gz` & `tmp/django-markup-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-markup-1.7.1.tar", last modified: Wed Apr 26 19:28:29 2023, max compression
+gzip compressed data, was "django-markup-1.7.2.tar", last modified: Mon May  1 15:40:38 2023, max compression
```

## Comparing `django-markup-1.7.1.tar` & `django-markup-1.7.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.711862 django-markup-1.7.1/
--rw-r--r--   0 martin     (501) staff       (20)     2776 2023-04-26 19:19:16.000000 django-markup-1.7.1/CHANGELOG.rst
--rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.7.1/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.7.1/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)     5617 2023-04-26 19:28:29.711967 django-markup-1.7.1/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      582 2023-04-26 19:09:41.000000 django-markup-1.7.1/Pipfile
--rw-r--r--   0 martin     (501) staff       (20)    21963 2023-04-26 19:09:52.000000 django-markup-1.7.1/Pipfile.lock
--rw-r--r--   0 martin     (501) staff       (20)     1888 2023-04-26 19:18:12.000000 django-markup-1.7.1/README.rst
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.703019 django-markup-1.7.1/django_markup/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1259 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/defaults.py
--rw-r--r--   0 martin     (501) staff       (20)     1053 2022-08-14 08:44:22.000000 django-markup-1.7.1/django_markup/fields.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.705373 django-markup-1.7.1/django_markup/filter/
--rw-r--r--   0 martin     (501) staff       (20)      288 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      235 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/creole_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      475 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/linebreaks_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1360 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/markdown_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      237 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/none_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      897 2022-08-14 08:44:39.000000 django-markup-1.7.1/django_markup/filter/rst_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      246 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/smartypants_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      226 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/textile_filter.py
--rw-r--r--   0 martin     (501) staff       (20)      206 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/filter/widont_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     3534 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/markup.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.705645 django-markup-1.7.1/django_markup/templatetags/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/templatetags/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/templatetags/markup_tags.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.706674 django-markup-1.7.1/django_markup/tests/
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/__init__.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.707537 django-markup-1.7.1/django_markup/tests/files/
--rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_header.txt
--rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_header_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_raw.txt
--rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/files/rst_with_pygments.txt
--rw-r--r--   0 martin     (501) staff       (20)      352 2023-04-26 19:13:49.000000 django-markup-1.7.1/django_markup/tests/files/rst_with_pygments_expected.txt
--rw-r--r--   0 martin     (501) staff       (20)     1213 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/markup_strings.py
--rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.7.1/django_markup/tests/settings.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.707851 django-markup-1.7.1/django_markup/tests/templates/
--rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.7.1/django_markup/tests/templates/test_templatetag.html
--rw-r--r--   0 martin     (501) staff       (20)       81 2023-04-26 19:13:10.000000 django-markup-1.7.1/django_markup/tests/templates/test_templatetag_filterwrapper.html
--rw-r--r--   0 martin     (501) staff       (20)     2478 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/test_custom_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     4169 2023-04-26 19:14:13.000000 django-markup-1.7.1/django_markup/tests/test_filter.py
--rw-r--r--   0 martin     (501) staff       (20)     1960 2023-02-26 22:47:46.000000 django-markup-1.7.1/django_markup/tests/test_templatetag.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.703979 django-markup-1.7.1/django_markup.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     5617 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1939 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-26 18:45:56.000000 django-markup-1.7.1/django_markup.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)      171 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       14 2023-04-26 19:28:29.000000 django-markup-1.7.1/django_markup.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.709463 django-markup-1.7.1/docs/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.710383 django-markup-1.7.1/docs/_static/
--rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/basic.css
--rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/default.css
--rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/_static/pygments.css
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-26 19:28:29.711710 django-markup-1.7.1/docs/bundled_filter/
--rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/creole.rst
--rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/linebreaks.rst
--rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/markdown.rst
--rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/none.rst
--rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/rst.rst
--rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/smartypants.rst
--rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/textile.rst
--rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/bundled_filter/widont.rst
--rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/conf.py
--rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/configuration.rst
--rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/filter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/filter_settings.rst
--rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/formatter.rst
--rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/index.rst
--rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/installation.rst
--rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_models.rst
--rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_python.rst
--rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.7.1/docs/usage_templates.rst
--rw-r--r--   0 martin     (501) staff       (20)     1733 2023-04-26 19:28:29.712429 django-markup-1.7.1/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)       59 2023-04-26 19:06:37.000000 django-markup-1.7.1/setup.py
--rw-r--r--   0 martin     (501) staff       (20)      800 2023-04-26 19:24:59.000000 django-markup-1.7.1/tox.ini
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.322691 django-markup-1.7.2/
+-rw-r--r--   0 martin     (501) staff       (20)     3032 2023-05-01 15:40:33.000000 django-markup-1.7.2/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1534 2022-08-14 08:39:58.000000 django-markup-1.7.2/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      266 2022-08-14 08:39:58.000000 django-markup-1.7.2/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     5897 2023-05-01 15:40:38.322777 django-markup-1.7.2/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      452 2023-04-26 19:40:18.000000 django-markup-1.7.2/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    21963 2023-04-26 19:09:52.000000 django-markup-1.7.2/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     1889 2023-05-01 15:38:25.000000 django-markup-1.7.2/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.314980 django-markup-1.7.2/django_markup/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1259 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/defaults.py
+-rw-r--r--   0 martin     (501) staff       (20)     1109 2023-04-26 19:40:21.000000 django-markup-1.7.2/django_markup/fields.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.317296 django-markup-1.7.2/django_markup/filter/
+-rw-r--r--   0 martin     (501) staff       (20)      280 2023-04-26 19:36:31.000000 django-markup-1.7.2/django_markup/filter/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      235 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/creole_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      475 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/linebreaks_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1360 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/markdown_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      237 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/none_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      898 2023-04-26 19:36:31.000000 django-markup-1.7.2/django_markup/filter/rst_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      246 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/smartypants_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      226 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/textile_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)      206 2023-02-26 22:47:46.000000 django-markup-1.7.2/django_markup/filter/widont_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     3566 2023-04-26 19:40:21.000000 django-markup-1.7.2/django_markup/markup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.317552 django-markup-1.7.2/django_markup/templatetags/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/templatetags/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      255 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/templatetags/markup_tags.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.318463 django-markup-1.7.2/django_markup/tests/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.319193 django-markup-1.7.2/django_markup/tests/files/
+-rw-r--r--   0 martin     (501) staff       (20)       85 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/files/rst_header.txt
+-rw-r--r--   0 martin     (501) staff       (20)      212 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/files/rst_header_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)       64 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/files/rst_raw.txt
+-rw-r--r--   0 martin     (501) staff       (20)       87 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/files/rst_with_pygments.txt
+-rw-r--r--   0 martin     (501) staff       (20)      352 2023-04-26 19:13:49.000000 django-markup-1.7.2/django_markup/tests/files/rst_with_pygments_expected.txt
+-rw-r--r--   0 martin     (501) staff       (20)     1172 2023-04-26 19:38:40.000000 django-markup-1.7.2/django_markup/tests/markup_strings.py
+-rw-r--r--   0 martin     (501) staff       (20)      756 2022-08-14 08:48:00.000000 django-markup-1.7.2/django_markup/tests/settings.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.319496 django-markup-1.7.2/django_markup/tests/templates/
+-rw-r--r--   0 martin     (501) staff       (20)       54 2022-08-14 08:39:58.000000 django-markup-1.7.2/django_markup/tests/templates/test_templatetag.html
+-rw-r--r--   0 martin     (501) staff       (20)       81 2023-04-26 19:13:10.000000 django-markup-1.7.2/django_markup/tests/templates/test_templatetag_filterwrapper.html
+-rw-r--r--   0 martin     (501) staff       (20)     2474 2023-04-26 19:38:40.000000 django-markup-1.7.2/django_markup/tests/test_custom_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     4166 2023-04-26 19:38:40.000000 django-markup-1.7.2/django_markup/tests/test_filter.py
+-rw-r--r--   0 martin     (501) staff       (20)     1932 2023-04-26 19:38:40.000000 django-markup-1.7.2/django_markup/tests/test_templatetag.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.315917 django-markup-1.7.2/django_markup.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     5897 2023-05-01 15:40:38.000000 django-markup-1.7.2/django_markup.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1954 2023-05-01 15:40:38.000000 django-markup-1.7.2/django_markup.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-01 15:40:38.000000 django-markup-1.7.2/django_markup.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-01 15:38:40.000000 django-markup-1.7.2/django_markup.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)      171 2023-05-01 15:40:38.000000 django-markup-1.7.2/django_markup.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       14 2023-05-01 15:40:38.000000 django-markup-1.7.2/django_markup.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.320992 django-markup-1.7.2/docs/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.321416 django-markup-1.7.2/docs/_static/
+-rw-r--r--   0 martin     (501) staff       (20)     6488 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/_static/basic.css
+-rw-r--r--   0 martin     (501) staff       (20)     3791 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/_static/default.css
+-rw-r--r--   0 martin     (501) staff       (20)     2717 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/_static/pygments.css
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-01 15:40:38.322558 django-markup-1.7.2/docs/bundled_filter/
+-rw-r--r--   0 martin     (501) staff       (20)      252 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/creole.rst
+-rw-r--r--   0 martin     (501) staff       (20)      300 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/linebreaks.rst
+-rw-r--r--   0 martin     (501) staff       (20)      418 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/markdown.rst
+-rw-r--r--   0 martin     (501) staff       (20)      126 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/none.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2263 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/rst.rst
+-rw-r--r--   0 martin     (501) staff       (20)      314 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/smartypants.rst
+-rw-r--r--   0 martin     (501) staff       (20)      500 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/textile.rst
+-rw-r--r--   0 martin     (501) staff       (20)      208 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/bundled_filter/widont.rst
+-rw-r--r--   0 martin     (501) staff       (20)     6322 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/conf.py
+-rw-r--r--   0 martin     (501) staff       (20)      384 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/configuration.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1211 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/filter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1351 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/filter_settings.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2689 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/formatter.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1183 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/index.rst
+-rw-r--r--   0 martin     (501) staff       (20)      773 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/installation.rst
+-rw-r--r--   0 martin     (501) staff       (20)      759 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/usage_models.rst
+-rw-r--r--   0 martin     (501) staff       (20)      107 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/usage_python.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1137 2022-08-14 08:39:58.000000 django-markup-1.7.2/docs/usage_templates.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2285 2023-04-26 19:42:47.000000 django-markup-1.7.2/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)     1185 2023-05-01 15:40:38.323111 django-markup-1.7.2/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)       59 2023-04-26 19:06:37.000000 django-markup-1.7.2/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      669 2023-05-01 15:22:27.000000 django-markup-1.7.2/tox.ini
```

### Comparing `django-markup-1.7.1/CHANGELOG.rst` & `django-markup-1.7.2/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+v1.7.2 (2023-05-01):
+--------------------
+
+- Fixed a setup.cfg bug that defined the minimal Django version to be v3.7 which does
+  not exist. The correct version is 3.2.
+
+v1.7.1 (2023-04-25):
+--------------------
+
+- Fixed Python classifiers in setup.cfg.
+
 v1.7 (2023-04-25):
 ------------------
 
 - Django 4.2 compatibility and tests.
 - Python 3.11 compatibility and tests.
 
 v1.6 (2022-08-14):
```

### Comparing `django-markup-1.7.1/LICENSE` & `django-markup-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/PKG-INFO` & `django-markup-1.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.7.1
+Version: 1.7.2
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Keywords: django,markup,markdown,restructuredtext,format,text
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
+Requires-Python: >=3.7
 Provides-Extra: all_filter_dependencies
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/django-markup.svg
     :target: https://pypi.org/project/django-markup/
 
 .. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
@@ -92,17 +93,29 @@
     $ pipenv run test
 
 You can also test against a variation of Django and Python versions
 using tox::
 
     $ tox
 
+
 Changelog
 =========
 
+v1.7.2 (2023-05-01):
+--------------------
+
+- Fixed a setup.cfg bug that defined the minimal Django version to be v3.7 which does
+  not exist. The correct version is 3.2.
+
+v1.7.1 (2023-04-25):
+--------------------
+
+- Fixed Python classifiers in setup.cfg.
+
 v1.7 (2023-04-25):
 ------------------
 
 - Django 4.2 compatibility and tests.
 - Python 3.11 compatibility and tests.
 
 v1.6 (2022-08-14):
```

### Comparing `django-markup-1.7.1/Pipfile.lock` & `django-markup-1.7.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/README.rst` & `django-markup-1.7.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,7 +67,8 @@
     % pipenv install --dev
     $ pipenv run test
 
 You can also test against a variation of Django and Python versions
 using tox::
 
     $ tox
+
```

### Comparing `django-markup-1.7.1/django_markup/defaults.py` & `django-markup-1.7.2/django_markup/defaults.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/django_markup/fields.py` & `django-markup-1.7.2/django_markup/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     """
 
     def __init__(self, default=False, formatter=formatter, *args, **kwargs):
         # Check that the default value is a valid filter
         if default:
             if default not in formatter.filter_list:
                 raise ImproperlyConfigured(
-                    "'%s' is not a registered markup filter. Registered filters are: %s."
-                    % (default, ", ".join(formatter.filter_list.keys()))
+                    "'{}' is not a registered markup filter. Registered filters are: {}.".format(
+                        default,
+                        ", ".join(formatter.filter_list.keys()),
+                    ),
                 )
             kwargs.setdefault("default", default)
 
         kwargs.setdefault("max_length", 255)
         kwargs.setdefault("choices", formatter.choices())
         kwargs.setdefault("verbose_name", gettext_lazy("markup"))
         CharField.__init__(self, *args, **kwargs)
```

### Comparing `django-markup-1.7.1/django_markup/filter/markdown_filter.py` & `django-markup-1.7.2/django_markup/filter/markdown_filter.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/django_markup/filter/rst_filter.py` & `django-markup-1.7.2/django_markup/filter/rst_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     title = "reStructuredText"
     rst_part_name = "html_body"
     kwargs = {
         "settings_overrides": {
             "raw_enabled": False,
             "file_insertion_enabled": False,
-        }
+        },
     }
 
     def render(self, text, **kwargs):
         if kwargs:
             self.kwargs.update(kwargs)
         from docutils import core
```

### Comparing `django-markup-1.7.1/django_markup/markup.py` & `django-markup-1.7.2/django_markup/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from django.conf import settings
 
-from django_markup.defaults import (
-    DEFAULT_MARKUP_CHOICES, DEFAULT_MARKUP_FILTER
-)
+from django_markup.defaults import DEFAULT_MARKUP_CHOICES, DEFAULT_MARKUP_FILTER
 
 
-class MarkupFormatter(object):
+class MarkupFormatter:
     def __init__(self, load_defaults=True):
         self.filter_list = {}
 
         if load_defaults:
             filter_list = getattr(settings, "MARKUP_FILTER", DEFAULT_MARKUP_FILTER)
             for filter_name, filter_class in filter_list.items():
                 self.register(filter_name, filter_class)
@@ -75,16 +73,18 @@
         filter_fallback = getattr(settings, "MARKUP_FILTER_FALLBACK", False)
         if not filter_name and filter_fallback:
             filter_name = filter_fallback
 
         # Check that the filter_name is a registered markup filter
         if filter_name not in self.filter_list:
             raise ValueError(
-                "'%s' is not a registered markup filter. Registered filters are: %s."
-                % (filter_name, ", ".join(self.filter_list.keys()))
+                "'{}' is not a registered markup filter. Registered filters are: {}.".format(
+                    filter_name,
+                    ", ".join(self.filter_list.keys()),
+                ),
             )
         filter_class = self.filter_list[filter_name]
 
         # Read global filter settings and apply it
         filter_kwargs = {}
         filter_settings = getattr(settings, "MARKUP_SETTINGS", {})
         if filter_name in filter_settings:
```

### Comparing `django-markup-1.7.1/django_markup/tests/markup_strings.py` & `django-markup-1.7.2/django_markup/tests/markup_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 """
 Sample Markup strings and their expected pendant.
 """
 
 NONE = ("*This* is some text.", "*This* is some text.")
 
 # Django's linebreaks filter
```

### Comparing `django-markup-1.7.1/django_markup/tests/settings.py` & `django-markup-1.7.2/django_markup/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/django_markup/tests/test_custom_filter.py` & `django-markup-1.7.2/django_markup/tests/test_custom_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 from django.test import TestCase
 
 from django_markup.filter import MarkupFilter
 from django_markup.markup import formatter
 
 
 class UppercaseMarkupFilter(MarkupFilter):
@@ -60,15 +58,18 @@
 
         # Unregistering an registered filter, and it no longer works and will
         # raise a ValueError.
         formatter.register("uppercase", UppercaseMarkupFilter)
         formatter.unregister("uppercase")
 
         self.assertRaises(
-            ValueError, formatter, "This is some text", filter_name="uppercase"
+            ValueError,
+            formatter,
+            "This is some text",
+            filter_name="uppercase",
         )
 
     def test_fallback_filter(self):
         """
         You can call the formatter without a `filter_name` as long as a
         `MARKUP_FILTER_FALLBACK` setting is set.
         """
```

### Comparing `django-markup-1.7.1/django_markup/tests/test_filter.py` & `django-markup-1.7.2/django_markup/tests/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 import os
 
 from django.test import TestCase
 
 from ..markup import formatter
 from . import markup_strings as s
 
@@ -16,15 +14,18 @@
     """
 
     def test_unregistered_filter_fails_loud(self):
         """
         Trying to call a unregistered filter will raise a ValueError.
         """
         self.assertRaises(
-            ValueError, formatter, "some text", filter_name="does-not-exist"
+            ValueError,
+            formatter,
+            "some text",
+            filter_name="does-not-exist",
         )
 
     def test_none_filter(self):
         text, expected = s.NONE
         result = formatter(text, filter_name="none")
         self.assertEqual(result, expected)
 
@@ -74,15 +75,15 @@
     def test_rst_with_pygments(self):
         """
         Having Pygments installed will automatically provide a ``.. code-block``
         directive in reStructredText to highlight code snippets.
         """
         text = open(os.path.join(FILES_DIR, "rst_with_pygments.txt")).read()
         expected = open(
-            os.path.join(FILES_DIR, "rst_with_pygments_expected.txt")
+            os.path.join(FILES_DIR, "rst_with_pygments_expected.txt"),
         ).read()
         result = formatter(text, filter_name="restructuredtext")
 
         self.assertEqual(result, expected)
 
     def test_rst_raw_default(self):
         """Raw file inclusion is disabled by default."""
```

### Comparing `django-markup-1.7.1/django_markup/tests/test_templatetag.py` & `django-markup-1.7.2/django_markup/tests/test_templatetag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 from django.template.loader import render_to_string
 from django.test import TestCase
 
 from ..templatetags.markup_tags import apply_markup
 from . import markup_strings as s
 
 
@@ -35,15 +33,16 @@
         """
         Test usage as a template tag:
 
             {{ "some text"|apply_markup:"markdown" }}
         """
         text, expected = s.MARKDOWN
         result = render_to_string(
-            "test_templatetag.html", {"text": text, "filter": "markdown"}
+            "test_templatetag.html",
+            {"text": text, "filter": "markdown"},
         )
 
         # Strip leading and trailing whitespace from the rendered HTL
         result = result.strip()
 
         self.assertEqual(result, expected)
```

### Comparing `django-markup-1.7.1/django_markup.egg-info/PKG-INFO` & `django-markup-1.7.2/django_markup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-markup
-Version: 1.7.1
+Version: 1.7.2
 Summary: A generic Django application to convert text with specific markup to html.
 Home-page: https://github.com/bartTC/django-markup
 Author: Martin Mahner
 Author-email: martin@mahner.org
 License: MIT
 Keywords: django,markup,markdown,restructuredtext,format,text
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
+Requires-Python: >=3.7
 Provides-Extra: all_filter_dependencies
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/django-markup.svg
     :target: https://pypi.org/project/django-markup/
 
 .. image:: https://github.com/bartTC/django-markup/actions/workflows/push.yml/badge.svg?branch=main
@@ -92,17 +93,29 @@
     $ pipenv run test
 
 You can also test against a variation of Django and Python versions
 using tox::
 
     $ tox
 
+
 Changelog
 =========
 
+v1.7.2 (2023-05-01):
+--------------------
+
+- Fixed a setup.cfg bug that defined the minimal Django version to be v3.7 which does
+  not exist. The correct version is 3.2.
+
+v1.7.1 (2023-04-25):
+--------------------
+
+- Fixed Python classifiers in setup.cfg.
+
 v1.7 (2023-04-25):
 ------------------
 
 - Django 4.2 compatibility and tests.
 - Python 3.11 compatibility and tests.
 
 v1.6 (2022-08-14):
```

### Comparing `django-markup-1.7.1/django_markup.egg-info/SOURCES.txt` & `django-markup-1.7.2/django_markup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 Pipfile
 Pipfile.lock
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 django_markup/__init__.py
 django_markup/defaults.py
 django_markup/fields.py
 django_markup/markup.py
```

### Comparing `django-markup-1.7.1/docs/_static/basic.css` & `django-markup-1.7.2/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/_static/default.css` & `django-markup-1.7.2/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/_static/pygments.css` & `django-markup-1.7.2/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/bundled_filter/rst.rst` & `django-markup-1.7.2/docs/bundled_filter/rst.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/conf.py` & `django-markup-1.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/filter.rst` & `django-markup-1.7.2/docs/filter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/filter_settings.rst` & `django-markup-1.7.2/docs/filter_settings.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/formatter.rst` & `django-markup-1.7.2/docs/formatter.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/index.rst` & `django-markup-1.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/installation.rst` & `django-markup-1.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/usage_models.rst` & `django-markup-1.7.2/docs/usage_models.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/docs/usage_templates.rst` & `django-markup-1.7.2/docs/usage_templates.rst`

 * *Files identical despite different names*

### Comparing `django-markup-1.7.1/tox.ini` & `django-markup-1.7.2/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 [tox]
 toxworkdir=/tmp/tox/django-markup
 skip_missing_interpreters=True
 envlist=
-    readme
     py{37,38,39,310,311}-django-{32}
     py{38,39,310,311}-django-{40,41,42}
 
 [gh-actions]
 python =
     readme: py37
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
 
-
 [testenv]
+install_command =
+    pip install {opts} {packages}
+setenv =
+    DJANGO_SETTINGS_MODULE=django_markup.tests.settings
 commands=
-    py.test --pyargs --cov={envsitepackagesdir}/django_markup django_markup
+    {envbindir}/django-admin --version
+    pytest {envsitepackagesdir}/django_markup
 extras=all_filter_dependencies
 deps=
     # Django versions
     django-32: django==3.2.*
     django-40: django==4.0.*
     django-41: django==4.1.*
-    coverage
     pytest
-    pytest-cov
-    pytest-Django
-
-[testenv:readme]
-skip_install = True
-deps =
-    docutils
-    Pygments
-commands =
-    rst2html.py --report=info --halt=warning README.rst /dev/null
-    rst2html.py --report=info --halt=warning CHANGELOG.rst /dev/null
+    pytest-django
```

