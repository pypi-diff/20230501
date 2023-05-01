# Comparing `tmp/cos-alerter-0.2.0.tar.gz` & `tmp/cos-alerter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos-alerter-0.2.0.tar", last modified: Thu Apr 13 15:16:30 2023, max compression
+gzip compressed data, was "cos-alerter-0.3.0.tar", last modified: Mon May  1 12:53:08 2023, max compression
```

## Comparing `cos-alerter-0.2.0.tar` & `cos-alerter-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    11357 2023-03-15 12:19:34.000000 cos-alerter-0.2.0/LICENSE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1300 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/cos_alerter/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     6324 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/cos_alerter/alerter.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3518 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/cos_alerter/daemon.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1126 2023-04-11 20:01:19.000000 cos-alerter-0.2.0/cos_alerter/logging.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1465 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/cos_alerter/server.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/cos_alerter.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      398 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       56 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/entry_points.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       61 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/requires.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       12 2023-04-13 15:16:30.000000 cos-alerter-0.2.0/cos_alerter.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1747 2023-04-13 15:16:12.000000 cos-alerter-0.2.0/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       38 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/setup.cfg
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-13 15:16:30.956799 cos-alerter-0.2.0/tests/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     6502 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/tests/test_alerter.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2477 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/tests/test_daemon.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2439 2023-04-13 15:13:25.000000 cos-alerter-0.2.0/tests/test_server.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)    11357 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/LICENSE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1300 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/cos_alerter/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     6442 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/alerter.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3738 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/daemon.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1126 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/logging.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1554 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/server.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/cos_alerter.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      398 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)       56 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/entry_points.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)       93 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/requires.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)       12 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1518 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)       38 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/tests/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     6547 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_alerter.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     2522 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_daemon.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     2607 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_server.py
```

### Comparing `cos-alerter-0.2.0/LICENSE` & `cos-alerter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.2.0/PKG-INFO` & `cos-alerter-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-alerter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A watcher for Alertmanager
 Author-email: Dylan Stephano-Shachter <dylan.stephano-shachter@canonical.com>
 Project-URL: Homepage, https://github.com/canonical/cos-alerter
 Project-URL: Bug Tracker, https://github.com/canonical/cos-alerter/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

### Comparing `cos-alerter-0.2.0/README.md` & `cos-alerter-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.2.0/cos_alerter/alerter.py` & `cos-alerter-0.3.0/cos_alerter/alerter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """Main logic for COS Alerter."""
 
 import datetime
 import logging
 import textwrap
 import threading
 import time
+from pathlib import Path
 
 import apprise
 import durationpy
 import yaml
 
 logger = logging.getLogger(__name__)
 
@@ -19,17 +20,21 @@
 class Config:
     """Representation of the config file."""
 
     def __getitem__(self, key):
         """Dict style access for config values."""
         return self.data[key]
 
+    def set_path(self, path: str):
+        """Set the config file path."""
+        self.path = Path(path)
+
     def reload(self):
         """Reload config values from the disk."""
-        with open("/etc/cos-alerter.yaml", "r") as f:
+        with open(self.path, "r") as f:
             self.data = yaml.safe_load(f)
         self.data["watch"]["down_interval"] = durationpy.from_str(
             self.data["watch"]["down_interval"]
         ).total_seconds()
         self.data["notify"]["repeat_interval"] = durationpy.from_str(
             self.data["notify"]["repeat_interval"]
         ).total_seconds()
```

### Comparing `cos-alerter-0.2.0/cos_alerter/daemon.py` & `cos-alerter-0.3.0/cos_alerter/daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,20 @@
     """Parse the command line arguments."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--log-level",
         choices=list(LEVELS),
         help='Logging level. Overrides config value "log_level"',
     )
+    parser.add_argument(
+        "--config",
+        required=False,
+        default="/etc/cos-alerter.yaml",
+        help="Path to config file. Defaults to /etc/cos-alerter.yaml",
+    )
     return parser.parse_args(args=args)
 
 
 def client_loop(clientid):
     """Run the main loop for the specified client."""
     # Main loop
     state = AlerterState(clientid=clientid)
@@ -64,14 +70,15 @@
 
     Args:
         run_for: This argument is for testing purposes. If set, only run for "run_for" seconds.
         argv: Can be used to override the cli args for testing purposes.
     """
     args = parse_args(argv[1:])
 
+    config.set_path(args.config)
     config.reload()
     init_logging(args)
     AlerterState.initialize()
 
     # Observe signal handlers
     try:  # pragma: no cover
         signal.signal(signal.SIGINT, sigint)
```

### Comparing `cos-alerter-0.2.0/cos_alerter/logging.py` & `cos-alerter-0.3.0/cos_alerter/logging.py`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.2.0/cos_alerter/server.py` & `cos-alerter-0.3.0/cos_alerter/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # See LICENSE file for licensing details.
 
 """HTTP server for COS Alerter."""
 
 import logging
 
 from flask import Flask, request
+from prometheus_flask_exporter import PrometheusMetrics
 
 from .alerter import AlerterState, config
 
 app = Flask(__name__)
+metrics = PrometheusMetrics(app)
 logger = logging.getLogger(__name__)
 
 
 @app.route("/alive", methods=["POST"])
 def alive():
     """Endpoint for Alertmanager instances to send their heartbeat alerts."""
     # TODO Decide if we should validate the request.
```

### Comparing `cos-alerter-0.2.0/cos_alerter.egg-info/PKG-INFO` & `cos-alerter-0.3.0/cos_alerter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-alerter
-Version: 0.2.0
+Version: 0.3.0
 Summary: A watcher for Alertmanager
 Author-email: Dylan Stephano-Shachter <dylan.stephano-shachter@canonical.com>
 Project-URL: Homepage, https://github.com/canonical/cos-alerter
 Project-URL: Bug Tracker, https://github.com/canonical/cos-alerter/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

### Comparing `cos-alerter-0.2.0/pyproject.toml` & `cos-alerter-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cos-alerter"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Dylan Stephano-Shachter", email="dylan.stephano-shachter@canonical.com" }
 ]
 description = "A watcher for Alertmanager"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,46 +18,41 @@
   "Topic :: System :: Monitoring",
   "Development Status :: 3 - Alpha",
 ]
 dependencies = [
   "apprise~=1.3",
   "durationpy",
   "flask~=2.2",
+  "prometheus_flask_exporter~=0.22",
   "waitress~=2.1",
   "pyyaml~=6.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/canonical/cos-alerter"
 "Bug Tracker" = "https://github.com/canonical/cos-alerter/issues"
 
 [project.scripts]
 cos-alerter = "cos_alerter.daemon:main"
 
 [tool.black]
 line-length = 99
 
-[tool.isort]
-profile = "black"
-
-[tool.flake8]
-max-line-length = 99
-max-doc-length = 99
-exclude = [".git", "__pycache__", ".tox", "build", "dist", "*.egg_info", "venv"]
-select = ["E", "W", "F", "C", "N", "R", "D", "H"]
-# Ignore W503, E501 because using black creates errors with this
+[tool.ruff]
+line-length = 99
+extend-exclude = ["__pycache__", "*.egg_info"]
+select = ["E", "W", "F", "C", "N", "R", "D", "I001"]
+# Ignore E501 because using black creates errors with this
 # Ignore D107 Missing docstring in __init__
-ignore = ["W503", "E501", "D107"]
+ignore = ["E501", "D107"]
 # D100, D101, D102, D103: Ignore missing docstrings in tests
-per-file-ignores = ["tests/*:D100,D101,D102,D103"]
-docstring-convention = "google"
-# Check for properly formatted copyright header in each file
-copyright-check = "True"
-copyright-author = "Canonical Ltd."
-copyright-regexp = "Copyright\\s\\d{4}([-,]\\d{4})*\\s+%(author)s"
+per-file-ignores = {"tests/*" = ["D100","D101","D102","D103"]}
+
+[tool.ruff.pydocstyle]
+convention = "google"
 
 [tool.pyright]
 include = ["cos_alerter"]
 pythonVersion = "3.8"
 pythonPlatform = "Linux"
 
 [tool.pytest.ini_options]
```

### Comparing `cos-alerter-0.2.0/tests/test_alerter.py` & `cos-alerter-0.3.0/tests/test_alerter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 @pytest.fixture
 def fake_fs(fs):
     fs.create_file("/etc/cos-alerter.yaml")
     with open("/etc/cos-alerter.yaml", "w") as f:
         f.write(yaml.dump(CONFIG))
+    config.set_path("/etc/cos-alerter.yaml")
     config.reload()
     return fs
 
 
 def assert_notifications(notify_mock, add_mock, title, body):
     add_mock.assert_has_calls([unittest.mock.call(x) for x in DESTINATIONS])
     notify_mock.assert_called_with(title=title, body=body)
```

### Comparing `cos-alerter-0.2.0/tests/test_daemon.py` & `cos-alerter-0.3.0/tests/test_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                         "destinations": DESTINATIONS,
                         "repeat_interval": "4s",
                     },
                     "log_level": "info",
                 }
             )
         )
+    config.set_path("/etc/cos-alerter.yaml")
     config.reload()
     return fs
 
 
 @pytest.mark.slow
 @unittest.mock.patch.object(apprise.Apprise, "add")
 @unittest.mock.patch.object(apprise.Apprise, "notify")
```

### Comparing `cos-alerter-0.2.0/tests/test_server.py` & `cos-alerter-0.3.0/tests/test_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 @pytest.fixture
 def fake_fs(fs):
     fs.create_file("/etc/cos-alerter.yaml")
     with open("/etc/cos-alerter.yaml", "w") as f:
         f.write(yaml.dump(CONFIG))
+    config.set_path("/etc/cos-alerter.yaml")
     config.reload()
     return fs
 
 
 @pytest.fixture
 def state_init():
     AlerterState.initialize()
@@ -59,14 +60,18 @@
 def test_alive_updates_time(flask_client, fake_fs, state_init):
     flask_client.post("/alive", query_string=PARAMS)
     state = AlerterState(clientid="client0")
     with state:
         assert state.data["alert_time"] > state.start_time
 
 
+def test_metrics_succeeds(flask_client, fake_fs, state_init):
+    assert flask_client.get("/metrics").status_code == 200
+
+
 def test_no_clientid(flask_client, fake_fs, state_init):
     assert flask_client.post("/alive").status_code == 400
 
 
 def test_wrong_clientid(flask_client, fake_fs, state_init):
     assert flask_client.post("/alive", query_string={"clientid": "client1"}).status_code == 404
```

