# Comparing `tmp/trytond_account_de_skr03-6.6.0.tar.gz` & `tmp/trytond_account_de_skr03-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_de_skr03-6.6.0.tar", last modified: Mon Oct 31 15:51:10 2022, max compression
+gzip compressed data, was "trytond_account_de_skr03-6.8.0.tar", last modified: Mon May  1 12:01:58 2023, max compression
```

## Comparing `trytond_account_de_skr03-6.6.0.tar` & `trytond_account_de_skr03-6.8.0.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:10.249452 trytond_account_de_skr03-6.6.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1925 2022-04-08 16:28:15.000000 trytond_account_de_skr03-6.6.0/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2020-10-16 17:15:34.000000 trytond_account_de_skr03-6.6.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2022-10-31 15:51:08.000000 trytond_account_de_skr03-6.6.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       57 2021-12-11 16:59:32.000000 trytond_account_de_skr03-6.6.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2323 2022-10-31 15:51:08.000000 trytond_account_de_skr03-6.6.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      762 2022-10-31 15:51:07.000000 trytond_account_de_skr03-6.6.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35146 2018-08-18 09:54:03.000000 trytond_account_de_skr03-6.6.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-10-16 12:14:46.000000 trytond_account_de_skr03-6.6.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     1613 2022-10-31 15:51:10.249452 trytond_account_de_skr03-6.6.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2019-06-04 16:49:43.000000 trytond_account_de_skr03-6.6.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2021-12-11 16:59:32.000000 trytond_account_de_skr03-6.6.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1720 2020-06-30 20:07:31.000000 trytond_account_de_skr03-6.6.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   392382 2021-04-30 07:13:51.000000 trytond_account_de_skr03-6.6.0/account_de.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:10.246119 trytond_account_de_skr03-6.6.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2019-06-04 16:49:43.000000 trytond_account_de_skr03-6.6.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2022-10-31 15:51:10.249452 trytond_account_de_skr03-6.6.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4289 2022-04-16 16:30:55.000000 trytond_account_de_skr03-6.6.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    85941 2020-06-30 20:07:31.000000 trytond_account_de_skr03-6.6.0/tax_de.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:10.246119 trytond_account_de_skr03-6.6.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-04-16 16:30:55.000000 trytond_account_de_skr03-6.6.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2022-04-16 16:30:55.000000 trytond_account_de_skr03-6.6.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      696 2022-10-31 15:10:09.000000 trytond_account_de_skr03-6.6.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       83 2022-10-31 15:51:06.000000 trytond_account_de_skr03-6.6.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2022-10-31 15:51:10.249452 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     1613 2022-10-31 15:51:09.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2022-10-31 15:51:10.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-10-31 15:51:09.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2022-10-31 15:51:09.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2019-06-04 16:43:12.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       44 2022-10-31 15:51:09.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2022-10-31 15:51:09.000000 trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:58.924254 trytond_account_de_skr03-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2486 2023-05-01 11:15:02.000000 trytond_account_de_skr03-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      762 2023-05-01 11:15:01.000000 trytond_account_de_skr03-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35146 2023-01-16 14:00:20.000000 trytond_account_de_skr03-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     1604 2023-05-01 12:01:58.924254 trytond_account_de_skr03-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_account_de_skr03-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1720 2023-04-15 07:12:15.000000 trytond_account_de_skr03-6.8.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   392382 2023-04-15 07:12:15.000000 trytond_account_de_skr03-6.8.0/account_de.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:58.920920 trytond_account_de_skr03-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 12:01:58.924254 trytond_account_de_skr03-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3476 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    85941 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/tax_de.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:58.920920 trytond_account_de_skr03-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_de_skr03-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_account_de_skr03-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_account_de_skr03-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       83 2023-05-01 11:14:56.000000 trytond_account_de_skr03-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 12:01:58.924254 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1604 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       44 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 12:01:58.000000 trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/top_level.txt
```

### Comparing `trytond_account_de_skr03-6.6.0/CHANGELOG` & `trytond_account_de_skr03-6.8.0/CHANGELOG`

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
 * Add support for Python 3.10
```

### Comparing `trytond_account_de_skr03-6.6.0/COPYRIGHT` & `trytond_account_de_skr03-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-6.6.0/LICENSE` & `trytond_account_de_skr03-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-6.6.0/PKG-INFO` & `trytond_account_de_skr03-6.8.0/trytond_account_de_skr03.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
-Name: trytond_account_de_skr03
-Version: 6.6.0
+Name: trytond-account-de-skr03
+Version: 6.8.0
 Summary: Tryton module with German chart of accounts SKR03
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_de_skr03
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart german SKR03
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: German
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
 
 German Account Module
 #####################
 
 The German account module define the SKR03 chart of account.
```

### Comparing `trytond_account_de_skr03-6.6.0/account.py` & `trytond_account_de_skr03-6.8.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-6.6.0/account_de.xml` & `trytond_account_de_skr03-6.8.0/account_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-6.6.0/setup.py` & `trytond_account_de_skr03-6.8.0/setup.py`

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
@@ -34,59 +31,39 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_account_de_skr03'
 
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
 
-dependency_links = []
-if minor_version % 2:
-    dependency_links.append(
-        'https://trydevpi.tryton.org/?local_version='
-        + '.'.join(local_version))
-
 setup(name=name,
     version=version,
     description='Tryton module with German chart of accounts SKR03',
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
-        "Source Code": 'https://hg.tryton.org/modules/account_de_skr03',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account chart german SKR03',
     package_dir={'trytond.modules.account_de_skr03': '.'},
     packages=(
         ['trytond.modules.account_de_skr03']
         + ['trytond.modules.account_de_skr03.%s' % p for p in find_packages()]
         ),
@@ -103,25 +80,24 @@
         'Intended Audience :: Legal Industry',
         'Intended Audience :: Manufacturing',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: German',
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
-    dependency_links=dependency_links,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     account_de_skr03 = trytond.modules.account_de_skr03
     """,
     )
```

### Comparing `trytond_account_de_skr03-6.6.0/tax_de.xml` & `trytond_account_de_skr03-6.8.0/tax_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_de_skr03-6.6.0/trytond_account_de_skr03.egg-info/PKG-INFO` & `trytond_account_de_skr03-6.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
-Name: trytond-account-de-skr03
-Version: 6.6.0
+Name: trytond_account_de_skr03
+Version: 6.8.0
 Summary: Tryton module with German chart of accounts SKR03
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
-Project-URL: Source Code, https://hg.tryton.org/modules/account_de_skr03
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account chart german SKR03
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: German
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
 
 German Account Module
 #####################
 
 The German account module define the SKR03 chart of account.
```

