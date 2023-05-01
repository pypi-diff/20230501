# Comparing `tmp/encrypt256-1.8.1.tar.gz` & `tmp/encrypt256-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt256-1.8.1.tar", last modified: Mon Apr 10 14:47:54 2023, max compression
+gzip compressed data, was "encrypt256-1.8.2.tar", last modified: Mon May  1 02:00:52 2023, max compression
```

## Comparing `encrypt256-1.8.1.tar` & `encrypt256-1.8.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8.1/LICENSE
--rw-r--r--   0        0        0     2403 2023-04-10 14:47:10.950942 encrypt256-1.8.1/README.md
--rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.1/encrypt256.py
--rw-r--r--   0        0        0      616 2023-04-10 14:46:25.823266 encrypt256-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 encrypt256-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-14 11:47:56.900367 encrypt256-1.8.2/LICENSE
+-rw-r--r--   0        0        0     2373 2023-04-29 18:08:03.699670 encrypt256-1.8.2/README.md
+-rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.2/encrypt256.py
+-rw-r--r--   0        0        0      632 2023-04-30 19:28:40.636989 encrypt256-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2752 1970-01-01 00:00:00.000000 encrypt256-1.8.2/PKG-INFO
```

### Comparing `encrypt256-1.8.1/LICENSE` & `encrypt256-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encrypt256-1.8.1/README.md` & `encrypt256-1.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,34 +45,31 @@
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
 ### 加密
 
 ```python
-# 加密str型数据
-p1 = '人生自古谁五死'
-c1 = enctool.encrypt(p1, checkSize=32)
-
-# 加密bytes型数据
-p2 = '莎士比亚'.encode('utf8')
-c2 = enctool.encrypt(p2, checkSize=64)
+p1 = '人生自古谁五死'  # 可加密str型数据
+p2 = '莎士比亚'.encode('utf8')  # 可加密bytes型数据
+
+c1 = enctool.encrypt(p1)
+c2 = enctool.encrypt(p2)
 ```
 
 ### 解密
 
 ```python
-p11 = enctool.decrypt(c1)
-p22 = enctool.decrypt(c2)
-
-assert p1 == p11
-assert p2 == p22
+r1 = enctool.decrypt(c1)
+r2 = enctool.decrypt(c2)
 
-assert type(p1) is type(p11)
-assert type(p2) is type(p22)
+assert p1 == r1
+assert p2 == r2
+assert type(p1) is type(r1)
+assert type(p2) is type(r2)
 ```
 
 当发生以下情况时，会解密失败并报错：
 
 1、密钥错误。
 
 2、由于密文被篡改，导致AES算法解密失败。
```

### Comparing `encrypt256-1.8.1/pyproject.toml` & `encrypt256-1.8.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "encrypt256"
-version = "1.8.1"
+version = "1.8.2"
 description = "一个用于加密str型和bytes型数据的加密器"
 dependencies = ["lccpy >=1.3"]
 keywords = ["encrypt256", "encrypt", "AES", "pycryptodome", "Crypto"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/encrypt256"
+HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme"
```

### Comparing `encrypt256-1.8.1/PKG-INFO` & `encrypt256-1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: encrypt256
-Version: 1.8.1
+Version: 1.8.2
 Summary: 一个用于加密str型和bytes型数据的加密器
 Keywords: encrypt256,encrypt,AES,pycryptodome,Crypto
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: lccpy >=1.3
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/encrypt256
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme
 
 # 项目描述
 
 一个用于加密str型和bytes型数据的加密器。
 
 1、底层加密算法为AES-CBC-256。
 
@@ -57,34 +57,31 @@
 
 enctool = Encrypt256(password1)  # 创建加密器
 ```
 
 ### 加密
 
 ```python
-# 加密str型数据
-p1 = '人生自古谁五死'
-c1 = enctool.encrypt(p1, checkSize=32)
-
-# 加密bytes型数据
-p2 = '莎士比亚'.encode('utf8')
-c2 = enctool.encrypt(p2, checkSize=64)
+p1 = '人生自古谁五死'  # 可加密str型数据
+p2 = '莎士比亚'.encode('utf8')  # 可加密bytes型数据
+
+c1 = enctool.encrypt(p1)
+c2 = enctool.encrypt(p2)
 ```
 
 ### 解密
 
 ```python
-p11 = enctool.decrypt(c1)
-p22 = enctool.decrypt(c2)
-
-assert p1 == p11
-assert p2 == p22
+r1 = enctool.decrypt(c1)
+r2 = enctool.decrypt(c2)
 
-assert type(p1) is type(p11)
-assert type(p2) is type(p22)
+assert p1 == r1
+assert p2 == r2
+assert type(p1) is type(r1)
+assert type(p2) is type(r2)
 ```
 
 当发生以下情况时，会解密失败并报错：
 
 1、密钥错误。
 
 2、由于密文被篡改，导致AES算法解密失败。
```

