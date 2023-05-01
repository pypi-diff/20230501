# Comparing `tmp/trytond_stock_supply_forecast-6.6.0.tar.gz` & `tmp/trytond_stock_supply_forecast-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply_forecast-6.6.0.tar", last modified: Mon Oct 31 16:22:10 2022, max compression
+gzip compressed data, was "trytond_stock_supply_forecast-6.8.0.tar", last modified: Mon May  1 11:59:00 2023, max compression
```

## Comparing `trytond_stock_supply_forecast-6.6.0.tar` & `trytond_stock_supply_forecast-6.8.0.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:10.840098 trytond_stock_supply_forecast-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:17.000000 trytond_stock_supply_forecast-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_stock_supply_forecast-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2022-10-31 16:22:09.000000 trytond_stock_supply_forecast-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:34.000000 trytond_stock_supply_forecast-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1882 2022-10-31 16:22:08.000000 trytond_stock_supply_forecast-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:22:08.000000 trytond_stock_supply_forecast-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:55:23.000000 trytond_stock_supply_forecast-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:48.000000 trytond_stock_supply_forecast-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2455 2022-10-31 16:22:10.840098 trytond_stock_supply_forecast-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2019-06-04 16:49:46.000000 trytond_stock_supply_forecast-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2022-04-08 16:23:27.000000 trytond_stock_supply_forecast-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:10.836765 trytond_stock_supply_forecast-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      150 2019-06-04 16:49:46.000000 trytond_stock_supply_forecast-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:22:10.840098 trytond_stock_supply_forecast-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5231 2022-10-29 07:39:12.000000 trytond_stock_supply_forecast-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2022-04-08 16:23:27.000000 trytond_stock_supply_forecast-6.6.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:10.836765 trytond_stock_supply_forecast-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:57.000000 trytond_stock_supply_forecast-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2956 2020-07-09 09:37:34.000000 trytond_stock_supply_forecast-6.6.0/tests/scenario_stock_supply_forecast.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2022-04-16 16:30:57.000000 trytond_stock_supply_forecast-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-04-25 16:11:54.000000 trytond_stock_supply_forecast-6.6.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2022-10-31 15:10:09.000000 trytond_stock_supply_forecast-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       75 2022-10-31 16:22:07.000000 trytond_stock_supply_forecast-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:22:10.840098 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2455 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:22:10.000000 trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:00.752043 trytond_stock_supply_forecast-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2045 2023-05-01 11:12:56.000000 trytond_stock_supply_forecast-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:12:56.000000 trytond_stock_supply_forecast-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_forecast-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2441 2023-05-01 11:59:00.748710 trytond_stock_supply_forecast-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:00.748710 trytond_stock_supply_forecast-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      150 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:59:00.752043 trytond_stock_supply_forecast-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4414 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:00.745376 trytond_stock_supply_forecast-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2897 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/tests/scenario_stock_supply_forecast.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock_supply_forecast-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       75 2023-05-01 11:12:51.000000 trytond_stock_supply_forecast-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:59:00.748710 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2441 2023-05-01 11:58:59.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      749 2023-05-01 11:59:00.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:58:59.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:58:59.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-05-01 11:58:59.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:58:59.000000 trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/top_level.txt
```

### Comparing `trytond_stock_supply_forecast-6.6.0/CHANGELOG` & `trytond_stock_supply_forecast-6.8.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+Version 6.8.0 - 2023-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
+
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
 * Setup forecast for all supplies
```

### Comparing `trytond_stock_supply_forecast-6.6.0/COPYRIGHT` & `trytond_stock_supply_forecast-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2011-2022 Cédric Krier.
-Copyright (C) 2011-2022 B2CK SPRL.
+Copyright (C) 2011-2023 Cédric Krier.
+Copyright (C) 2011-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_supply_forecast-6.6.0/LICENSE` & `trytond_stock_supply_forecast-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-6.6.0/PKG-INFO` & `trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_stock_supply_forecast
-Version: 6.6.0
+Name: trytond-stock-supply-forecast
+Version: 6.8.0
 Summary: Tryton module to add forecast to supply computation
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply_forecast
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Stock Supply Forecast Module
 ############################
 
 The stock supply forecast module takes forecast into account to compute
```

### Comparing `trytond_stock_supply_forecast-6.6.0/setup.py` & `trytond_stock_supply_forecast-6.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 def read(fname):
     return io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -34,60 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock_supply_forecast'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
 if minor_version % 2:
-    version = '%s.%s.dev0' % (major_version, minor_version)
-    download_url = (
-        'hg+http://hg.tryton.org/modules/%s#egg=%s-%s' % (
-            name[8:], name, version))
-local_version = []
-if os.environ.get('CI_JOB_ID'):
-    local_version.append(os.environ['CI_JOB_ID'])
+    download_url = ''
 else:
-    for build in ['CI_BUILD_NUMBER', 'CI_JOB_NUMBER']:
-        if os.environ.get(build):
-            local_version.append(os.environ[build])
-        else:
-            local_version = []
-            break
-if local_version:
-    version += '+' + '.'.join(local_version)
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module to add forecast to supply computation',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/stock_supply_forecast',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock supply forecast',
     package_dir={'trytond.modules.stock_supply_forecast': '.'},
     packages=(
         ['trytond.modules.stock_supply_forecast']
         + ['trytond.modules.stock_supply_forecast.%s' % p
             for p in find_packages()]
@@ -125,27 +103,26 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'test': tests_require,
         },
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     stock_supply_forecast = trytond.modules.stock_supply_forecast
     """,
     )
```

### Comparing `trytond_stock_supply_forecast-6.6.0/stock.py` & `trytond_stock_supply_forecast-6.8.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_forecast-6.6.0/tests/scenario_stock_supply_forecast.rst` & `trytond_stock_supply_forecast-6.8.0/tests/scenario_stock_supply_forecast.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 ==============================
 Stock Supply Forecast Scenario
 ==============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
     >>> from trytond.modules.account.tests.tools import (create_chart,
     ...     get_accounts)
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
-    >>> tomorrow = today + relativedelta(days=1)
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply_forecast')
 
 Create company::
```

### Comparing `trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/PKG-INFO` & `trytond_stock_supply_forecast-6.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-stock-supply-forecast
-Version: 6.6.0
+Name: trytond_stock_supply_forecast
+Version: 6.8.0
 Summary: Tryton module to add forecast to supply computation
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock_supply_forecast
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock supply forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Stock Supply Forecast Module
 ############################
 
 The stock supply forecast module takes forecast into account to compute
```

### Comparing `trytond_stock_supply_forecast-6.6.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt` & `trytond_stock_supply_forecast-6.8.0/trytond_stock_supply_forecast.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-.drone.yml
-.flake8
-.hgtags
-.isort.cfg
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 setup.py
@@ -15,14 +11,15 @@
 ./__init__.py
 ./stock.py
 ./tryton.cfg
 ./tests/__init__.py
 ./tests/scenario_stock_supply_forecast.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
+doc/conf.py
 doc/index.rst
 tests/__init__.py
 tests/scenario_stock_supply_forecast.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_stock_supply_forecast.egg-info/PKG-INFO
 trytond_stock_supply_forecast.egg-info/SOURCES.txt
```

