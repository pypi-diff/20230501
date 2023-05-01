# Comparing `tmp/tencentcloud-sdk-python-mna-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-mna-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.883.tar", last modified: Thu Apr 27 00:40:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.885.tar", last modified: Mon May  1 00:45:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mna-3.0.883.tar` & `tencentcloud-sdk-python-mna-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43030 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/models.py
--rw-r--r--   0 root         (0) root         (0)    12081 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/mna_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:40:41.000000 tencentcloud-sdk-python-mna-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43030 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/models.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/mna_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:45:05.000000 tencentcloud-sdk-python-mna-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mna-3.0.883/README.rst` & `tencentcloud-sdk-python-mna-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/errorcodes.py` & `tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/models.py` & `tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.883/tencentcloud/mna/v20210119/mna_client.py` & `tencentcloud-sdk-python-mna-3.0.885/tencentcloud/mna/v20210119/mna_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mna-3.0.885/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.883'
+__version__ = '3.0.885'
```

### Comparing `tencentcloud-sdk-python-mna-3.0.883/tencentcloud_sdk_python_mna.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.885/tencentcloud_sdk_python_mna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.883
+Version: 3.0.885
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.885/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.883
+Version: 3.0.885
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.883/setup.py` & `tencentcloud-sdk-python-mna-3.0.885/setup.py`

 * *Files identical despite different names*

