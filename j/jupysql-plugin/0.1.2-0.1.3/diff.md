# Comparing `tmp/jupysql_plugin-0.1.2.tar.gz` & `tmp/jupysql_plugin-0.1.3.tar.gz`

## Comparing `jupysql_plugin-0.1.2.tar` & `jupysql_plugin-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,47 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/babel.config.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/environment.dev.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jest.config.js
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/setup.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/tsconfig.json
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/_version.py
--rw-r--r--   0        0        0    21156 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/build_log.json
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/package.json
--rw-r--r--   0        0        0    16219 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/lib_index_js.6de74611b3c4c6ceb06b.js
--rw-r--r--   0        0        0    17606 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/lib_index_js.6de74611b3c4c6ceb06b.js.map
--rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/remoteEntry.cf34b2483199c5b69bb8.js
--rw-r--r--   0        0        0    27748 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/remoteEntry.cf34b2483199c5b69bb8.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/style.js
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js.map
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js.map
--rw-r--r--   0        0        0   273206 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js
--rw-r--r--   0        0        0   120157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js.map
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/src/connector.ts
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/src/customconnector.ts
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/src/index.ts
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/src/keywords.json
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/src/__tests__/jupysql_plugin.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/ui-tests/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/ui-tests/tests/jupysql_plugin.spec.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/LICENSE
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/babel.config.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/environment.dev.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jest.config.js
+-rw-r--r--   0        0        0   667313 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/package-lock.json
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/setup.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/doc/README.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/_version.py
+-rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/build_log.json
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/package.json
+-rw-r--r--   0        0        0    22000 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/lib_index_js.add99e517bcda3011598.js
+-rw-r--r--   0        0        0    25486 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/lib_index_js.add99e517bcda3011598.js.map
+-rw-r--r--   0        0        0    30195 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/remoteEntry.2fe7ef943493a06cc3dc.js
+-rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/remoteEntry.2fe7ef943493a06cc3dc.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/style.js
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js.map
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js
+-rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js.map
+-rw-r--r--   0        0        0   449391 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.8cb979a4708c9a13b429.js
+-rw-r--r--   0        0        0   725049 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.8cb979a4708c9a13b429.js.map
+-rw-r--r--   0        0        0   273206 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js
+-rw-r--r--   0        0        0   120157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js.map
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/connector.ts
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/customconnector.ts
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/formatter.ts
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/index.ts
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/keywords.json
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/src/__tests__/jupysql_plugin.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/ui-tests/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/ui-tests/tests/jupysql_plugin.spec.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.3/PKG-INFO
```

### Comparing `jupysql_plugin-0.1.2/RELEASE.md` & `jupysql_plugin-0.1.3/RELEASE.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 
 Create conda environment:
 
 ```bash
 conda env create  -f environment.dev.yml -y
 ```
 
-Bump the version using `hatch`. By default this will create a tag.
-See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
+Bump the version using `hatch`. See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
 
 ```bash
 hatch version <new-version>
 ```
 
+The previous command will update the version in the `package.json` file. You have to manually commit and create the tag:
+
+```bash
+```
+
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 *Note:* The following command needs NodeJS
 
 ```bash
 python -m build
 ```
```

### Comparing `jupysql_plugin-0.1.2/jest.config.js` & `jupysql_plugin-0.1.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/package.json` & `jupysql_plugin-0.1.3/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724999999999999%*

 * *Differences: {"'dependencies'": "{'sql-formatter': '^12.2.0'}", "'version'": "'0.1.3'"}*

```diff
@@ -11,14 +11,15 @@
         "@jupyterlab/codeeditor": "^3.6.2",
         "@jupyterlab/codemirror": "^3.6.3",
         "@jupyterlab/completer": "^3.6.2",
         "@jupyterlab/notebook": "^3.6.2",
         "@jupyterlab/statedb": "^3.6.2",
         "@types/codemirror": "^5.60.7",
         "@types/underscore": "^1.11.4",
+        "sql-formatter": "^12.2.0",
         "underscore": "^1.13.6"
     },
     "description": "Jupyterlab extension for JupySQL",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
@@ -95,9 +96,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupysql_plugin-0.1.2/tsconfig.json` & `jupysql_plugin-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/build_log.json` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/build_log.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998992257343551%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^3.6.3'}, '@jupyterlab/application-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/colla […]*

```diff
@@ -119,436 +119,441 @@
                         ],
                         "type": "var"
                     },
                     "name": "jupysql-plugin",
                     "shared": {
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^0.2.0",
+                            "requiredVersion": "^0.2.3",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/collaboration": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/collaboration-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.6.1",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.6.1"
+                            "requiredVersion": "^4.6.3"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.6.1",
+                            "requiredVersion": "^6.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
+                        },
+                        "@jupyterlab/shared-models": {
+                            "import": false,
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.6.1",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.6.1"
+                            "requiredVersion": "^5.6.3"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.6.1",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.1"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.31.3",
+                            "requiredVersion": "^1.31.4",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
                             "requiredVersion": "^1.19.0",
                             "singleton": true
                         },
@@ -590,34 +595,35 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.37.1",
+                            "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "@types/codemirror": {},
                         "@types/underscore": {},
                         "jupysql-plugin": {
                             "import": "/Users/eduardo/dev/jupysql-plugin/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.0"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
+                        "sql-formatter": {},
                         "underscore": {},
                         "yjs": {
                             "import": false,
                             "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
```

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/package.json` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9718055555555555%*

 * *Differences: {"'dependencies'": "{'sql-formatter': '^12.2.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2fe7ef943493a06cc3dc.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -11,14 +11,15 @@
         "@jupyterlab/codeeditor": "^3.6.2",
         "@jupyterlab/codemirror": "^3.6.3",
         "@jupyterlab/completer": "^3.6.2",
         "@jupyterlab/notebook": "^3.6.2",
         "@jupyterlab/statedb": "^3.6.2",
         "@types/codemirror": "^5.60.7",
         "@types/underscore": "^1.11.4",
+        "sql-formatter": "^12.2.0",
         "underscore": "^1.13.6"
     },
     "description": "Jupyterlab extension for JupySQL",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
@@ -45,15 +46,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ploomber/jupysql-plugin.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cf34b2483199c5b69bb8.js",
+            "load": "static/remoteEntry.2fe7ef943493a06cc3dc.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupysql_plugin/labextension"
     },
     "keywords": [
         "jupyter",
@@ -100,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.2"
 }
```

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/lib_index_js.6de74611b3c4c6ceb06b.js.map` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/lib_index_js.add99e517bcda3011598.js.map`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7964285714285715%*

 * *Differences: {"'file'": "'lib_index_js.add99e517bcda3011598.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;AAAA,0CAA0C;AAC1C,2DAA2D;AAE3D,+DAA+D;AAEX;AAGpD;;GAEG;AACI,MAAM,mBAAoB,SAAQ,8DAIxC;IACC;;;;OAIG;IACH,YACE,UAIG;QAEH,KAAK,EAAE,CAAC;QACR,IAAI,CAAC,WAAW,GAAG,UAAU,CAAC;IAChC,CAAC;IAED;;;;;OAKG;IACH,KAAK,CACH,OAAmC;QAEnC,OAAO,OAAO,CAAC,GAAG,CAChB,IAAI,CAAC,WAAW,CAAC,GAAG,CAAC,CAAC,SAAS,EAAE,EAAE,CAAC,SAAS,CAAC,KAAK,CAAC,OAAO,CAAC,CAAC,CAC9D,CAAC,IAAI,CAAC,CAAC,OAAO,EAAE,EAAE;YACjB,MAAM,cAAc,GAAG,OAAO,CAAC,MAAM,CACnC,CAAC,KAAK […]*

```diff
@@ -1,17 +1,19 @@
 {
-    "file": "lib_index_js.6de74611b3c4c6ceb06b.js",
-    "mappings": "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",
+    "file": "lib_index_js.add99e517bcda3011598.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupysql-plugin/./src/connector.ts",
         "webpack://jupysql-plugin/./src/customconnector.ts",
+        "webpack://jupysql-plugin/./src/formatter.ts",
         "webpack://jupysql-plugin/./src/index.ts"
     ],
     "sourcesContent": [
         "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\n// Modified from jupyterlab/packages/completer/src/connector.ts\n\nimport { DataConnector } from '@jupyterlab/statedb';\nimport { CompletionHandler } from '@jupyterlab/completer';\n\n/**\n * A multi-connector connector for completion handlers.\n */\nexport class CompletionConnector extends DataConnector<\n  CompletionHandler.IReply,\n  void,\n  CompletionHandler.IRequest\n> {\n  /**\n   * Create a new connector for completion requests.\n   *\n   * @param connectors - Connectors to request matches from, ordered by metadata preference (descending).\n   */\n  constructor(\n    connectors: DataConnector<\n      CompletionHandler.IReply,\n      void,\n      CompletionHandler.IRequest\n    >[]\n  ) {\n    super();\n    this._connectors = connectors;\n  }\n\n  /**\n   * Fetch completion requests.\n   *\n   * @param request - The completion request text and details.\n   * @returns Completion reply\n   */\n  fetch(\n    request: CompletionHandler.IRequest\n  ): Promise<CompletionHandler.IReply> {\n    return Promise.all(\n      this._connectors.map((connector) => connector.fetch(request))\n    ).then((replies) => {\n      const definedReplies = replies.filter(\n        (reply): reply is CompletionHandler.IReply => !!reply\n      );\n      return Private.mergeReplies(definedReplies);\n    });\n  }\n\n  private _connectors: DataConnector<\n    CompletionHandler.IReply,\n    void,\n    CompletionHandler.IRequest\n  >[];\n}\n\n/**\n * A namespace for private functionality.\n */\nnamespace Private {\n  /**\n   * Merge results from multiple connectors.\n   *\n   * @param replies - Array of completion results.\n   * @returns IReply with a superset of all matches.\n   */\n  export function mergeReplies(\n    replies: Array<CompletionHandler.IReply>\n  ): CompletionHandler.IReply {\n    // Filter replies with matches.\n    const repliesWithMatches = replies.filter((rep) => rep.matches.length > 0);\n    // If no replies contain matches, return an empty IReply.\n    if (repliesWithMatches.length === 0) {\n      return replies[0];\n    }\n    // If only one reply contains matches, return it.\n    if (repliesWithMatches.length === 1) {\n      return repliesWithMatches[0];\n    }\n\n    // Collect unique matches from all replies.\n    const matches: Set<string> = new Set();\n    repliesWithMatches.forEach((reply) => {\n      reply.matches.forEach((match) => matches.add(match));\n    });\n\n    // Note that the returned metadata field only contains items in the first member of repliesWithMatches.\n    return { ...repliesWithMatches[0], matches: [...matches] };\n  }\n}\n",
         "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\n// Modified from jupyterlab/packages/completer/src/contextconnector.ts\n\nimport { CodeEditor } from '@jupyterlab/codeeditor';\nimport { DataConnector } from '@jupyterlab/statedb';\nimport { CompletionHandler } from '@jupyterlab/completer';\n\nimport {\n  ISessionContext\n} from '@jupyterlab/apputils';\n\nimport keywords from './keywords.json';\n\n/**\n * A custom connector for completion handlers.\n */\nexport class CustomConnector extends DataConnector<\n  CompletionHandler.IReply,\n  void,\n  CompletionHandler.IRequest\n> {\n  /**\n   * Create a new custom connector for completion requests.\n   *\n   * @param options - The instatiation options for the custom connector.\n   */\n  constructor(options: CustomConnector.IOptions) {\n    super();\n    this._editor = options.editor;\n    this._sessionContext = options.sessionContext;\n  }\n\n  /**\n   * Fetch completion requests.\n   *\n   * @param request - The completion request text and details.\n   * @returns Completion reply\n   */\n  fetch(\n    request: CompletionHandler.IRequest\n  ): Promise<CompletionHandler.IReply> {\n    if (!this._editor) {\n      return Promise.reject('No editor');\n    }\n    return new Promise<CompletionHandler.IReply>((resolve) => {\n      resolve(Private.completionHint(this._editor, this._sessionContext));\n    });\n  }\n\n  private _editor: CodeEditor.IEditor | null;\n  private _sessionContext: ISessionContext | null;\n\n}\n\n/**\n * A namespace for custom connector statics.\n */\nexport namespace CustomConnector {\n  /**\n   * The instantiation options for cell completion handlers.\n   */\n  export interface IOptions {\n    /**\n     * The session used by the custom connector.\n     */\n    editor: CodeEditor.IEditor | null;\n    sessionContext: ISessionContext | null;\n  }\n\n}\n\n\n\n/**\n * A namespace for Private functionality.\n */\nnamespace Private {\n  /**\n   * Get a list of mocked completion hints.\n   *\n   * @param editor Editor\n   * @returns Completion reply\n   */\n\n\n\n\n  export function completionHint(\n    editor: CodeEditor.IEditor,\n    sessionContext: ISessionContext\n  ): CompletionHandler.IReply {\n    // Find the token at the cursor\n    const cursor = editor.getCursorPosition();\n    const token = editor.getTokenForPosition(cursor);\n\n    var newTokenList = keywords[\"keywords\"]\n\n    const completionList = newTokenList.filter((t) => t.value.startsWith(token.value.toUpperCase())).map((t) => t.value);\n\n    // Remove duplicate completions from the list\n    const matches = Array.from(new Set<string>(completionList));\n\n    return {\n      start: token.offset,\n      end: token.offset + token.value.length,\n      matches,\n      metadata: {},\n    };\n  }\n}\n",
-        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin,\n} from '@jupyterlab/application';\n\nimport {\n  ContextConnector,\n  ICompletionManager,\n  KernelConnector,\n} from '@jupyterlab/completer';\n\nimport { INotebookTracker, NotebookPanel } from '@jupyterlab/notebook';\n\nimport { CompletionConnector } from './connector';\n\nimport { CustomConnector } from './customconnector';\n\n\n// for syntax highlighting\nimport { CodeMirrorEditor, ICodeMirror } from '@jupyterlab/codemirror';\nimport * as _ from 'underscore';\n\n/**\n * The command IDs used by the console plugin.\n */\nnamespace CommandIDs {\n  export const invoke = 'completer:invoke';\n\n  export const invokeNotebook = 'completer:invoke-notebook';\n\n  export const select = 'completer:select';\n\n  export const selectNotebook = 'completer:select-notebook';\n}\n\n/**\n * Initialization data for the extension.\n */\nconst extension: JupyterFrontEndPlugin<void> = {\n  id: 'completer',\n  autoStart: true,\n  requires: [ICompletionManager, INotebookTracker],\n  activate: async (\n    app: JupyterFrontEnd,\n    completionManager: ICompletionManager,\n    notebooks: INotebookTracker\n  ) => {\n    console.log('JupyterLab custom completer extension is activated!');\n\n    // Modelled after completer-extension's notebooks plugin\n    notebooks.widgetAdded.connect(\n      (sender: INotebookTracker, panel: NotebookPanel) => {\n        let editor = panel.content.activeCell?.editor ?? null;\n        const session = panel.sessionContext.session;\n        const sessionContext = panel.sessionContext;\n        const options = { session, editor, sessionContext };\n        const connector = new CompletionConnector([]);\n        const handler = completionManager.register({\n          connector,\n          editor,\n          parent: panel,\n        });\n\n        const updateConnector = () => {\n          editor = panel.content.activeCell?.editor ?? null;\n          options.session = panel.sessionContext.session;\n          options.sessionContext = panel.sessionContext;\n          options.editor = editor;\n          handler.editor = editor;\n\n          const kernel = new KernelConnector(options);\n          const context = new ContextConnector(options);\n          const custom = new CustomConnector(options);\n          handler.connector = new CompletionConnector([\n            kernel,\n            context,\n            custom\n          ]);\n        };\n\n        // Update the handler whenever the prompt or session changes\n        panel.content.activeCellChanged.connect(updateConnector);\n        panel.sessionContext.sessionChanged.connect(updateConnector);\n      }\n    );\n\n    // Add notebook completer command.\n    app.commands.addCommand(CommandIDs.invokeNotebook, {\n      execute: () => {\n        const panel = notebooks.currentWidget;\n        if (panel && panel.content.activeCell?.model.type === 'code') {\n          return app.commands.execute(CommandIDs.invoke, { id: panel.id });\n        }\n      },\n    });\n\n    // Add notebook completer select command.\n    app.commands.addCommand(CommandIDs.selectNotebook, {\n      execute: () => {\n        const id = notebooks.currentWidget && notebooks.currentWidget.id;\n\n        if (id) {\n          return app.commands.execute(CommandIDs.select, { id });\n        }\n      },\n    });\n\n    // Set enter key for notebook completer select command.\n    app.commands.addKeyBinding({\n      command: CommandIDs.selectNotebook,\n      keys: ['Enter'],\n      selector: '.jp-Notebook .jp-mod-completer-active',\n    });\n  },\n};\n\n\n// %%sql highlighting\nclass SqlCodeMirror {\n  constructor(\n    protected app: JupyterFrontEnd,\n    protected tracker: INotebookTracker,\n    protected code_mirror: ICodeMirror\n  ) {\n    this.tracker?.activeCellChanged?.connect(() => {\n      if (this.tracker?.activeCell !== null) {\n        const cell = this.tracker.activeCell;\n        if (cell !== null && cell?.model.type === 'code') {\n          const code_mirror_editor = cell?.editor as CodeMirrorEditor;\n          const debounced_on_change = _.debounce(() => {\n            // check for editor with first line starting with %%sql\n            const line = code_mirror_editor\n              .getLine(code_mirror_editor.firstLine())\n              ?.trim();\n            if (line?.startsWith('%%sql')) {\n              code_mirror_editor.editor.setOption('mode', 'text/x-sql');\n            } else {\n              code_mirror_editor.editor.setOption('mode', 'text/x-ipython');\n            }\n          }, 300);\n          code_mirror_editor.editor.on('change', debounced_on_change);\n          debounced_on_change();\n        }\n      }\n    });\n  }\n}\n\nfunction activate_syntax(\n  app: JupyterFrontEnd,\n  tracker: INotebookTracker,\n  code_mirror: ICodeMirror\n): void {\n  new SqlCodeMirror(app, tracker, code_mirror);\n  console.log('SQLCodeMirror loaded.');\n}\n\n/**\n * Initialization data for the jupyterlabs_sql_codemirror extension.\n */\nconst extension_sql: JupyterFrontEndPlugin<void> = {\n  id: '@ploomber/sql-syntax-highlighting',\n  autoStart: true,\n  requires: [INotebookTracker, ICodeMirror],\n  optional: [],\n  activate: activate_syntax\n};\n\n\nexport default [extension, extension_sql];\n"
+        "// inspired by: https://github.com/ryantam626/jupyterlab_code_formatter\nimport { Cell, CodeCell } from '@jupyterlab/cells';\nimport { INotebookTracker, Notebook } from '@jupyterlab/notebook';\nimport { Widget } from '@lumino/widgets';\nimport { showErrorMessage } from '@jupyterlab/apputils';\nimport { format } from 'sql-formatter';\n\nexport class JupyterlabNotebookCodeFormatter {\n    protected working: boolean;\n    protected notebookTracker: INotebookTracker;\n\n    constructor(\n        notebookTracker: INotebookTracker\n    ) {\n        this.notebookTracker = notebookTracker;\n    }\n\n\n    public async formatAllCodeCells(\n        config: any,\n        formatter?: string,\n        notebook?: Notebook\n    ) {\n        return this.formatCells(false, config, formatter, notebook);\n    }\n\n    private getCodeCells(selectedOnly = true, notebook?: Notebook): CodeCell[] {\n        if (!this.notebookTracker.currentWidget) {\n            return [];\n        }\n        const codeCells: CodeCell[] = [];\n        notebook = notebook || this.notebookTracker.currentWidget.content;\n        notebook.widgets.forEach((cell: Cell) => {\n            if (cell.model.type === 'code') {\n                if (!selectedOnly || notebook.isSelectedOrActive(cell)) {\n                    codeCells.push(cell as CodeCell);\n                }\n            }\n        });\n        return codeCells;\n    }\n\n\n    private async formatCells(\n        selectedOnly: boolean,\n        config: any,\n        formatter?: string,\n        notebook?: Notebook\n    ) {\n\n        if (this.working) {\n            return;\n        }\n        try {\n            this.working = true;\n            const selectedCells = this.getCodeCells(selectedOnly, notebook);\n            if (selectedCells.length === 0) {\n                this.working = false;\n                return;\n            }\n\n            for (let i = 0; i < selectedCells.length; ++i) {\n                const cell = selectedCells[i];\n                const text = cell.model.value.text\n\n                if (text.startsWith(\"%%sql\")) {\n                    const lines = text.split(\"\\n\");\n                    const sqlCommand = lines.shift();\n\n                    try {\n                        const query = format(lines.join(\"\\n\"), { language: 'sql', keywordCase: 'upper' })\n                        cell.model.value.text = sqlCommand + \"\\n\" + query;\n                    } catch (error) {\n                    }\n\n\n                }\n            }\n        } catch (error) {\n            await showErrorMessage('Jupysql plugin formatting', error);\n        }\n        this.working = false;\n    }\n\n    applicable(formatter: string, currentWidget: Widget) {\n        const currentNotebookWidget = this.notebookTracker.currentWidget;\n        // TODO: Handle showing just the correct formatter for the language later\n        return currentNotebookWidget && currentWidget === currentNotebookWidget;\n    }\n}\n",
+        "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin,\n} from '@jupyterlab/application';\n\nimport {\n  ContextConnector,\n  ICompletionManager,\n  KernelConnector,\n} from '@jupyterlab/completer';\n\nimport { INotebookTracker, NotebookPanel, INotebookModel } from '@jupyterlab/notebook';\n\nimport { CompletionConnector } from './connector';\n\nimport { CustomConnector } from './customconnector';\n\n\n// for syntax highlighting\nimport { CodeMirrorEditor, ICodeMirror } from '@jupyterlab/codemirror';\nimport * as _ from 'underscore';\n\n\nimport { IDisposable, DisposableDelegate } from '@lumino/disposable';\n\n\nimport { ToolbarButton } from '@jupyterlab/apputils';\n\nimport { DocumentRegistry } from '@jupyterlab/docregistry';\nimport { JupyterlabNotebookCodeFormatter } from './formatter';\n\n\n\n/**\n * The command IDs used by the console plugin.\n */\nnamespace CommandIDs {\n  export const invoke = 'completer:invoke';\n\n  export const invokeNotebook = 'completer:invoke-notebook';\n\n  export const select = 'completer:select';\n\n  export const selectNotebook = 'completer:select-notebook';\n}\n\n/**\n * Initialization data for the extension.\n */\nconst extension: JupyterFrontEndPlugin<void> = {\n  id: 'completer',\n  autoStart: true,\n  requires: [ICompletionManager, INotebookTracker],\n  activate: async (\n    app: JupyterFrontEnd,\n    completionManager: ICompletionManager,\n    notebooks: INotebookTracker\n  ) => {\n    console.log('JupyterLab custom completer extension is activated!');\n\n    // Modelled after completer-extension's notebooks plugin\n    notebooks.widgetAdded.connect(\n      (sender: INotebookTracker, panel: NotebookPanel) => {\n        let editor = panel.content.activeCell?.editor ?? null;\n        const session = panel.sessionContext.session;\n        const sessionContext = panel.sessionContext;\n        const options = { session, editor, sessionContext };\n        const connector = new CompletionConnector([]);\n        const handler = completionManager.register({\n          connector,\n          editor,\n          parent: panel,\n        });\n\n        const updateConnector = () => {\n          editor = panel.content.activeCell?.editor ?? null;\n          options.session = panel.sessionContext.session;\n          options.sessionContext = panel.sessionContext;\n          options.editor = editor;\n          handler.editor = editor;\n\n          const kernel = new KernelConnector(options);\n          const context = new ContextConnector(options);\n          const custom = new CustomConnector(options);\n          handler.connector = new CompletionConnector([\n            kernel,\n            context,\n            custom\n          ]);\n        };\n\n        // Update the handler whenever the prompt or session changes\n        panel.content.activeCellChanged.connect(updateConnector);\n        panel.sessionContext.sessionChanged.connect(updateConnector);\n      }\n    );\n\n    // Add notebook completer command.\n    app.commands.addCommand(CommandIDs.invokeNotebook, {\n      execute: () => {\n        const panel = notebooks.currentWidget;\n        if (panel && panel.content.activeCell?.model.type === 'code') {\n          return app.commands.execute(CommandIDs.invoke, { id: panel.id });\n        }\n      },\n    });\n\n    // Add notebook completer select command.\n    app.commands.addCommand(CommandIDs.selectNotebook, {\n      execute: () => {\n        const id = notebooks.currentWidget && notebooks.currentWidget.id;\n\n        if (id) {\n          return app.commands.execute(CommandIDs.select, { id });\n        }\n      },\n    });\n\n    // Set enter key for notebook completer select command.\n    app.commands.addKeyBinding({\n      command: CommandIDs.selectNotebook,\n      keys: ['Enter'],\n      selector: '.jp-Notebook .jp-mod-completer-active',\n    });\n  },\n};\n\n\n// %%sql highlighting\nclass SqlCodeMirror {\n  constructor(\n    protected app: JupyterFrontEnd,\n    protected tracker: INotebookTracker,\n    protected code_mirror: ICodeMirror\n  ) {\n    this.tracker?.activeCellChanged?.connect(() => {\n      if (this.tracker?.activeCell !== null) {\n        const cell = this.tracker.activeCell;\n        if (cell !== null && cell?.model.type === 'code') {\n          const code_mirror_editor = cell?.editor as CodeMirrorEditor;\n          const debounced_on_change = _.debounce(() => {\n            // check for editor with first line starting with %%sql\n            const line = code_mirror_editor\n              .getLine(code_mirror_editor.firstLine())\n              ?.trim();\n            if (line?.startsWith('%%sql')) {\n              code_mirror_editor.editor.setOption('mode', 'text/x-sql');\n            } else {\n              code_mirror_editor.editor.setOption('mode', 'text/x-ipython');\n            }\n          }, 300);\n          code_mirror_editor.editor.on('change', debounced_on_change);\n          debounced_on_change();\n        }\n      }\n    });\n  }\n}\n\nfunction activate_syntax(\n  app: JupyterFrontEnd,\n  tracker: INotebookTracker,\n  code_mirror: ICodeMirror\n): void {\n  new SqlCodeMirror(app, tracker, code_mirror);\n  console.log('SQLCodeMirror loaded.');\n}\n\n/**\n * Initialization data for the jupyterlabs_sql_codemirror extension.\n * this is based on:\n * https://github.com/surdouski/jupyterlabs_sql_codemirror\n */\nconst extension_sql: JupyterFrontEndPlugin<void> = {\n  id: '@ploomber/sql-syntax-highlighting',\n  autoStart: true,\n  requires: [INotebookTracker, ICodeMirror],\n  optional: [],\n  activate: activate_syntax\n};\n\n\n\n\n/**\n * A notebook widget extension that adds a button to the toolbar.\n */\nexport class FormattingExtension\n  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>\n{\n  /**\n   * Create a new extension for the notebook panel widget.\n   *\n   * @param panel Notebook panel\n   * @param context Notebook context\n   * @returns Disposable on the added button\n   */\n\n  private notebookCodeFormatter: JupyterlabNotebookCodeFormatter;\n\n\n  constructor(\n    tracker: INotebookTracker\n  ) {\n    this.notebookCodeFormatter = new JupyterlabNotebookCodeFormatter(\n      tracker\n    );\n  }\n\n\n  createNew(\n    panel: NotebookPanel,\n    context: DocumentRegistry.IContext<INotebookModel>\n  ): IDisposable {\n    const clearOutput = () => {\n      this.notebookCodeFormatter.formatAllCodeCells(undefined, undefined, panel.content)\n    };\n    const button = new ToolbarButton({\n      className: 'format-sql-button',\n      label: 'Format SQL',\n      onClick: clearOutput,\n      tooltip: 'Format all %%sql cells',\n    });\n\n    panel.toolbar.insertItem(10, 'formatSQL', button);\n    return new DisposableDelegate(() => {\n      button.dispose();\n    });\n  }\n}\n\n\n\n\n/**\n * Activate the extension.\n *\n * @param app Main application object\n */\nconst formatting_plugin: JupyterFrontEndPlugin<void> = {\n  activate: (\n    app: JupyterFrontEnd,\n    tracker: INotebookTracker,\n  ) => {\n\n    app.docRegistry.addWidgetExtension('Notebook', new FormattingExtension(\n      tracker,\n    ));\n  },\n  autoStart: true,\n  id: \"formatting\",\n  requires: [\n    INotebookTracker,\n  ]\n};\n\n\n\nexport default [extension, extension_sql, formatting_plugin];\n"
     ],
     "version": 3
 }
```

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/remoteEntry.cf34b2483199c5b69bb8.js` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/remoteEntry.2fe7ef943493a06cc3dc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -83,15 +83,15 @@
             /******/
             exports: {}
             /******/
         };
         /******/
         /******/ // Execute the module function
         /******/
-        __webpack_modules__[moduleId](module, module.exports, __webpack_require__);
+        __webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);
         /******/
         /******/ // Return the exports of the module
         /******/
         return module.exports;
         /******/
     }
     /******/
@@ -182,17 +182,18 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "6de74611b3c4c6ceb06b",
+                "lib_index_js": "add99e517bcda3011598",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "4552f03d4f09d840178e",
                 "style_index_js": "d2d1cdf7cc4936cb793a",
+                "vendors-node_modules_sql-formatter_lib_index_js": "8cb979a4708c9a13b429",
                 "vendors-node_modules_underscore_modules_index-all_js": "8220176670f4f625110f"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -424,15 +425,17 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupysql-plugin", "0.1.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupysql-plugin", "0.1.2", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    /******/
+                    register("sql-formatter", "12.2.0", () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/sql-formatter/lib/index.js */ "./node_modules/sql-formatter/lib/index.js"))))));
                     /******/
                     register("underscore", "1.13.6", () => (__webpack_require__.e("vendors-node_modules_underscore_modules_index-all_js").then(() => (() => (__webpack_require__( /*! ./node_modules/underscore/modules/index-all.js */ "./node_modules/underscore/modules/index-all.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -815,23 +818,29 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/completer": () => (loadSingletonVersionCheck("default", "@jupyterlab/completer", [1, 3, 6, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/completer": () => (loadSingletonVersionCheck("default", "@jupyterlab/completer", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/codemirror": () => (loadSingletonVersionCheck("default", "@jupyterlab/codemirror", [1, 3, 6, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/codemirror": () => (loadSingletonVersionCheck("default", "@jupyterlab/codemirror", [1, 3, 6, 3])),
             /******/
             "webpack/sharing/consume/default/underscore/underscore": () => (loadStrictVersionCheckFallback("default", "underscore", [1, 1, 13, 6], () => (__webpack_require__.e("vendors-node_modules_underscore_modules_index-all_js").then(() => (() => (__webpack_require__( /*! underscore */ "./node_modules/underscore/modules/index-all.js"))))))),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 6, 1]))
+            "webpack/sharing/consume/default/@lumino/disposable": () => (loadSingletonVersionCheck("default", "@lumino/disposable", [1, 1, 10, 0])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 6, 3])),
+            /******/
+            "webpack/sharing/consume/default/sql-formatter/sql-formatter": () => (loadStrictVersionCheckFallback("default", "sql-formatter", [1, 12, 2, 0], () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! sql-formatter */ "./node_modules/sql-formatter/lib/index.js")))))))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -840,15 +849,21 @@
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/notebook",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/codemirror",
                 /******/
                 "webpack/sharing/consume/default/underscore/underscore",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/statedb"
+                "webpack/sharing/consume/default/@lumino/disposable",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/apputils",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/statedb",
+                /******/
+                "webpack/sharing/consume/default/sql-formatter/sql-formatter"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1075,8 +1090,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupysql-plugin");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupysql-plugin"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.cf34b2483199c5b69bb8.js.map
+//# sourceMappingURL=remoteEntry.2fe7ef943493a06cc3dc.js.map
```

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/remoteEntry.cf34b2483199c5b69bb8.js.map` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/remoteEntry.2fe7ef943493a06cc3dc.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8311688311688312%*

 * *Differences: {"'file'": "'remoteEntry.2fe7ef943493a06cc3dc.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.cf34b2483199c5b69bb8.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,0RAA0R;WACxT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC/KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.2fe7ef943493a06cc3dc.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,mWAAmW;WACjY;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCrLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupysql-plugin/webpack/container-entry",
         "webpack://jupysql-plugin/webpack/bootstrap",
         "webpack://jupysql-plugin/webpack/runtime/compat get default export",
         "webpack://jupysql-plugin/webpack/runtime/define property getters",
@@ -21,26 +21,26 @@
         "webpack://jupysql-plugin/webpack/runtime/nonce",
         "webpack://jupysql-plugin/webpack/before-startup",
         "webpack://jupysql-plugin/webpack/startup",
         "webpack://jupysql-plugin/webpack/after-startup"
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
-        "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
+        "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"6de74611b3c4c6ceb06b\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"4552f03d4f09d840178e\",\"style_index_js\":\"d2d1cdf7cc4936cb793a\",\"vendors-node_modules_underscore_modules_index-all_js\":\"8220176670f4f625110f\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"add99e517bcda3011598\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"4552f03d4f09d840178e\",\"style_index_js\":\"d2d1cdf7cc4936cb793a\",\"vendors-node_modules_sql-formatter_lib_index_js\":\"8cb979a4708c9a13b429\",\"vendors-node_modules_underscore_modules_index-all_js\":\"8220176670f4f625110f\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupysql-plugin:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupysql-plugin\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupysql-plugin\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"underscore\", \"1.13.6\", () => (__webpack_require__.e(\"vendors-node_modules_underscore_modules_index-all_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/underscore/modules/index-all.js */ \"./node_modules/underscore/modules/index-all.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupysql-plugin\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupysql-plugin\", \"0.1.2\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"12.2.0\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t\tregister(\"underscore\", \"1.13.6\", () => (__webpack_require__.e(\"vendors-node_modules_underscore_modules_index-all_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/underscore/modules/index-all.js */ \"./node_modules/underscore/modules/index-all.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/completer\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/completer\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/underscore/underscore\": () => (loadStrictVersionCheckFallback(\"default\", \"underscore\", [1,1,13,6], () => (__webpack_require__.e(\"vendors-node_modules_underscore_modules_index-all_js\").then(() => (() => (__webpack_require__(/*! underscore */ \"./node_modules/underscore/modules/index-all.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,6,1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/completer\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/underscore/underscore\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/completer\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/completer\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/underscore/underscore\": () => (loadStrictVersionCheckFallback(\"default\", \"underscore\", [1,1,13,6], () => (__webpack_require__.e(\"vendors-node_modules_underscore_modules_index-all_js\").then(() => (() => (__webpack_require__(/*! underscore */ \"./node_modules/underscore/modules/index-all.js\"))))))),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [1,12,2,0], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/completer\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/underscore/underscore\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupysql-plugin\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupysql_plugin\"] = self[\"webpackChunkjupysql_plugin\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupysql-plugin\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js.map` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js.map`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js.map` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js.map`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js.map` & `jupysql_plugin-0.1.3/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js.map`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/src/connector.ts` & `jupysql_plugin-0.1.3/src/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/src/customconnector.ts` & `jupysql_plugin-0.1.3/src/customconnector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/src/keywords.json` & `jupysql_plugin-0.1.3/src/keywords.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/ui-tests/README.md` & `jupysql_plugin-0.1.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/ui-tests/jupyter_server_test_config.py` & `jupysql_plugin-0.1.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/ui-tests/tests/jupysql_plugin.spec.ts` & `jupysql_plugin-0.1.3/ui-tests/tests/jupysql_plugin.spec.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/.gitignore` & `jupysql_plugin-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/LICENSE` & `jupysql_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/README.md` & `jupysql_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/pyproject.toml` & `jupysql_plugin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.2/PKG-INFO` & `jupysql_plugin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jupyterlab extension for JupySQL
 Project-URL: Homepage, https://github.com/ploomber/jupysql-plugin.git
 Project-URL: Bug Tracker, https://github.com/ploomber/jupysql-plugin.git/issues
 Project-URL: Repository, https://github.com/ploomber/jupysql-plugin.git.git
 Author-email: Ploomber <contact@ploomber.io>
 License: BSD 3-Clause License
```

