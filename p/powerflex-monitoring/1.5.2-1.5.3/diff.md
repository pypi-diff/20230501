# Comparing `tmp/powerflex-monitoring-1.5.2.tar.gz` & `tmp/powerflex-monitoring-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerflex-monitoring-1.5.2.tar", last modified: Thu Dec 22 22:58:07 2022, max compression
+gzip compressed data, was "powerflex-monitoring-1.5.3.tar", last modified: Mon May  1 17:58:26 2023, max compression
```

## Comparing `powerflex-monitoring-1.5.2.tar` & `powerflex-monitoring-1.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hugo      (1000) hugo      (1000)        0 2022-12-22 22:58:07.689718 powerflex-monitoring-1.5.2/
--rw-r--r--   0 hugo      (1000) hugo      (1000)     5459 2022-12-22 22:58:07.689718 powerflex-monitoring-1.5.2/PKG-INFO
--rw-r--r--   0 hugo      (1000) hugo      (1000)     4504 2022-12-22 20:15:07.000000 powerflex-monitoring-1.5.2/README.md
--rw-r--r--   0 hugo      (1000) hugo      (1000)      100 2022-07-22 16:39:13.000000 powerflex-monitoring-1.5.2/pyproject.toml
--rw-r--r--   0 hugo      (1000) hugo      (1000)       38 2022-12-22 22:58:07.689718 powerflex-monitoring-1.5.2/setup.cfg
--rw-r--r--   0 hugo      (1000) hugo      (1000)     2050 2022-12-22 20:15:07.000000 powerflex-monitoring-1.5.2/setup.py
-drwxr-xr-x   0 hugo      (1000) hugo      (1000)        0 2022-12-22 22:58:07.686384 powerflex-monitoring-1.5.2/src/
-drwxr-xr-x   0 hugo      (1000) hugo      (1000)        0 2022-12-22 22:58:07.689718 powerflex-monitoring-1.5.2/src/powerflex_monitoring/
--rw-r--r--   0 hugo      (1000) hugo      (1000)        6 2022-12-22 22:57:55.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/VERSION
--rw-r--r--   0 hugo      (1000) hugo      (1000)      171 2022-07-22 16:39:13.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/__init__.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     2110 2022-12-22 20:15:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/diagnostic_recorder.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)      333 2022-07-22 16:39:13.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/format_exception.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     1419 2022-12-22 22:26:58.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/health_check.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     2466 2022-08-11 14:44:57.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/monitoring.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     8938 2022-12-22 20:15:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/nats_health_check.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     1549 2022-12-22 20:52:51.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/prometheus_metrics.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)        0 2022-08-08 18:01:31.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/py.typed
--rw-r--r--   0 hugo      (1000) hugo      (1000)     4603 2022-12-22 22:57:55.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/ready_check.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     9471 2022-12-22 20:15:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/redis_health_check.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     1320 2022-08-08 18:01:31.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/server_base.py
--rw-r--r--   0 hugo      (1000) hugo      (1000)     3119 2022-07-22 16:39:13.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring/wait_for_service_ready.py
-drwxr-xr-x   0 hugo      (1000) hugo      (1000)        0 2022-12-22 22:58:07.689718 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/
--rw-r--r--   0 hugo      (1000) hugo      (1000)     5459 2022-12-22 22:58:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 hugo      (1000) hugo      (1000)      863 2022-12-22 22:58:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 hugo      (1000) hugo      (1000)        1 2022-12-22 22:58:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 hugo      (1000) hugo      (1000)      149 2022-12-22 22:58:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/requires.txt
--rw-r--r--   0 hugo      (1000) hugo      (1000)       21 2022-12-22 22:58:07.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/top_level.txt
--rw-r--r--   0 hugo      (1000) hugo      (1000)        1 2022-07-22 16:44:08.000000 powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/zip-safe
+drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.588663 powerflex-monitoring-1.5.3/
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     5459 2023-05-01 17:58:26.588271 powerflex-monitoring-1.5.3/PKG-INFO
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     4504 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/README.md
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)      100 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/pyproject.toml
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)       38 2023-05-01 17:58:26.588882 powerflex-monitoring-1.5.3/setup.cfg
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2050 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/setup.py
+drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.554098 powerflex-monitoring-1.5.3/src/
+drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.584193 powerflex-monitoring-1.5.3/src/powerflex_monitoring/
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)        6 2023-05-01 17:24:25.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/VERSION
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)      171 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/__init__.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2110 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/diagnostic_recorder.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)      333 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/format_exception.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1419 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/health_check.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2466 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/monitoring.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     9687 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/nats_health_check.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1549 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/prometheus_metrics.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)        0 2022-08-10 21:43:07.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/py.typed
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     4603 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/ready_check.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     9471 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/redis_health_check.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1320 2022-08-10 21:43:07.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/server_base.py
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     3119 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/wait_for_service_ready.py
+drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.587256 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)     5459 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)      863 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)        1 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)      149 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/requires.txt
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)       21 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/top_level.txt
+-rw-r--r--   0 mark.zanfardino   (501) staff       (20)        1 2022-08-08 15:26:44.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/zip-safe
```

### Comparing `powerflex-monitoring-1.5.2/PKG-INFO` & `powerflex-monitoring-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerflex-monitoring
-Version: 1.5.2
+Version: 1.5.3
 Summary:  Tools to assist in monitoring a Python service.
 Home-page: https://github.com/edf-re/powerflex_python_monitoring
 Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_python_monitoring/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `powerflex-monitoring-1.5.2/README.md` & `powerflex-monitoring-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/setup.py` & `powerflex-monitoring-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/diagnostic_recorder.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/diagnostic_recorder.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/health_check.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/health_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/monitoring.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/nats_health_check.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/nats_health_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,14 +155,21 @@
         except (nats.errors.Error, nats.errors.TimeoutError) as exc:
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause=f"NATS request to test subject failed after timeout={timeout}. Exception: "
                 + format_exception(exc),
             )
             return
+        except Exception as unexpected_nats_request_exception:  # pylint: disable=broad-except
+            self.on_unhealthy(
+                health_check_name=health_check_name,
+                cause="Unexpected exception when checking NATS service request. Exception: "
+                + format_exception(unexpected_nats_request_exception),
+            )
+            return
         test_response = json.loads(response.data)
         if test_payload != test_response:
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause="NATS request to test subject returned incorrect data. "
                 f"Expected {test_payload}. "
                 f"Received {test_response}.",
@@ -186,14 +193,21 @@
         except requests.exceptions.ConnectionError as exc:
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause=f"Could not connect to NATS service health check address={address}. Exception: "
                 + format_exception(exc),
             )
             return
+        except Exception as unexpected_nats_health_exception:  # pylint: disable=broad-except
+            self.on_unhealthy(
+                health_check_name=health_check_name,
+                cause="Unexpected exception when checking NATS service health. Exception: "
+                + format_exception(unexpected_nats_health_exception),
+            )
+            return
 
         status = response.status_code
 
         if status != 200:
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause=f"NATS service health check returned non-200 status code {status}, address={address}",
```

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/prometheus_metrics.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/ready_check.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/ready_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/redis_health_check.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/redis_health_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/server_base.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/server_base.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring/wait_for_service_ready.py` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring/wait_for_service_ready.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/PKG-INFO` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerflex-monitoring
-Version: 1.5.2
+Version: 1.5.3
 Summary:  Tools to assist in monitoring a Python service.
 Home-page: https://github.com/edf-re/powerflex_python_monitoring
 Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_python_monitoring/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `powerflex-monitoring-1.5.2/src/powerflex_monitoring.egg-info/SOURCES.txt` & `powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

