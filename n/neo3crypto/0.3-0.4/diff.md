# Comparing `tmp/neo3crypto-0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/neo3crypto-0.4-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 104437 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   225280 b- defN 22-Aug-08 08:55 neo3crypto.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2433 b- defN 22-Aug-08 08:55 neo3crypto-0.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2469 b- defN 22-Aug-08 08:55 neo3crypto-0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Aug-08 08:55 neo3crypto-0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Aug-08 08:55 neo3crypto-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      484 b- defN 22-Aug-08 08:55 neo3crypto-0.3.dist-info/RECORD
-6 files, 230777 bytes uncompressed, 103565 bytes compressed:  55.1%
+Zip file size: 106214 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   237568 b- defN 23-May-01 09:36 neo3crypto.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-May-01 09:36 neo3crypto-0.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2375 b- defN 23-May-01 09:36 neo3crypto-0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-01 09:36 neo3crypto-0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-01 09:36 neo3crypto-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      485 b- defN 23-May-01 09:36 neo3crypto-0.4.dist-info/RECORD
+6 files, 242974 bytes uncompressed, 105340 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: neo3crypto.cp39-win_amd64.pyd
+Filename: neo3crypto.cp311-win_amd64.pyd
 Comment: 
 
-Filename: neo3crypto-0.3.dist-info/LICENSE.txt
+Filename: neo3crypto-0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: neo3crypto-0.3.dist-info/METADATA
+Filename: neo3crypto-0.4.dist-info/METADATA
 Comment: 
 
-Filename: neo3crypto-0.3.dist-info/WHEEL
+Filename: neo3crypto-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: neo3crypto-0.3.dist-info/top_level.txt
+Filename: neo3crypto-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: neo3crypto-0.3.dist-info/RECORD
+Filename: neo3crypto-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neo3crypto-0.3.dist-info/LICENSE.txt` & `neo3crypto-0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `neo3crypto-0.3.dist-info/METADATA` & `neo3crypto-0.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: neo3crypto
-Version: 0.3
+Version: 0.4
 Summary: Native crypto functions for the NEO 3 Blockchain
 Home-page: https://github.com/CityOfZion/neo3crypto
 Author: Erik van den Brink
 Author-email: erik@coz.io
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: C++
-Requires-Python: >=3.8.*
+Requires-Python: >=3.10.0,<=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 .. image:: https://raw.githubusercontent.com/CityOfZion/visual-identity/develop/_CoZ%20Branding/_Logo/_Logo%20icon/_PNG%20200x178px/CoZ_Icon_DARKBLUE_200x178px.png
     :alt: CoZ logo
 
 
 NEO3VM
 ------
-C++ implementations of cryptographic functions used in the NEO3 Blockchain with bindings for Python 3.8, 3.9 & 3.10.
+C++ implementations of cryptographic functions used in the NEO3 Blockchain with bindings for Python 3.10 & 3.11.
 
 The current version supports `mmh3` and EllipticCurve functions by wrapping (part of `smhasher <https://github.com/aappleby/smhasher>`_ and `micro-ecc <https://github.com/kmackay/micro-ecc>`_)
 and exposing helper classes. ``SECP256R1`` (a.k.a ``NIST256P``) and ``SECP256K1`` are the only curves exposed, but others can easily
 be enabled if needed.
 
 Installation
 ~~~~~~~~~~~~
@@ -35,15 +33,15 @@
 
     pip install neo3crypto
 
 Or download the wheels from the Github releases page.
 
 Windows users
 =============
-If installing fails with the error ``No Matching distribution found`` then upgrade your Python installation to use the latest post release version (i.e. ``3.8.8`` instead of ``3.8.0``)
+If installing fails with the error ``No Matching distribution found`` then upgrade your Python installation to use the latest post release version (i.e. ``3.10.8`` instead of ``3.10.0``)
 
 Usage
 ~~~~~
 
 ::
 
     import hashlib
```

