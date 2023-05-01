# Comparing `tmp/usepy-0.1.46.tar.gz` & `tmp/usepy-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy-0.1.46.tar", max compression
+gzip compressed data, was "usepy-0.1.47.tar", max compression
```

## Comparing `usepy-0.1.46.tar` & `usepy-0.1.47.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      749 2023-04-26 05:50:47.132387 usepy-0.1.46/README.md
--rw-r--r--   0        0        0      752 2023-04-26 05:50:47.144387 usepy-0.1.46/pyproject.toml
--rw-r--r--   0        0        0     1759 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/__init__.py
--rw-r--r--   0        0        0     6407 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_datetime.py
--rw-r--r--   0        0        0     3119 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_path.py
--rw-r--r--   0        0        0     1217 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/_thread.py
--rw-r--r--   0        0        0        0 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/__init__.py
--rw-r--r--   0        0        0     1302 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/pydantic_.py
--rw-r--r--   0        0        0     2039 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/contrib/tenacity_.py
--rw-r--r--   0        0        0      156 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/__init__.py
--rw-r--r--   0        0        0     6773 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/_string.py
--rw-r--r--   0        0        0     5000 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/addict.py
--rw-r--r--   0        0        0     8331 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/dict.py
--rw-r--r--   0        0        0     7116 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/data/list.py
--rw-r--r--   0        0        0      681 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/__init__.py
--rw-r--r--   0        0        0      457 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/cache.py
--rw-r--r--   0        0        0      415 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/catch_error.py
--rw-r--r--   0        0        0      382 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/except_debug.py
--rw-r--r--   0        0        0      416 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/listify.py
--rw-r--r--   0        0        0     1879 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/retry.py
--rw-r--r--   0        0        0      377 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/run_in_thread.py
--rw-r--r--   0        0        0      510 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/singleton.py
--rw-r--r--   0        0        0      410 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/decorator/timeit.py
--rw-r--r--   0        0        0      138 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/__init__.py
--rw-r--r--   0        0        0     3429 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/curl.py
--rw-r--r--   0        0        0     1379 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/parser/url.py
--rw-r--r--   0        0        0      599 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/__init__.py
--rw-r--r--   0        0        0      677 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/_is.py
--rw-r--r--   0        0        0     1550 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/_to.py
--rw-r--r--   0        0        0     1929 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/bloom_filter.py
--rw-r--r--   0        0        0      307 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/func.py
--rw-r--r--   0        0        0      879 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/html.py
--rw-r--r--   0        0        0     1528 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/import_object.py
--rw-r--r--   0        0        0     4727 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/timer.py
--rw-r--r--   0        0        0   684816 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/useragent.py
--rw-r--r--   0        0        0     1406 2023-04-26 05:50:47.144387 usepy-0.1.46/src/usepy/utils/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 usepy-0.1.46/PKG-INFO
+-rw-r--r--   0        0        0      749 2023-05-01 12:02:41.208303 usepy-0.1.47/README.md
+-rw-r--r--   0        0        0      752 2023-05-01 12:02:41.224303 usepy-0.1.47/pyproject.toml
+-rw-r--r--   0        0        0     1865 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/__init__.py
+-rw-r--r--   0        0        0     6407 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/_datetime.py
+-rw-r--r--   0        0        0     3119 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/_path.py
+-rw-r--r--   0        0        0     1217 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/_thread.py
+-rw-r--r--   0        0        0        0 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/contrib/__init__.py
+-rw-r--r--   0        0        0     1302 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/contrib/pydantic_.py
+-rw-r--r--   0        0        0     2039 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/contrib/tenacity_.py
+-rw-r--r--   0        0        0      202 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/__init__.py
+-rw-r--r--   0        0        0     6773 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/_string.py
+-rw-r--r--   0        0        0     5000 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/addict.py
+-rw-r--r--   0        0        0     1059 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/counter.py
+-rw-r--r--   0        0        0     8331 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/dict.py
+-rw-r--r--   0        0        0     7116 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/data/list.py
+-rw-r--r--   0        0        0      681 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/__init__.py
+-rw-r--r--   0        0        0      457 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/cache.py
+-rw-r--r--   0        0        0      415 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/catch_error.py
+-rw-r--r--   0        0        0      382 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/except_debug.py
+-rw-r--r--   0        0        0      416 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/listify.py
+-rw-r--r--   0        0        0     1879 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/retry.py
+-rw-r--r--   0        0        0      377 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/run_in_thread.py
+-rw-r--r--   0        0        0      510 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/singleton.py
+-rw-r--r--   0        0        0      410 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/decorator/timeit.py
+-rw-r--r--   0        0        0      138 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/parser/__init__.py
+-rw-r--r--   0        0        0     3429 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/parser/curl.py
+-rw-r--r--   0        0        0     1379 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/parser/url.py
+-rw-r--r--   0        0        0      645 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/_is.py
+-rw-r--r--   0        0        0     1550 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/_to.py
+-rw-r--r--   0        0        0     1929 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/bloom_filter.py
+-rw-r--r--   0        0        0      307 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/func.py
+-rw-r--r--   0        0        0      879 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/html.py
+-rw-r--r--   0        0        0     1528 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/import_object.py
+-rw-r--r--   0        0        0      840 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/timeout.py
+-rw-r--r--   0        0        0     4727 2023-05-01 12:02:41.224303 usepy-0.1.47/src/usepy/utils/timer.py
+-rw-r--r--   0        0        0   684816 2023-05-01 12:02:41.228303 usepy-0.1.47/src/usepy/utils/useragent.py
+-rw-r--r--   0        0        0     1406 2023-05-01 12:02:41.228303 usepy-0.1.47/src/usepy/utils/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 usepy-0.1.47/PKG-INFO
```

### Comparing `usepy-0.1.46/README.md` & `usepy-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/pyproject.toml` & `usepy-0.1.47/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usepy"
-version = "0.1.46"
+version = "0.1.47"
 description = "usepy"
 homepage = "https://usepy.code05.com/"
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'usepy', from = 'src' }
 ]
```

### Comparing `usepy-0.1.46/src/usepy/__init__.py` & `usepy-0.1.47/src/usepy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from ._datetime import useDateTime
 from ._path import usePath
 from ._thread import useThread
 from .data import (
     useDict,
     useList,
     useString,
-    useAdDict
+    useAdDict,
+    useCounter
 )
 from .decorator import (
     useDecorator,
     useSingleton,
     useTimeIt,
     useRunInThread,
     useCatchError,
@@ -23,14 +24,16 @@
     useParser,
     useCURL,
     useURL
 )
 from .utils import (
     useTimer,
     useTimerManager,
+    useTimeoutFn,
+    useTimeout,
     useUserAgent,
     useImport,
     useLazyImport,
     useUniqueId,
     useDataToDict,
     useCookieToDict,
     useHeadersToDict,
@@ -53,14 +56,15 @@
 
 __all__ = [
     # data
     'useDict',
     'useList',
     'useString',
     'useAdDict',
+    'useCounter',
     # decorator
     'useDecorator',
     'useSingleton',
     'useTimeIt',
     'useRunInThread',
     'useCatchError',
     'useExceptDebug',
@@ -72,14 +76,16 @@
     'useCURL',
     'useURL',
     # utils
     'useIs',
     'useTo',
     'useTimer',
     'useTimerManager',
+    'useTimeoutFn',
+    'useTimeout',
     'useUserAgent',
     'useImport',
     'useLazyImport',
     'useUniqueId',
     'useDataToDict',
     'useCookieToDict',
     'useHeadersToDict',
```

### Comparing `usepy-0.1.46/src/usepy/_datetime.py` & `usepy-0.1.47/src/usepy/_datetime.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/_path.py` & `usepy-0.1.47/src/usepy/_path.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/_thread.py` & `usepy-0.1.47/src/usepy/_thread.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/contrib/pydantic_.py` & `usepy-0.1.47/src/usepy/contrib/pydantic_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/contrib/tenacity_.py` & `usepy-0.1.47/src/usepy/contrib/tenacity_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/data/_string.py` & `usepy-0.1.47/src/usepy/data/_string.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/data/addict.py` & `usepy-0.1.47/src/usepy/data/addict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/data/dict.py` & `usepy-0.1.47/src/usepy/data/dict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/data/list.py` & `usepy-0.1.47/src/usepy/data/list.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/decorator/__init__.py` & `usepy-0.1.47/src/usepy/decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/decorator/retry.py` & `usepy-0.1.47/src/usepy/decorator/retry.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/parser/curl.py` & `usepy-0.1.47/src/usepy/parser/curl.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/parser/url.py` & `usepy-0.1.47/src/usepy/parser/url.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/__init__.py` & `usepy-0.1.47/src/usepy/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from . import _is as useIs
 from . import _to as useTo
 from . import useragent as useUserAgent
 from .bloom_filter import BloomFilter as useBloomFilter
 from .html import clean_html as useCleanHtml
 from .import_object import import_object as useImport, LazyImport as useLazyImport
 from .timer import Timer as useTimer, TimerManager as useTimerManager
+from .timeout import useTimeoutFn, useTimeout
 from .utils import (
     gen_unique_id as useUniqueId,
     cookie_to_dict as useCookieToDict,
     headers_to_dict as useHeadersToDict,
     data_to_dict as useDataToDict,
     sizeof_fmt as useSizeofFmt,
 )
```

### Comparing `usepy-0.1.46/src/usepy/utils/_is.py` & `usepy-0.1.47/src/usepy/utils/_is.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/_to.py` & `usepy-0.1.47/src/usepy/utils/_to.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/bloom_filter.py` & `usepy-0.1.47/src/usepy/utils/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/html.py` & `usepy-0.1.47/src/usepy/utils/html.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/import_object.py` & `usepy-0.1.47/src/usepy/utils/import_object.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/timer.py` & `usepy-0.1.47/src/usepy/utils/timer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/useragent.py` & `usepy-0.1.47/src/usepy/utils/useragent.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/src/usepy/utils/utils.py` & `usepy-0.1.47/src/usepy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `usepy-0.1.46/PKG-INFO` & `usepy-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usepy
-Version: 0.1.46
+Version: 0.1.47
 Summary: usepy
 Home-page: https://usepy.code05.com/
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usepy Version: 0.1.46 Summary: usepy Home-page:
+Metadata-Version: 2.1 Name: usepy Version: 0.1.47 Summary: usepy Home-page:
 https://usepy.code05.com/ Author: miclon Author-email: jcnd@163.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: logger Provides-Extra:
 notify Requires-Dist: usepy-plugin-logger (>=0.1.0,<0.2.0) ; extra == "logger"
 Requires-Dist: usepy-plugin-notify (>=0.2.2,<0.3.0) ; extra == "notify"
```

