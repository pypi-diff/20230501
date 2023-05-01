# Comparing `tmp/drf-exceptions-hog-0.3.0.tar.gz` & `tmp/drf-exceptions-hog-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-exceptions-hog-0.3.0.tar", last modified: Mon Nov 21 17:52:31 2022, max compression
+gzip compressed data, was "drf-exceptions-hog-0.3.1.tar", last modified: Mon May  1 14:40:12 2023, max compression
```

## Comparing `drf-exceptions-hog-0.3.0.tar` & `drf-exceptions-hog-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:52:31.233649 drf-exceptions-hog-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-11-21 17:52:31.233649 drf-exceptions-hog-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:52:31.233649 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-11-21 17:52:31.000000 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-21 17:52:31.000000 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 17:52:31.000000 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-21 17:52:31.000000 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-21 17:52:31.000000 drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:52:31.233649 drf-exceptions-hog-0.3.0/exceptions_hog/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10580 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/exceptions_hog/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-21 17:52:31.233649 drf-exceptions-hog-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-11-21 17:52:19.000000 drf-exceptions-hog-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8467 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-01 14:40:12.000000 drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/exceptions_hog/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10784 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/exceptions_hog/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:40:12.134745 drf-exceptions-hog-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7636 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18090 2023-05-01 14:40:01.000000 drf-exceptions-hog-0.3.1/tests/test_handler.py
```

### Comparing `drf-exceptions-hog-0.3.0/LICENSE` & `drf-exceptions-hog-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.0/PKG-INFO` & `drf-exceptions-hog-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-exceptions-hog
-Version: 0.3.0
+Version: 0.3.1
 Summary: Standardized and easy-to-parse API error responses for DRF.
 Home-page: https://github.com/posthog/drf-exceptions-hog
 Author: PostHog
 Author-email: hey@posthog.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="drf-exceptions-hog.png" alt="Logo" height="125" />
 
 # DRF Exceptions Hog
+[![PyPI version](https://badge.fury.io/py/drf-exceptions-hog.svg)](https://badge.fury.io/py/drf-exceptions-hog) [![License: MIT](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/psf/black/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Standardized and **easy-to-parse** API error responses for [Django REST Framework][drf].
 
 After reusing similar code in multiple projects, we realized this might actually help others. The problem we're trying to solve is that DRF exceptions tend to vary in format and therefore require complex parsing logic on the frontend, which generally needs to be implemented in more than one language or framework. This simple package standardizes the exception responses to simplify the parsing logic on the frontend and enable developers to provide clear errors to their users (instead of the cryptic or even shady-looking parsing errors). This package is inspired on the way [Stripe API](https://stripe.com/docs/api/errors) handles errors. See an example below.
 
 You will get predictable responses like these:
```

### Comparing `drf-exceptions-hog-0.3.0/README.md` & `drf-exceptions-hog-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <img src="drf-exceptions-hog.png" alt="Logo" height="125" />
 
 # DRF Exceptions Hog
+[![PyPI version](https://badge.fury.io/py/drf-exceptions-hog.svg)](https://badge.fury.io/py/drf-exceptions-hog) [![License: MIT](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/psf/black/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Standardized and **easy-to-parse** API error responses for [Django REST Framework][drf].
 
 After reusing similar code in multiple projects, we realized this might actually help others. The problem we're trying to solve is that DRF exceptions tend to vary in format and therefore require complex parsing logic on the frontend, which generally needs to be implemented in more than one language or framework. This simple package standardizes the exception responses to simplify the parsing logic on the frontend and enable developers to provide clear errors to their users (instead of the cryptic or even shady-looking parsing errors). This package is inspired on the way [Stripe API](https://stripe.com/docs/api/errors) handles errors. See an example below.
 
 You will get predictable responses like these:
```

### Comparing `drf-exceptions-hog-0.3.0/drf_exceptions_hog.egg-info/PKG-INFO` & `drf-exceptions-hog-0.3.1/drf_exceptions_hog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-exceptions-hog
-Version: 0.3.0
+Version: 0.3.1
 Summary: Standardized and easy-to-parse API error responses for DRF.
 Home-page: https://github.com/posthog/drf-exceptions-hog
 Author: PostHog
 Author-email: hey@posthog.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="drf-exceptions-hog.png" alt="Logo" height="125" />
 
 # DRF Exceptions Hog
+[![PyPI version](https://badge.fury.io/py/drf-exceptions-hog.svg)](https://badge.fury.io/py/drf-exceptions-hog) [![License: MIT](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/psf/black/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Standardized and **easy-to-parse** API error responses for [Django REST Framework][drf].
 
 After reusing similar code in multiple projects, we realized this might actually help others. The problem we're trying to solve is that DRF exceptions tend to vary in format and therefore require complex parsing logic on the frontend, which generally needs to be implemented in more than one language or framework. This simple package standardizes the exception responses to simplify the parsing logic on the frontend and enable developers to provide clear errors to their users (instead of the cryptic or even shady-looking parsing errors). This package is inspired on the way [Stripe API](https://stripe.com/docs/api/errors) handles errors. See an example below.
 
 You will get predictable responses like these:
```

### Comparing `drf-exceptions-hog-0.3.0/exceptions_hog/exceptions.py` & `drf-exceptions-hog-0.3.1/exceptions_hog/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.0/exceptions_hog/handler.py` & `drf-exceptions-hog-0.3.1/exceptions_hog/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from django.core.signals import got_request_exception
 from django.db.models import ProtectedError
 from django.http import Http404
 from django.utils.translation import gettext as _
@@ -107,15 +107,15 @@
             )
         else:
             items.append({"parsed_keys": keys, "exception_code": exception_code})
     return items
 
 
 def _get_main_exception_and_code(
-    exception_codes: Union[Dict, str, List]
+    exception_codes: Union[Dict, str, List, None]
 ) -> Tuple[str, Optional[str]]:
     def override_or_return(code: str) -> str:
         """
         Returns overridden code if needs to change or provided code.
         """
         if code == "invalid":
             # Special handling for validation errors. Use `invalid_input` instead
@@ -194,15 +194,17 @@
 
         if final_key == drf_api_settings.NON_FIELD_ERRORS_KEY:
             return None
 
         return final_key if final_key else None
 
     if isinstance(exception_key, list):
-        return override_or_return(api_settings.NESTED_KEY_SEPARATOR.join(exception_key))
+        return override_or_return(
+            api_settings.NESTED_KEY_SEPARATOR.join(map(str, exception_key))
+        )
 
     return override_or_return(exception_key)
 
 
 def _get_http_status(exc) -> int:
     return (
         exc.status_code
@@ -252,27 +254,30 @@
         # See https://github.com/django/django/blob/3.2.9/django/test/client.py#L712
         got_request_exception.send(
             sender=None,
             request=request,
         )
         return None
 
+    base_exception_list: Union[
+        List[List[Any]], List[None], List[Dict[str, Union[str, List[str]]]]
+    ]
     if isinstance(exc, exceptions.ValidationError):
         codes = exc.get_codes()
-        if type(codes) is list:
-            exception_list = [codes]
+        if isinstance(codes, list):
+            base_exception_list = [codes]
         else:
-            exception_list = _normalize_exception_codes(codes)
+            base_exception_list = _normalize_exception_codes(cast(Dict, codes))
     elif hasattr(exc, "get_codes"):
-        exception_list = [exc.get_codes()]  # type: ignore
+        base_exception_list = [exc.get_codes()]  # type: ignore
     else:
-        exception_list = [None]
+        base_exception_list = [None]
 
     exception_list = [
-        _get_main_exception_and_code(exception) for exception in exception_list
+        _get_main_exception_and_code(exception) for exception in base_exception_list
     ]
 
     event_id = api_settings.EXCEPTION_REPORTING(exc, context)
 
     set_rollback()
 
     if api_settings.SUPPORT_MULTIPLE_EXCEPTIONS and len(exception_list) > 1:
```

### Comparing `drf-exceptions-hog-0.3.0/exceptions_hog/settings.py` & `drf-exceptions-hog-0.3.1/exceptions_hog/settings.py`

 * *Files identical despite different names*

### Comparing `drf-exceptions-hog-0.3.0/setup.py` & `drf-exceptions-hog-0.3.1/setup.py`

 * *Files identical despite different names*

