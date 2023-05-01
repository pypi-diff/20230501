# Comparing `tmp/ewhs-api-python-1.0.0b8.tar.gz` & `tmp/ewhs_api_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewhs-api-python-1.0.0b8.tar", max compression
+gzip compressed data, was "ewhs_api_python-1.0.3.tar", max compression
```

## Comparing `ewhs-api-python-1.0.0b8.tar` & `ewhs_api_python-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1079 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/LICENSE
--rw-r--r--   0        0        0        0 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/ewhs/__init__.py
--rw-r--r--   0        0        0     5906 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/ewhs/client.py
--rw-r--r--   0        0        0      254 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/ewhs/exceptions.py
--rw-r--r--   0        0        0      660 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/ewhs/mixins.py
--rw-r--r--   0        0        0      691 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/ewhs/resources.py
--rw-r--r--   0        0        0      504 2022-03-10 10:09:39.425117 ewhs-api-python-1.0.0b8/pyproject.toml
--rw-r--r--   0        0        0      640 2022-03-10 10:10:03.853217 ewhs-api-python-1.0.0b8/setup.py
--rw-r--r--   0        0        0      492 2022-03-10 10:10:03.853535 ewhs-api-python-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/ewhs/__init__.py
+-rw-r--r--   0        0        0     6081 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/ewhs/client.py
+-rw-r--r--   0        0        0      254 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/ewhs/exceptions.py
+-rw-r--r--   0        0        0      660 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/ewhs/mixins.py
+-rw-r--r--   0        0        0      961 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/ewhs/resources.py
+-rw-r--r--   0        0        0      497 2023-05-01 14:53:16.904338 ewhs_api_python-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 ewhs_api_python-1.0.3/PKG-INFO
```

### Comparing `ewhs-api-python-1.0.0b8/LICENSE` & `ewhs_api_python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ewhs-api-python-1.0.0b8/ewhs/client.py` & `ewhs_api_python-1.0.3/ewhs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import platform
 import re
 import time
 from collections import OrderedDict
 
 from requests import Request, Session
-from .resources import Order, Shipment, Stock
+from .resources import Order, Article, Webhook, Shipment, Stock
 from .exceptions import ServerError, BadRequest, AuthenticationError
 
 
 class EwhsClient:
     UNAME = " ".join(platform.uname())
-    CLIENT_VERSION = "0.1.0"
+    CLIENT_VERSION = "0.1.1"
 
-    API_URL = "https://api.ewarehousing.com"
+    API_URL = "https://eu.middleware.ewarehousing-solutions.com"
 
     def __init__(self, username, password, customer_code=None, wms_code=None, api_url=None):
         self.session = Session()
 
         self.username = username
         self.password = password
         self.customer_code = customer_code
@@ -30,14 +30,16 @@
         self.user_agent_components = OrderedDict()
         self.set_user_agent_component("Ewarehousing", self.CLIENT_VERSION)
         self.set_user_agent_component("Python", platform.python_version())
 
         # initialize resources
         self.shipment = Shipment(self)
         self.order = Order(self)
+        self.article = Article(self)
+        self.webhook = Webhook(self)
         self.stock = Stock(self)
 
     def set_user_agent_component(self, key, value, sanitize=True):
         """Add or replace new user-agent component strings.
 
         Given strings are formatted along the format agreed upon by eWarehousing and implementers:
         - key and values are separated by a forward slash ("/").
@@ -58,14 +60,17 @@
         """Return the formatted user agent string."""
         components = ["/".join(x) for x in self.user_agent_components.items()]
         return " ".join(components)
 
     def _send(self, method, resource, resource_id=None, data=None, params=None, expand=None, **kwargs):
         url = 'wms/{}'.format(resource)
 
+        if resource == 'webhooks':
+            url = resource
+
         if resource_id is not None:
             url = '{}/{}'.format(url, resource_id)
 
         self._authenticate()
 
         headers = dict(self._get_headers(), **{"Authorization": "Bearer {}".format(self.access_token)})
```

### Comparing `ewhs-api-python-1.0.0b8/ewhs/mixins.py` & `ewhs_api_python-1.0.3/ewhs/mixins.py`

 * *Files identical despite different names*

### Comparing `ewhs-api-python-1.0.0b8/ewhs/resources.py` & `ewhs_api_python-1.0.3/ewhs/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,17 @@
     resource = 'shipments'
 
 
 class Order(ListResourceMixin, DetailResourceMixin, CreateResourceMixin, UpdateResourceMixin, Resource):
     resource = 'orders'
 
 
+class Article(ListResourceMixin, DetailResourceMixin, CreateResourceMixin, UpdateResourceMixin, Resource):
+    resource = 'articles'
+
+
+class Webhook(ListResourceMixin, DetailResourceMixin, CreateResourceMixin, UpdateResourceMixin, Resource):
+    resource = 'webhooks'
+
+
 class Stock(ListResourceMixin, Resource):
     resource = 'stock'
```

