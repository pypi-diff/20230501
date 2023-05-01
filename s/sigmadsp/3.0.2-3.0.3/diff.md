# Comparing `tmp/sigmadsp-3.0.2.tar.gz` & `tmp/sigmadsp-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmadsp-3.0.2.tar", max compression
+gzip compressed data, was "sigmadsp-3.0.3.tar", max compression
```

## Comparing `sigmadsp-3.0.2.tar` & `sigmadsp-3.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/LICENSE
--rw-r--r--   0        0        0     3615 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/README.md
--rw-r--r--   0        0        0     1198 2023-04-30 06:28:27.613323 sigmadsp-3.0.2/pyproject.toml
--rw-r--r--   0        0        0       99 2023-04-30 06:28:27.613323 sigmadsp-3.0.2/sigmadsp/__init__.py
--rw-r--r--   0        0        0    14651 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/backend.py
--rw-r--r--   0        0        0       92 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/__init__.py
--rw-r--r--   0        0        0     3108 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/adau14xx.py
--rw-r--r--   0        0        0     3006 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/adau1x01.py
--rw-r--r--   0        0        0     9870 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/common.py
--rw-r--r--   0        0        0     3297 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/dsp/factory.py
--rw-r--r--   0        0        0     5268 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/frontend.py
--rw-r--r--   0        0        0       53 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/__init__.py
--rw-r--r--   0        0        0      223 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/__init__.py
--rw-r--r--   0        0        0     4802 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.py
--rw-r--r--   0        0        0     5651 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.pyi
--rw-r--r--   0        0        0     4033 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2_grpc.py
--rw-r--r--   0        0        0       86 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/__init__.py
--rw-r--r--   0        0        0     7388 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/conversion.py
--rw-r--r--   0        0        0     9510 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/parser.py
--rw-r--r--   0        0        0     2262 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/helper/settings.py
--rw-r--r--   0        0        0       78 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/__init__.py
--rw-r--r--   0        0        0     2981 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/common.py
--rw-r--r--   0        0        0     1855 2023-04-30 06:28:09.860748 sigmadsp-3.0.2/sigmadsp/protocols/i2c.py
--rw-r--r--   0        0        0     4404 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/protocols/spi.py
--rw-r--r--   0        0        0       64 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/__init__.py
--rw-r--r--   0        0        0     1722 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/adau14xx.py
--rw-r--r--   0        0        0     1505 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/adau1x01.py
--rw-r--r--   0        0        0      695 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/common.py
--rw-r--r--   0        0        0    11449 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/header.py
--rw-r--r--   0        0        0     8600 2023-04-30 06:28:09.864748 sigmadsp-3.0.2/sigmadsp/sigmastudio/server.py
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 sigmadsp-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-01 21:18:22.947966 sigmadsp-3.0.3/LICENSE
+-rw-r--r--   0        0        0     3755 2023-05-01 21:18:22.947966 sigmadsp-3.0.3/README.md
+-rw-r--r--   0        0        0     1198 2023-05-01 21:18:43.448146 sigmadsp-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-05-01 21:18:43.452146 sigmadsp-3.0.3/sigmadsp/__init__.py
+-rw-r--r--   0        0        0    14651 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/backend.py
+-rw-r--r--   0        0        0       92 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/__init__.py
+-rw-r--r--   0        0        0     3108 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/adau14xx.py
+-rw-r--r--   0        0        0     3006 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/adau1x01.py
+-rw-r--r--   0        0        0     9870 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/common.py
+-rw-r--r--   0        0        0     3297 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/dsp/factory.py
+-rw-r--r--   0        0        0     5268 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/frontend.py
+-rw-r--r--   0        0        0       53 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/__init__.py
+-rw-r--r--   0        0        0     4802 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.py
+-rw-r--r--   0        0        0     5651 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.pyi
+-rw-r--r--   0        0        0     4033 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2_grpc.py
+-rw-r--r--   0        0        0       86 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/__init__.py
+-rw-r--r--   0        0        0     7388 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/conversion.py
+-rw-r--r--   0        0        0     9510 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/parser.py
+-rw-r--r--   0        0        0     2262 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/helper/settings.py
+-rw-r--r--   0        0        0       78 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/__init__.py
+-rw-r--r--   0        0        0     2981 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/common.py
+-rw-r--r--   0        0        0     1855 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/i2c.py
+-rw-r--r--   0        0        0     4404 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/protocols/spi.py
+-rw-r--r--   0        0        0       64 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/adau14xx.py
+-rw-r--r--   0        0        0     1505 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/adau1x01.py
+-rw-r--r--   0        0        0      695 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/common.py
+-rw-r--r--   0        0        0    11449 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/header.py
+-rw-r--r--   0        0        0     8600 2023-05-01 21:18:22.951966 sigmadsp-3.0.3/sigmadsp/sigmastudio/server.py
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 sigmadsp-3.0.3/PKG-INFO
```

### Comparing `sigmadsp-3.0.2/LICENSE` & `sigmadsp-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/README.md` & `sigmadsp-3.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -46,38 +46,39 @@
 cd sigmadsp &&
 ./install.sh
 ```
 
 The script installs the Python package, which includes the `sigmadsp-backend` (the backend) and `sigmadsp` (the frontend) executables.
 It also sets up a system service, which runs `sigmadsp-backend` in the background.
 
-## Upgrading
+[pipx](https://pypa.github.io/pipx/) is used for installing the Python package in an isolated way, without having to use `sudo pip install <package>`.
 
-For upgrading, the installation procedure can be repeated, but will overwrite the current configuration file.
+## Upgrading
 
-Instead, simply upgrade the Python package and restart the backend service:
+For upgrading, use `pipx` to upgrade the Python package and restart the backend service afterwards:
 
 ```bash
-sudo pip3 install sigmadsp --upgrade &&
+pipx upgrade sigmadsp &&
 sudo systemctl restart sigmadsp-backend.service
 ```
 
-
 ## Removal
 
 From within the previously cloned repository folder `sigmadsp` run
 
 ```bash
 ./uninstall.sh
 ```
 
+If you find that this removal procedure leaves any files unremoved, please open an issue.
+
 ## Configuration
 
 Configuration of `sigmadsp` is done via a `*.yaml` file, which is created during installation. Its default path is `/var/lib/sigmadsp/config.yaml`.
 
 ## Usage
 
-For a list of commands that can be emitted by the frontend, simply type
+For a list of commands that can be emitted by the frontend, please type
 
 ```bash
 sigmadsp -h
 ```
```

### Comparing `sigmadsp-3.0.2/pyproject.toml` & `sigmadsp-3.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sigmadsp"
 license = "GPL-3.0-or-later"
-version = "3.0.2"
+version = "3.0.3"
 description = "A package for controlling Analog Devices Sigma DSP chipsets."
 readme = "README.md"
 authors = ["Adrian Figueroa <elagil@takanome.de>"]
 repository = "https://github.com/elagil/sigmadsp"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `sigmadsp-3.0.2/sigmadsp/backend.py` & `sigmadsp-3.0.3/sigmadsp/backend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/dsp/adau14xx.py` & `sigmadsp-3.0.3/sigmadsp/dsp/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/dsp/adau1x01.py` & `sigmadsp-3.0.3/sigmadsp/dsp/adau1x01.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/dsp/common.py` & `sigmadsp-3.0.3/sigmadsp/dsp/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/dsp/factory.py` & `sigmadsp-3.0.3/sigmadsp/dsp/factory.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/frontend.py` & `sigmadsp-3.0.3/sigmadsp/frontend.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.py` & `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2.pyi` & `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/generated/backend_service/control_pb2_grpc.py` & `sigmadsp-3.0.3/sigmadsp/generated/backend_service/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/helper/conversion.py` & `sigmadsp-3.0.3/sigmadsp/helper/conversion.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/helper/parser.py` & `sigmadsp-3.0.3/sigmadsp/helper/parser.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/helper/settings.py` & `sigmadsp-3.0.3/sigmadsp/helper/settings.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/protocols/common.py` & `sigmadsp-3.0.3/sigmadsp/protocols/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/protocols/i2c.py` & `sigmadsp-3.0.3/sigmadsp/protocols/i2c.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/protocols/spi.py` & `sigmadsp-3.0.3/sigmadsp/protocols/spi.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/sigmastudio/adau14xx.py` & `sigmadsp-3.0.3/sigmadsp/sigmastudio/adau14xx.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/sigmastudio/adau1x01.py` & `sigmadsp-3.0.3/sigmadsp/sigmastudio/adau1x01.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/sigmastudio/common.py` & `sigmadsp-3.0.3/sigmadsp/sigmastudio/common.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/sigmastudio/header.py` & `sigmadsp-3.0.3/sigmadsp/sigmastudio/header.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/sigmadsp/sigmastudio/server.py` & `sigmadsp-3.0.3/sigmadsp/sigmastudio/server.py`

 * *Files identical despite different names*

### Comparing `sigmadsp-3.0.2/PKG-INFO` & `sigmadsp-3.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmadsp
-Version: 3.0.2
+Version: 3.0.3
 Summary: A package for controlling Analog Devices Sigma DSP chipsets.
 Home-page: https://github.com/elagil/sigmadsp
 License: GPL-3.0-or-later
 Author: Adrian Figueroa
 Author-email: elagil@takanome.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -73,39 +73,40 @@
 cd sigmadsp &&
 ./install.sh
 ```
 
 The script installs the Python package, which includes the `sigmadsp-backend` (the backend) and `sigmadsp` (the frontend) executables.
 It also sets up a system service, which runs `sigmadsp-backend` in the background.
 
-## Upgrading
+[pipx](https://pypa.github.io/pipx/) is used for installing the Python package in an isolated way, without having to use `sudo pip install <package>`.
 
-For upgrading, the installation procedure can be repeated, but will overwrite the current configuration file.
+## Upgrading
 
-Instead, simply upgrade the Python package and restart the backend service:
+For upgrading, use `pipx` to upgrade the Python package and restart the backend service afterwards:
 
 ```bash
-sudo pip3 install sigmadsp --upgrade &&
+pipx upgrade sigmadsp &&
 sudo systemctl restart sigmadsp-backend.service
 ```
 
-
 ## Removal
 
 From within the previously cloned repository folder `sigmadsp` run
 
 ```bash
 ./uninstall.sh
 ```
 
+If you find that this removal procedure leaves any files unremoved, please open an issue.
+
 ## Configuration
 
 Configuration of `sigmadsp` is done via a `*.yaml` file, which is created during installation. Its default path is `/var/lib/sigmadsp/config.yaml`.
 
 ## Usage
 
-For a list of commands that can be emitted by the frontend, simply type
+For a list of commands that can be emitted by the frontend, please type
 
 ```bash
 sigmadsp -h
 ```
```

