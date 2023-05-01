# Comparing `tmp/async_shell-1.0.2.tar.gz` & `tmp/async_shell-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_shell-1.0.2.tar", max compression
+gzip compressed data, was "async_shell-1.0.3.tar", max compression
```

## Comparing `async_shell-1.0.2.tar` & `async_shell-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1057 2023-01-23 11:40:06.628424 async_shell-1.0.2/LICENSE
--rw-r--r--   0        0        0      112 2023-01-23 11:42:18.450080 async_shell-1.0.2/README.md
--rw-r--r--   0        0        0     3785 2023-02-07 11:24:21.304697 async_shell-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5894 2023-02-07 11:22:01.512367 async_shell-1.0.2/src/async_shell/__init__.py
--rw-r--r--   0        0        0      172 2023-02-05 15:45:42.212083 async_shell-1.0.2/src/async_shell/constants.py
--rw-r--r--   0        0        0        0 2023-01-23 11:40:06.646331 async_shell-1.0.2/src/async_shell/py.typed
--rw-r--r--   0        0        0      328 2023-01-23 11:40:06.643709 async_shell-1.0.2/src/async_shell/version.py
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 async_shell-1.0.2/setup.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 async_shell-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-01-23 11:40:06.628424 async_shell-1.0.3/LICENSE
+-rw-r--r--   0        0        0      112 2023-01-23 11:42:18.450080 async_shell-1.0.3/README.md
+-rw-r--r--   0        0        0     3785 2023-05-01 20:06:54.996571 async_shell-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6026 2023-05-01 20:12:22.335451 async_shell-1.0.3/src/async_shell/__init__.py
+-rw-r--r--   0        0        0      172 2023-02-05 15:45:42.212083 async_shell-1.0.3/src/async_shell/constants.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:40:06.646331 async_shell-1.0.3/src/async_shell/py.typed
+-rw-r--r--   0        0        0      328 2023-01-23 11:40:06.643709 async_shell-1.0.3/src/async_shell/version.py
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 async_shell-1.0.3/setup.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 async_shell-1.0.3/PKG-INFO
```

### Comparing `async_shell-1.0.2/LICENSE` & `async_shell-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_shell-1.0.2/pyproject.toml` & `async_shell-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-shell"
-version = "1.0.2"
+version = "1.0.3"
 description = "Asyncio subprocess shell command wrapper"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/async-shell"
```

### Comparing `async_shell-1.0.2/src/async_shell/__init__.py` & `async_shell-1.0.3/src/async_shell/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     ) -> None:
         self._command: str = command
         self._proc: t.Optional[Process] = None
         self._encoding: str = encoding or self._DEFAULT_ENCODING
         self._start_time: t.Optional[float] = None
         self._post_validate: bool = False
         self._was_stopped: bool = False
+        self._was_finalized: bool = False
 
     @property
     def was_stopped(self) -> bool:
         """Tell if the process was stopped during execution"""
         return self._was_stopped
 
     @property
@@ -97,15 +98,15 @@
             self.logger.trace(f"Starting subprocess: {self._command!r}")
             self._proc = await create_subprocess_shell(
                 cmd=self._command,
                 stdin=None,
                 stdout=PIPE,
                 stderr=PIPE,
             )
-        self.logger.debug(f"Started process with PID {self.pid}")
+            self.logger.debug(f"Started process with PID {self.pid}")
         return self._proc
 
     async def read_stdout(self, strip_linesep: bool = True) -> t.AsyncGenerator[str, None]:
         """Run through stdout data and yield decoded strings line by line"""
         proc: Process = await self._get_proc()
         stdout: StreamReader = proc.stdout  # type: ignore
         async for chunk in stdout:  # type: bytes
@@ -154,14 +155,16 @@
         return exc_type is None
 
     def poll(self) -> bool:
         """Check if the subprocess has finished"""
         return self._proc is not None and self._proc.returncode is not None
 
     async def _finalize(self) -> None:
+        if self._was_finalized:
+            return
         if self._proc is None:
             self.logger.warning("Finalizing non-started process")
             return
         self.logger.debug(f"Finalizing process with PID {self.pid}")
         if self._proc.returncode is None:
             self.logger.trace(f"Killing process with PID {self.pid}")
             self._proc.kill()
@@ -169,7 +172,8 @@
         # Close communication anyway
         await self._proc.communicate()
         for stream in (self._proc.stdout, self._proc.stderr, self._proc.stdin):
             if stream is None:
                 continue
             self.logger.trace(f"Closing stream: {stream}")
             stream._transport.close()  # type: ignore[union-attr]  # pylint: disable=protected-access
+        self._was_finalized = True
```

### Comparing `async_shell-1.0.2/setup.py` & `async_shell-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['classlogging>=1.0.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'async-shell',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Asyncio subprocess shell command wrapper',
     'long_description': '# async-shell\n\nAsyncio subprocess shell command wrapper.\n\n## Installation\n\n```shell\npip install async-shell\n```\n',
     'author': 'Artem Novikov',
     'author_email': 'artnew@list.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/reartnew/async-shell',
```

### Comparing `async_shell-1.0.2/PKG-INFO` & `async_shell-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-shell
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asyncio subprocess shell command wrapper
 Home-page: https://github.com/reartnew/async-shell
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

