# Comparing `tmp/edx-enterprise-subsidy-client-0.3.0.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.0.tar", last modified: Fri Apr 28 18:46:58 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.1.tar", last modified: Mon May  1 19:26:27 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.0.tar` & `edx-enterprise-subsidy-client-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.754784 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.348353 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9747 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.0/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.1/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.1]
+*******
+* fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
+
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
 
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
```

### Comparing `edx-enterprise-subsidy-client-0.3.0/LICENSE` & `edx-enterprise-subsidy-client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.1]
+*******
+* fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
+
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
 
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
```

### Comparing `edx-enterprise-subsidy-client-0.3.0/README.rst` & `edx-enterprise-subsidy-client-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     To use this within your service, ensure the service's settings contain the following vars:
     OAUTH2_PROVIDER_URL=backend-service-oauth-provider-url
     BACKEND_SERVICE_EDX_OAUTH2_KEY=your-services-application-key
     BACKEND_SERVICE_EDX_OAUTH2_SECRET=your-services-application-secret
     ENTERPRISE_SUBSIDY_URL=enterprise-subsidy-service-base-url
     """
     V2_BASE_URL = EnterpriseSubsidyAPIClient.API_BASE_URL + 'v2/'
-    TRANSACTIONS_LIST_ENDPOINT = V2_BASE_URL + 'subsidies/{subsidy_uuid}/transactions/'
+    TRANSACTIONS_LIST_ENDPOINT = V2_BASE_URL + 'subsidies/{subsidy_uuid}/admin/transactions/'
 
     def list_subsidy_transactions(
         self, subsidy_uuid, include_aggregates=True,
         lms_user_id=None, content_key=None,
         subsidy_access_policy_uuid=None,
     ):
         """
@@ -240,15 +240,15 @@
             query_params['lms_user_id'] = lms_user_id
         if content_key:
             query_params['content_key'] = content_key
         if subsidy_access_policy_uuid:
             query_params['subsidy_access_policy_uuid'] = str(subsidy_access_policy_uuid)
 
         response = self.client.get(
-            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid),
+            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid=subsidy_uuid),
             params=query_params,
         )
         response.raise_for_status()
         return response.json()
 
     def create_subsidy_transaction(self, subsidy_uuid, lms_user_id, content_key, subsidy_access_policy_uuid, metadata):
         """
@@ -258,12 +258,12 @@
             'subsidy_uuid': str(subsidy_uuid),
             'lms_user_id': lms_user_id,
             'content_key': content_key,
             'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
             'metadata': metadata,
         }
         response = self.client.post(
-            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid),
+            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid=subsidy_uuid),
             json=request_payload,
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.1]
+*******
+* fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
+
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
 
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
```

### Comparing `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/setup.py` & `edx-enterprise-subsidy-client-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.0/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.1/tests/test_client.py`

 * *Files identical despite different names*

