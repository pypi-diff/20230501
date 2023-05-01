# Comparing `tmp/ipref-0.2.0rc2.tar.gz` & `tmp/ipref-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipref-0.2.0rc2.tar", last modified: Tue Jan 17 11:29:55 2023, max compression
+gzip compressed data, was "ipref-0.2.1.tar", last modified: Mon May  1 08:30:17 2023, max compression
```

## Comparing `ipref-0.2.0rc2.tar` & `ipref-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/ipref/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/config-geolite.yaml.orig
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/config.yaml.orig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/ipref/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/data/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/data/geoip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.503382 ipref-0.2.0rc2/ipref/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/ipref/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/static/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/ipref/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/ipref/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/ipref.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-17 11:29:55.000000 ipref-0.2.0rc2/ipref.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-17 11:29:55.507382 ipref-0.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-17 11:29:46.000000 ipref-0.2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 08:30:03.000000 ipref-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-01 08:30:17.069049 ipref-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-01 08:30:03.000000 ipref-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/ipref/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/config-geolite.yaml.orig
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/config.yaml.orig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/ipref/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/data/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/data/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.065049 ipref-0.2.1/ipref/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/ipref/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/static/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/ipref/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-01 08:30:03.000000 ipref-0.2.1/ipref/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:30:17.069049 ipref-0.2.1/ipref.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 08:30:17.000000 ipref-0.2.1/ipref.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-01 08:30:03.000000 ipref-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-01 08:30:17.073049 ipref-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 08:30:03.000000 ipref-0.2.1/setup.py
```

### Comparing `ipref-0.2.0rc2/PKG-INFO` & `ipref-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipref
-Version: 0.2.0rc2
+Version: 0.2.1
 Summary: A simple utility to lookup IP addresses by MaxMind's GeoIP databases (CLI & WEB).
 Home-page: https://github.com/md-irohas/ipref-py
 Author: mkt
 Author-email: md.irohas@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-irohas/ipref-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,24 +57,23 @@
 # Create a virtualenv
 $ python3 -m venv env
 
 # Activate the virtualenv
 $ source env/bin/activate
 ```
 
-Download a .whl file from the [GitHub release](https://github.com/md-irohas/ipref-py/releases) page.
+You can install `ipref-py` via pypi (plus, the wheel file is available from
+[GitHub release](https://github.com/md-irohas/ipref-py/releases) page).
 
 ```sh
-(env) $ wget https://github.com/md-irohas/ipref-py/releases/download/v0.2.0/ipref-0.2.0-py3-none-any.whl
-
 # if you want CLI only
-(env) $ pip install ipref-0.2.0-py3-none-any.whl
+(env) $ pip install ipref
 
 # if you want CLI and web interface
-(env) $ pip install ipref-0.2.0-py3-none-any.whl[web]
+(env) $ pip install ipref[web]
 ```
 
 
 ## Configuration
 
 Make a configuration file.
 The template files for configurations are available.
```

### Comparing `ipref-0.2.0rc2/README.md` & `ipref-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,24 +41,23 @@
 # Create a virtualenv
 $ python3 -m venv env
 
 # Activate the virtualenv
 $ source env/bin/activate
 ```
 
-Download a .whl file from the [GitHub release](https://github.com/md-irohas/ipref-py/releases) page.
+You can install `ipref-py` via pypi (plus, the wheel file is available from
+[GitHub release](https://github.com/md-irohas/ipref-py/releases) page).
 
 ```sh
-(env) $ wget https://github.com/md-irohas/ipref-py/releases/download/v0.2.0/ipref-0.2.0-py3-none-any.whl
-
 # if you want CLI only
-(env) $ pip install ipref-0.2.0-py3-none-any.whl
+(env) $ pip install ipref
 
 # if you want CLI and web interface
-(env) $ pip install ipref-0.2.0-py3-none-any.whl[web]
+(env) $ pip install ipref[web]
 ```
 
 
 ## Configuration
 
 Make a configuration file.
 The template files for configurations are available.
```

### Comparing `ipref-0.2.0rc2/ipref/__main__.py` & `ipref-0.2.1/ipref/__main__.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/config-geolite.yaml.orig` & `ipref-0.2.1/ipref/config-geolite.yaml.orig`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/config.py` & `ipref-0.2.1/ipref/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,15 +78,20 @@
                 "The config version is invalid. The current version is '%d', but '%d' is used."
                 % (
                     self.CONFIG_VERSION,
                     version,
                 )
             )
 
+    def _expand_path(self, filename):
+        return os.path.expanduser(filename)
+
     def _load(self, filename, silent=True):
+        filename = self._expand_path(filename)
+
         if not os.path.exists(filename):
             if silent:
                 log.info("load config: %s (not-found)", filename)
             else:
                 log.error("load config: %s (not-found)", filename)
             return
```

### Comparing `ipref-0.2.0rc2/ipref/config.yaml.orig` & `ipref-0.2.1/ipref/config.yaml.orig`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/data/dns.py` & `ipref-0.2.1/ipref/data/dns.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/data/geoip.py` & `ipref-0.2.1/ipref/data/geoip.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/lookup.py` & `ipref-0.2.1/ipref/lookup.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/static/css/bootstrap.min.css` & `ipref-0.2.1/ipref/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/templates/search.html` & `ipref-0.2.1/ipref/templates/search.html`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/util.py` & `ipref-0.2.1/ipref/util.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref/web.py` & `ipref-0.2.1/ipref/web.py`

 * *Files identical despite different names*

### Comparing `ipref-0.2.0rc2/ipref.egg-info/PKG-INFO` & `ipref-0.2.1/ipref.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipref
-Version: 0.2.0rc2
+Version: 0.2.1
 Summary: A simple utility to lookup IP addresses by MaxMind's GeoIP databases (CLI & WEB).
 Home-page: https://github.com/md-irohas/ipref-py
 Author: mkt
 Author-email: md.irohas@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-irohas/ipref-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,24 +57,23 @@
 # Create a virtualenv
 $ python3 -m venv env
 
 # Activate the virtualenv
 $ source env/bin/activate
 ```
 
-Download a .whl file from the [GitHub release](https://github.com/md-irohas/ipref-py/releases) page.
+You can install `ipref-py` via pypi (plus, the wheel file is available from
+[GitHub release](https://github.com/md-irohas/ipref-py/releases) page).
 
 ```sh
-(env) $ wget https://github.com/md-irohas/ipref-py/releases/download/v0.2.0/ipref-0.2.0-py3-none-any.whl
-
 # if you want CLI only
-(env) $ pip install ipref-0.2.0-py3-none-any.whl
+(env) $ pip install ipref
 
 # if you want CLI and web interface
-(env) $ pip install ipref-0.2.0-py3-none-any.whl[web]
+(env) $ pip install ipref[web]
 ```
 
 
 ## Configuration
 
 Make a configuration file.
 The template files for configurations are available.
```

### Comparing `ipref-0.2.0rc2/setup.cfg` & `ipref-0.2.1/setup.cfg`

 * *Files identical despite different names*

