# Comparing `tmp/typer_tinydb-0.1.2.tar.gz` & `tmp/typer_tinydb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_tinydb-0.1.2.tar", max compression
+gzip compressed data, was "typer_tinydb-0.1.4.tar", max compression
```

## Comparing `typer_tinydb-0.1.2.tar` & `typer_tinydb-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-24 09:25:26.352787 typer_tinydb-0.1.2/LICENSE
--rw-r--r--   0        0        0      909 2023-04-24 08:38:44.364321 typer_tinydb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2659 2023-04-24 14:01:43.062943 typer_tinydb-0.1.2/README.md
--rw-r--r--   0        0        0       67 2023-04-24 08:17:32.671020 typer_tinydb-0.1.2/typer_tinydb/__init__.py
--rw-r--r--   0        0        0       31 2023-04-24 08:39:15.333006 typer_tinydb-0.1.2/typer_tinydb/static/config.json
--rw-r--r--   0        0        0       23 2023-04-24 05:58:42.137034 typer_tinydb-0.1.2/typer_tinydb/tests/__init__.py
--rw-r--r--   0        0        0     4959 2023-04-24 06:40:12.321673 typer_tinydb-0.1.2/typer_tinydb/tests/test_upsert.py
--rw-r--r--   0        0        0    10881 2023-04-24 08:38:08.056830 typer_tinydb-0.1.2/typer_tinydb/typerdb.py
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 typer_tinydb-0.1.2/setup.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 typer_tinydb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:13:33.735228 typer_tinydb-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2659 2023-04-30 23:13:33.739228 typer_tinydb-0.1.4/README.md
+-rw-r--r--   0        0        0      906 2023-04-30 23:23:51.902066 typer_tinydb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      446 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/__main__.py
+-rw-r--r--   0        0        0      896 2023-04-30 23:23:22.950306 typer_tinydb-0.1.4/typer_tinydb/static/config.json
+-rw-r--r--   0        0        0    11362 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tdb.py
+-rw-r--r--   0        0        0       21 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tests/__init__.py
+-rw-r--r--   0        0        0     4812 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tests/test_upsert.py
+-rw-r--r--   0        0        0    14287 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/utils.py
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 typer_tinydb-0.1.4/PKG-INFO
```

### Comparing `typer_tinydb-0.1.2/LICENSE` & `typer_tinydb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.2/pyproject.toml` & `typer_tinydb-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "typer-tinydb"
-version = "0.1.2"
+version = "0.1.4"
 description = "A Python Typer CLI subcommand boilerplate to manage config files using tinydb"
 authors = ["arnos-stuff <bcda0276@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_tinydb"}]
 homepage = "https://arnos-stuff.github.io/typer-tinydb/"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.7,<4.0"
 typer = {extras = ["all"], version = "^0.7.0"}
 tinydb = "^4.7.1"
 
 
 [tool.poetry.scripts]
-typer-tinydb-config = 'typer_tinydb.typerdb:config'
-tcfg = 'typer_tinydb.typerdb:cfg'
+typer-tinydb-config = 'typer_tinydb.db:app'
+tcfg = 'typer_tinydb.tdb:cfg'
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-dracula-theme = "^1.0.4"
 mkdocs-material = "^9.1.7"
 pillow = "^9.5.0"
 cairosvg = "^2.7.0"
 mike = "^1.1.2"
 shtab = "^1.6.1"
 mkdocs-glightbox = "^0.3.3"
-flake8 = "^6.0.0"
 pytest = "^7.3.1"
 codecov = "^2.1.13"
 pytest-cov = "^4.0.0"
+mkgendocs = "^0.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typer_tinydb-0.1.2/README.md` & `typer_tinydb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.2/typer_tinydb/tests/test_upsert.py` & `typer_tinydb-0.1.4/typer_tinydb/tests/test_upsert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from random import shuffle, seed
-from ..typerdb import db, globals, where, Query, upsert_param, getKey, getValue
-
-# use the db to find the user
-# find the user in the globals table
-# find the user in the users table
-# add the user to the globals table
-# add the user to the users table
-
-
-class UpsertTest:
-    
-    def __init__(self, salt = 3.3, seedv=0) -> None:
-        self.salt = salt
-        self.txtsalt = str(salt)
-        self.seed = seedv
-        
-        
-    
-    def truncate(self):
-        globals.truncate()
-        
-    def upset_floats_clear(self):
-        seed(self.seed)
-        keys = list('aghwes')
-        keys = [k+self.txtsalt for k in keys]
-        shuffle(keys)
-        values = [3.33+self.salt, 2.2+self.salt, 1.0+self.salt, -2243.221+self.salt, -2.2222222+self.salt, 4.4+self.salt]
-        for k,v in zip(keys,values):
-            upsert_param(param=k, value=v, obfuscate=False)
-            
-        assert len(globals.all()) == 6
-        
-    def upsert_param_avoid_duplicates(self):
-        seed(self.seed)
-        keys = list('aes')
-        keys = [k+self.txtsalt for k in keys]
-        shuffle(keys)
-        values = [999+self.salt, 7777+self.salt, 2222+self.salt]
-        
-        for k,v in zip(keys,values):
-            upsert_param(param=k, value=v, obfuscate=False)
-            
-        assert len(globals.all()) == 6
-        
-    def get_keys(self):
-        seed(self.seed)
-        keys = list('aes')
-        keys = [k+self.txtsalt for k in keys]
-        shuffle(keys)
-        values = [999+self.salt, 7777+self.salt, 2222+self.salt]
-        for k,v in zip(keys,values):
-            assert getValue(param=k) == str(v)
-    
-    def add_obfuscation(self):
-        prefix = 'secret-key-number-'
-        words = ['one', 'two', 'three', 'BOOM']
-        keys = [prefix+w for w in words]
-        
-        values = ['wfwef890fwe0w', 'w98w89e0789bf78', '098880988', 31243434.311278766]
-        
-        for k,v in zip(keys,values):
-            upsert_param(param=k, value=v, obfuscate=True)
-            
-        for k in keys:
-            assert not len(globals.search(where('param') == k)) # all keys are encrypted
-        
-    def decode_obfuscation(self):
-        prefix = 'secret-key-number-'
-        words = ['one', 'two', 'three', 'BOOM']
-        keys = [prefix+w for w in words]
-        
-        values = ['wfwef890fwe0w', 'w98w89e0789bf78', '098880988', 31243434.311278766]
-        for k,v in zip(keys,values):
-            assert getValue(param=k) == str(v)
-
-    def reset(self):
-        globals.truncate()
-        assert not len(globals.all())
-
-def random_upserts(salt:float ,seedv:float):     
-    test = UpsertTest(salt=salt, seedv=seedv)
-    
-    test.truncate()
-    test.upset_floats_clear()
-    test.upsert_param_avoid_duplicates()
-    test.get_keys()
-    test.add_obfuscation()
-    test.decode_obfuscation()
-    test.reset()
-    
-salts = [1, 6, -3, 4]
-seeds = [12, 0, 232]
-
-# for i,salt in enumerate(salts):
-#     for j,seedv in enumerate(seeds):
-#         print(f'def test_random_upserts_num{i}x{j}():\n    random_upserts(salt={salt}, seedv={seedv})')
-        
-def test_random_upserts_num0x0():
-    random_upserts(salt=1, seedv=12)
-def test_random_upserts_num0x1():
-    random_upserts(salt=1, seedv=0)
-def test_random_upserts_num0x2():
-    random_upserts(salt=1, seedv=232)
-def test_random_upserts_num1x0():
-    random_upserts(salt=6, seedv=12)
-def test_random_upserts_num1x1():
-    random_upserts(salt=6, seedv=0)
-def test_random_upserts_num1x2():
-    random_upserts(salt=6, seedv=232)
-def test_random_upserts_num2x0():
-    random_upserts(salt=-3, seedv=12)
-def test_random_upserts_num2x1():
-    random_upserts(salt=-3, seedv=0)
-def test_random_upserts_num2x2():
-    random_upserts(salt=-3, seedv=232)
-def test_random_upserts_num3x0():
-    random_upserts(salt=4, seedv=12)
-def test_random_upserts_num3x1():
-    random_upserts(salt=4, seedv=0)
-def test_random_upserts_num3x2():
-    random_upserts(salt=4, seedv=232)
-def test_random_upserts_num0x0():
-    random_upserts(salt=1, seedv=12)
-def test_random_upserts_num0x1():
-    random_upserts(salt=1, seedv=0)
-def test_random_upserts_num0x2():
-    random_upserts(salt=1, seedv=232)
-def test_random_upserts_num1x0():
-    random_upserts(salt=6, seedv=12)
-def test_random_upserts_num1x1():
-    random_upserts(salt=6, seedv=0)
-def test_random_upserts_num1x2():
-    random_upserts(salt=6, seedv=232)
-def test_random_upserts_num2x0():
-    random_upserts(salt=-3, seedv=12)
-def test_random_upserts_num2x1():
-    random_upserts(salt=-3, seedv=0)
-def test_random_upserts_num2x2():
-    random_upserts(salt=-3, seedv=232)
-def test_random_upserts_num3x0():
-    random_upserts(salt=4, seedv=12)
-def test_random_upserts_num3x1():
-    random_upserts(salt=4, seedv=0)
-def test_random_upserts_num3x2():
+from random import shuffle, seed
+from ..utils import db, globals, where, Query, upsert_param, getKey, getValue
+
+# use the db to find the user
+# find the user in the globals table
+# find the user in the users table
+# add the user to the globals table
+# add the user to the users table
+
+
+class UpsertTest:
+    
+    def __init__(self, salt = 3.3, seedv=0) -> None:
+        self.salt = salt
+        self.txtsalt = str(salt)
+        self.seed = seedv
+        
+        
+    
+    def truncate(self):
+        globals.truncate()
+        
+    def upset_floats_clear(self):
+        seed(self.seed)
+        keys = list('aghwes')
+        keys = [k+self.txtsalt for k in keys]
+        shuffle(keys)
+        values = [3.33+self.salt, 2.2+self.salt, 1.0+self.salt, -2243.221+self.salt, -2.2222222+self.salt, 4.4+self.salt]
+        for k,v in zip(keys,values):
+            upsert_param(param=k, value=v, obfuscate=False)
+            
+        assert len(globals.all()) == 6
+        
+    def upsert_param_avoid_duplicates(self):
+        seed(self.seed)
+        keys = list('aes')
+        keys = [k+self.txtsalt for k in keys]
+        shuffle(keys)
+        values = [999+self.salt, 7777+self.salt, 2222+self.salt]
+        
+        for k,v in zip(keys,values):
+            upsert_param(param=k, value=v, obfuscate=False)
+            
+        assert len(globals.all()) == 6
+        
+    def get_keys(self):
+        seed(self.seed)
+        keys = list('aes')
+        keys = [k+self.txtsalt for k in keys]
+        shuffle(keys)
+        values = [999+self.salt, 7777+self.salt, 2222+self.salt]
+        for k,v in zip(keys,values):
+            assert getValue(param=k) == str(v)
+    
+    def add_obfuscation(self):
+        prefix = 'secret-key-number-'
+        words = ['one', 'two', 'three', 'BOOM']
+        keys = [prefix+w for w in words]
+        
+        values = ['wfwef890fwe0w', 'w98w89e0789bf78', '098880988', 31243434.311278766]
+        
+        for k,v in zip(keys,values):
+            upsert_param(param=k, value=v, obfuscate=True)
+            
+        for k in keys:
+            assert not len(globals.search(where('param') == k)) # all keys are encrypted
+        
+    def decode_obfuscation(self):
+        prefix = 'secret-key-number-'
+        words = ['one', 'two', 'three', 'BOOM']
+        keys = [prefix+w for w in words]
+        
+        values = ['wfwef890fwe0w', 'w98w89e0789bf78', '098880988', 31243434.311278766]
+        for k,v in zip(keys,values):
+            assert getValue(param=k) == str(v)
+
+    def reset(self):
+        globals.truncate()
+        assert not len(globals.all())
+
+def random_upserts(salt:float ,seedv:float):     
+    test = UpsertTest(salt=salt, seedv=seedv)
+    
+    test.truncate()
+    test.upset_floats_clear()
+    test.upsert_param_avoid_duplicates()
+    test.get_keys()
+    test.add_obfuscation()
+    test.decode_obfuscation()
+    test.reset()
+    
+salts = [1, 6, -3, 4]
+seeds = [12, 0, 232]
+
+# for i,salt in enumerate(salts):
+#     for j,seedv in enumerate(seeds):
+#         print(f'def test_random_upserts_num{i}x{j}():\n    random_upserts(salt={salt}, seedv={seedv})')
+        
+def test_random_upserts_num0x0():
+    random_upserts(salt=1, seedv=12)
+def test_random_upserts_num0x1():
+    random_upserts(salt=1, seedv=0)
+def test_random_upserts_num0x2():
+    random_upserts(salt=1, seedv=232)
+def test_random_upserts_num1x0():
+    random_upserts(salt=6, seedv=12)
+def test_random_upserts_num1x1():
+    random_upserts(salt=6, seedv=0)
+def test_random_upserts_num1x2():
+    random_upserts(salt=6, seedv=232)
+def test_random_upserts_num2x0():
+    random_upserts(salt=-3, seedv=12)
+def test_random_upserts_num2x1():
+    random_upserts(salt=-3, seedv=0)
+def test_random_upserts_num2x2():
+    random_upserts(salt=-3, seedv=232)
+def test_random_upserts_num3x0():
+    random_upserts(salt=4, seedv=12)
+def test_random_upserts_num3x1():
+    random_upserts(salt=4, seedv=0)
+def test_random_upserts_num3x2():
+    random_upserts(salt=4, seedv=232)
+def test_random_upserts_num0x0():
+    random_upserts(salt=1, seedv=12)
+def test_random_upserts_num0x1():
+    random_upserts(salt=1, seedv=0)
+def test_random_upserts_num0x2():
+    random_upserts(salt=1, seedv=232)
+def test_random_upserts_num1x0():
+    random_upserts(salt=6, seedv=12)
+def test_random_upserts_num1x1():
+    random_upserts(salt=6, seedv=0)
+def test_random_upserts_num1x2():
+    random_upserts(salt=6, seedv=232)
+def test_random_upserts_num2x0():
+    random_upserts(salt=-3, seedv=12)
+def test_random_upserts_num2x1():
+    random_upserts(salt=-3, seedv=0)
+def test_random_upserts_num2x2():
+    random_upserts(salt=-3, seedv=232)
+def test_random_upserts_num3x0():
+    random_upserts(salt=4, seedv=12)
+def test_random_upserts_num3x1():
+    random_upserts(salt=4, seedv=0)
+def test_random_upserts_num3x2():
     random_upserts(salt=4, seedv=232)
```

### Comparing `typer_tinydb-0.1.2/setup.py` & `typer_tinydb-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: typer-tinydb
+Version: 0.1.4
+Summary: A Python Typer CLI subcommand boilerplate to manage config files using tinydb
+Home-page: https://arnos-stuff.github.io/typer-tinydb/
+Author: arnos-stuff
+Author-email: bcda0276@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: tinydb (>=4.7.1,<5.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['typer_tinydb', 'typer_tinydb.tests']
 
-package_data = \
-{'': ['*'], 'typer_tinydb': ['static/*']}
+[![PyPI version](https://badge.fury.io/py/typer-tinydb.svg)](https://badge.fury.io/py/typer-tinydb) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/arnos-stuff/typer-tinydb/master/LICENSE)
+[![codecov](https://codecov.io/gh/arnos-stuff/typer-tinydb/branch/master/graph/badge.svg?token=7MP5WBU8GI)](https://codecov.io/gh/arnos-stuff/typer-tinydb)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/arnos-stuff/typer-tinydb/tree/master.svg?style=shield "CircleCI Build Status")](https://dl.circleci.com/status-badge/redirect/gh/arnos-stuff/typer-tinydb/tree/master)
 
-install_requires = \
-['tinydb>=4.7.1,<5.0.0', 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['tcfg = typer_tinydb.typerdb:cfg',
-                     'typer-tinydb-config = typer_tinydb.typerdb:config']}
-
-setup_kwargs = {
-    'name': 'typer-tinydb',
-    'version': '0.1.2',
-    'description': 'A Python Typer CLI subcommand boilerplate to manage config files using tinydb',
-    'long_description': '\n[![PyPI version](https://badge.fury.io/py/typer-tinydb.svg)](https://badge.fury.io/py/typer-tinydb) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/arnos-stuff/typer-tinydb/master/LICENSE)\n[![codecov](https://codecov.io/gh/arnos-stuff/typer-tinydb/branch/master/graph/badge.svg?token=7MP5WBU8GI)](https://codecov.io/gh/arnos-stuff/typer-tinydb)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/arnos-stuff/typer-tinydb/tree/master.svg?style=shield "CircleCI Build Status")](https://dl.circleci.com/status-badge/redirect/gh/arnos-stuff/typer-tinydb/tree/master)\n\n# A Typer config file get/set boilerplate\n\n# Using the boilerplate\n\n## Aliases and subcommands\n\nWe recommand the following aliases, which are readily available out of the box.\n\n- `config`\n- `cfg`\n- `c`\n\nThis way, if your app is named `super-app`\n\nAnd is defined in `super_app.py` roughly as follows:\n\n```python\n\nimport typer\n\n# ... some imports\n\napp = typer.Typer(\n    name=\'super-app\',\n    # ... other args\n)\n```\n\nYou just have to add the following below:\n\n```python\nfrom typer_tinydb import cfg, config # those are typer apps\n\napp.add_typer(cfg) # the cfg app\napp.add_typer(config) # the config app\n```\n\nYou can rename them however you like by using\n\n```python\napp.add_typer(cfg, name=\'my-super-config\')\n```\n\n## Using it on the command line\n\nWith the same configuration as above, your new app can now run the commands:\n\n```bash\nsuper-app cfg list # list config key:value pairs\nsuper-app cfg get some-key # get the values linked to the key \'some-key\'\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\' # store some hash or token into your settings file\nsuper-app cfg set some-key \'20-hS407zuqYKQ8tPP2r5\'\n```\n\nYou can obviously use `super-app config get` and others, or any name you attribute to it.\n\n## Using it within python modules\n\nThe CLI key-values are stored in a tinydb instance that is available by just importing the table named `globals`:\n\n```python\nfrom typer_tinydb import db, globals, where\n```\n\nYou can create any table using the database object `db`, please [check out the tinydb docs !](https://tinydb.readthedocs.io/)\n\nTo get the key just use `where` :\n\n```python\nreturns = globals.search(where(\'param\') == param)\n```\n\nTo insert new values or update existing, use the `upsert` function:\n\n```python\nParam = Query()\n\nglobals.upsert({\n    "param": param,\n    "value": value,\n    "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),\n    "machine": socket.gethostname(),\n    },\n    Param.param == param\n)\n```\n# Commands\n\nGo check out the [documentation page 🚀](https://arnos-stuff.github.io/typer-tinydb)',
-    'author': 'arnos-stuff',
-    'author_email': 'bcda0276@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://arnos-stuff.github.io/typer-tinydb/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+# A Typer config file get/set boilerplate
 
+# Using the boilerplate
 
-setup(**setup_kwargs)
+## Aliases and subcommands
+
+We recommand the following aliases, which are readily available out of the box.
+
+- `config`
+- `cfg`
+- `c`
+
+This way, if your app is named `super-app`
+
+And is defined in `super_app.py` roughly as follows:
+
+```python
+
+import typer
+
+# ... some imports
+
+app = typer.Typer(
+    name='super-app',
+    # ... other args
+)
+```
+
+You just have to add the following below:
+
+```python
+from typer_tinydb import cfg, config # those are typer apps
+
+app.add_typer(cfg) # the cfg app
+app.add_typer(config) # the config app
+```
+
+You can rename them however you like by using
+
+```python
+app.add_typer(cfg, name='my-super-config')
+```
+
+## Using it on the command line
+
+With the same configuration as above, your new app can now run the commands:
+
+```bash
+super-app cfg list # list config key:value pairs
+super-app cfg get some-key # get the values linked to the key 'some-key'
+super-app cfg set some-key '20-hS407zuqYKQ8tPP2r5' # store some hash or token into your settings file
+super-app cfg set some-key '20-hS407zuqYKQ8tPP2r5'
+```
+
+You can obviously use `super-app config get` and others, or any name you attribute to it.
+
+## Using it within python modules
+
+The CLI key-values are stored in a tinydb instance that is available by just importing the table named `globals`:
+
+```python
+from typer_tinydb import db, globals, where
+```
+
+You can create any table using the database object `db`, please [check out the tinydb docs !](https://tinydb.readthedocs.io/)
+
+To get the key just use `where` :
+
+```python
+returns = globals.search(where('param') == param)
+```
+
+To insert new values or update existing, use the `upsert` function:
+
+```python
+Param = Query()
+
+globals.upsert({
+    "param": param,
+    "value": value,
+    "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),
+    "machine": socket.gethostname(),
+    },
+    Param.param == param
+)
+```
+# Commands
+
+Go check out the [documentation page 🚀](https://arnos-stuff.github.io/typer-tinydb)
```

