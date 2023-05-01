# Comparing `tmp/edge_logger-0.0.5.tar.gz` & `tmp/edge_logger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.5.tar", max compression
+gzip compressed data, was "edge_logger-0.0.6.tar", max compression
```

## Comparing `edge_logger-0.0.5.tar` & `edge_logger-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.5/edge_logger/__init__.py
--rw-r--r--   0        0        0     5700 2023-04-28 06:17:30.970678 edge_logger-0.0.5/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      380 2023-04-28 06:26:05.689175 edge_logger-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.6/edge_logger/__init__.py
+-rw-r--r--   0        0        0     5765 2023-05-01 16:14:44.418206 edge_logger-0.0.6/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      380 2023-05-01 16:22:07.102204 edge_logger-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.6/PKG-INFO
```

### Comparing `edge_logger-0.0.5/LICENSE` & `edge_logger-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_logger-0.0.5/edge_logger/edge_logger.py` & `edge_logger-0.0.6/edge_logger/edge_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def format(self, record):
         log_data = {
             'time': self.formatTime(record),
             'level': record.levelname,
             'name': record.name,
             'message': record.getMessage(),
-            # 'line': record.lineno,
+            'line': record.lineno,
         }
         # If we added extra information, update log record
         if record.__getattribute__("_extra"):
             log_data.update(record.__getattribute__("_extra"))
         if self._indent:
             return json.dumps(log_data, indent=4)
         else:
@@ -90,26 +90,28 @@
 
 class EdgeLogger(logging.Logger):
     """
     Subclass logging.Logger so we can extend makeRecord to add dynamic information on a per-log basis
     https://docs.python.org/3/library/logging.html#logging.Logger
     """
 
-    def __init__(self, name: str, stream=sys.stdout):
+    def __init__(self, name: str, stream=sys.stdout, logger_level="INFO", console_level="DEBUG"):
+
+        # root logger
         super().__init__(name)
 
         # Base logger level. Messages will be further filtered by each handler.
-        self.setLevel(logging.DEBUG)
+        self.setLevel(logger_level)
 
         # create console handler and set level to info
         ch = logging.StreamHandler(stream=stream)
         ch.set_name("console_handler")
 
         # Console handler log level will filter the messages that are actually sent to stdout.
-        ch.setLevel(logging.INFO)
+        ch.setLevel(console_level)
         ch.setFormatter(JsonFormatter())
 
         # add ch to logger
         self.addHandler(ch)
 
     def makeRecord(
             self,
```

