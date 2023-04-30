# Comparing `tmp/drf-social-oauth2-2.1.1.tar.gz` & `tmp/drf-social-oauth2-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-2.1.1.tar", last modified: Wed Apr 26 12:03:38 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.1.2.tar", last modified: Sun Apr 30 22:35:56 2023, max compression
```

## Comparing `drf-social-oauth2-2.1.1.tar` & `drf-social-oauth2-2.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.893978 drf-social-oauth2-2.1.1/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     6286 2023-04-24 13:22:06.000000 drf-social-oauth2-2.1.1/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.1/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.1/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-26 12:03:38.893609 drf-social-oauth2-2.1.1/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.1/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.884583 drf-social-oauth2-2.1.1/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-26 11:59:21.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2036 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2288 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     8784 2023-04-26 11:59:21.000000 drf-social-oauth2-2.1.1/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.888647 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-26 12:03:38.000000 drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.1/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-26 12:03:38.894089 drf-social-oauth2-2.1.1/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.1/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.889415 drf-social-oauth2-2.1.1/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.1/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-26 12:03:38.892630 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/drf_fixtures.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4268 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7034 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.068858 drf-social-oauth2-2.1.2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7573 2023-04-30 22:28:15.000000 drf-social-oauth2-2.1.2/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.2/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.2/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-30 22:35:56.068215 drf-social-oauth2-2.1.2/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.2/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.033633 drf-social-oauth2-2.1.2/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-30 22:25:23.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2962 2023-04-29 12:15:45.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-29 12:03:43.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4637 2023-04-29 12:18:12.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-04-28 21:11:59.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2135 2023-04-29 10:42:22.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2158 2023-04-29 12:31:18.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     8791 2023-04-29 10:43:00.000000 drf-social-oauth2-2.1.2/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.044849 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1733 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-30 22:35:55.000000 drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.2/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-30 22:35:56.069093 drf-social-oauth2-2.1.2/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.2/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.045653 drf-social-oauth2-2.1.2/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.2/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-30 22:35:56.065447 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/drf_fixtures.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     3241 2023-04-29 11:09:24.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4538 2023-04-29 12:04:19.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7226 2023-04-29 11:10:01.000000 drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_views.py
```

### Comparing `drf-social-oauth2-2.1.1/CHANGELOG.rst` & `drf-social-oauth2-2.1.2/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 Change log
 ==========
 
+2.1.1 - 2023-04-26
+------------------
+
+## What's Changed
+* 175 create readthedocs documentation by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/176
+* Running convert-token for the second time returns html headers with user environment variables by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/177
+
+**Full Changelog**: https://github.com/wagnerdelima/drf-social-oauth2/compare/2.1.0...2.1.1
+
+2.1.0 - 2023-04-24
+------------------
+
+## What's Changed
+* chore: 👷 fix codecov.yml by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/165
+* doc: 📝 add CONTRIBUTING.md file. by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/166
+* Create SECURITY.md by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/167
+* 104 use serializers for views by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/170
+* docs: 📝 add missing documentation about invalidate refresh tokens. by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/173
+* Update CHANGELOG.rst by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/174
+
+**Full Changelog**: https://github.com/wagnerdelima/drf-social-oauth2/compare/2.0.0...2.1.0
+
+
 2.0.0 - 2023-04-16
 ------------------
 
 ## What's Changed
 * Google id token setup by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/163
 * Create codecov.yml by @wagnerdelima in https://github.com/wagnerdelima/drf-social-oauth2/pull/164
```

### Comparing `drf-social-oauth2-2.1.1/LICENSE.txt` & `drf-social-oauth2-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/PKG-INFO` & `drf-social-oauth2-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.1.1
+Version: 2.1.2
 Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `drf-social-oauth2-2.1.1/README.rst` & `drf-social-oauth2-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 drf-social-oauth2 offers support to oauth2 authentication and authorization.
 It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
 By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
 and a ton more!
 """
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/authentication.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import List, Union, Callable
+from functools import wraps
+
 try:
     from django.urls import reverse
 except ImportError:  # Will be removed in Django 2.0
     from django.core.urlresolvers import reverse
 
 from rest_framework.authentication import BaseAuthentication, get_authorization_header
 from rest_framework import HTTP_HEADER_ENCODING
@@ -9,59 +12,68 @@
 
 from social_django.views import NAMESPACE
 from social_django.utils import load_backend, load_strategy
 from social_core.exceptions import MissingBackend
 from social_core.utils import requests
 
 
+def validator(function: Callable):
+    @wraps(function)
+    def wrapper_validation(*args, **kwargs):
+        request = args[1]
+        auth_header = get_authorization_header(request).decode(HTTP_HEADER_ENCODING)
+        auth: Union[List[str], List[str, str, str]] = auth_header.split()
+
+        if not auth or auth[0].lower() != 'bearer':
+            return None
+
+        if len(auth) == 1:
+            raise AuthenticationFailed('Invalid token header. No backend provided.')
+        elif len(auth) == 2:
+            raise AuthenticationFailed('Invalid token header. No credentials provided.')
+        elif len(auth) > 3:
+            raise AuthenticationFailed(
+                'Invalid token header. Token string should not contain spaces.'
+            )
+
+        return function(*args, backend=auth[1], token=auth[2], **kwargs)
+
+    return wrapper_validation
+
+
 class SocialAuthentication(BaseAuthentication):
     """
     Authentication backend using `python-social-auth`
 
     Clients should authenticate by passing the token key in the "Authorization"
     HTTP header with the backend used, prepended with the string "Bearer ".
 
     For example:
 
         Authorization: Bearer facebook 401f7ac837da42b97f613d789819ff93537bee6a
     """
 
     www_authenticate_realm = 'api'
 
-    def authenticate(self, request):
+    @validator
+    def authenticate(self, request, **kwargs):
         """
         Returns two-tuple of (user, token) if authentication succeeds,
         or None otherwise.
         """
-        auth_header = get_authorization_header(request).decode(HTTP_HEADER_ENCODING)
-        auth = auth_header.split()
-
-        if not auth or auth[0].lower() != 'bearer':
-            return None
-
-        if len(auth) == 1:
-            message = 'Invalid token header. No backend provided.'
-            raise AuthenticationFailed(message)
-        elif len(auth) == 2:
-            message = 'Invalid token header. No credentials provided.'
-            raise AuthenticationFailed(message)
-        elif len(auth) > 3:
-            message = 'Invalid token header. Token string should not contain spaces.'
-            raise AuthenticationFailed(message)
-
-        token = auth[2]
-        backend = auth[1]
-
+        token: str = kwargs['token']
+        backend: str = kwargs['backend']
         strategy = load_strategy(request=request)
 
         try:
             backend = load_backend(
-                strategy, backend, reverse(f'{NAMESPACE}:complete', args=(backend,)),
+                strategy,
+                backend,
+                reverse(f"{NAMESPACE}:complete", args=(backend,)),
             )
-
             user = backend.do_auth(access_token=token)
         except MissingBackend:
             message = 'Invalid token header. Invalid backend.'
             raise AuthenticationFailed(message)
         except requests.HTTPError as e:
             raise AuthenticationFailed(e.response.text)
 
@@ -69,8 +81,8 @@
             raise AuthenticationFailed('Bad credentials')
         return user, token
 
     def authenticate_header(self, request):
         """
         Bearer is the only finalized type currently
         """
-        return 'Bearer backend realm="%s"' % self.www_authenticate_realm
+        return f'Bearer backend realm="{self.www_authenticate_realm}"'
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/backends.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/backends.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 
 class DjangoOAuth2(BaseOAuth2):
     """Default OAuth2 authentication backend used by this package"""
 
     name = DRFSO2_PROPRIETARY_BACKEND_NAME
     AUTHORIZATION_URL = reverse(
-        DRFSO2_URL_NAMESPACE + ':authorize' if DRFSO2_URL_NAMESPACE else 'authorize'
+        f'{DRFSO2_URL_NAMESPACE}:authorize' if DRFSO2_URL_NAMESPACE else 'authorize'
     )
     ACCESS_TOKEN_URL = reverse(
-        DRFSO2_URL_NAMESPACE + ':token' if DRFSO2_URL_NAMESPACE else 'token'
+        f'{DRFSO2_URL_NAMESPACE}:token' if DRFSO2_URL_NAMESPACE else 'token'
     )
 
 
 class GoogleIdentityBackend(GooglePlusAuth):
     """
     Google has shifted to Open ID instead of access token. This authentication backend makes it possible to
     authenticate with google id_token.
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/oauth2_grants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging
+from logging import getLogger
 
 try:
     from django.urls import reverse
 except ImportError:  # Will be removed in Django 2.0
     from django.core.urlresolvers import reverse
 
 from oauthlib.oauth2.rfc6749 import errors
@@ -12,15 +12,15 @@
 from social_django.utils import load_backend, load_strategy
 from social_core.exceptions import MissingBackend, SocialAuthBaseException
 from social_core.utils import requests
 
 from drf_social_oauth2.settings import DRFSO2_URL_NAMESPACE
 
 
-log = logging.getLogger(__name__)
+log = getLogger(__name__)
 
 
 class SocialTokenGrant(RefreshTokenGrant):
 
     """`Refresh token grant`_
     .. _`Refresh token grant`: http://tools.ietf.org/html/rfc6749#section-6
     """
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/test_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'oauth2_provider',
+    'social_django',
+    'drf_social_oauth2',
+    'rest_framework',
+    'rest_framework.authtoken',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
@@ -68,13 +72,12 @@
         'USER': 'postgres',
         'PASSWORD': '0119',
     }
 }
 
 
 DRFSO2_PROPRIETARY_BACKEND_NAME = 'Django'
-
 DRFSO2_URL_NAMESPACE = 'drf'
 
 ROOT_URLCONF = 'drf_social_oauth2.urls'
 
 USE_TZ = True
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 try:
     from django.conf.urls import url, include
-
 except ImportError:
     from django.urls import re_path, include
 
-from django.urls import path
-
 from oauth2_provider.views import AuthorizationView
-from social_django.views import complete
+
 
 from drf_social_oauth2.views import (
     ConvertTokenView,
     TokenView,
     RevokeTokenView,
     InvalidateSessions,
     DisconnectBackendView,
     InvalidateRefreshTokens,
 )
 
-app_name = 'drfso2'
-
+app_name = 'drf'
 
-urlpatterns = [path('complete/<str:backend>/', complete, name='complete')]
+urlpatterns = []
 
 try:
     urlpatterns += [
         url(r'^authorize/?$', AuthorizationView.as_view(), name='authorize'),
         url(r'^token/?$', TokenView.as_view(), name='token'),
         url('', include('social_django.urls', namespace='social')),
         url(r'^convert-token/?$', ConvertTokenView.as_view(), name='convert_token'),
         url(r'^revoke-token/?$', RevokeTokenView.as_view(), name='revoke_token'),
         url(
             r'^invalidate-sessions/?$',
             InvalidateSessions.as_view(),
             name='invalidate_sessions',
         ),
         url(
-            r'invalidate-refresh-tokens/?$',
+            r'^ invalidate-refresh-tokens/?$',
             InvalidateRefreshTokens.as_view(),
             name='invalidate_refresh_tokens',
         ),
         url(
             r'^disconnect-backend/?$',
             DisconnectBackendView.as_view(),
             name='disconnect_backend',
@@ -55,15 +51,15 @@
         re_path(r'^revoke-token/?$', RevokeTokenView.as_view(), name='revoke_token'),
         re_path(
             r'^invalidate-sessions/?$',
             InvalidateSessions.as_view(),
             name='invalidate_sessions',
         ),
         re_path(
-            r'invalidate-refresh-tokens/?$',
+            r'^invalidate-refresh-tokens/?$',
             InvalidateRefreshTokens.as_view(),
             name='invalidate_refresh_tokens',
         ),
         re_path(
             r'^disconnect-backend/?$',
             DisconnectBackendView.as_view(),
             name='disconnect_backend',
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2/views.py` & `drf-social-oauth2-2.1.2/drf_social_oauth2/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     """
     Implements an endpoint to revoke access or refresh tokens
     """
 
     server_class = oauth2_settings.OAUTH2_SERVER_CLASS
     validator_class = oauth2_settings.OAUTH2_VALIDATOR_CLASS
     oauthlib_backend_class = oauth2_settings.OAUTH2_BACKEND_CLASS
-    permission_classes = (AllowAny,)
+    permission_classes = (IsAuthenticated,)
 
     def post(self, request: Request, *args, **kwargs):
         serializer = RevokeTokenSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         # Use the rest framework `.data` to fake the post body of the django request.
         request._request.POST = request._request.POST.copy()
         for key, value in serializer.validated_data.items():
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/PKG-INFO` & `drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.1.1
+Version: 2.1.2
 Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `drf-social-oauth2-2.1.1/drf_social_oauth2.egg-info/SOURCES.txt` & `drf-social-oauth2-2.1.2/drf_social_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/setup.py` & `drf-social-oauth2-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/drf_fixtures.py` & `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/drf_fixtures.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_authentication.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 
 def test_authenticate_no_auth_header_fail():
     authenticated = SocialAuthentication()
     assert not authenticated.authenticate(HttpRequest())
 
 
 def test_authenticate_no_backend_fail():
+    request = create_request('JWT')
+    authenticated = SocialAuthentication()
+
+    assert not authenticated.authenticate(request)
+
+
+def test_authenticate_no_bearer_token_type():
     request = create_request('Bearer')
     authenticated = SocialAuthentication()
 
     with raises(AuthenticationFailed):
         authenticated.authenticate(request)
 
 
@@ -57,17 +64,44 @@
     request.session = None
     request.META = {'HTTP_AUTHORIZATION': token}
 
     mocker.patch('drf_social_oauth2.authentication.load_backend')
     authenticated = SocialAuthentication()
     user, token = authenticated.authenticate(request)
     assert user
-    assert token
+    assert token == '401f7ac837da42b97f613d789819ff93537bee6a'
 
 
 def test_authenticate_missing_backend():
     token = 'Bearer unknown 401f7ac837da42b97f613d789819ff93537bee6a'
     request = create_request(token)
 
     authenticated = SocialAuthentication()
     with raises(AuthenticationFailed):
         authenticated.authenticate(request)
+
+
+def test_authenticate_user_not_found(mocker):
+    token = 'Bearer facebook 401f7ac837da42b97f613d789819ff93537bee6a'
+
+    request = mocker.patch('django.http.request.HttpRequest')
+    request.session = None
+    request.META = {'HTTP_AUTHORIZATION': token}
+
+    load_backend_mocker = mocker.patch('drf_social_oauth2.authentication.load_backend')
+    load_backend_mocker.return_value.do_auth.return_value = None
+
+    authenticated = SocialAuthentication()
+    with raises(AuthenticationFailed):
+        authenticated.authenticate(request)
+
+
+def test_authenticate_header(mocker):
+    token = 'Bearer facebook 401f7ac837da42b97f613d789819ff93537bee6a'
+
+    request = mocker.patch('django.http.request.HttpRequest')
+    request.session = None
+    request.META = {'HTTP_AUTHORIZATION': token}
+
+    authenticated = SocialAuthentication()
+    text = authenticated.authenticate_header(request)
+    assert text == 'Bearer backend realm="api"'
```

### Comparing `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from json import loads
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'drf_social_oauth2.test_settings')
 
 from django import setup
 
 setup()
 
 from django.contrib.auth.models import User
 
-from oauth2_provider.models import Application, AccessToken, RefreshToken
+from oauth2_provider.models import Application, AccessToken
 
 from drf_social_oauth2.oauth2_endpoints import SocialTokenServer
 from drf_social_oauth2 import generate_token
 from tests.drf_social_oauth2.drf_fixtures import application, user, save
 
 
 def assign_request_application(request):
@@ -35,16 +35,26 @@
     backend.return_value.do_auth.return_value = user
 
     social = SocialTokenServer(
         request_validator=request_validator,
         token_generator=generate_token,
     )
 
-    uri = '/auth/convert-token/?grant_type=convert_token&backend=facebook&client_id=code&client_secret=code&token=token'
-    _, data, status = social.create_token_response(uri=uri, http_method='POST', body='')
+    uri = '/auth/convert-token'
+    _, data, status = social.create_token_response(
+        uri=uri,
+        http_method='POST',
+        body={
+            'grant_type': 'convert_token',
+            'backend': 'facebook',
+            'client_id': 'code',
+            'client_secret': 'code',
+            'token': 'token',
+        },
+    )
     data = loads(data)
 
     assert status == 200
     assert 'access_token' in data
     assert data['expires_in'] == 3600
 
 
@@ -58,23 +68,31 @@
     backend.return_value.do_auth.return_value = user
 
     social = SocialTokenServer(
         request_validator=request_validator,
         token_generator=generate_token,
     )
 
-    uri = (
-        f'/auth/convert-token/?grant_type=convert_token&'
-        f'backend=facebook&client_id={application.client_id}&client_secret={application.client_secret}&token=token'
-    )
+    uri = '/auth/convert-token'
+    body = {
+        'grant_type': 'convert_token',
+        'backend': 'facebook',
+        'client_id': application.client_id,
+        'client_secret': application.client_secret,
+        'token': 'token',
+    }
     # create the first token.
-    _, data, status = social.create_token_response(uri=uri, http_method='POST', body='')
+    _, data, status = social.create_token_response(
+        uri=uri, http_method='POST', body=body
+    )
 
     # if an access token already exists, then the token is returned and no new token is created.
-    _, data, status = social.create_token_response(uri=uri, http_method='POST', body='')
+    _, data, status = social.create_token_response(
+        uri=uri, http_method='POST', body=body
+    )
     data = loads(data)
 
     assert status == 200
     assert 'access_token' in data
     # if there is a valid token, the expiry date will be smaller than the number when the token was created.
     assert data['expires_in'] < 3600
 
@@ -89,28 +107,36 @@
     backend.return_value.do_auth.return_value = user
 
     social = SocialTokenServer(
         request_validator=request_validator,
         token_generator=generate_token,
     )
 
-    uri = (
-        f'/auth/convert-token/?grant_type=convert_token&'
-        f'backend=facebook&client_id={application.client_id}&client_secret={application.client_secret}&token=token'
-    )
+    uri = '/auth/convert-token'
+    body = {
+        'grant_type': 'convert_token',
+        'backend': 'facebook',
+        'client_id': application.client_id,
+        'client_secret': application.client_secret,
+        'token': 'token',
+    }
     # create the first token.
-    _, data, status = social.create_token_response(uri=uri, http_method='POST', body='')
+    _, data, status = social.create_token_response(
+        uri=uri, http_method='POST', body=body
+    )
     data = loads(data)
 
     # if the access token is expired, a nw access token is generated.
     access_token = AccessToken.objects.get(token=data['access_token'])
     access_token.expires = datetime.now(tz=timezone.utc)
     access_token.save()
 
     # if an access token already exists, then the token is returned and no new token is created.
-    _, data, status = social.create_token_response(uri=uri, http_method='POST', body='')
+    _, data, status = social.create_token_response(
+        uri=uri, http_method='POST', body=body
+    )
     data = loads(data)
 
     assert status == 200
     assert 'access_token' in data
     # if there is a valid token, the expiry date will be smaller than the number when the token was created.
     assert data['expires_in'] == 3600
```

### Comparing `drf-social-oauth2-2.1.1/tests/drf_social_oauth2/test_views.py` & `drf-social-oauth2-2.1.2/tests/drf_social_oauth2/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,43 +76,47 @@
     assert 'access_token' in response.data
     assert 'refresh_token' in response.data
     assert 'expires_in' in response.data
     assert 'token_type' in response.data
     assert 'scope' in response.data
 
 
-def test_revoke_token_endpoint_with_no_post_params(client_api):
+def test_revoke_token_endpoint_with_no_post_params(client_api, user):
+    client_api.force_authenticate(user=user)
     response = client_api.post(
         reverse('revoke_token'),
         format='json',
     )
 
     assert response.status_code == 400
 
 
-def test_revoke_token_endpoint_with_missing_params(client_api):
+def test_revoke_token_endpoint_with_missing_params(client_api, user):
+    client_api.force_authenticate(user=user)
     response = client_api.post(
         reverse('revoke_token'),
         data={'client_id': 'id', 'client_secret': 'secret'},
         format='json',
     )
 
     assert response.status_code == 400
 
 
 def test_revoke_invalid_token_endpoint(client_api, user, application):
+    client_api.force_authenticate(user=user)
     response = client_api.post(
         reverse('revoke_token'),
         data={'client_id': 'code', 'client_secret': 'code', 'token': 'token'},
         format='json',
     )
     assert response.status_code == 401
 
 
 def test_revoke_token_endpoint(client_api, user, application):
+    client_api.force_authenticate(user=user)
     response = client_api.post(
         reverse('revoke_token'),
         data={
             'client_id': application.client_id,
             'client_secret': application.client_secret,
             'token': 'token',
         },
```

