# Comparing `tmp/dcicutils-7.3.2.1b2.tar.gz` & `tmp/dcicutils-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.3.2.1b2.tar", max compression
+gzip compressed data, was "dcicutils-7.4.0.tar", max compression
```

## Comparing `dcicutils-7.3.2.1b2.tar` & `dcicutils-7.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1098 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/README.rst
--rw-r--r--   0        0        0        0 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3587 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-28 02:08:00.222899 dcicutils-7.3.2.1b2/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     8131 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    31947 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154304 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-28 02:08:00.226899 dcicutils-7.3.2.1b2/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3991 2023-04-28 02:08:00.230899 dcicutils-7.3.2.1b2/pyproject.toml
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 dcicutils-7.3.2.1b2/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.3.2.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-01 13:05:57.392337 dcicutils-7.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-01 13:05:57.392337 dcicutils-7.4.0/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3587 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46729 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-01 13:05:57.392337 dcicutils-7.4.0/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    31947 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154304 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-01 13:05:57.396337 dcicutils-7.4.0/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3987 2023-05-01 13:05:57.396337 dcicutils-7.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 dcicutils-7.4.0/setup.py
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.0/PKG-INFO
```

### Comparing `dcicutils-7.3.2.1b2/LICENSE.txt` & `dcicutils-7.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/README.rst` & `dcicutils-7.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/base.py` & `dcicutils-7.4.0/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.0/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.0/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/codebuild_utils.py` & `dcicutils-7.4.0/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/command_utils.py` & `dcicutils-7.4.0/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/common.py` & `dcicutils-7.4.0/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/creds_utils.py` & `dcicutils-7.4.0/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/data_utils.py` & `dcicutils-7.4.0/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/deployment_utils.py` & `dcicutils-7.4.0/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/diff_utils.py` & `dcicutils-7.4.0/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/docker_utils.py` & `dcicutils-7.4.0/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ecr_scripts.py` & `dcicutils-7.4.0/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ecr_utils.py` & `dcicutils-7.4.0/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ecs_utils.py` & `dcicutils-7.4.0/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/env_base.py` & `dcicutils-7.4.0/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/env_manager.py` & `dcicutils-7.4.0/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/env_scripts.py` & `dcicutils-7.4.0/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/env_utils.py` & `dcicutils-7.4.0/dcicutils/env_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,15 @@
     if entry:
         return entry
 
 
 def get_portal_url(envname: EnvName) -> UrlString:
     """
     Returns the Portal URL for the given environment name.
-    Effectively same ase get_env_real_url (below) but does not actually access
+    Effectively same as get_env_real_url (below) but does not actually access
     the URL (to get the health page is that function does); i.e. so we can get
     the URL without exception even if there is a problem with the Portal.
     """
     return get_env_real_url(full_env_name(envname))
 
 
 @if_orchestrated
```

### Comparing `dcicutils-7.3.2.1b2/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.0/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/es_utils.py` & `dcicutils-7.4.0/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/exceptions.py` & `dcicutils-7.4.0/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ff_mocks.py` & `dcicutils-7.4.0/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ff_utils.py` & `dcicutils-7.4.0/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.0/dcicutils/function_cache_decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from collections import namedtuple, OrderedDict
 from datetime import datetime, timedelta
+import timeit
 from typing import Optional, Union
 import json
 import sys
 
 
+# Global list of all @function_decorator instances; for debugging/testing/troubleshooting.
 _function_cache_list = []
 
 
 def function_cache(*decorator_args, **decorator_kwargs):
     """
     Exactly analogous to the functools.lru_cache decorator, but also allows specifying
-    hat if the return value of the function is None then no caching is to be done; use
-    the do_not_cache_none (nocache_none) set to True as a decorator argument to do this.
+    that if the return value of the function is None then no caching is to be done;
+    use the nocache_none decorator kwarg set to True to do this. And more generally, use
+    the nocache decorator kwart set to anything to not cache any value which equals that.
 
     Also like @lru_cache, this supports the maxsize decorator argument, as well
     as the cache_info and cache_clear functions on the decorated function.
     The maxsize can be specified either as the first argument to the
     decorator or as a maxsize kwarg to the decorator.
 
-    In addition we support a time_to_live (ttl) decorator kwarg which can be specified,
+    In addition we support a ttl (time to live) decorator kwarg which can be specified,
     as a timedelta type. If the cached value for the function is more than the specified
     ttl then it is considered stale and the function will be called to get a fresh value.
-    And, there is a separate time_to_live_none (ttl_none) supported which will do the
-    same as ttl but will apply only if the cached value is None.
+    And, there is a separate ttl_none supported which will do the same as ttl but will
+    apply only if the cached value is None.
 
-    There is also a serialize_key (serialize) decorator kwarg which if specified as True,
-    will serialize the arguments (args and kwargs) to the function call and use that value,
+    There is also a serialize_key decorator kwarg which if specified as True, will
+    serialize the arguments (args and kwargs) to the function call and use that value,
     converted to a string, as the key for caching the function result; this will allow
     caching for functions which take non-hashable structured types (i.e. dict or list)
     as arguments, which normally would not be possible, i.e. e.g. in which case this
     error would be generated: TypeError: unhashable type: 'dict'
 
     And a custom key decorator kwarg may be specified as a lambda/callable which
-    computes the key by which the function results should be cached; it is passed
-    the exact same arguments as the function itself.
+    computes the key by which the function results should be cached; this lambda
+    is passed the exact same arguments as the function itself.
+
+    Lastly, if the nokey kwarg is specified for the decorator then no key at all
+    will used (or more precisely, and single/constant key will be used) by which
+    to cache the function result.
 
     Looked/tried and could not find an way to do this using @lru_cache;
     and also had issues trying to wrap @lru_cache with this functionality.
     First created (April 2023) to try simplify some of the caching in foursight-core APIs.
     """
     cache = OrderedDict()
     nhits = nmisses = 0
@@ -47,137 +54,175 @@
         decorator_invoked_without_args = True
         decorator_target_function = decorator_args[0]
         decorator_args = decorator_args[1:]
     else:
         decorator_invoked_without_args = False
         decorator_target_function = None
 
+    null_object = object()
     maxsize = sys.maxsize
     ttl = None
     ttl_none = None
-    nocache_none = False
+    nocache = null_object
     key = None
     serialize_key = False
+    nokey = False
 
     if decorator_args:
         maxsize_arg = decorator_args[0]
         if isinstance(maxsize_arg, int) and maxsize_arg > 0:
             maxsize = maxsize_arg
     if decorator_kwargs:
         maxsize_kwarg = decorator_kwargs.get("maxsize")
         if isinstance(maxsize_kwarg, int) and maxsize_kwarg > 0:
             maxsize = maxsize_kwarg
-        ttl_kwarg = decorator_kwargs.get("ttl", decorator_kwargs.get("time_to_live"))
+        ttl_kwarg = decorator_kwargs.get("ttl")
         if isinstance(ttl_kwarg, timedelta):
             ttl = ttl_kwarg
-        ttl_none_kwarg = decorator_kwargs.get("ttl_none", decorator_kwargs.get("time_to_live_none"))
+        ttl_none_kwarg = decorator_kwargs.get("ttl_none")
         if isinstance(ttl_none_kwarg, timedelta):
             ttl_none = ttl_none_kwarg
-        nocache_none_kwarg = decorator_kwargs.get("nocache_none", decorator_kwargs.get("do_not_cache_none"))
-        if isinstance(nocache_none_kwarg, bool):
-            nocache_none = nocache_none_kwarg
-        key_kwarg = decorator_kwargs.get("key", decorator_kwargs.get("key_function"))
+        nocache_kwarg = decorator_kwargs.get("nocache", null_object)
+        if nocache_kwarg is not null_object:
+            nocache = nocache_kwarg
+        nocache_none_kwarg = decorator_kwargs.get("nocache_none")
+        if isinstance(nocache_none_kwarg, bool) and nocache_none_kwarg:
+            nocache = None
+        key_kwarg = decorator_kwargs.get("key")
         if callable(key_kwarg):
             key = key_kwarg
         serialize_key_kwarg = decorator_kwargs.get("serialize_key")
         if isinstance(serialize_key_kwarg, bool):
             serialize_key = serialize_key_kwarg
+        nokey_kwarg = decorator_kwargs.get("nokey")
+        if isinstance(nokey_kwarg, bool):
+            nokey = nokey_kwarg
 
-    def function_cache_decorator_registration(wrapped_function):
+    def function_cache_decorator(wrapped_function):
 
         def function_wrapper(*args, **kwargs):
 
-            cache_key = key(*args, **kwargs) if key else args + tuple(sorted(kwargs.items()))
-            if serialize_key:
-                cache_key = json.dumps(cache_key, default=str, separators=(",", ":"))
+            if nokey:
+                cache_key = 0
+            else:
+                cache_key = key(*args, **kwargs) if key else args + tuple(sorted(kwargs.items()))
+                if serialize_key:
+                    cache_key = json.dumps(cache_key, default=str, separators=(",", ":"))
             cached = cache.get(cache_key, None)
-            now = None  # do not call datetime.now more than once
+
+            now = None  # Do not call datetime.now more than once
 
             if cached is not None:
 
                 if ttl or ttl_none:
                     now = datetime.now()
 
                 def is_stale():
-                    # Uses outer variables: ttl, ttl_none, cached, now
+                    """
+                    Returns True iff the cached value for the @function_cache decorated
+                    function is stale, according to any ttl related decorator kwargs.
+                    Uses outer variables: ttl, ttl_none, cached, now
+                    """
                     if ttl and now > cached["timestamp"] + ttl:
                         return True
                     if ttl_none and cached["value"] is None and now > cached["timestamp"] + ttl_none:
                         return True
                     return False
 
                 if not is_stale():
                     nonlocal nhits
                     nhits += 1
                     cache.move_to_end(cache_key)
                     return cached["value"]
 
             nonlocal nmisses
             nmisses += 1
+            start_time = timeit.default_timer()
             value = wrapped_function(*args, **kwargs)
+            duration = timeit.default_timer() - start_time
 
-            if value is not None or not nocache_none:
+            if nocache is null_object or nocache != value:
                 if len(cache) >= maxsize:
                     cache.popitem(last=False)
                 if not now:
                     now = datetime.now()
-                cache[cache_key] = {"value": value, "timestamp": now}
+                cache[cache_key] = {"value": value, "timestamp": now, "duration": duration}
 
             return value
 
         def cache_info(as_dict: bool = False) -> Union[namedtuple, dict]:
-            cache_info = namedtuple("cache_info", ["hits", "misses", "size", "maxsize", "ttl", "ttl_none",
-                                                   "nocache_none", "key", "serialize_key", "updated"])
-            updated = next(iter(cache.items()))[1]["timestamp"] if len(cache) > 0 else None
-            updated = updated.strftime("%Y-%m-%d %H:%M:%S") if updated else None
+            """
+            Returns a named tuple with sundry info about the function cache
+            for the @function_cache decorated function.
+            """
+            cache_info = namedtuple("cache_info",
+                                    ["hits", "misses", "size", "maxsize", "ttl", "ttl_none",
+                                     "nocache_none", "nocache_other",
+                                     "key", "serialize_key", "updated", "duration", "name"])
+            if len(cache) > 0:
+                cached = next(iter(cache.items()))[1]
+                # This is the timstamp of the most recent call to the wrapped function.
+                updated = cached["timestamp"].strftime("%Y-%m-%d %H:%M:%S")
+                # This is the duration in milliseconds of the most recent call to the wrapped function.
+                duration = cached["duration"] * 1000
+            else:
+                updated = None
+                duration = None
             info = cache_info(nhits, nmisses, len(cache), maxsize, ttl, ttl_none,
-                              nocache_none, key, serialize_key, updated)
+                              nocache is None, nocache is not None and nocache is not null_object,
+                              key, serialize_key, updated, duration, _get_function_name(wrapped_function))
             return dict(info._asdict()) if as_dict else info
 
         def cache_clear() -> None:
+            """
+            Clears the cache for the @function_cache decorated function.
+            """
             nonlocal nhits, nmisses
             nhits = nmisses = 0
             cache.clear()
 
         function_wrapper.cache_info = cache_info
         function_wrapper.cache_clear = cache_clear
         _function_cache_list.append({"function_wrapper": function_wrapper, "wrapped_function": wrapped_function})
 
         return function_wrapper
 
     if decorator_invoked_without_args:
-        return function_cache_decorator_registration(decorator_target_function)
-    return function_cache_decorator_registration
+        return function_cache_decorator(decorator_target_function)
+    return function_cache_decorator
 
 
 def _get_function_name(wrapped_function: callable) -> str:
+    """
+    Returns a unique name for the given function/callable.
+    """
     return f"{wrapped_function.__module__}.{wrapped_function.__qualname__}"
 
 
 def function_cache_info() -> dict:
     """
     Returns a list of dictionaries representing all of the function_cache instances
     which exist; each dictonary containing detailed info about the function cache.
     Only for debugging/testing/troubleshooting.
     """
     info = []
     for function_cache in _function_cache_list:
         function_wrapper = function_cache["function_wrapper"]
         wrapped_function = function_cache["wrapped_function"]
         cache_info = function_wrapper.cache_info(as_dict=True)
-        cache_info["function"] = _get_function_name(wrapped_function)
+        cache_info["name"] = _get_function_name(wrapped_function)
         info.append(cache_info)
-    return info
+    return sorted(info, key=lambda item: item["name"])
 
 
 def function_cache_clear(function_name: Optional[str] = None) -> int:
     """
-    Clears the cache for the given named function (as per function_cache_info),
-    of for all existing caches of no given name function.
-    Returns the number of caches cleared.
+    Clears the cache for the given named function (as per function_cache_info), OR for
+    ALL existing caches if no named function given. Returns the number of caches cleared.
+    Only for debugging/testing/troubleshooting.
     """
     ncleared = 0
     for function_cache in _function_cache_list:
         wrapped_function = function_cache["wrapped_function"]
         if not function_name or _get_function_name(wrapped_function) == function_name:
             function_wrapper = function_cache["function_wrapper"]
             function_wrapper.cache_clear()
```

### Comparing `dcicutils-7.3.2.1b2/dcicutils/glacier_utils.py` & `dcicutils-7.4.0/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/jh_utils.py` & `dcicutils-7.4.0/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.0/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/kibana/readme.md` & `dcicutils-7.4.0/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/lang_utils.py` & `dcicutils-7.4.0/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/log_utils.py` & `dcicutils-7.4.0/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/misc_utils.py` & `dcicutils-7.4.0/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.0/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/opensearch_utils.py` & `dcicutils-7.4.0/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/qa_checkers.py` & `dcicutils-7.4.0/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/qa_utils.py` & `dcicutils-7.4.0/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/redis_tools.py` & `dcicutils-7.4.0/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/redis_utils.py` & `dcicutils-7.4.0/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/s3_utils.py` & `dcicutils-7.4.0/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.0/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/secrets_utils.py` & `dcicutils-7.4.0/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/snapshot_utils.py` & `dcicutils-7.4.0/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.0/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/task_utils.py` & `dcicutils-7.4.0/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/dcicutils/trace_utils.py` & `dcicutils-7.4.0/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.3.2.1b2/pyproject.toml` & `dcicutils-7.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.3.2.1b2"
+version = "7.4.0"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -61,15 +61,15 @@
 PyJWT = "^2.6.0"
 tqdm = "^4.65.0"
 
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = "1.21.22"
 boto3-stubs = "1.18.23"
-coverage = ">=5.3.1"
+coverage = ">=7.2.3"
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 pytest = ">=4.5.0"
 pytest-cov = ">=2.7.1"
```

### Comparing `dcicutils-7.3.2.1b2/setup.py` & `dcicutils-7.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.3.2.1b2',
+    'version': '7.4.0',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.3.2.1b2/PKG-INFO` & `dcicutils-7.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.3.2.1b2
+Version: 7.4.0
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

