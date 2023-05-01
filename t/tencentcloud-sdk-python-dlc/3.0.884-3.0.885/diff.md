# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.884.tar", last modified: Fri Apr 28 02:14:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.885.tar", last modified: Mon May  1 00:35:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.884.tar` & `tencentcloud-sdk-python-dlc-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)    78374 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   323205 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:14:38.000000 tencentcloud-sdk-python-dlc-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)    78374 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   323205 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:35:11.000000 tencentcloud-sdk-python-dlc-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/README.rst` & `tencentcloud-sdk-python-dlc-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/dlc/v20210125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.885/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.884'
+__version__ = '3.0.885'
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.885/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/setup.py` & `tencentcloud-sdk-python-dlc-3.0.885/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.884/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.885/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

