# Comparing `tmp/guify-0.1.3.tar.gz` & `tmp/guify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guify-0.1.3.tar", last modified: Mon May  1 13:18:50 2023, max compression
+gzip compressed data, was "guify-0.2.0.tar", last modified: Mon May  1 20:45:06 2023, max compression
```

## Comparing `guify-0.1.3.tar` & `guify-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.746131 guify-0.1.3/
--rw-rw-rw-   0        0        0     1090 2023-05-01 11:05:53.000000 guify-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       79 2023-05-01 11:05:53.000000 guify-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2658 2023-05-01 13:18:50.747130 guify-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2383 2023-05-01 13:16:54.000000 guify-0.1.3/README.md
--rw-rw-rw-   0        0        0       95 2023-05-01 11:05:53.000000 guify-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1185 2023-05-01 13:18:50.749131 guify-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.612612 guify-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.691132 guify-0.1.3/src/guify/
--rw-rw-rw-   0        0        0     2517 2023-05-01 13:16:54.000000 guify-0.1.3/src/guify/App.py
--rw-rw-rw-   0        0        0     1366 2023-05-01 11:10:03.000000 guify-0.1.3/src/guify/BaseTest.py
--rw-rw-rw-   0        0        0     1355 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/ConfigTab.py
--rw-rw-rw-   0        0        0      329 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/Monitor.py
--rw-rw-rw-   0        0        0     1603 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/TestPool.py
--rw-rw-rw-   0        0        0     8449 2023-05-01 11:10:03.000000 guify-0.1.3/src/guify/TestWorker.py
--rw-rw-rw-   0        0        0     2959 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/__init__.py
--rw-rw-rw-   0        0        0      156 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/constants.py
--rw-rw-rw-   0        0        0     1295 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.723632 guify-0.1.3/src/guify/web/
--rw-rw-rw-   0        0        0      817 2023-05-01 11:08:07.000000 guify-0.1.3/src/guify/web/App.js
--rw-rw-rw-   0        0        0      381 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/asset-manifest.json
--rw-rw-rw-   0        0        0    16958 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/favicon.ico
--rw-rw-rw-   0        0        0      596 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/index.html
--rw-rw-rw-   0        0        0      332 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/manifest.json
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.617611 guify-0.1.3/src/guify/web/static/
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.730630 guify-0.1.3/src/guify/web/static/css/
--rw-rw-rw-   0        0        0   144140 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/static/css/main.a0d815e9.css
--rw-rw-rw-   0        0        0   482231 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/static/css/main.a0d815e9.css.map
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.743133 guify-0.1.3/src/guify/web/static/js/
--rw-rw-rw-   0        0        0   208103 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/static/js/main.94803c24.js
--rw-rw-rw-   0        0        0     1138 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/static/js/main.94803c24.js.LICENSE.txt
--rw-rw-rw-   0        0        0   664664 2023-05-01 11:05:53.000000 guify-0.1.3/src/guify/web/static/js/main.94803c24.js.map
-drwxrwxrwx   0        0        0        0 2023-05-01 13:18:50.707634 guify-0.1.3/src/guify.egg-info/
--rw-rw-rw-   0        0        0     2658 2023-05-01 13:18:50.000000 guify-0.1.3/src/guify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-05-01 13:18:50.000000 guify-0.1.3/src/guify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:18:50.000000 guify-0.1.3/src/guify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      606 2023-05-01 13:18:50.000000 guify-0.1.3/src/guify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 13:18:50.000000 guify-0.1.3/src/guify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:45:06.080561 guify-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 20:44:05.000000 guify-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 20:44:05.000000 guify-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-01 20:45:06.080561 guify-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-01 20:44:05.000000 guify-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-01 20:44:05.000000 guify-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-01 20:45:06.080561 guify-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:45:06.080561 guify-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:45:06.080561 guify-0.2.0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:45:06.080561 guify-0.2.0/src/python/guify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-01 20:45:06.000000 guify-0.2.0/src/python/guify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 20:45:06.000000 guify-0.2.0/src/python/guify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:45:06.000000 guify-0.2.0/src/python/guify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 20:45:06.000000 guify-0.2.0/src/python/guify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:45:06.000000 guify-0.2.0/src/python/guify.egg-info/top_level.txt
```

### Comparing `guify-0.1.3/PKG-INFO` & `guify-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,105 @@
-Metadata-Version: 2.1
-Name: guify
-Version: 0.1.3
-Summary: A tool that will GUI-ify your functions
-Author: Michael Druyan
-Author-email: michael@druyan.net
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GUIfy
-
----
-
-Simplest form of GUI for automation scripts.
-
-Made with eel as python backend and react used as frontend.
-
-main branch has built&optimized react app
-
-dev branch has development version of react app
-
-## Main tab
-
-![main_tab](main_tab.png)
-
-## Config tab
-
-![config_tab](config_tab.png)
-
-## How to use
-
----
-
-### Quick start
-
-```bash
-pip install guify
-```
-
-Look inside [this example](docs/example.py) or follow the instructions below:
-
-```py
-# main.py
-import GUIfy from guify
-
-app = GUIfy(app_name='GUIfy') # default app_name is 'GUIfy'
-
-@app.register(name='Test 1', priority=0, description='This is a test')
-def test_1(example_arg):
-   app.monitor.clear_text()
-   app.monitor.set_text('This is a test\n')
-   app.monitor.append_text('This is a test2\n')
-   result = app.prompt_user('This is a prompt') # True if user clicked OK, False if user clicked Cancel
-   foo = app.config.get('example','foo') # == bar
-
-
-
-app.run()
-
-```
-
----
-
-### Monitor object
-
-app.monitor is the monitor object representing the preview window on right hand side of the GUI,
-
-- set_text(text: str) -> None // will set the text in the monitor to whatever passed in "text" argument
-- append_text(text: str) -> None // will append the next to the monitor
-- clear_text(text: str) -> None // will clear all text in the monitor
-
----
-
-## Config tab
-
-"app.config" is an object representing the config tab.
-All configurations are stored in config.ini.
-
-### self.config methods:
-
-- save() // Save config to config.ini
-- load() // Load config from config.ini
-- get_section() // load() and return an entire section as a dictionary
-- get(section, attribute) // load() and get value of attribute in section
-- set(section, attribute, value) // load() and set value of attribute in section and then save().
-
-### config file:
-
-```ini
-[example]
-foo = bar
-```
-
-```py
-get_secion('example') -> {'foo': 'bar'}
-get('example', 'foo') -> 'bar'
-```
-
----
-
-## Settings
-
-in settings.ini you can change the following settings:
-
-- reports_dir - the directory where the reports will be saved
-- report_name_prefix - can be one of the variables passed in to your run() functions, uses this variable name as identification for reports
-
----
-
-## Building
-
-To build an executable in dist folder, run the following:
-
-`npm run build`
+# GUIfy
+
+---
+
+Simplest form of GUI for automation scripts.
+
+Made with eel as python backend and react used as frontend.
+
+main branch has built&optimized react app
+
+dev branch has development version of react app
+
+## Main tab
+
+![main_tab](main_tab.png)
+
+## Config tab
+
+![config_tab](config_tab.png)
+
+## How to use
+
+---
+
+### Quick start
+
+```bash
+pip install guify
+```
+
+Look inside [this example](docs/example.py) or follow the instructions below:
+
+```py
+# main.py
+import GUIfy from guify
+
+app = GUIfy(app_name='GUIfy') # default app_name is 'GUIfy'
+
+@app.register(name='Test 1', priority=0, description='This is a test')
+def test_1(example_arg):
+   app.monitor.clear_text()
+   app.monitor.set_text('This is a test\n')
+   app.monitor.append_text('This is a test2\n')
+   result = app.prompt_user('This is a prompt') # True if user clicked OK, False if user clicked Cancel
+   foo = app.config.get('example','foo') # == bar
+
+
+
+app.run()
+
+```
+
+---
+
+### Monitor object
+
+app.monitor is the monitor object representing the preview window on right hand side of the GUI,
+
+- set_text(text: str) -> None // will set the text in the monitor to whatever passed in "text" argument
+- append_text(text: str) -> None // will append the next to the monitor
+- clear_text(text: str) -> None // will clear all text in the monitor
+
+---
+
+## Config tab
+
+"app.config" is an object representing the config tab.
+All configurations are stored in config.ini.
+
+### self.config methods:
+
+- save() // Save config to config.ini
+- load() // Load config from config.ini
+- get_section() // load() and return an entire section as a dictionary
+- get(section, attribute) // load() and get value of attribute in section
+- set(section, attribute, value) // load() and set value of attribute in section and then save().
+
+### Config file:
+
+```ini
+[example]
+foo = bar
+```
+
+```py
+get_section('example') -> {'foo': 'bar'}
+get('example', 'foo') -> 'bar'
+```
+
+---
+
+## Settings
+
+in settings.ini you can change the following settings:
+
+- reports_dir - the directory where the reports will be saved
+- report_name_prefix - can be one of the variables passed in to your run() functions, uses this variable name as identification for reports
+
+---
+
+## Building
+
+To build an executable in dist folder, run the following:
+
+`npm run build`
```

### Comparing `guify-0.1.3/setup.cfg` & `guify-0.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2067 7569 6679 0d0a 7665 7273 696f   = guify..versio
-00000020: 6e20 3d20 302e 312e 330d 0a61 7574 686f  n = 0.1.3..autho
-00000030: 7220 3d20 4d69 6368 6165 6c20 4472 7579  r = Michael Druy
-00000040: 616e 0d0a 6175 7468 6f72 5f65 6d61 696c  an..author_email
-00000050: 203d 206d 6963 6861 656c 4064 7275 7961   = michael@druya
-00000060: 6e2e 6e65 740d 0a64 6573 6372 6970 7469  n.net..descripti
-00000070: 6f6e 203d 2041 2074 6f6f 6c20 7468 6174  on = A tool that
-00000080: 2077 696c 6c20 4755 492d 6966 7920 796f   will GUI-ify yo
-00000090: 7572 2066 756e 6374 696f 6e73 0d0a 6c6f  ur functions..lo
-000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000b0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
-000000c0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000d0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-000000e0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
-000000f0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000100: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000110: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000120: 203a 3a20 330d 0a0d 0a5b 6f70 7469 6f6e   :: 3....[option
-00000130: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000140: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000150: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000160: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000170: 7461 203d 2074 7275 650d 0a69 6e73 7461  ta = true..insta
-00000180: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000190: 0962 6f74 746c 653d 3d30 2e31 322e 3235  .bottle==0.12.25
-000001a0: 0d0a 0962 6f74 746c 652d 7765 6273 6f63  ...bottle-websoc
-000001b0: 6b65 743d 3d30 2e32 2e39 0d0a 0963 6666  ket==0.2.9...cff
-000001c0: 693d 3d31 2e31 352e 3120 3b20 706c 6174  i==1.15.1 ; plat
-000001d0: 666f 726d 5f70 7974 686f 6e5f 696d 706c  form_python_impl
-000001e0: 656d 656e 7461 7469 6f6e 203d 3d20 2743  ementation == 'C
-000001f0: 5079 7468 6f6e 2720 616e 6420 7379 735f  Python' and sys_
-00000200: 706c 6174 666f 726d 203d 3d20 2777 696e  platform == 'win
-00000210: 3332 270d 0a09 6565 6c3d 3d30 2e31 362e  32'...eel==0.16.
-00000220: 300d 0a09 6675 7475 7265 3d3d 302e 3138  0...future==0.18
-00000230: 2e33 203b 2070 7974 686f 6e5f 7665 7273  .3 ; python_vers
-00000240: 696f 6e20 3e3d 2027 322e 3627 2061 6e64  ion >= '2.6' and
-00000250: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-00000260: 6e6f 7420 696e 2027 332e 302c 2033 2e31  not in '3.0, 3.1
-00000270: 2c20 332e 322c 2033 2e33 270d 0a09 6765  , 3.2, 3.3'...ge
-00000280: 7665 6e74 3d3d 3232 2e31 302e 3220 3b20  vent==22.10.2 ; 
-00000290: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
-000002a0: 3d20 2732 2e37 2720 616e 6420 7079 7468  = '2.7' and pyth
-000002b0: 6f6e 5f76 6572 7369 6f6e 206e 6f74 2069  on_version not i
-000002c0: 6e20 2733 2e30 2c20 332e 312c 2033 2e32  n '3.0, 3.1, 3.2
-000002d0: 2c20 332e 332c 2033 2e34 2c20 332e 3527  , 3.3, 3.4, 3.5'
-000002e0: 0d0a 0967 6576 656e 742d 7765 6273 6f63  ...gevent-websoc
-000002f0: 6b65 743d 3d30 2e31 302e 310d 0a09 6772  ket==0.10.1...gr
-00000300: 6565 6e6c 6574 3d3d 322e 302e 3220 3b20  eenlet==2.0.2 ; 
-00000310: 706c 6174 666f 726d 5f70 7974 686f 6e5f  platform_python_
-00000320: 696d 706c 656d 656e 7461 7469 6f6e 203d  implementation =
-00000330: 3d20 2743 5079 7468 6f6e 270d 0a09 7079  = 'CPython'...py
-00000340: 6370 6172 7365 723d 3d32 2e32 310d 0a09  cparser==2.21...
-00000350: 7079 6d73 6762 6f78 3d3d 312e 302e 390d  pymsgbox==1.0.9.
-00000360: 0a09 7079 7061 7273 696e 673d 3d33 2e30  ..pyparsing==3.0
-00000370: 2e39 203b 2070 7974 686f 6e5f 6675 6c6c  .9 ; python_full
-00000380: 5f76 6572 7369 6f6e 203e 3d20 2733 2e36  _version >= '3.6
-00000390: 2e38 270d 0a09 7365 7475 7074 6f6f 6c73  .8'...setuptools
-000003a0: 3d3d 3637 2e37 2e32 203b 2070 7974 686f  ==67.7.2 ; pytho
-000003b0: 6e5f 7665 7273 696f 6e20 3e3d 2027 332e  n_version >= '3.
-000003c0: 3727 0d0a 0977 6869 6368 6372 6166 743d  7'...whichcraft=
-000003d0: 3d30 2e36 2e31 0d0a 097a 6f70 652e 6576  =0.6.1...zope.ev
-000003e0: 656e 743d 3d34 2e36 0d0a 097a 6f70 652e  ent==4.6...zope.
-000003f0: 696e 7465 7266 6163 653d 3d36 2e30 203b  interface==6.0 ;
-00000400: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-00000410: 3e3d 2027 332e 3727 0d0a 0d0a 5b6f 7074  >= '3.7'....[opt
-00000420: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000430: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-00000440: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000450: 6b61 6765 5f64 6174 615d 0d0a 6775 6966  kage_data]..guif
-00000460: 7920 3d20 7372 632f 6775 6966 792f 7765  y = src/guify/we
-00000470: 622f 2a0d 0a0d 0a5b 6567 675f 696e 666f  b/*....[egg_info
-00000480: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000490: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000004a0: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6775 6966 790a 7665 7273 696f 6e20  = guify.version 
+00000020: 3d20 302e 322e 300a 6175 7468 6f72 203d  = 0.2.0.author =
+00000030: 204d 6963 6861 656c 2044 7275 7961 6e0a   Michael Druyan.
+00000040: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
+00000050: 6963 6861 656c 4064 7275 7961 6e2e 6e65  ichael@druyan.ne
+00000060: 740a 6465 7363 7269 7074 696f 6e20 3d20  t.description = 
+00000070: 4120 746f 6f6c 2074 6861 7420 7769 6c6c  A tool that will
+00000080: 2047 5549 2d69 6679 2079 6f75 7220 6675   GUI-ify your fu
+00000090: 6e63 7469 6f6e 730a 6c6f 6e67 5f64 6573  nctions.long_des
+000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000b0: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
+000000c0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+000000d0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+000000e0: 6d61 726b 646f 776e 0a63 6c61 7373 6966  markdown.classif
+000000f0: 6965 7273 203d 200a 0950 726f 6772 616d  iers = ..Program
+00000100: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000110: 2050 7974 686f 6e20 3a3a 2033 0a0a 5b6f   Python :: 3..[o
+00000120: 7074 696f 6e73 5d0a 7061 636b 6167 655f  ptions].package_
+00000130: 6469 7220 3d20 0a09 3d20 7372 632f 7079  dir = ..= src/py
+00000140: 7468 6f6e 0a70 6163 6b61 6765 7320 3d20  thon.packages = 
+00000150: 6669 6e64 3a0a 696e 636c 7564 655f 7061  find:.include_pa
+00000160: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
+00000170: 650a 696e 7374 616c 6c5f 7265 7175 6972  e.install_requir
+00000180: 6573 203d 200a 0962 6f74 746c 653d 3d30  es = ..bottle==0
+00000190: 2e31 322e 3235 0a09 626f 7474 6c65 2d77  .12.25..bottle-w
+000001a0: 6562 736f 636b 6574 3d3d 302e 322e 390a  ebsocket==0.2.9.
+000001b0: 0963 6666 693d 3d31 2e31 352e 3120 3b20  .cffi==1.15.1 ; 
+000001c0: 706c 6174 666f 726d 5f70 7974 686f 6e5f  platform_python_
+000001d0: 696d 706c 656d 656e 7461 7469 6f6e 203d  implementation =
+000001e0: 3d20 2743 5079 7468 6f6e 2720 616e 6420  = 'CPython' and 
+000001f0: 7379 735f 706c 6174 666f 726d 203d 3d20  sys_platform == 
+00000200: 2777 696e 3332 270a 0965 656c 3d3d 302e  'win32'..eel==0.
+00000210: 3136 2e30 0a09 6675 7475 7265 3d3d 302e  16.0..future==0.
+00000220: 3138 2e33 203b 2070 7974 686f 6e5f 7665  18.3 ; python_ve
+00000230: 7273 696f 6e20 3e3d 2027 322e 3627 2061  rsion >= '2.6' a
+00000240: 6e64 2070 7974 686f 6e5f 7665 7273 696f  nd python_versio
+00000250: 6e20 6e6f 7420 696e 2027 332e 302c 2033  n not in '3.0, 3
+00000260: 2e31 2c20 332e 322c 2033 2e33 270a 0967  .1, 3.2, 3.3'..g
+00000270: 6576 656e 743d 3d32 322e 3130 2e32 203b  event==22.10.2 ;
+00000280: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
+00000290: 3e3d 2027 322e 3727 2061 6e64 2070 7974  >= '2.7' and pyt
+000002a0: 686f 6e5f 7665 7273 696f 6e20 6e6f 7420  hon_version not 
+000002b0: 696e 2027 332e 302c 2033 2e31 2c20 332e  in '3.0, 3.1, 3.
+000002c0: 322c 2033 2e33 2c20 332e 342c 2033 2e35  2, 3.3, 3.4, 3.5
+000002d0: 270a 0967 6576 656e 742d 7765 6273 6f63  '..gevent-websoc
+000002e0: 6b65 743d 3d30 2e31 302e 310a 0967 7265  ket==0.10.1..gre
+000002f0: 656e 6c65 743d 3d32 2e30 2e32 203b 2070  enlet==2.0.2 ; p
+00000300: 6c61 7466 6f72 6d5f 7079 7468 6f6e 5f69  latform_python_i
+00000310: 6d70 6c65 6d65 6e74 6174 696f 6e20 3d3d  mplementation ==
+00000320: 2027 4350 7974 686f 6e27 0a09 7079 6370   'CPython'..pycp
+00000330: 6172 7365 723d 3d32 2e32 310a 0970 796d  arser==2.21..pym
+00000340: 7367 626f 783d 3d31 2e30 2e39 0a09 7079  sgbox==1.0.9..py
+00000350: 7061 7273 696e 673d 3d33 2e30 2e39 203b  parsing==3.0.9 ;
+00000360: 2070 7974 686f 6e5f 6675 6c6c 5f76 6572   python_full_ver
+00000370: 7369 6f6e 203e 3d20 2733 2e36 2e38 270a  sion >= '3.6.8'.
+00000380: 0973 6574 7570 746f 6f6c 733d 3d36 372e  .setuptools==67.
+00000390: 372e 3220 3b20 7079 7468 6f6e 5f76 6572  7.2 ; python_ver
+000003a0: 7369 6f6e 203e 3d20 2733 2e37 270a 0977  sion >= '3.7'..w
+000003b0: 6869 6368 6372 6166 743d 3d30 2e36 2e31  hichcraft==0.6.1
+000003c0: 0a09 7a6f 7065 2e65 7665 6e74 3d3d 342e  ..zope.event==4.
+000003d0: 360a 097a 6f70 652e 696e 7465 7266 6163  6..zope.interfac
+000003e0: 653d 3d36 2e30 203b 2070 7974 686f 6e5f  e==6.0 ; python_
+000003f0: 7665 7273 696f 6e20 3e3d 2027 332e 3727  version >= '3.7'
+00000400: 0a0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000410: 6765 732e 6669 6e64 5d0a 7768 6572 6520  ges.find].where 
+00000420: 3d20 7372 632f 7079 7468 6f6e 0a0a 5b6f  = src/python..[o
+00000430: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+00000440: 6174 615d 0a67 7569 6679 203d 2062 7569  ata].guify = bui
+00000450: 6c64 2f2a 0a0a 5b65 6767 5f69 6e66 6f5d  ld/*..[egg_info]
+00000460: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
+00000470: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
```

### Comparing `guify-0.1.3/src/guify.egg-info/requires.txt` & `guify-0.2.0/src/python/guify.egg-info/requires.txt`

 * *Files identical despite different names*

