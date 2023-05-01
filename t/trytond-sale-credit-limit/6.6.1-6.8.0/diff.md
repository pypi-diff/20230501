# Comparing `tmp/trytond_sale_credit_limit-6.6.1.tar.gz` & `tmp/trytond_sale_credit_limit-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_credit_limit-6.6.1.tar", last modified: Sat Mar  4 11:36:39 2023, max compression
+gzip compressed data, was "trytond_sale_credit_limit-6.8.0.tar", last modified: Mon May  1 11:46:09 2023, max compression
```

## Comparing `trytond_sale_credit_limit-6.6.1.tar` & `trytond_sale_credit_limit-6.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:36:39.016703 trytond_sale_credit_limit-6.6.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1622 2023-03-04 11:36:34.000000 trytond_sale_credit_limit-6.6.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-03-04 11:36:33.000000 trytond_sale_credit_limit-6.6.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:55.000000 trytond_sale_credit_limit-6.6.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2480 2023-03-04 11:36:39.013369 trytond_sale_credit_limit-6.6.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2022-12-19 12:02:57.000000 trytond_sale_credit_limit-6.6.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:36:39.013369 trytond_sale_credit_limit-6.6.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2013 2023-02-23 20:19:08.000000 trytond_sale_credit_limit-6.6.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      888 2022-12-19 12:02:53.000000 trytond_sale_credit_limit-6.6.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-03-04 11:36:39.016703 trytond_sale_credit_limit-6.6.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4285 2022-12-19 12:02:56.000000 trytond_sale_credit_limit-6.6.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:36:39.010036 trytond_sale_credit_limit-6.6.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5192 2022-12-19 12:02:54.000000 trytond_sale_credit_limit-6.6.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2022-12-19 12:02:57.000000 trytond_sale_credit_limit-6.6.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      118 2022-12-19 12:03:07.000000 trytond_sale_credit_limit-6.6.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-03-04 11:36:39.013369 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2480 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-03-04 11:36:38.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-03-04 11:36:37.000000 trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:09.639140 trytond_sale_credit_limit-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-05-01 11:04:09.000000 trytond_sale_credit_limit-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:04:09.000000 trytond_sale_credit_limit-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_credit_limit-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2470 2023-05-01 11:46:09.639140 trytond_sale_credit_limit-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-04-27 20:43:50.000000 trytond_sale_credit_limit-6.8.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:09.635807 trytond_sale_credit_limit-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2038 2023-04-27 20:43:50.000000 trytond_sale_credit_limit-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      888 2023-04-27 20:43:50.000000 trytond_sale_credit_limit-6.8.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:46:09.639140 trytond_sale_credit_limit-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4247 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:09.635807 trytond_sale_credit_limit-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5192 2023-04-27 20:43:50.000000 trytond_sale_credit_limit-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_sale_credit_limit-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      118 2023-05-01 11:04:03.000000 trytond_sale_credit_limit-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:46:09.639140 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2470 2023-05-01 11:46:08.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-05-01 11:46:09.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:46:08.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-05-01 11:46:08.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-05-01 11:46:08.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:46:08.000000 trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/top_level.txt
```

### Comparing `trytond_sale_credit_limit-6.6.1/CHANGELOG` & `trytond_sale_credit_limit-6.8.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-Version 6.6.1 - 2023-03-04
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Remove support for Python 3.7
+* Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_credit_limit-6.6.1/COPYRIGHT` & `trytond_sale_credit_limit-6.8.0/COPYRIGHT`

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

### Comparing `trytond_sale_credit_limit-6.6.1/LICENSE` & `trytond_sale_credit_limit-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-6.6.1/PKG-INFO` & `trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond_sale_credit_limit
-Version: 6.6.1
+Name: trytond-sale-credit-limit
+Version: 6.8.0
 Summary: Tryton module for sale credit limit
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_credit_limit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale credit limit
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
 License-File: LICENSE
 
 Sale Credit Limit
 #################
 
 The sale_credit_limit module adds confirmed sale but not yet invoiced to the
 "Credit Amount" of the Party and check the credit limit of the party when
```

### Comparing `trytond_sale_credit_limit-6.6.1/doc/conf.py` & `trytond_sale_credit_limit-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
```

### Comparing `trytond_sale_credit_limit-6.6.1/party.py` & `trytond_sale_credit_limit-6.8.0/party.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 ('party', 'in', [p.id for p in parties]),
                 ('state', 'in', ['confirmed', 'processing']),
                 ])
         for sale in sales:
             amount = 0
             for line in sale.lines:
                 quantity = line.quantity
-                if not quantity:
+                if not quantity or (line.type != 'line'):
                     continue
                 for invoice_line in line.invoice_lines:
                     if invoice_line.type != 'line':
                         continue
                     invoice = invoice_line.invoice
                     if invoice and invoice.move:
                         quantity -= Uom.compute_qty(
```

### Comparing `trytond_sale_credit_limit-6.6.1/sale.py` & `trytond_sale_credit_limit-6.8.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-6.6.1/setup.py` & `trytond_sale_credit_limit-6.8.0/setup.py`

 * *Files 4% similar despite different names*

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
@@ -34,36 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_sale_credit_limit'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 setup(name=name,
     version=version,
     description='Tryton module for sale credit limit',
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
-        "Source Code": 'https://hg.tryton.org/modules/sale_credit_limit',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale credit limit',
     package_dir={'trytond.modules.sale_credit_limit': '.'},
     packages=(
         ['trytond.modules.sale_credit_limit']
         + ['trytond.modules.sale_credit_limit.%s' % p for p in find_packages()]
         ),
@@ -99,24 +99,24 @@
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
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     sale_credit_limit = trytond.modules.sale_credit_limit
     """,
     )
```

### Comparing `trytond_sale_credit_limit-6.6.1/tests/test_module.py` & `trytond_sale_credit_limit-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_credit_limit-6.6.1/tox.ini` & `trytond_sale_credit_limit-6.8.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tox]
-envlist = {py37,py38,py39,py310}-{sqlite,postgresql}
+envlist = {py38,py39,py310,py311}-{sqlite,postgresql}
 
 [testenv]
+usedevelop = true
 commands =
-    coverage run --include=./**/sale_credit_limit/* -m unittest discover -s tests
-    coverage report --include=./**/sale_credit_limit/* --omit=*/tests/*
+    coverage run --omit=*/tests/* -m xmlrunner discover -s tests {posargs}
+commands_post =
+    coverage report
+    coverage xml
 deps =
     coverage
+    unittest-xml-reporting
     postgresql: psycopg2 >= 2.7.0
 passenv = *
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
     postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:DB_NAME::memory:}
     postgresql: DB_NAME={env:DB_NAME:test}
```

### Comparing `trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/PKG-INFO` & `trytond_sale_credit_limit-6.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: trytond-sale-credit-limit
-Version: 6.6.1
+Name: trytond_sale_credit_limit
+Version: 6.8.0
 Summary: Tryton module for sale credit limit
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
-Project-URL: Source Code, https://hg.tryton.org/modules/sale_credit_limit
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale credit limit
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
 License-File: LICENSE
 
 Sale Credit Limit
 #################
 
 The sale_credit_limit module adds confirmed sale but not yet invoiced to the
 "Credit Amount" of the Party and check the credit limit of the party when
```

### Comparing `trytond_sale_credit_limit-6.6.1/trytond_sale_credit_limit.egg-info/SOURCES.txt` & `trytond_sale_credit_limit-6.8.0/trytond_sale_credit_limit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

