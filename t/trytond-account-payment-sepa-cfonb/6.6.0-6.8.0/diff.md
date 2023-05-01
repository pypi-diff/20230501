# Comparing `tmp/trytond_account_payment_sepa_cfonb-6.6.0.tar.gz` & `tmp/trytond_account_payment_sepa_cfonb-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_sepa_cfonb-6.6.0.tar", last modified: Mon Oct 31 16:18:47 2022, max compression
+gzip compressed data, was "trytond_account_payment_sepa_cfonb-6.8.0.tar", last modified: Mon May  1 11:51:57 2023, max compression
```

## Comparing `trytond_account_payment_sepa_cfonb-6.6.0.tar` & `trytond_account_payment_sepa_cfonb-6.8.0.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:47.306878 trytond_account_payment_sepa_cfonb-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_payment_sepa_cfonb-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_payment_sepa_cfonb-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      752 2022-10-31 16:18:45.000000 trytond_account_payment_sepa_cfonb-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_payment_sepa_cfonb-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1315 2022-10-31 16:18:45.000000 trytond_account_payment_sepa_cfonb-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2022-10-31 16:18:44.000000 trytond_account_payment_sepa_cfonb-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 09:54:16.000000 trytond_account_payment_sepa_cfonb-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2466 2022-10-31 16:18:47.306878 trytond_account_payment_sepa_cfonb-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2018-08-18 09:54:16.000000 trytond_account_payment_sepa_cfonb-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2021-12-11 16:59:32.000000 trytond_account_payment_sepa_cfonb-6.6.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:47.303545 trytond_account_payment_sepa_cfonb-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2018-08-18 09:54:16.000000 trytond_account_payment_sepa_cfonb-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1709 2021-12-11 16:59:32.000000 trytond_account_payment_sepa_cfonb-6.6.0/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 16:18:47.306878 trytond_account_payment_sepa_cfonb-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5337 2022-10-29 07:39:10.000000 trytond_account_payment_sepa_cfonb-6.6.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:47.303545 trytond_account_payment_sepa_cfonb-6.6.0/template/
--rw-r--r--   0 ced       (1000) ced       (1000)     2627 2019-10-11 23:09:47.000000 trytond_account_payment_sepa_cfonb-6.6.0/template/base-cfonb.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4052 2020-02-17 22:15:13.000000 trytond_account_payment_sepa_cfonb-6.6.0/template/pain.001.001.03-cfonb.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4729 2020-04-20 12:46:41.000000 trytond_account_payment_sepa_cfonb-6.6.0/template/pain.008.001.02-cfonb.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:47.303545 trytond_account_payment_sepa_cfonb-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:56.000000 trytond_account_payment_sepa_cfonb-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      952 2022-04-16 16:30:56.000000 trytond_account_payment_sepa_cfonb-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2022-10-31 15:10:09.000000 trytond_account_payment_sepa_cfonb-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2022-10-31 16:18:43.000000 trytond_account_payment_sepa_cfonb-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 16:18:47.306878 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2466 2022-10-31 16:18:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      876 2022-10-31 16:18:47.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 16:18:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-10-31 16:18:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:02.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2022-10-31 16:18:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 16:18:46.000000 trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:57.683459 trytond_account_payment_sepa_cfonb-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1478 2023-05-01 11:08:02.000000 trytond_account_payment_sepa_cfonb-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:08:01.000000 trytond_account_payment_sepa_cfonb-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2447 2023-05-01 11:51:57.683459 trytond_account_payment_sepa_cfonb-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:57.680126 trytond_account_payment_sepa_cfonb-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:20.000000 trytond_account_payment_sepa_cfonb-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1709 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:51:57.683459 trytond_account_payment_sepa_cfonb-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4500 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:57.676793 trytond_account_payment_sepa_cfonb-6.8.0/template/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2627 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/template/base-cfonb.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4052 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/template/pain.001.001.03-cfonb.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4729 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/template/pain.008.001.02-cfonb.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:57.680126 trytond_account_payment_sepa_cfonb-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      952 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_payment_sepa_cfonb-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-05-01 11:07:55.000000 trytond_account_payment_sepa_cfonb-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:51:57.683459 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2447 2023-05-01 11:51:56.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      850 2023-05-01 11:51:57.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:51:56.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 11:51:56.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-05-01 11:51:56.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:51:56.000000 trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/top_level.txt
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/CHANGELOG` & `trytond_account_payment_sepa_cfonb-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

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
 * Add support for Python 3.10
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/COPYRIGHT` & `trytond_account_payment_sepa_cfonb-6.8.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2014-2022 Cédric Krier.
-Copyright (C) 2014-2022 B2CK SPRL.
+Copyright (C) 2014-2023 Cédric Krier.
+Copyright (C) 2014-2023 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/LICENSE` & `trytond_account_payment_sepa_cfonb-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/PKG-INFO` & `trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_account_payment_sepa_cfonb
-Version: 6.6.0
+Name: trytond-account-payment-sepa-cfonb
+Version: 6.8.0
 Summary: Tryton module for CFONB SEPA payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_sepa_cfonb
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment SEPA CFONB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Account Payment SEPA CFONB Module
 #################################
 
 The account_payment_sepa_cfonb module adds CFONB flavors to SEPA messages.
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/payment.py` & `trytond_account_payment_sepa_cfonb-6.8.0/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/setup.py` & `trytond_account_payment_sepa_cfonb-6.8.0/setup.py`

 * *Files 18% similar despite different names*

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
@@ -34,61 +31,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_payment_sepa_cfonb'
 
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
 
 requires = ['Genshi', 'lxml']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = []
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
 
 setup(name=name,
     version=version,
     description='Tryton module for CFONB SEPA payment',
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
-        "Source Code": (
-            'https://hg.tryton.org/modules/account_payment_sepa_cfonb'),
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment SEPA CFONB',
     package_dir={'trytond.modules.account_payment_sepa_cfonb': '.'},
     packages=(
         ['trytond.modules.account_payment_sepa_cfonb']
         + ['trytond.modules.account_payment_sepa_cfonb.%s' % p
             for p in find_packages()]
@@ -126,28 +103,27 @@
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
         'Topic :: Office/Business :: Financial :: Accounting',
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
     account_payment_sepa_cfonb = trytond.modules.account_payment_sepa_cfonb
     """,
     )
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/template/base-cfonb.xml` & `trytond_account_payment_sepa_cfonb-6.8.0/template/base-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/template/pain.001.001.03-cfonb.xml` & `trytond_account_payment_sepa_cfonb-6.8.0/template/pain.001.001.03-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/template/pain.008.001.02-cfonb.xml` & `trytond_account_payment_sepa_cfonb-6.8.0/template/pain.008.001.02-cfonb.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/tests/test_module.py` & `trytond_account_payment_sepa_cfonb-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO` & `trytond_account_payment_sepa_cfonb-6.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-sepa-cfonb
-Version: 6.6.0
+Name: trytond_account_payment_sepa_cfonb
+Version: 6.8.0
 Summary: Tryton module for CFONB SEPA payment
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_payment_sepa_cfonb
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment SEPA CFONB
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -38,22 +38,22 @@
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
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE
 
 Account Payment SEPA CFONB Module
 #################################
 
 The account_payment_sepa_cfonb module adds CFONB flavors to SEPA messages.
```

### Comparing `trytond_account_payment_sepa_cfonb-6.6.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt` & `trytond_account_payment_sepa_cfonb-6.8.0/trytond_account_payment_sepa_cfonb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
 payment.py
@@ -16,14 +12,15 @@
 ./payment.py
 ./tryton.cfg
 ./template/base-cfonb.xml
 ./template/pain.001.001.03-cfonb.xml
 ./template/pain.008.001.02-cfonb.xml
 ./tests/__init__.py
 ./tests/test_module.py
+doc/conf.py
 doc/index.rst
 template/base-cfonb.xml
 template/pain.001.001.03-cfonb.xml
 template/pain.008.001.02-cfonb.xml
 tests/__init__.py
 tests/test_module.py
 trytond_account_payment_sepa_cfonb.egg-info/PKG-INFO
```

