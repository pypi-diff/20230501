# Comparing `tmp/asymongo-1.3.1.tar.gz` & `tmp/asymongo-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymongo-1.3.1.tar", last modified: Mon May  1 01:47:53 2023, max compression
+gzip compressed data, was "asymongo-1.3.2.tar", last modified: Mon May  1 01:56:11 2023, max compression
```

## Comparing `asymongo-1.3.1.tar` & `asymongo-1.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.1/LICENSE
--rw-r--r--   0        0        0     5175 2023-04-16 20:01:06.324279 asymongo-1.3.1/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.1/asymongo.py
--rw-r--r--   0        0        0      583 2023-05-01 01:47:43.619310 asymongo-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 asymongo-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5184 2023-05-01 01:51:56.097037 asymongo-1.3.2/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.2/asymongo.py
+-rw-r--r--   0        0        0      583 2023-05-01 01:53:26.451415 asymongo-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 asymongo-1.3.2/PKG-INFO
```

### Comparing `asymongo-1.3.1/LICENSE` & `asymongo-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asymongo-1.3.1/README.md` & `asymongo-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install asymongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/asymongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

### Comparing `asymongo-1.3.1/pyproject.toml` & `asymongo-1.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymongo"
-version = "1.3.1"
+version = "1.3.2"
 description = "异步的 MongoDB ORM"
 dependencies = ["lccpy >=1.3.1"]
 keywords = ["asymongo", "motor", "mongodb", "pymongo"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `asymongo-1.3.1/PKG-INFO` & `asymongo-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asymongo
-Version: 1.3.1
+Version: 1.3.2
 Summary: 异步的 MongoDB ORM
 Keywords: asymongo,motor,mongodb,pymongo
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.3.1
@@ -14,15 +14,15 @@
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install asymongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/asymongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

