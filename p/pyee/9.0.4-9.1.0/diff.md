# Comparing `tmp/pyee-9.0.4.tar.gz` & `tmp/pyee-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyee-9.0.4.tar", last modified: Fri Feb  4 19:53:30 2022, max compression
+gzip compressed data, was "pyee-9.1.0.tar", last modified: Sun Apr 30 22:14:02 2023, max compression
```

## Comparing `pyee-9.0.4.tar` & `pyee-9.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2022-02-04 19:53:30.644342 pyee-9.0.4/
--rw-rw-r--   0 josh      (1000) josh      (1000)     6894 2022-02-04 19:53:07.000000 pyee-9.0.4/CHANGELOG.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)      518 2022-01-18 01:05:07.000000 pyee-9.0.4/CONTRIBUTORS.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     2518 2022-01-12 02:21:32.000000 pyee-9.0.4/DEVELOPMENT.rst
--rw-rw-r--   0 josh      (1000) josh      (1000)     1080 2022-01-12 02:21:32.000000 pyee-9.0.4/LICENSE
--rw-rw-r--   0 josh      (1000) josh      (1000)      177 2022-02-04 19:51:49.000000 pyee-9.0.4/MANIFEST.in
--rw-rw-r--   0 josh      (1000) josh      (1000)     1992 2022-02-04 19:53:30.644342 pyee-9.0.4/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      811 2021-08-19 23:33:50.000000 pyee-9.0.4/README.rst
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2022-02-04 19:53:30.643342 pyee-9.0.4/pyee/
--rw-rw-r--   0 josh      (1000) josh      (1000)     3728 2022-01-12 05:10:56.000000 pyee-9.0.4/pyee/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2607 2022-01-12 02:21:32.000000 pyee-9.0.4/pyee/asyncio.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     7783 2022-01-18 14:48:06.000000 pyee-9.0.4/pyee/base.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2913 2022-01-12 04:14:45.000000 pyee-9.0.4/pyee/cls.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2463 2022-01-12 02:21:32.000000 pyee-9.0.4/pyee/executor.py
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2022-01-12 02:21:32.000000 pyee-9.0.4/pyee/py.typed
--rw-rw-r--   0 josh      (1000) josh      (1000)     4520 2022-01-17 21:33:19.000000 pyee-9.0.4/pyee/trio.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2979 2022-01-17 21:33:19.000000 pyee-9.0.4/pyee/twisted.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     6611 2022-01-18 06:28:28.000000 pyee-9.0.4/pyee/uplift.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2022-02-04 19:53:30.643342 pyee-9.0.4/pyee.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)     1992 2022-02-04 19:53:30.000000 pyee-9.0.4/pyee.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      543 2022-02-04 19:53:30.000000 pyee-9.0.4/pyee.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2022-02-04 19:53:30.000000 pyee-9.0.4/pyee.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       18 2022-02-04 19:53:30.000000 pyee-9.0.4/pyee.egg-info/requires.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        5 2022-02-04 19:53:30.000000 pyee-9.0.4/pyee.egg-info/top_level.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       98 2022-01-22 19:36:15.000000 pyee-9.0.4/pyproject.toml
--rw-rw-r--   0 josh      (1000) josh      (1000)       90 2022-02-04 19:53:30.644342 pyee-9.0.4/setup.cfg
--rw-rw-r--   0 josh      (1000) josh      (1000)     1324 2022-02-04 19:51:59.000000 pyee-9.0.4/setup.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2022-02-04 19:53:30.644342 pyee-9.0.4/tests/
--rw-rw-r--   0 josh      (1000) josh      (1000)      235 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/conftest.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     3976 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/test_async.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      993 2022-01-12 04:14:45.000000 pyee-9.0.4/tests/test_cls.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1228 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/test_executor.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     6086 2022-01-18 14:39:46.000000 pyee-9.0.4/tests/test_sync.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2440 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/test_trio.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1623 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/test_twisted.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     6308 2022-01-12 02:21:32.000000 pyee-9.0.4/tests/test_uplift.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.412626 pyee-9.1.0/
+-rw-r--r--   0 josh      (1000) josh      (1000)     7159 2023-04-30 22:13:43.000000 pyee-9.1.0/CHANGELOG.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)      518 2023-04-30 21:23:40.000000 pyee-9.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)     2518 2023-04-30 21:23:40.000000 pyee-9.1.0/DEVELOPMENT.rst
+-rw-r--r--   0 josh      (1000) josh      (1000)     1080 2023-04-30 21:23:40.000000 pyee-9.1.0/LICENSE
+-rw-r--r--   0 josh      (1000) josh      (1000)      177 2023-04-30 21:23:40.000000 pyee-9.1.0/MANIFEST.in
+-rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-04-30 22:14:02.412626 pyee-9.1.0/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)      811 2023-04-30 21:23:40.000000 pyee-9.1.0/README.rst
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.411626 pyee-9.1.0/pyee/
+-rw-r--r--   0 josh      (1000) josh      (1000)     3728 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/__init__.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2607 2023-04-30 22:03:07.000000 pyee-9.1.0/pyee/asyncio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     8099 2023-04-30 21:55:18.000000 pyee-9.1.0/pyee/base.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2913 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/cls.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2463 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/executor.py
+-rw-r--r--   0 josh      (1000) josh      (1000)        0 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/py.typed
+-rw-r--r--   0 josh      (1000) josh      (1000)     4520 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/trio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     3005 2023-04-30 21:55:18.000000 pyee-9.1.0/pyee/twisted.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6611 2023-04-30 21:23:40.000000 pyee-9.1.0/pyee/uplift.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.411626 pyee-9.1.0/pyee.egg-info/
+-rw-r--r--   0 josh      (1000) josh      (1000)     1699 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)      543 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/SOURCES.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        1 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/dependency_links.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       18 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/requires.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        5 2023-04-30 22:14:02.000000 pyee-9.1.0/pyee.egg-info/top_level.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       98 2023-04-30 21:23:40.000000 pyee-9.1.0/pyproject.toml
+-rw-r--r--   0 josh      (1000) josh      (1000)       90 2023-04-30 22:14:02.412626 pyee-9.1.0/setup.cfg
+-rw-r--r--   0 josh      (1000) josh      (1000)     1324 2023-04-30 22:13:43.000000 pyee-9.1.0/setup.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2023-04-30 22:14:02.412626 pyee-9.1.0/tests/
+-rw-r--r--   0 josh      (1000) josh      (1000)      235 2023-04-30 21:23:40.000000 pyee-9.1.0/tests/conftest.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     4018 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_async.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1003 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_cls.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1245 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_executor.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6297 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_sync.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     2444 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_trio.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     1860 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_twisted.py
+-rw-r--r--   0 josh      (1000) josh      (1000)     6318 2023-04-30 21:55:18.000000 pyee-9.1.0/tests/test_uplift.py
```

### Comparing `pyee-9.0.4/CHANGELOG.rst` & `pyee-9.1.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2023/04/30 Version 9.1.0
+------------------------
+- ``EventEmitter`` supports pickling
+- Development dependencies updated to latest
+- Dependency on mock removed in favor of unittest.mock
+- Additional type hints so pyright check passes on latest
+- Drop 3.7 support
+
 2022/02/04 Version 9.0.4
 ------------------------
 
 - Add ``py.typed`` file to ``MANIFEST.in`` (ensures mypy actually respects the
   type annotations)
 
 2022/01/18 Version 9.0.3
```

### Comparing `pyee-9.0.4/CONTRIBUTORS.rst` & `pyee-9.1.0/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/DEVELOPMENT.rst` & `pyee-9.1.0/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/LICENSE` & `pyee-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/README.rst` & `pyee-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/__init__.py` & `pyee-9.1.0/pyee/__init__.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/asyncio.py` & `pyee-9.1.0/pyee/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/base.py` & `pyee-9.1.0/pyee/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # -*- coding: utf-8 -*-
 
 from collections import OrderedDict
 from threading import Lock
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 
 class PyeeException(Exception):
     """An exception internal to pyee."""
 
 
 Handler = TypeVar(name="Handler", bound=Callable)
@@ -42,14 +53,23 @@
     def __init__(self) -> None:
         self._events: Dict[
             str,
             "OrderedDict[Callable, Callable]",
         ] = dict()
         self._lock: Lock = Lock()
 
+    def __getstate__(self) -> Mapping[str, Any]:
+        state = self.__dict__.copy()
+        del state["_lock"]
+        return state
+
+    def __setstate__(self, state: Mapping[str, Any]) -> None:
+        self.__dict__.update(state)
+        self._lock = Lock()
+
     def on(
         self, event: str, f: Optional[Handler] = None
     ) -> Union[Handler, Callable[[Handler], Handler]]:
         """Registers the function ``f`` to the event name ``event``, if provided.
 
         If ``f`` isn't provided, this method calls ``EventEmitter#listens_to`, and
         otherwise calls ``EventEmitter#add_listener``. In other words, you may either
```

### Comparing `pyee-9.0.4/pyee/cls.py` & `pyee-9.1.0/pyee/cls.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/executor.py` & `pyee-9.1.0/pyee/executor.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/trio.py` & `pyee-9.1.0/pyee/trio.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee/twisted.py` & `pyee-9.1.0/pyee/twisted.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from typing import Any, Callable, Dict, Tuple
+from typing import Any, Callable, Dict, Optional, Tuple
 
 from twisted.internet.defer import Deferred, ensureDeferred
 from twisted.python.failure import Failure
 
 from pyee.base import EventEmitter, PyeeException
 
 try:
@@ -53,25 +53,25 @@
 
     def _emit_run(
         self,
         f: Callable,
         args: Tuple[Any, ...],
         kwargs: Dict[str, Any],
     ) -> None:
-        d = None
+        d: Optional[Deferred[Any]] = None
         try:
             result = f(*args, **kwargs)
         except Exception:
             self.emit("failure", Failure())
         else:
             if iscoroutine and iscoroutine(result):
-                d: Deferred[Any] = ensureDeferred(result)
+                d = ensureDeferred(result)
             elif isinstance(result, Deferred):
                 d = result
-            else:
+            elif not d:
                 return
 
             def errback(failure: Failure) -> None:
                 if failure:
                     self.emit("failure", failure)
 
             d.addErrback(errback)
```

### Comparing `pyee-9.0.4/pyee/uplift.py` & `pyee-9.1.0/pyee/uplift.py`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/pyee.egg-info/SOURCES.txt` & `pyee-9.1.0/pyee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyee-9.0.4/setup.py` & `pyee-9.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_rst = path.join(path.abspath(path.dirname(__file__)), "README.rst")
 
 with open(README_rst, "r") as f:
     long_description = f.read()
 
 setup(
     name="pyee",
-    version="9.0.4",
+    version="9.1.0",
     packages=find_packages(),
     include_package_data=True,
     description="A port of node.js's EventEmitter to python.",
     long_description=long_description,
     author="Josh Holbrook",
     author_email="josh.holbrook@gmail.com",
     url="https://github.com/jfhbrook/pyee",
```

### Comparing `pyee-9.0.4/tests/test_async.py` & `pyee-9.1.0/tests/test_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import pytest_asyncio.plugin  # noqa
 
 try:
     from asyncio.exceptions import TimeoutError  # type: ignore
 except ImportError:
     from concurrent.futures import TimeoutError  # type: ignore
 
-from mock import Mock
+from unittest.mock import Mock
+
 from twisted.internet.defer import succeed
 
-from pyee import AsyncIOEventEmitter, TwistedEventEmitter
+from pyee.asyncio import AsyncIOEventEmitter
+from pyee.twisted import TwistedEventEmitter
 
 
 class PyeeTestError(Exception):
     pass
 
 
 @pytest.mark.asyncio
```

### Comparing `pyee-9.0.4/tests/test_cls.py` & `pyee-9.1.0/tests/test_cls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-from mock import Mock
+from unittest.mock import Mock
+
 import pytest
 
 from pyee import EventEmitter
 from pyee.cls import evented, on
 
 
 @evented
```

### Comparing `pyee-9.0.4/tests/test_executor.py` & `pyee-9.1.0/tests/test_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from time import sleep
+from unittest.mock import Mock
 
-from mock import Mock
-
-from pyee import ExecutorEventEmitter
+from pyee.executor import ExecutorEventEmitter
 
 
 class PyeeTestError(Exception):
     pass
 
 
 def test_executor_emit():
```

### Comparing `pyee-9.0.4/tests/test_sync.py` & `pyee-9.1.0/tests/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from collections import OrderedDict
+from pickle import dumps, loads
+from unittest.mock import Mock
 
-from mock import Mock
 from pytest import raises
 
 from pyee import EventEmitter
 
 
 class PyeeTestException(Exception):
     pass
@@ -274,7 +275,15 @@
     call_me_also.assert_called_once()
 
     call_me_also.reset_mock()
 
     # Calling the event handler directly doesn't clear the handler
     ee.emit("once")
     call_me_also.assert_called_once()
+
+
+def test_if_serializable():
+    """`pickle`ing should not throw."""
+    ee = EventEmitter()
+    ee_copy = loads(dumps(ee))
+    assert ee._lock
+    assert ee_copy._lock
```

### Comparing `pyee-9.0.4/tests/test_trio.py` & `pyee-9.1.0/tests/test_trio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 import pytest_trio.plugin  # noqa
 import trio
 
-from pyee import TrioEventEmitter
+from pyee.trio import TrioEventEmitter
 
 
 class PyeeTestError(Exception):
     pass
 
 
 @pytest.mark.trio
 async def test_trio_emit():
     """Test that the trio event emitter can handle wrapping
     coroutines
     """
 
     async with TrioEventEmitter() as ee:
-
         should_call = trio.Event()
 
         @ee.on("event")
         async def event_handler():
             should_call.set()
 
         ee.emit("event")
```

### Comparing `pyee-9.0.4/tests/test_twisted.py` & `pyee-9.1.0/tests/test_twisted.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
-from mock import Mock
-from twisted.internet.defer import inlineCallbacks
+from typing import Generator
+from unittest.mock import Mock
+
+from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.python.failure import Failure
 
-from pyee import TwistedEventEmitter
+from pyee.twisted import TwistedEventEmitter
 
 
 class PyeeTestError(Exception):
     pass
 
 
 def test_propagates_failure():
@@ -17,16 +19,18 @@
     """
     ee = TwistedEventEmitter()
 
     should_call = Mock()
 
     @ee.on("event")
     @inlineCallbacks
-    def event_handler():
-        yield Failure(PyeeTestError())
+    def event_handler() -> Generator[Deferred[object], object, None]:
+        d = Deferred()
+        d.callback(Failure(PyeeTestError()))
+        yield d
 
     @ee.on("failure")
     def handle_failure(f):
         assert isinstance(f, Failure)
         should_call(f)
 
     ee.emit("event")
@@ -63,16 +67,18 @@
 
     ee = TwistedEventEmitter()
 
     should_call = Mock()
 
     @ee.on("event")
     @inlineCallbacks
-    def event_handler():
-        yield Failure(PyeeTestError())
+    def event_handler() -> Generator[Deferred[object], object, None]:
+        d = Deferred()
+        d.callback(Failure(PyeeTestError()))
+        yield d
 
     @ee.on("error")
     def handle_error(exc):
         assert isinstance(exc, Exception)
         should_call(exc)
 
     ee.emit("event")
```

### Comparing `pyee-9.0.4/tests/test_uplift.py` & `pyee-9.1.0/tests/test_uplift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
-from mock import call, Mock
+from unittest.mock import call, Mock
+
 import pytest
 
 from pyee import EventEmitter
 from pyee.uplift import unwrap, uplift
 
 
 class UpliftedEventEmitter(EventEmitter):
```

