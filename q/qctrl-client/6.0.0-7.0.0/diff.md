# Comparing `tmp/qctrl_client-6.0.0.tar.gz` & `tmp/qctrl_client-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-6.0.0.tar", max compression
+gzip compressed data, was "qctrl_client-7.0.0.tar", max compression
```

## Comparing `qctrl_client-6.0.0.tar` & `qctrl_client-7.0.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    36653 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/LICENSE
--rw-r--r--   0        0        0      214 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/README.md
--rw-r--r--   0        0        0     2614 2023-04-27 05:39:36.128281 qctrl_client-6.0.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-04-27 05:39:36.140282 qctrl_client-6.0.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-04-27 05:39:36.136282 qctrl_client-6.0.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     5885 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-04-27 05:39:15.191514 qctrl_client-6.0.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4308 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/client.py
--rw-r--r--   0        0        0      809 2023-04-27 05:39:36.144282 qctrl_client-6.0.0/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0      859 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/constants.py
--rw-r--r--   0        0        0     2999 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/functions.py
--rw-r--r--   0        0        0     1180 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/products.py
--rw-r--r--   0        0        0      638 2023-04-27 05:39:36.148282 qctrl_client-6.0.0/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0    12204 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     2677 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/settings.py
--rw-r--r--   0        0        0     1154 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-04-27 05:39:36.140282 qctrl_client-6.0.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-04-27 05:39:15.195514 qctrl_client-6.0.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 qctrl_client-6.0.0/setup.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-05-01 06:27:49.675506 qctrl_client-7.0.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-05-01 06:27:49.675506 qctrl_client-7.0.0/README.md
+-rw-r--r--   0        0        0     2614 2023-05-01 06:28:12.876545 qctrl_client-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-05-01 06:28:12.892546 qctrl_client-7.0.0/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-01 06:28:12.888546 qctrl_client-7.0.0/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     5885 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4308 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/client.py
+-rw-r--r--   0        0        0      809 2023-05-01 06:28:12.892546 qctrl_client-7.0.0/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0     2999 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0      995 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-05-01 06:28:12.896546 qctrl_client-7.0.0/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    11628 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1154 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-05-01 06:28:12.888546 qctrl_client-7.0.0/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-05-01 06:27:49.679506 qctrl_client-7.0.0/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 qctrl_client-7.0.0/setup.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.0.0/PKG-INFO
```

### Comparing `qctrl_client-6.0.0/LICENSE` & `qctrl_client-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/pyproject.toml` & `qctrl_client-7.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "6.0.0"
+version = "7.0.0"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_client-6.0.0/qctrlclient/__init__.py` & `qctrl_client-7.0.0/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/__init__.py` & `qctrl_client-7.0.0/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/base.py` & `qctrl_client-7.0.0/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/cli.py` & `qctrl_client-7.0.0/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/helpers.py` & `qctrl_client-7.0.0/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/keycloak.py` & `qctrl_client-7.0.0/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/oidc.py` & `qctrl_client-7.0.0/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/password.py` & `qctrl_client-7.0.0/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-7.0.0/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/auth/service_account.py` & `qctrl_client-7.0.0/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/client.py` & `qctrl_client-7.0.0/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/__init__.py` & `qctrl_client-7.0.0/qctrlclient/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/constants.py` & `qctrl_client-7.0.0/qctrlclient/core/products.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,31 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-INVALID_SUBSCRIPTION_ERROR_PATTERN = """
----------------------------------------------------------------------
-Your authentication succeeded, but your subscription is invalid for
-this product.
-
-Please access `{url}` for more details.
----------------------------------------------------------------------
-"""
+from dataclasses import dataclass
+from enum import Enum
+
+
+@dataclass
+class ProductInfo:
+    """Basic information about a product."""
+
+    name: str
+    registry: str
+
+
+class Product(Enum):
+    """Products which can be accessed using a core client."""
+
+    BOULDER_OPAL = ProductInfo(
+        name="boulder-opal",
+        registry="BOULDER_OPAL",
+    )
+
+    FIRE_OPAL = ProductInfo(
+        name="fire-opal",
+        registry="FIRE_OPAL",
+    )
```

### Comparing `qctrl_client-6.0.0/qctrlclient/core/functions.py` & `qctrl_client-7.0.0/qctrlclient/core/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/router/__init__.py` & `qctrl_client-7.0.0/qctrlclient/core/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/router/api.py` & `qctrl_client-7.0.0/qctrlclient/core/router/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     retry,
     retry_if_result,
     wait_chain,
     wait_fixed,
 )
 
 from qctrlclient import GraphQLClient
-from qctrlclient.core.constants import INVALID_SUBSCRIPTION_ERROR_PATTERN
 from qctrlclient.core.settings import CoreClientSettings
 from qctrlclient.core.utils import (
     get_installed_version,
     show_error_message,
 )
 from qctrlclient.exceptions import GraphQLClientError
 
@@ -156,16 +155,14 @@
 
     def _validate(self):
         """Performs validation checks on the settings."""
 
         if not self._settings.product:
             raise GraphQLClientError("`product` must be configured in settings")
 
-        self._check_user_role_permission()
-
         organizations = self._get_organizations()
 
         # if organization explicitly configured by user
         if self._settings.organization:
             self._check_organization_permission(organizations)
 
         # if no organizations found
@@ -182,27 +179,14 @@
             error_message += "Please configure an organization:\n\n"
 
             for organization in organizations:
                 error_message += f"- {organization.slug}\n"
 
             show_error_message(error_message)
 
-    def _check_user_role_permission(self):
-        """Checks the user has required access role according
-        to the configured settings.
-        """
-        try:
-            self._client.check_user_role(self._settings.product.value.role)
-        except GraphQLClientError:
-            show_error_message(
-                INVALID_SUBSCRIPTION_ERROR_PATTERN.format(
-                    url=self._settings.product.value.url
-                )
-            )
-
     def _check_organization_permission(self, organizations: List[Organization]):
         """Checks that the user is assigned to the configured
         organization. Requires that the `organization` setting
         is configured.
 
         Parameters
         ----------
```

### Comparing `qctrl_client-6.0.0/qctrlclient/core/router/base.py` & `qctrl_client-7.0.0/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/router/local.py` & `qctrl_client-7.0.0/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/settings.py` & `qctrl_client-7.0.0/qctrlclient/core/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/core/utils.py` & `qctrl_client-7.0.0/qctrlclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/defaults.py` & `qctrl_client-7.0.0/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/exceptions.py` & `qctrl_client-7.0.0/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/globals.py` & `qctrl_client-7.0.0/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/pytest_plugin.py` & `qctrl_client-7.0.0/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/transports/__init__.py` & `qctrl_client-7.0.0/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-7.0.0/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-6.0.0/setup.py` & `qctrl_client-7.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'gql>=3.4.0,<4.0.0',
  'qctrl-commons>=18.0.0,<19.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'qctrl-client',
-    'version': '6.0.0',
+    'version': '7.0.0',
     'description': 'Q-CTRL Client',
     'long_description': "# Q-CTRL Python Client\n\nThe Q-CTRL Python Client package provides a Python client to access Q-CTRL's GraphQL API. It is used as a base for Q-CTRL's client-side product packages and for inter-service communication.\n",
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `qctrl_client-6.0.0/PKG-INFO` & `qctrl_client-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 6.0.0
+Version: 7.0.0
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

