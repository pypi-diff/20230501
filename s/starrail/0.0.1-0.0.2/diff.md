# Comparing `tmp/starrail-0.0.1.tar.gz` & `tmp/starrail-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Coding\Python\Workspace\starrail\dist\.tmp-e3wxdoor\starrail-0.0.1.tar", last modified: Wed Apr 26 10:45:14 2023, max compression
+gzip compressed data, was "C:\Coding\Python\Workspace\starrail\dist\.tmp-w572st2a\starrail-0.0.2.tar", last modified: Sun Apr 30 23:17:37 2023, max compression
```

## Comparing `starrail-0.0.1.tar` & `starrail-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.488475 starrail-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-26 09:19:23.000000 starrail-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      940 2023-04-26 10:45:14.488475 starrail-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-26 10:41:55.000000 starrail-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-04-26 08:07:25.000000 starrail-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      835 2023-04-26 10:45:14.490494 starrail-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.461547 starrail-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.470523 starrail-0.0.1/src/starrail/
--rw-rw-rw-   0        0        0     1318 2023-04-26 10:23:12.000000 starrail-0.0.1/src/starrail/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.486481 starrail-0.0.1/src/starrail/cmd/
--rw-rw-rw-   0        0        0     1154 2023-04-26 10:23:22.000000 starrail-0.0.1/src/starrail/cmd/__init__.py
--rw-rw-rw-   0        0        0     1264 2023-04-26 10:28:53.000000 starrail-0.0.1/src/starrail/cmd/start_star_rail.py
--rw-rw-rw-   0        0        0     1154 2023-04-26 09:40:50.000000 starrail-0.0.1/src/starrail/constants.py
--rw-rw-rw-   0        0        0     1450 2023-04-26 10:23:05.000000 starrail-0.0.1/src/starrail/honkai_star_rail.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.483488 starrail-0.0.1/src/starrail.egg-info/
--rw-rw-rw-   0        0        0      940 2023-04-26 10:45:14.000000 starrail-0.0.1/src/starrail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-26 10:45:14.000000 starrail-0.0.1/src/starrail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:45:14.000000 starrail-0.0.1/src/starrail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-26 10:45:14.000000 starrail-0.0.1/src/starrail.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 10:45:14.000000 starrail-0.0.1/src/starrail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:14.487478 starrail-0.0.1/tests/
--rw-rw-rw-   0        0        0     1175 2023-04-26 10:28:32.000000 starrail-0.0.1/tests/test_starrail.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.546932 starrail-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-26 09:19:23.000000 starrail-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-04-30 13:54:30.000000 starrail-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4357 2023-04-30 23:17:37.546932 starrail-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3778 2023-04-30 07:35:56.000000 starrail-0.0.2/README.md
+-rw-rw-rw-   0        0        0      186 2023-04-30 13:53:57.000000 starrail-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      858 2023-04-30 23:17:37.551917 starrail-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.494617 starrail-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.506585 starrail-0.0.2/src/starrail/
+-rw-rw-rw-   0        0        0     1532 2023-04-29 07:07:18.000000 starrail-0.0.2/src/starrail/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.527982 starrail-0.0.2/src/starrail/_config/
+-rw-rw-rw-   0        0        0     1154 2023-04-26 22:07:12.000000 starrail-0.0.2/src/starrail/_config/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-04-30 13:53:06.000000 starrail-0.0.2/src/starrail/_config/config.json
+-rw-rw-rw-   0        0        0     4890 2023-04-30 13:41:40.000000 starrail-0.0.2/src/starrail/_config/config_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.530974 starrail-0.0.2/src/starrail/_data/
+-rw-rw-rw-   0        0        0     1154 2023-04-29 02:53:27.000000 starrail-0.0.2/src/starrail/_data/__init__.py
+-rw-rw-rw-   0        0        0     1851 2023-04-29 04:06:27.000000 starrail-0.0.2/src/starrail/_data/disclaimer.txt
+-rw-rw-rw-   0        0        0      534 2023-04-30 22:39:19.000000 starrail-0.0.2/src/starrail/_data/path_config_ex.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.531972 starrail-0.0.2/src/starrail/_exceptions/
+-rw-rw-rw-   0        0        0     1154 2023-04-26 22:07:19.000000 starrail-0.0.2/src/starrail/_exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2477 2023-04-30 13:40:45.000000 starrail-0.0.2/src/starrail/_exceptions/_exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.533966 starrail-0.0.2/src/starrail/_utils/
+-rw-rw-rw-   0        0        0     1154 2023-04-26 22:07:20.000000 starrail-0.0.2/src/starrail/_utils/__init__.py
+-rw-rw-rw-   0        0        0     4610 2023-04-30 22:47:04.000000 starrail-0.0.2/src/starrail/_utils/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.536959 starrail-0.0.2/src/starrail/_utils/loader/
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:46:40.000000 starrail-0.0.2/src/starrail/_utils/loader/__init__.py
+-rw-rw-rw-   0        0        0     1724 2023-04-30 22:24:42.000000 starrail-0.0.2/src/starrail/_utils/loader/loader.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.538953 starrail-0.0.2/src/starrail/_utils/pick/
+-rw-rw-rw-   0        0        0     1133 2023-04-30 03:42:59.000000 starrail-0.0.2/src/starrail/_utils/pick/__init__.py
+-rw-rw-rw-   0        0        0     7912 2023-04-30 05:02:23.000000 starrail-0.0.2/src/starrail/_utils/pick/pick.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.541945 starrail-0.0.2/src/starrail/cmd/
+-rw-rw-rw-   0        0        0     1154 2023-04-26 10:23:22.000000 starrail-0.0.2/src/starrail/cmd/__init__.py
+-rw-rw-rw-   0        0        0    14399 2023-04-30 23:09:25.000000 starrail-0.0.2/src/starrail/cmd/cl_endpoints.py
+-rw-rw-rw-   0        0        0     1187 2023-04-27 02:10:01.000000 starrail-0.0.2/src/starrail/constants.py
+-rw-rw-rw-   0        0        0     3629 2023-04-30 13:34:34.000000 starrail-0.0.2/src/starrail/honkai_star_rail.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.544937 starrail-0.0.2/src/starrail/user_interface/
+-rw-rw-rw-   0        0        0     1154 2023-04-30 13:31:07.000000 starrail-0.0.2/src/starrail/user_interface/__init__.py
+-rw-rw-rw-   0        0        0     1154 2023-04-30 23:09:45.000000 starrail-0.0.2/src/starrail/user_interface/ui_backend.py
+-rw-rw-rw-   0        0        0     1172 2023-04-30 13:31:01.000000 starrail-0.0.2/src/starrail/user_interface/ui_frontend.py
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.525020 starrail-0.0.2/src/starrail.egg-info/
+-rw-rw-rw-   0        0        0     4357 2023-04-30 23:17:37.000000 starrail-0.0.2/src/starrail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-04-30 23:17:37.000000 starrail-0.0.2/src/starrail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 23:17:37.000000 starrail-0.0.2/src/starrail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-04-30 23:17:37.000000 starrail-0.0.2/src/starrail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 23:17:37.000000 starrail-0.0.2/src/starrail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 23:17:37.545940 starrail-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1288 2023-04-30 23:10:09.000000 starrail-0.0.2/tests/test_starrail.py
```

### Comparing `starrail-0.0.1/LICENSE` & `starrail-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-0.0.1/setup.cfg` & `starrail-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7461 7272 6169 6c0d 0a76 6572   = starrail..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6175  sion = 0.0.1..au
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
 00000030: 7468 6f72 203d 204b 6576 696e 204c 2e0d  thor = Kevin L..
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6b65 7669 6e6c 6975 4076 742e 6564 750d  kevinliu@vt.edu.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2048  .description = H
 00000070: 6f6e 6b61 693a 2053 7461 7220 5261 696c  onkai: Star Rail
 00000080: 2041 7574 6f6d 6174 696f 6e20 5061 636b   Automation Pack
 00000090: 6167 6520 2861 7574 6f2d 6772 696e 6420  age (auto-grind 
@@ -32,22 +32,23 @@
 000001f0: 6570 656e 6465 6e74 0d0a 0944 6576 656c  ependent...Devel
 00000200: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
 00000210: 2031 202d 2050 6c61 6e6e 696e 670d 0a0d   1 - Planning...
 00000220: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 00000230: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
 00000240: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
 00000250: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000260: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
-00000270: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000280: 6573 2e66 696e 645d 0d0a 7061 636b 6167  es.find]..packag
-00000290: 6573 203d 2073 7461 7272 6169 6c0d 0a77  es = starrail..w
-000002a0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
-000002b0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000002c0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-000002d0: 7269 7074 7320 3d20 0d0a 0973 7461 7274  ripts = ...start
-000002e0: 2d73 7461 722d 7261 696c 203d 2073 7461  -star-rail = sta
-000002f0: 7272 6169 6c2e 636d 642e 7374 6172 745f  rrail.cmd.start_
-00000300: 7374 6172 5f72 6169 6c3a 7361 6d70 6c65  star_rail:sample
-00000310: 5f66 756e 630d 0a0d 0a5b 6567 675f 696e  _func....[egg_in
-00000320: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000330: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000340: 0a0d 0a                                  ...
+00000260: 7569 7265 7320 3d20 3e3d 332e 360d 0a69  uires = >=3.6..i
+00000270: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000280: 6174 6120 3d20 5472 7565 0d0a 0d0a 5b6f  ata = True....[o
+00000290: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+000002a0: 6669 6e64 5d0d 0a70 6163 6b61 6765 7320  find]..packages 
+000002b0: 3d20 7374 6172 7261 696c 0d0a 7768 6572  = starrail..wher
+000002c0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
+000002d0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000002e0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+000002f0: 7473 203d 200d 0a09 7374 6172 7261 696c  ts = ...starrail
+00000300: 203d 2073 7461 7272 6169 6c2e 636d 642e   = starrail.cmd.
+00000310: 636c 5f65 6e64 706f 696e 7473 3a65 7865  cl_endpoints:exe
+00000320: 6375 7465 5f63 6f6d 6d61 6e64 0d0a 0d0a  cute_command....
+00000330: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000340: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000350: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `starrail-0.0.1/src/starrail/__init__.py` & `starrail-0.0.2/tests/test_starrail.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__author__ = "Kevin L."
-__version__ = "0.0.1"
-__support__ = "Honkai: Star Rail"
-
-from .honkai_star_rail import HonkaiStarRail
-
-def start_game():
-    pass
+import subprocess
+import psutil
+import pytest
+import time
+import os
+from starrail import HonkaiStarRail
+h = HonkaiStarRail()
```

### Comparing `starrail-0.0.1/src/starrail/cmd/__init__.py` & `starrail-0.0.2/src/starrail/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-0.0.1/src/starrail/cmd/start_star_rail.py` & `starrail-0.0.2/src/starrail/_data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,8 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import sys
-
-def sample_func():
-    print(sys.argv)
-    
-if __name__ == "__main__":
-    sample_func()
+# SOFTWARE.
```

### Comparing `starrail-0.0.1/src/starrail/constants.py` & `starrail-0.0.2/src/starrail/_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-0.0.1/src/starrail/honkai_star_rail.py` & `starrail-0.0.2/src/starrail/_utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,8 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import os
-import sys
-
-class HonkaiStarRail:
-    """
-    Honkai: Star Rail game instance blueprint.
-    """
-    
-    def __init__(self):
-        self.pid            = None
-        self.instance_name  = None
-        self.is_focused     = False
-    
-    def run(self):
-        pass
+# SOFTWARE.
```

### Comparing `starrail-0.0.1/tests/test_starrail.py` & `starrail-0.0.2/src/starrail/user_interface/ui_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import starrail
+import tkinter
```

