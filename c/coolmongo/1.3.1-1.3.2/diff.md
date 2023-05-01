# Comparing `tmp/coolmongo-1.3.1.tar.gz` & `tmp/coolmongo-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.1.tar", last modified: Tue Apr 25 12:40:53 2023, max compression
+gzip compressed data, was "coolmongo-1.3.2.tar", last modified: Mon May  1 02:00:03 2023, max compression
```

## Comparing `coolmongo-1.3.1.tar` & `coolmongo-1.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.1/LICENSE
--rw-r--r--   0        0        0     5025 2023-04-24 17:37:54.832465 coolmongo-1.3.1/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.1/coolmongo.py
--rw-r--r--   0        0        0      570 2023-04-25 12:38:48.061938 coolmongo-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 coolmongo-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5034 2023-05-01 01:52:29.170682 coolmongo-1.3.2/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.2/coolmongo.py
+-rw-r--r--   0        0        0      586 2023-04-30 19:28:19.809211 coolmongo-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5314 1970-01-01 00:00:00.000000 coolmongo-1.3.2/PKG-INFO
```

### Comparing `coolmongo-1.3.1/LICENSE` & `coolmongo-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.1/README.md` & `coolmongo-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 史上最优雅的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

### Comparing `coolmongo-1.3.1/pyproject.toml` & `coolmongo-1.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.3.1"
+version = "1.3.2"
 description = "史上最优雅的 MongoDB ORM"
 dependencies = ["lccpy >=1.4.5"]
 keywords = ["coolmongo", "pymongo", "mongodb"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/coolmongo"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme"
```

### Comparing `coolmongo-1.3.1/PKG-INFO` & `coolmongo-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3.1
+Version: 1.3.2
 Summary: 史上最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.5
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmongo
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme
 
 # 项目描述
 
 史上最优雅的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/coolmongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

