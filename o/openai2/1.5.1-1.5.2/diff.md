# Comparing `tmp/openai2-1.5.1.tar.gz` & `tmp/openai2-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.1.tar", last modified: Sun Apr  9 11:43:44 2023, max compression
+gzip compressed data, was "openai2-1.5.2.tar", last modified: Mon May  1 02:01:39 2023, max compression
```

## Comparing `openai2-1.5.1.tar` & `openai2-1.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.1/LICENSE
--rw-r--r--   0        0        0     2353 2023-04-09 11:34:19.920750 openai2-1.5.1/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.1/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.1/openai2/__init__.py
--rw-r--r--   0        0        0     2016 2023-03-28 03:12:38.016827 openai2-1.5.1/openai2/openai2.py
--rw-r--r--   0        0        0      618 2023-04-09 11:33:28.584926 openai2-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 openai2-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2257 2023-04-30 18:48:25.007298 openai2-1.5.2/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.2/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.2/openai2/__init__.py
+-rw-r--r--   0        0        0     2016 2023-03-28 03:12:38.016827 openai2-1.5.2/openai2/openai2.py
+-rw-r--r--   0        0        0      634 2023-04-30 19:31:38.138340 openai2-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 openai2-1.5.2/PKG-INFO
```

### Comparing `openai2-1.5.1/LICENSE` & `openai2-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.1/README.md` & `openai2-1.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -98,8 +98,8 @@
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/tree/main/coolmysql#readme)
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
```

### Comparing `openai2-1.5.1/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.2/openai2/Licenses of dependent packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.1/openai2/openai2.py` & `openai2-1.5.2/openai2/openai2.py`

 * *Files identical despite different names*

### Comparing `openai2-1.5.1/pyproject.toml` & `openai2-1.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.1"
+version = "1.5.2"
 description = "根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。"
 dependencies = ["openai >=0.27.0"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/openai2"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme"
```

### Comparing `openai2-1.5.1/PKG-INFO` & `openai2-1.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.1
+Version: 1.5.2
 Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/openai2
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme
 
 # 项目描述
 
 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 
 # 安装
 
@@ -110,9 +110,8 @@
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/tree/main/coolmysql#readme)
-
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
```

