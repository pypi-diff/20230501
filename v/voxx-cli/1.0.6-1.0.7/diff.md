# Comparing `tmp/voxx-cli-1.0.6.tar.gz` & `tmp/voxx-cli-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxx-cli-1.0.6.tar", last modified: Mon May  1 07:45:42 2023, max compression
+gzip compressed data, was "voxx-cli-1.0.7.tar", last modified: Mon May  1 07:55:29 2023, max compression
```

## Comparing `voxx-cli-1.0.6.tar` & `voxx-cli-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:42.987412 voxx-cli-1.0.6/
--rw-rw-rw-   0        0        0     1084 2023-05-01 07:45:42.986907 voxx-cli-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-04-30 08:19:16.000000 voxx-cli-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 07:45:42.987412 voxx-cli-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:42.965863 voxx-cli-1.0.6/voxx/
--rw-rw-rw-   0        0        0      140 2023-05-01 07:41:25.000000 voxx-cli-1.0.6/voxx/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.6/voxx/__main__.py
--rw-rw-rw-   0        0        0     4039 2023-05-01 07:44:07.000000 voxx-cli-1.0.6/voxx/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:42.966869 voxx-cli-1.0.6/voxx/css/
--rw-rw-rw-   0        0        0     1247 2023-05-01 06:48:14.000000 voxx-cli-1.0.6/voxx/css/tui.css
--rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.6/voxx/model.py
--rw-rw-rw-   0        0        0     6441 2023-05-01 07:38:19.000000 voxx-cli-1.0.6/voxx/tui.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:45:42.985903 voxx-cli-1.0.6/voxx_cli.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       29 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-01 07:45:42.000000 voxx-cli-1.0.6/voxx_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.015932 voxx-cli-1.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-05-01 07:55:29.015932 voxx-cli-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-04-30 08:19:16.000000 voxx-cli-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:55:29.016433 voxx-cli-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.006422 voxx-cli-1.0.7/voxx/
+-rw-rw-rw-   0        0        0      140 2023-05-01 07:53:35.000000 voxx-cli-1.0.7/voxx/__init__.py
+-rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.7/voxx/__main__.py
+-rw-rw-rw-   0        0        0     4065 2023-05-01 07:51:28.000000 voxx-cli-1.0.7/voxx/connection.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.007422 voxx-cli-1.0.7/voxx/css/
+-rw-rw-rw-   0        0        0     1247 2023-05-01 06:48:14.000000 voxx-cli-1.0.7/voxx/css/tui.css
+-rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.7/voxx/model.py
+-rw-rw-rw-   0        0        0     6441 2023-05-01 07:38:19.000000 voxx-cli-1.0.7/voxx/tui.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.014933 voxx-cli-1.0.7/voxx_cli.egg-info/
+-rw-rw-rw-   0        0        0     1084 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       29 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/top_level.txt
```

### Comparing `voxx-cli-1.0.6/PKG-INFO` & `voxx-cli-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxx-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: A command line interface client for Voxx
 Home-page: https://github.com/CyR1en/voxx-client-cli
 Download-URL: https://github.com/CyR1en/voxx-client-cli
 Author: CyR1en
 Author-email: ethan.bacurio@ucdenver.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `voxx-cli-1.0.6/README.md` & `voxx-cli-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/setup.py` & `voxx-cli-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/voxx/__main__.py` & `voxx-cli-1.0.7/voxx/__main__.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/voxx/connection.py` & `voxx-cli-1.0.7/voxx/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             while (data := self.recv(1024).decode("utf-8")) is not None:
                 msg = json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
                 console.log(msg)
                 key = getattr(msg, 'update-message')
                 if key in UM_HANDLERS:
                     func = UM_HANDLERS[key]
                     func(self._owning_instance, msg)
-        except ConnectionResetError:
+        except (ConnectionResetError, ConnectionAbortedError):
             if self._on_close is not None:
                 self._on_close()
             self.close()
 
 
 res_req_conn: ResReqClient
 um_conn: UMClient
```

### Comparing `voxx-cli-1.0.6/voxx/css/tui.css` & `voxx-cli-1.0.7/voxx/css/tui.css`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/voxx/model.py` & `voxx-cli-1.0.7/voxx/model.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/voxx/tui.py` & `voxx-cli-1.0.7/voxx/tui.py`

 * *Files identical despite different names*

### Comparing `voxx-cli-1.0.6/voxx_cli.egg-info/PKG-INFO` & `voxx-cli-1.0.7/voxx_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxx-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: A command line interface client for Voxx
 Home-page: https://github.com/CyR1en/voxx-client-cli
 Download-URL: https://github.com/CyR1en/voxx-client-cli
 Author: CyR1en
 Author-email: ethan.bacurio@ucdenver.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

