# Comparing `tmp/increment-1.3.tar.gz` & `tmp/increment-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increment-1.3.tar", last modified: Mon Apr 10 14:19:46 2023, max compression
+gzip compressed data, was "increment-1.3.1.tar", last modified: Mon May  1 02:01:16 2023, max compression
```

## Comparing `increment-1.3.tar` & `increment-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3/LICENSE
--rw-r--r--   0        0        0     1691 2023-04-08 16:28:37.947596 increment-1.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3/increment.py
--rw-r--r--   0        0        0      582 2023-04-10 09:20:39.407916 increment-1.3/pyproject.toml
--rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 increment-1.3/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1699 2023-04-30 13:10:09.947977 increment-1.3.1/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.1/increment.py
+-rw-r--r--   0        0        0      606 2023-04-30 19:29:45.948669 increment-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 increment-1.3.1/PKG-INFO
```

### Comparing `increment-1.3/LICENSE` & `increment-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `increment-1.3/README.md` & `increment-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 项目描述
 
-主键生成器，支持多机器|多进程|多线程高并发生成。
+分布式主键生成器，支持多机器|多进程|多线程并发生成。
 
 # 安装
 
 ```
 pip install increment
 ```
 
@@ -69,8 +69,8 @@
 
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
```

### Comparing `increment-1.3/pyproject.toml` & `increment-1.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "increment"
-version = "1.3"
-description = "主键生成器，支持多机器|多进程|多线程高并发生成"
+version = "1.3.1"
+description = "分布式主键生成器，支持多机器|多进程|多线程并发生成"
 dependencies = ["lccpy >=1.3"]
 keywords = ["increment"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/increment"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme"
```

### Comparing `increment-1.3/PKG-INFO` & `increment-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: increment
-Version: 1.3
-Summary: 主键生成器，支持多机器|多进程|多线程高并发生成
+Version: 1.3.1
+Summary: 分布式主键生成器，支持多机器|多进程|多线程并发生成
 Keywords: increment
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.3
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/increment
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme
 
 # 项目描述
 
-主键生成器，支持多机器|多进程|多线程高并发生成。
+分布式主键生成器，支持多机器|多进程|多线程并发生成。
 
 # 安装
 
 ```
 pip install increment
 ```
 
@@ -82,7 +82,8 @@
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
 ![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+
```

