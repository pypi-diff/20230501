# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.884.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.885.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.884.tar", last modified: Fri Apr 28 02:13:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.885.tar", last modified: Mon May  1 00:34:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.884.tar` & `tencentcloud-sdk-python-cynosdb-3.0.885.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    74122 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   273887 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:13:40.000000 tencentcloud-sdk-python-cynosdb-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)    74122 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   273887 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-01 00:34:14.000000 tencentcloud-sdk-python-cynosdb-3.0.885/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.885/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/cynosdb/v20190107/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.885/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.885/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.884
+Version: 3.0.885
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.884/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.885/setup.py`

 * *Files identical despite different names*

