# Comparing `tmp/coinkite-tap-protocol-1.2.1.tar.gz` & `tmp/coinkite-tap-protocol-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinkite-tap-protocol-1.2.1.tar", last modified: Thu Oct 13 15:03:12 2022, max compression
+gzip compressed data, was "coinkite-tap-protocol-1.2.2.tar", last modified: Fri Apr 28 15:16:23 2023, max compression
```

## Comparing `coinkite-tap-protocol-1.2.1.tar` & `coinkite-tap-protocol-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2022-10-13 15:03:12.641387 coinkite-tap-protocol-1.2.1/
--rw-r--r--   0 peter      (501) staff       (20)     1982 2022-02-16 16:15:17.000000 coinkite-tap-protocol-1.2.1/COPYING-CC
--rw-r--r--   0 peter      (501) staff       (20)     1982 2022-02-16 16:15:17.000000 coinkite-tap-protocol-1.2.1/LICENSE
--rw-r--r--   0 peter      (501) staff       (20)    11236 2022-10-13 15:03:12.641105 coinkite-tap-protocol-1.2.1/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)    10625 2022-08-12 16:05:28.000000 coinkite-tap-protocol-1.2.1/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2022-10-13 15:03:12.639268 coinkite-tap-protocol-1.2.1/cktap/
--rw-r--r--   0 peter      (501) staff       (20)      118 2022-09-06 13:46:10.000000 coinkite-tap-protocol-1.2.1/cktap/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     9163 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.1/cktap/_ecdsa.py
--rw-r--r--   0 peter      (501) staff       (20)     2206 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.1/cktap/base58.py
--rw-r--r--   0 peter      (501) staff       (20)     5021 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.1/cktap/bech32.py
--rw-r--r--   0 peter      (501) staff       (20)    16731 2022-06-28 14:13:01.000000 coinkite-tap-protocol-1.2.1/cktap/bip32.py
--rwxr-xr-x   0 peter      (501) staff       (20)    37581 2022-09-07 15:10:06.000000 coinkite-tap-protocol-1.2.1/cktap/cli.py
--rw-r--r--   0 peter      (501) staff       (20)     3106 2022-07-01 12:24:19.000000 coinkite-tap-protocol-1.2.1/cktap/compat.py
--rw-r--r--   0 peter      (501) staff       (20)     1583 2022-04-21 15:19:44.000000 coinkite-tap-protocol-1.2.1/cktap/constants.py
--rw-r--r--   0 peter      (501) staff       (20)     2257 2022-04-19 16:28:44.000000 coinkite-tap-protocol-1.2.1/cktap/descriptors.py
--rw-r--r--   0 peter      (501) staff       (20)      282 2022-01-04 16:55:25.000000 coinkite-tap-protocol-1.2.1/cktap/exceptions.py
--rw-r--r--   0 peter      (501) staff       (20)    19043 2022-09-07 14:49:27.000000 coinkite-tap-protocol-1.2.1/cktap/proto.py
--rw-r--r--   0 peter      (501) staff       (20)    14679 2021-11-19 14:33:56.000000 coinkite-tap-protocol-1.2.1/cktap/ripemd.py
--rw-r--r--   0 peter      (501) staff       (20)     4699 2022-10-13 15:01:10.000000 coinkite-tap-protocol-1.2.1/cktap/sweep.py
--rw-r--r--   0 peter      (501) staff       (20)     5181 2022-07-05 12:55:57.000000 coinkite-tap-protocol-1.2.1/cktap/transport.py
--rw-r--r--   0 peter      (501) staff       (20)     2459 2022-06-28 15:56:53.000000 coinkite-tap-protocol-1.2.1/cktap/uploads.py
--rw-r--r--   0 peter      (501) staff       (20)    12344 2022-09-07 13:58:53.000000 coinkite-tap-protocol-1.2.1/cktap/utils.py
--rw-r--r--   0 peter      (501) staff       (20)     3211 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.1/cktap/verify_link.py
--rw-r--r--   0 peter      (501) staff       (20)     2378 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.1/cktap/wrap_coincurve.py
--rw-r--r--   0 peter      (501) staff       (20)     2049 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.1/cktap/wrap_ecdsa.py
--rw-r--r--   0 peter      (501) staff       (20)     3046 2022-09-06 13:40:11.000000 coinkite-tap-protocol-1.2.1/cktap/wrap_pysecp.py
--rw-r--r--   0 peter      (501) staff       (20)     2540 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.1/cktap/wrap_wally.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2022-10-13 15:03:12.640753 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)    11236 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      682 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       60 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/entry_points.txt
--rw-r--r--   0 peter      (501) staff       (20)      250 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)        6 2022-10-13 15:03:12.000000 coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2022-10-13 15:03:12.641455 coinkite-tap-protocol-1.2.1/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)     2272 2022-06-28 15:03:38.000000 coinkite-tap-protocol-1.2.1/setup.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-28 15:16:23.174309 coinkite-tap-protocol-1.2.2/
+-rw-r--r--   0 peter      (501) staff       (20)     1982 2022-02-16 16:15:17.000000 coinkite-tap-protocol-1.2.2/COPYING-CC
+-rw-r--r--   0 peter      (501) staff       (20)     1982 2022-02-16 16:15:17.000000 coinkite-tap-protocol-1.2.2/LICENSE
+-rw-r--r--   0 peter      (501) staff       (20)    11751 2023-04-28 15:16:23.173986 coinkite-tap-protocol-1.2.2/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)    11140 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/README.md
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-28 15:16:23.172937 coinkite-tap-protocol-1.2.2/cktap/
+-rw-r--r--   0 peter      (501) staff       (20)      118 2023-04-28 15:14:07.000000 coinkite-tap-protocol-1.2.2/cktap/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     9163 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.2/cktap/_ecdsa.py
+-rw-r--r--   0 peter      (501) staff       (20)     2206 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.2/cktap/base58.py
+-rw-r--r--   0 peter      (501) staff       (20)     5021 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.2/cktap/bech32.py
+-rw-r--r--   0 peter      (501) staff       (20)    16736 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/cktap/bip32.py
+-rwxr-xr-x   0 peter      (501) staff       (20)    38674 2023-04-27 13:30:04.000000 coinkite-tap-protocol-1.2.2/cktap/cli.py
+-rw-r--r--   0 peter      (501) staff       (20)     3097 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/cktap/compat.py
+-rw-r--r--   0 peter      (501) staff       (20)     1741 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/cktap/constants.py
+-rw-r--r--   0 peter      (501) staff       (20)     2257 2022-04-19 16:28:44.000000 coinkite-tap-protocol-1.2.2/cktap/descriptors.py
+-rw-r--r--   0 peter      (501) staff       (20)      282 2022-01-04 16:55:25.000000 coinkite-tap-protocol-1.2.2/cktap/exceptions.py
+-rw-r--r--   0 peter      (501) staff       (20)    19043 2022-09-07 14:49:27.000000 coinkite-tap-protocol-1.2.2/cktap/proto.py
+-rw-r--r--   0 peter      (501) staff       (20)     5071 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/cktap/ripemd.py
+-rw-r--r--   0 peter      (501) staff       (20)     4699 2023-04-26 14:56:42.000000 coinkite-tap-protocol-1.2.2/cktap/sweep.py
+-rw-r--r--   0 peter      (501) staff       (20)     5181 2022-07-05 12:55:57.000000 coinkite-tap-protocol-1.2.2/cktap/transport.py
+-rw-r--r--   0 peter      (501) staff       (20)     2459 2022-06-28 15:56:53.000000 coinkite-tap-protocol-1.2.2/cktap/uploads.py
+-rw-r--r--   0 peter      (501) staff       (20)    12344 2022-09-07 13:58:53.000000 coinkite-tap-protocol-1.2.2/cktap/utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     3211 2022-04-21 15:29:37.000000 coinkite-tap-protocol-1.2.2/cktap/verify_link.py
+-rw-r--r--   0 peter      (501) staff       (20)     2378 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.2/cktap/wrap_coincurve.py
+-rw-r--r--   0 peter      (501) staff       (20)     2049 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.2/cktap/wrap_ecdsa.py
+-rw-r--r--   0 peter      (501) staff       (20)     3046 2022-09-06 13:40:11.000000 coinkite-tap-protocol-1.2.2/cktap/wrap_pysecp.py
+-rw-r--r--   0 peter      (501) staff       (20)     2540 2022-05-04 15:46:13.000000 coinkite-tap-protocol-1.2.2/cktap/wrap_wally.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-28 15:16:23.173812 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)    11751 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      682 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)       60 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/entry_points.txt
+-rw-r--r--   0 peter      (501) staff       (20)      250 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)        6 2023-04-28 15:16:23.000000 coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2023-04-28 15:16:23.174360 coinkite-tap-protocol-1.2.2/setup.cfg
+-rw-r--r--   0 peter      (501) staff       (20)     2272 2022-06-28 15:03:38.000000 coinkite-tap-protocol-1.2.2/setup.py
```

### Comparing `coinkite-tap-protocol-1.2.1/COPYING-CC` & `coinkite-tap-protocol-1.2.2/COPYING-CC`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/LICENSE` & `coinkite-tap-protocol-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/PKG-INFO` & `coinkite-tap-protocol-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,22 @@
-Metadata-Version: 2.1
-Name: coinkite-tap-protocol
-Version: 1.2.1
-Summary: Communicate with your TAPSIGNER or SATSCARD using Python
-Home-page: https://github.com/coinkite/coinkite-tap-proto
-Author: Coinkite Inc.
-Author-email: support@coinkite.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: test
-Provides-Extra: test_plus
-License-File: LICENSE
-License-File: COPYING-CC
-
 # Coinkite Tap Protocol and Helper Program
 
 This Python library enables easy communication with **TAPSIGNER<sup>&trade;</sup>**,  **SATSCARD<sup>&trade;</sup>** and **SATSCHIP<sup>&trade;</sup>**.
 
 **-==[Request card development samples [here](https://coinkite.cards/dev)]==-**
 
 Repository contents:
 
 1. The protocol specification
 2. Python library for speaking the protocol
 3. Supporting documentation
 
-Examples/Libraries in other languages will be added when available.
+Examples/Libraries in other languages:
+- C++ https://github.com/nunchuk-io/tap-protocol
+- React Native https://github.com/bithyve/cktap-protocol-react-native
 
 ## Documentation Links
 
 - **[Docs and Spec subdirectory (./docs)](docs)**
   - [Protocol specification](docs/protocol.md)
   - [NFC specification](docs/nfc-spec.md)
   - [Best Practices and Warnings](docs/best-practices.md)
@@ -86,27 +68,40 @@
 - Python 3.6 or higher
 - `pyscard` for access to smart card readers
 - A supported smart card reader. In theory, all smart card USB CCID class-compliant
   devices should work. Our observations:
     - **ACS ACR1252U** - okay and widely available, and for sale by Coinkite
     - **Identiv uTrust 3700F** - reliable and looks nice
     - **HID Omnikey 5022 CL** (not 5021) - fast, cute, and small
+    - **HID OmniKey 5427 CK** - tested Gen1 device, fast, reliable, must disable keyboard wedge via EEM interface on device at `http://192.168.63.99/`, when correct will identify as VID:PID `076b:5427`
     - **NOT recommended:** ACS ACR122U. It can work, and is widely available, but is not reliable.
 - See `requirements.txt` file for python packages needed.
 
 
 ## Ubuntu/Debian Notes
+
 Installing `pyscard` require SWIG and libpcsclite:
+
 ```shell
 # run below before installing dependencies with pip
 # tested on Ubuntu 20.04 (only)
 sudo apt-get install swig
 sudo apt-get install libpcsclite-dev
 ```
 
+## Fedora/Red Hat Notes
+
+Installing `pyscard` requires SWIG and the pcsc-lite library:
+
+```shell
+# run below before installing dependencies with pip
+# tested on Fedora 37 (only)
+sudo dnf install swig pcsc-lite-devel
+```
+
 ## Windows Notes
 
 Installing `pyscard` may require SWIG:
 
 1. Download .zip from <http://swig.org>.
 2. Extract and move into `C:\Program Files`.
 3. Add that to system PATH.
@@ -364,9 +359,7 @@
 00000040  26 6c 98 59 34 95 aa 78  a1 0b 7a 2b 77 98 1f 7a  |&l.Y4..x..z+w..z|
 00000050  d1 cf d6 e6 fd 31 b3 88  1a d9 df 68 03 a3 8b 06  |.....1.....h....|
 00000060  db 66 ef d6 ea 5f 5f 08  9a ed f2 2a 71           |.f...__....*q|
 0000006d
 
 ```
 For more information about specific `cktap` commands check `docs/cli.md`
-
-
```

### Comparing `coinkite-tap-protocol-1.2.1/README.md` & `coinkite-tap-protocol-1.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,42 @@
+Metadata-Version: 2.1
+Name: coinkite-tap-protocol
+Version: 1.2.2
+Summary: Communicate with your TAPSIGNER or SATSCARD using Python
+Home-page: https://github.com/coinkite/coinkite-tap-proto
+Author: Coinkite Inc.
+Author-email: support@coinkite.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: cli
+Provides-Extra: test
+Provides-Extra: test_plus
+License-File: LICENSE
+License-File: COPYING-CC
+
 # Coinkite Tap Protocol and Helper Program
 
 This Python library enables easy communication with **TAPSIGNER<sup>&trade;</sup>**,  **SATSCARD<sup>&trade;</sup>** and **SATSCHIP<sup>&trade;</sup>**.
 
 **-==[Request card development samples [here](https://coinkite.cards/dev)]==-**
 
 Repository contents:
 
 1. The protocol specification
 2. Python library for speaking the protocol
 3. Supporting documentation
 
-Examples/Libraries in other languages will be added when available.
+Examples/Libraries in other languages:
+- C++ https://github.com/nunchuk-io/tap-protocol
+- React Native https://github.com/bithyve/cktap-protocol-react-native
 
 ## Documentation Links
 
 - **[Docs and Spec subdirectory (./docs)](docs)**
   - [Protocol specification](docs/protocol.md)
   - [NFC specification](docs/nfc-spec.md)
   - [Best Practices and Warnings](docs/best-practices.md)
@@ -66,27 +88,40 @@
 - Python 3.6 or higher
 - `pyscard` for access to smart card readers
 - A supported smart card reader. In theory, all smart card USB CCID class-compliant
   devices should work. Our observations:
     - **ACS ACR1252U** - okay and widely available, and for sale by Coinkite
     - **Identiv uTrust 3700F** - reliable and looks nice
     - **HID Omnikey 5022 CL** (not 5021) - fast, cute, and small
+    - **HID OmniKey 5427 CK** - tested Gen1 device, fast, reliable, must disable keyboard wedge via EEM interface on device at `http://192.168.63.99/`, when correct will identify as VID:PID `076b:5427`
     - **NOT recommended:** ACS ACR122U. It can work, and is widely available, but is not reliable.
 - See `requirements.txt` file for python packages needed.
 
 
 ## Ubuntu/Debian Notes
+
 Installing `pyscard` require SWIG and libpcsclite:
+
 ```shell
 # run below before installing dependencies with pip
 # tested on Ubuntu 20.04 (only)
 sudo apt-get install swig
 sudo apt-get install libpcsclite-dev
 ```
 
+## Fedora/Red Hat Notes
+
+Installing `pyscard` requires SWIG and the pcsc-lite library:
+
+```shell
+# run below before installing dependencies with pip
+# tested on Fedora 37 (only)
+sudo dnf install swig pcsc-lite-devel
+```
+
 ## Windows Notes
 
 Installing `pyscard` may require SWIG:
 
 1. Download .zip from <http://swig.org>.
 2. Extract and move into `C:\Program Files`.
 3. Add that to system PATH.
@@ -344,7 +379,9 @@
 00000040  26 6c 98 59 34 95 aa 78  a1 0b 7a 2b 77 98 1f 7a  |&l.Y4..x..z+w..z|
 00000050  d1 cf d6 e6 fd 31 b3 88  1a d9 df 68 03 a3 8b 06  |.....1.....h....|
 00000060  db 66 ef d6 ea 5f 5f 08  9a ed f2 2a 71           |.f...__....*q|
 0000006d
 
 ```
 For more information about specific `cktap` commands check `docs/cli.md`
+
+
```

### Comparing `coinkite-tap-protocol-1.2.1/cktap/_ecdsa.py` & `coinkite-tap-protocol-1.2.2/cktap/_ecdsa.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/base58.py` & `coinkite-tap-protocol-1.2.2/cktap/base58.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/bech32.py` & `coinkite-tap-protocol-1.2.2/cktap/bech32.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/bip32.py` & `coinkite-tap-protocol-1.2.2/cktap/bip32.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,14 @@
 
 
 HARDENED = 2 ** 31
 
 Prv_or_PubKeyNode = Union["PrvKeyNode", "PubKeyNode"]
 
 
-def hash160(s: bytes) -> bytes:
-    """
-    sha256 followed by ripemd160
-
-    :param s: data
-    :return: hashed data
-    """
-    return hashlib.new('ripemd160', hashlib.sha256(s).digest()).digest()
-
-
 def big_endian_to_int(b: bytes) -> int:
     """
     Big endian representation to integer.
 
     :param b: big endian representation
     :return: integer
     """
@@ -180,14 +170,15 @@
 
     def fingerprint(self) -> bytes:
         """
         Gets current node fingerprint.
 
         :return: first four bytes of SHA256(RIPEMD160(public key))
         """
+        from cktap.compat import hash160
         return hash160(self.sec())[:4]
 
     @classmethod
     def parse(cls, s: Union[str, bytes, BytesIO],
               testnet: bool = False) -> Prv_or_PubKeyNode:
         """
         Initializes private/public key node from serialized node or
@@ -455,15 +446,20 @@
             (Note: this has probability lower than 1 in 2**127.)
 
         :param index: derivation index
         :return: derived child
         """
         if index >= HARDENED:
             # hardened
-            data = b"\x00" + self.key + int_to_big_endian(index, 4)
+            if len(self.key) < 33:
+                to_pad = 33 - len(self.key)
+                key = (b"\x00" * to_pad) + self.key
+            else:
+                key = self.key
+            data = key + int_to_big_endian(index, 4)
         else:
             data = privkey_to_pubkey(self.key) + int_to_big_endian(index, 4)
         I = hmac.new(key=self.chain_code, msg=data, digestmod=hashlib.sha512).digest()
         IL, IR = I[:32], I[32:]
         if big_endian_to_int(IL) >= N:
             InvalidKeyError(
                 "private key {} is greater/equal to curve order".format(
```

### Comparing `coinkite-tap-protocol-1.2.1/cktap/cli.py` & `coinkite-tap-protocol-1.2.2/cktap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,17 +305,16 @@
     sig = str(b64encode(rec_sig), 'ascii').replace('\n', '')
 
     if just_sig or card.is_tapsigner:
         click.echo(str(sig))
     else:
         addr = card.get_address(slot=be_slot)
         if verbose:
-            click.echo('-----BEGIN SIGNED MESSAGE-----\n{msg}\n-----BEGIN '
-                      'SIGNATURE-----\n{addr}\n{sig}\n-----END SIGNED MESSAGE-----'.format(
-                            msg=message.decode('ascii'), addr=addr, sig=sig))
+            click.echo(RFC_SIGNATURE_TEMPLATE.format(msg=message.decode('ascii'),
+                                                     addr=addr, sig=sig))
         else:
             click.echo('%s\n%s\n%s' % (message.decode('ascii'), addr, sig))
     
 @main.command('version')
 def get_version():
     "Get the version of the card's firmware installed (but not upgradable)"
 
@@ -896,17 +895,21 @@
                 card.send('wait')
                 bar.update(1)
 
 @main.command('upload')
 @click.argument('cvc', default='123456', type=str, metavar="(PIN code)", required=False)
 @click.option('--localhost', '-l', is_flag=True, help="Upload to local dev server")
 @click.option('--skip-prompts', '-q', is_flag=True, help="Skip prompts for new values")
+@click.option('--init-card', '--init', is_flag=True, help="Setup private key if needed")
+@click.option('--offline', is_flag=True, help="Skip check for previous data online")
 @click.option('--image', '-i', type=click.Path(exists=True, dir_okay=False),
                         help="Image to upload (PNG or JPEG)", required=False)
-def upload_artwork(cvc, image, localhost, skip_prompts):
+@click.option('--meta', '-m', multiple=True, help="Provide meta values by name (can be repeated)",
+                                metavar="key='Value'")
+def upload_artwork(cvc, image, localhost, skip_prompts, init_card, meta, offline):
     "[SATSCHIP] Upload an image and artwork's metadata to public website"
     from urllib.parse import urlparse
     import cbor2, requests, datetime
     from . import __version__
 
     card = get_card(only_chip=True)
     cvc = cleanup_cvc(card, cvc)
@@ -926,74 +929,100 @@
 
     while 1:
         st = card.get_status()
         path = st.get('path', None)
         if path is not None:
             break
 
-        if not click.confirm(f'No private key picked yet. Pick now?', default=True):
-            click.echo("Private required to continue.", err=True)
-            sys.exit(1)
-            continue
+        if not init_card:
+            if not click.confirm(f'No private key picked yet. Pick now?', default=True):
+                click.echo("Private required to continue.", err=True)
+                sys.exit(1)
+                continue
 
         # do basic setup now
         args = dict(chain_code=sha256s(sha256s(os.urandom(128))), slot=0)
         ses_key, resp = card.send_auth('new', cvc, **args)
 
     # enforce a default for which subkey
     EXPECT_PATH = 'm/84h/0h/0h'
     if path2str(path) != 'm/84h/0h/0h':
         click.echo(f"Require default path of {EXPECT_PATH}", err=True)
         sys.exit(1)
     subpath = '420/69'
 
-    my_pubkey = card.get_pubkey(cvc, subpath=subpath)
+    try:
+        my_pubkey = card.get_pubkey(cvc, subpath=subpath)
+    except CardRuntimeError:
+        # wrong cvc -> prompt
+        cvc = getpass("Enter spending code: ")
+        cvc = cleanup_cvc(card, cvc)
+        my_pubkey = card.get_pubkey(cvc, subpath=subpath)
+
     my_address = render_address(my_pubkey)
 
     ses = requests.Session()
     #ses.headers['user-agent'] = f'cktap/{__version__}'
 
     from .uploads import META_VERSION, MAX_IMG_SIZE, META_FIELDS, ALL_FIELDS
 
     # collect data to be stored.
     data = dict((fn, None) for fn,_ in META_FIELDS)
     data['is_public'] = True
     data['created_at'] = datetime.datetime.now()
 
-    # see if we can restore a previous upload, or run
-    try:
-        print("Checking for previousiously uploaded values... ", end='')
-        old = ses.get(url + '.cbor').body()
-        seq = cbor2.loads(old)
-
-        if seq[0] != META_VERSION or len(seq[2]) == 65:
-            raise ValueError('version?')
-
-        # assume server verified signature
-        data.update(cbor2.loads(seq[1]))
-        print(" Done")
-    except:
-        print(" (failed or got none)")
+    if not offline:
+        # see if we can restore a previous upload, or run
+        try:
+            print("Checking for previousiously uploaded values... ", end='')
+            old = ses.get(url + '.cbor').body()
+            seq = cbor2.loads(old)
+
+            if seq[0] != META_VERSION or len(seq[2]) == 65:
+                raise ValueError('version?')
+
+            # assume server verified signature
+            data.update(cbor2.loads(seq[1]))
+            print(" Done")
+        except:
+            print(" (failed or got none)")
 
     if os.path.exists(fname):
         print(f"Loading from previous attempt... {fname}")
         try:
             old = open(fname, 'rb').read()
             seq = cbor2.loads(old)
             if seq[0] == META_VERSION and len(seq[2]) == 65:
                 data.update(cbor2.loads(seq[1]))
         except:
             raise
-            print("(failed) ignoring previous run's data")
+            #print("(failed) ignoring previous run's data")
 
     for k in list(data.keys()):
         if k not in ALL_FIELDS:
             print(f"Removing obsolete field: {k}")
             del data[k]
 
+    if meta:
+        mlabels = dict(META_FIELDS)
+        for ln in meta:
+            if '=' not in ln:
+                fail(f'Need = in meta arg: {ln}')
+
+            k,v = ln.split('=')
+            k = k.strip()
+            if k not in ALL_FIELDS:
+                fail(f'Unknown meta value key: {k}')
+
+            if k.startswith('is_'):
+                v = True if v.lower() in {'1', 'true', 'yes'} else False
+
+            data[k] = v
+            print(f'{mlabels[k]}: {v}')
+
     while not skip_prompts:
         print("\nEnter updated metadata values. Any may be left blank and all are optional.\n\n")
 
         for fn, label in META_FIELDS:
             if fn == 'image':
                 if image:
                     print(f"Image will be from: {image}")
@@ -1002,22 +1031,14 @@
                     continue
                 else:
                     image = click.prompt('Enter image file to use',
                                     type=click.Path(exists=False, dir_okay=False),
                                     default='')
                     if not image: continue
 
-                # will let server validate the image contents because I don't 
-                # want to add Pillow to dependances here
-                data[fn] = open(image, 'rb').read()
-
-                if len(data[fn]) >= MAX_IMG_SIZE:
-                    print(f"Image file must be less than {int(MAX_IMG_SIZE/1E6)} megabytes.")
-                    sys.exit(1)
-
             elif fn.startswith('is_'):
                 data[fn] = click.confirm(label, default=data[fn])
             else:
                 # text values
                 while 1:
                     v = click.prompt(label, default=data[fn] or '')
                     v = v.strip()
@@ -1046,14 +1067,25 @@
             else:
                 print(data[fn])
 
         print('\n\n')
         if click.confirm("All correct?", default=True): break
         if click.confirm("Quit now?"): sys.exit(0)
 
+
+    if image and not data['image']:
+        # will let server validate the image contents because I don't 
+        # want to add Pillow to dependances here
+        raw = open(image, 'rb').read()
+
+        if len(raw) >= MAX_IMG_SIZE:
+            print(f"Image file must be less than {int(MAX_IMG_SIZE/1E6)} megabytes.")
+            sys.exit(1)
+        data['image'] = raw
+
     data['pubkey'] = my_pubkey
     data['card_ident'] = card.card_ident        # redundent, but useful
     data['card_pubkey'] = card.card_pubkey
     data['applet_version'] = card.applet_version
     data['birth_height'] = card.birth_height
     data['updated_at'] = datetime.datetime.now()
     data['cert_chain'] = card.send('certs')['cert_chain']
@@ -1077,15 +1109,14 @@
 
     complete = cbor2.dumps( (META_VERSION, body, rec_sig, card_nonce, check['auth_sig']) )
 
     open(fname, 'wb').write(complete)
 
     print(f"\nData captured into local file: {fname}")
 
-    full_url = url+'.cbor/'+host.fragment
-
-    if click.confirm("Upload to server?", default=True):
+    if not offline and click.confirm("Upload to server?", default=True):
+        full_url = url+'.cbor/'+host.fragment
         resp = ses.put(full_url, data=complete, headers={'content-type': 'application/cbor'})
         print("Server says:\n")
         print(resp.text)
 
 # EOF
```

### Comparing `coinkite-tap-protocol-1.2.1/cktap/compat.py` & `coinkite-tap-protocol-1.2.2/cktap/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 def sha256s(msg):
     # single-shot SHA256
     from hashlib import sha256
     return sha256(msg).digest()
 
 def hash160(x):
     # classic bitcoin nested hashes
-    from .ripemd import RIPEMD160
-    return RIPEMD160(sha256s(x)).digest()
+    from .ripemd import ripemd160
+    return ripemd160(sha256s(x))
 
 # Other codes must be implemented elsewhere...
 #
 
 def CT_pick_keypair():
     # return (priv, pub)
     raise NotImplementedError
```

### Comparing `coinkite-tap-protocol-1.2.1/cktap/descriptors.py` & `coinkite-tap-protocol-1.2.2/cktap/descriptors.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/proto.py` & `coinkite-tap-protocol-1.2.2/cktap/proto.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/sweep.py` & `coinkite-tap-protocol-1.2.2/cktap/sweep.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/transport.py` & `coinkite-tap-protocol-1.2.2/cktap/transport.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/uploads.py` & `coinkite-tap-protocol-1.2.2/cktap/uploads.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/utils.py` & `coinkite-tap-protocol-1.2.2/cktap/utils.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/verify_link.py` & `coinkite-tap-protocol-1.2.2/cktap/verify_link.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/wrap_coincurve.py` & `coinkite-tap-protocol-1.2.2/cktap/wrap_coincurve.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/wrap_ecdsa.py` & `coinkite-tap-protocol-1.2.2/cktap/wrap_ecdsa.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/wrap_pysecp.py` & `coinkite-tap-protocol-1.2.2/cktap/wrap_pysecp.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/cktap/wrap_wally.py` & `coinkite-tap-protocol-1.2.2/cktap/wrap_wally.py`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/PKG-INFO` & `coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinkite-tap-protocol
-Version: 1.2.1
+Version: 1.2.2
 Summary: Communicate with your TAPSIGNER or SATSCARD using Python
 Home-page: https://github.com/coinkite/coinkite-tap-proto
 Author: Coinkite Inc.
 Author-email: support@coinkite.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
@@ -26,15 +26,17 @@
 
 Repository contents:
 
 1. The protocol specification
 2. Python library for speaking the protocol
 3. Supporting documentation
 
-Examples/Libraries in other languages will be added when available.
+Examples/Libraries in other languages:
+- C++ https://github.com/nunchuk-io/tap-protocol
+- React Native https://github.com/bithyve/cktap-protocol-react-native
 
 ## Documentation Links
 
 - **[Docs and Spec subdirectory (./docs)](docs)**
   - [Protocol specification](docs/protocol.md)
   - [NFC specification](docs/nfc-spec.md)
   - [Best Practices and Warnings](docs/best-practices.md)
@@ -86,27 +88,40 @@
 - Python 3.6 or higher
 - `pyscard` for access to smart card readers
 - A supported smart card reader. In theory, all smart card USB CCID class-compliant
   devices should work. Our observations:
     - **ACS ACR1252U** - okay and widely available, and for sale by Coinkite
     - **Identiv uTrust 3700F** - reliable and looks nice
     - **HID Omnikey 5022 CL** (not 5021) - fast, cute, and small
+    - **HID OmniKey 5427 CK** - tested Gen1 device, fast, reliable, must disable keyboard wedge via EEM interface on device at `http://192.168.63.99/`, when correct will identify as VID:PID `076b:5427`
     - **NOT recommended:** ACS ACR122U. It can work, and is widely available, but is not reliable.
 - See `requirements.txt` file for python packages needed.
 
 
 ## Ubuntu/Debian Notes
+
 Installing `pyscard` require SWIG and libpcsclite:
+
 ```shell
 # run below before installing dependencies with pip
 # tested on Ubuntu 20.04 (only)
 sudo apt-get install swig
 sudo apt-get install libpcsclite-dev
 ```
 
+## Fedora/Red Hat Notes
+
+Installing `pyscard` requires SWIG and the pcsc-lite library:
+
+```shell
+# run below before installing dependencies with pip
+# tested on Fedora 37 (only)
+sudo dnf install swig pcsc-lite-devel
+```
+
 ## Windows Notes
 
 Installing `pyscard` may require SWIG:
 
 1. Download .zip from <http://swig.org>.
 2. Extract and move into `C:\Program Files`.
 3. Add that to system PATH.
```

### Comparing `coinkite-tap-protocol-1.2.1/coinkite_tap_protocol.egg-info/SOURCES.txt` & `coinkite-tap-protocol-1.2.2/coinkite_tap_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinkite-tap-protocol-1.2.1/setup.py` & `coinkite-tap-protocol-1.2.2/setup.py`

 * *Files identical despite different names*

