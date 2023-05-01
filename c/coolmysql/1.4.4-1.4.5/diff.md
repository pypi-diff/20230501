# Comparing `tmp/coolmysql-1.4.4.tar.gz` & `tmp/coolmysql-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.4.tar", last modified: Tue Apr 25 12:41:11 2023, max compression
+gzip compressed data, was "coolmysql-1.4.5.tar", last modified: Mon May  1 02:00:29 2023, max compression
```

## Comparing `coolmysql-1.4.4.tar` & `coolmysql-1.4.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.4/LICENSE
--rw-r--r--   0        0        0     4252 2023-04-24 17:37:44.639289 coolmysql-1.4.4/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.4/coolmysql.py
--rw-r--r--   0        0        0      566 2023-04-25 12:38:10.810919 coolmysql-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 coolmysql-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.5/LICENSE
+-rw-r--r--   0        0        0     4261 2023-05-01 01:52:37.715384 coolmysql-1.4.5/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.5/coolmysql.py
+-rw-r--r--   0        0        0      582 2023-04-30 19:28:27.619336 coolmysql-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 coolmysql-1.4.5/PKG-INFO
```

### Comparing `coolmysql-1.4.4/LICENSE` & `coolmysql-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.4/README.md` & `coolmysql-1.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

### Comparing `coolmysql-1.4.4/pyproject.toml` & `coolmysql-1.4.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.4"
+version = "1.4.5"
 description = "史上最优雅的 mysql ORM"
 dependencies = ["lccpy >=1.4.5"]
 keywords = ["coolmysql", "pymysql", "mysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/coolmysql"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme"
```

### Comparing `coolmysql-1.4.4/PKG-INFO` & `coolmysql-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.4
+Version: 1.4.5
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.4.5
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmysql
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
 
 # 关于作者
```

