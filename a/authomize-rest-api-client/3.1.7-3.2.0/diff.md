# Comparing `tmp/authomize-rest-api-client-3.1.7.tar.gz` & `tmp/authomize-rest-api-client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-3.1.7.tar", last modified: Sun Apr 30 12:19:10 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-3.2.0.tar", last modified: Mon May  1 08:34:45 2023, max compression
```

## Comparing `authomize-rest-api-client-3.1.7.tar` & `authomize-rest-api-client-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2160 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.090364 authomize-rest-api-client-3.1.7/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10105 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73614 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24331 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185721 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64787 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-30 12:18:51.000000 authomize-rest-api-client-3.1.7/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 12:19:10.000000 authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-04-30 12:19:10.094364 authomize-rest-api-client-3.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-04-30 12:18:54.000000 authomize-rest-api-client-3.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10105 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73614 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24531 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185721 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64932 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-01 08:34:21.000000 authomize-rest-api-client-3.2.0/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-01 08:34:45.000000 authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-01 08:34:45.723454 authomize-rest-api-client-3.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-05-01 08:34:44.000000 authomize-rest-api-client-3.2.0/setup.py
```

### Comparing `authomize-rest-api-client-3.1.7/LICENSE.txt` & `authomize-rest-api-client-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/README.md` & `authomize-rest-api-client-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-04-30T11:50:50+00:00
+#   timestamp: 2023-05-01T07:04:37+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -49,18 +49,23 @@
     Misconfiguration = 'Misconfiguration'
     Exposure = 'Exposure'
     Privileged_Access = 'Privileged Access'
     Suspicious_Behavior = 'Suspicious Behavior'
     Least_Privilege = 'Least Privilege'
     Custom = 'Custom'
     IAM_Infrastructure_Security = 'IAM Infrastructure Security'
-    Detection = 'Detection'
+    Account_Takeover_Protection = 'Account Takeover Protection'
     Stale_Access = 'Stale Access'
+    Initial_Access = 'Initial Access'
     Over_privileges = 'Over-privileges'
     Privilege_Escalation = 'Privilege Escalation'
+    Lateral_Movement = 'Lateral Movement'
+    Detection = 'Detection'
+    Persistence = 'Persistence'
+    Evasion = 'Evasion'
     Account_Takeover = 'Account Takeover'
     Account_Impersonation__PE__LM_ = 'Account Impersonation (PE, LM)'
 
 
 class AttackTacticType(Enum):
     Collection = 'Collection'
     Credential_Access = 'Credential Access'
```

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-3.2.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999892769607843%*

 * *Differences: {"'components'": "{'schemas': {'AlertCategoryType': {'enum': {insert: [(8, 'Account Takeover "*

 * *                 "Protection'), (10, 'Initial Access'), (13, 'Lateral Movement'), (14, "*

 * *                 "'Detection'), (15, 'Persistence'), (16, 'Evasion')], delete: [8]}}}}"}*

```diff
@@ -88,18 +88,23 @@
                     "Misconfiguration",
                     "Exposure",
                     "Privileged Access",
                     "Suspicious Behavior",
                     "Least Privilege",
                     "Custom",
                     "IAM Infrastructure Security",
-                    "Detection",
+                    "Account Takeover Protection",
                     "Stale Access",
+                    "Initial Access",
                     "Over-privileges",
                     "Privilege Escalation",
+                    "Lateral Movement",
+                    "Detection",
+                    "Persistence",
+                    "Evasion",
                     "Account Takeover",
                     "Account Impersonation (PE, LM)"
                 ],
                 "title": "AlertCategoryType"
             },
             "AttackTacticType": {
                 "description": "An enumeration.",
```

### Comparing `authomize-rest-api-client-3.1.7/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-3.2.0/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-3.1.7/setup.py` & `authomize-rest-api-client-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='3.1.7',
+        version='3.2.0',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

