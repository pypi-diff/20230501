# Comparing `tmp/pytest-wake-0.3.4.tar.gz` & `tmp/pytest-wake-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-wake-0.3.4.tar", last modified: Mon Feb 27 03:18:45 2023, max compression
+gzip compressed data, was "pytest-wake-0.3.5.tar", last modified: Mon May  1 07:58:20 2023, max compression
```

## Comparing `pytest-wake-0.3.4.tar` & `pytest-wake-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-02-27 03:18:45.381362 pytest-wake-0.3.4/
--rw-r--r--   0 sh00494ml   (503) staff       (20)     1056 2022-09-05 03:57:41.000000 pytest-wake-0.3.4/.gitignore
--rw-r--r--   0 sh00494ml   (503) staff       (20)    11357 2022-09-05 03:57:41.000000 pytest-wake-0.3.4/LICENSE
--rw-r--r--   0 sh00494ml   (503) staff       (20)      652 2023-02-27 03:18:45.381218 pytest-wake-0.3.4/PKG-INFO
--rw-r--r--   0 sh00494ml   (503) staff       (20)       20 2022-09-28 08:12:17.000000 pytest-wake-0.3.4/README.md
--rw-r--r--   0 sh00494ml   (503) staff       (20)      915 2022-09-05 03:57:41.000000 pytest-wake-0.3.4/__setup.py
-drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-02-27 03:18:45.380014 pytest-wake-0.3.4/pytest_wake/
--rw-r--r--   0 sh00494ml   (503) staff       (20)      251 2023-02-27 03:04:10.000000 pytest-wake-0.3.4/pytest_wake/__init__.py
--rw-r--r--   0 sh00494ml   (503) staff       (20)     3604 2023-02-27 03:17:28.000000 pytest-wake-0.3.4/pytest_wake/client.py
--rw-r--r--   0 sh00494ml   (503) staff       (20)     6694 2023-02-27 03:03:20.000000 pytest-wake-0.3.4/pytest_wake/core.py
--rw-r--r--   0 sh00494ml   (503) staff       (20)      249 2023-02-27 02:27:42.000000 pytest-wake-0.3.4/pytest_wake/exception.py
--rw-r--r--   0 sh00494ml   (503) staff       (20)     2811 2023-02-24 08:37:36.000000 pytest-wake-0.3.4/pytest_wake/signature.py
--rw-r--r--   0 sh00494ml   (503) staff       (20)      516 2023-02-27 03:17:54.000000 pytest-wake-0.3.4/pytest_wake/utils.py
-drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-02-27 03:18:45.381013 pytest-wake-0.3.4/pytest_wake.egg-info/
--rw-r--r--   0 sh00494ml   (503) staff       (20)      652 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/PKG-INFO
--rw-r--r--   0 sh00494ml   (503) staff       (20)      397 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/SOURCES.txt
--rw-r--r--   0 sh00494ml   (503) staff       (20)        1 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/dependency_links.txt
--rw-r--r--   0 sh00494ml   (503) staff       (20)       42 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/entry_points.txt
--rw-r--r--   0 sh00494ml   (503) staff       (20)        7 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/requires.txt
--rw-r--r--   0 sh00494ml   (503) staff       (20)       12 2023-02-27 03:18:45.000000 pytest-wake-0.3.4/pytest_wake.egg-info/top_level.txt
--rw-r--r--   0 sh00494ml   (503) staff       (20)       38 2023-02-27 03:18:45.381423 pytest-wake-0.3.4/setup.cfg
--rw-r--r--   0 sh00494ml   (503) staff       (20)     3805 2023-02-27 03:17:20.000000 pytest-wake-0.3.4/setup.py
+drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-05-01 07:58:20.774187 pytest-wake-0.3.5/
+-rw-r--r--   0 sh00494ml   (503) staff       (20)     1056 2023-04-25 14:28:23.000000 pytest-wake-0.3.5/.gitignore
+-rw-r--r--   0 sh00494ml   (503) staff       (20)    11357 2022-09-05 03:57:41.000000 pytest-wake-0.3.5/LICENSE
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      667 2023-05-01 07:58:20.774042 pytest-wake-0.3.5/PKG-INFO
+-rw-r--r--   0 sh00494ml   (503) staff       (20)       35 2023-04-25 14:28:23.000000 pytest-wake-0.3.5/README.md
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      915 2022-09-05 03:57:41.000000 pytest-wake-0.3.5/__setup.py
+drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-05-01 07:58:20.772791 pytest-wake-0.3.5/pytest_wake/
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      251 2023-04-25 14:28:23.000000 pytest-wake-0.3.5/pytest_wake/__init__.py
+-rw-r--r--   0 sh00494ml   (503) staff       (20)     3445 2023-04-24 07:55:21.000000 pytest-wake-0.3.5/pytest_wake/client.py
+-rw-r--r--   0 sh00494ml   (503) staff       (20)     7282 2023-04-24 07:55:21.000000 pytest-wake-0.3.5/pytest_wake/core.py
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      249 2023-04-24 07:55:21.000000 pytest-wake-0.3.5/pytest_wake/exception.py
+-rw-r--r--   0 sh00494ml   (503) staff       (20)     2828 2023-04-24 07:55:21.000000 pytest-wake-0.3.5/pytest_wake/signature.py
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      516 2023-04-24 07:55:21.000000 pytest-wake-0.3.5/pytest_wake/utils.py
+drwxr-xr-x   0 sh00494ml   (503) staff       (20)        0 2023-05-01 07:58:20.773820 pytest-wake-0.3.5/pytest_wake.egg-info/
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      667 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/PKG-INFO
+-rw-r--r--   0 sh00494ml   (503) staff       (20)      397 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/SOURCES.txt
+-rw-r--r--   0 sh00494ml   (503) staff       (20)        1 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/dependency_links.txt
+-rw-r--r--   0 sh00494ml   (503) staff       (20)       42 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/entry_points.txt
+-rw-r--r--   0 sh00494ml   (503) staff       (20)        7 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/requires.txt
+-rw-r--r--   0 sh00494ml   (503) staff       (20)       12 2023-05-01 07:58:20.000000 pytest-wake-0.3.5/pytest_wake.egg-info/top_level.txt
+-rw-r--r--   0 sh00494ml   (503) staff       (20)       38 2023-05-01 07:58:20.774241 pytest-wake-0.3.5/setup.cfg
+-rw-r--r--   0 sh00494ml   (503) staff       (20)     3820 2023-05-01 07:58:13.000000 pytest-wake-0.3.5/setup.py
```

### Comparing `pytest-wake-0.3.4/.gitignore` & `pytest-wake-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-wake-0.3.4/LICENSE` & `pytest-wake-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-wake-0.3.4/PKG-INFO` & `pytest-wake-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-wake
-Version: 0.3.4
+Version: 0.3.5
 Home-page: 
 Author: You can call me V
 Author-email: 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,8 +14,8 @@
 Classifier: Framework :: Pytest
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Info
-Now or Never.
+There are many things to do.
```

### Comparing `pytest-wake-0.3.4/__setup.py` & `pytest-wake-0.3.5/__setup.py`

 * *Files identical despite different names*

### Comparing `pytest-wake-0.3.4/pytest_wake/client.py` & `pytest-wake-0.3.5/pytest_wake/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
-"""
-@File    :   client.py
-@Time    :   2023/02/17 14:15:57
-@Version :   1.0
-@Desc    :
-"""
+
 import json
 
 from requests import Response
 from requests import request as _request
 
 from .exception import UnImplementedMethodError, UnSupportVersionError
 from .signature import SignatureImpl
@@ -23,65 +18,63 @@
 
         if api_key and api_secret:
             self.signimpl = SignatureImpl(self.api_key, self.api_secret, self.recv_window)
 
     def request(self, method: str, url: str, params_or_body: dict = None, **kwargs) -> Response:
         method = method.lower()
         if method not in ("get", "post"):
-            raise UnImplementedMethodError(f"Unimplemented request method: {method}")
+            raise UnImplementedMethodError(f"Unimplemented request method yet: {method}")
 
-        need_auth = HttpClient.need_auth(url)
+        is_private: bool = HttpClient.is_private(url)
 
         if "/v2" in url:
             headers = {"Content-Type": "application/json"}
             if method == "get":
-                if "private" in url:
+                if is_private:
                     params_or_body["api_key"] = self.api_key
                     params_or_body["timestamp"] = self.signimpl.now_timestamp
                     params_or_body["recv_window"] = self.recv_window
                     params_or_body["sign"] = self.signimpl.generate(method, url, params_or_body)
                 return _request(method, url, params=params_or_body, headers=headers, **kwargs)
             else:
                 params_or_body["api_key"] = self.api_key
                 params_or_body["timestamp"] = self.signimpl.now_timestamp
                 params_or_body["recv_window"] = self.recv_window
                 params_or_body["sign"] = self.signimpl.generate(url, params_or_body)
                 return _request(method, url, data=json.dumps(params_or_body), headers=headers, **kwargs)
 
         elif "/v3" in url:
             if method == "get":
-                if "private" in url:
+                if is_private:
                     sign = self.signimpl.generate(method, url, params_or_body)
                     headers = self.signimpl.get_auth_headers(sign)
             else:
                 sign = self.signimpl.generate(method, url, params_or_body)
                 headers = self.signimpl.get_auth_headers(sign)
             return _request(method, url, data=json.dumps(params_or_body), headers=headers, **kwargs)
 
         elif "/v5" in url:
             if method == "get":
-                if need_auth:
+                if is_private:
                     sign = self.signimpl.generate(method, url, params_or_body)
                 else:
                     sign = None
                 headers = self.signimpl.get_auth_headers(sign)
-                print(f"headers: {headers}")
                 return _request(method, url, params=params_or_body, headers=headers, **kwargs)
             else:
                 sign = self.signimpl.generate(method, url, params_or_body)
                 headers = self.signimpl.get_auth_headers(sign)
-                print(f"headers: {headers}")
                 return _request(method, url, data=json.dumps(params_or_body), headers=headers, **kwargs)
         else:
             raise UnSupportVersionError(f"Unrecognized request url: {url}")
 
     @staticmethod
-    def need_auth(url) -> bool:
-        flag = False
+    def is_private(url) -> bool:
+        need_auth = False
         if "/v5/" in url:
             # exclude path like `/orderbook/`
             if "/position/" in url or "/order/" in url or "/execution/" in url:
-                flag = True
+                need_auth = True
         elif "private" in url:
-            flag = True
+            need_auth = True
 
-        return flag
+        return need_auth
```

### Comparing `pytest-wake-0.3.4/pytest_wake/core.py` & `pytest-wake-0.3.5/pytest_wake/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 
 import json
 import os
-from typing import List, Sequence
+from typing import Dict, Sequence
 from urllib import parse
 
 import pytest
 
 from .client import HttpClient, Response
 
 
-def respdiff(src_resp: Response, dst_resp: Response = None, key_whitelist=None, **kwargs) -> dict:
+def respdiff(src_resp: Response, dst_resp: Response = None, key_whitelist: Sequence[str] = None, **kwargs) -> Dict[str]:
+    """Compare two `<class> requests.Response` , and return return detailed results.
+
+    Args:
+        src_resp (Response): source response.
+        dst_resp (Response, optional): dest response. Defaults to None.
+        key_whitelist (Sequence[str], optional): Whitelist keys, will skip comparison. #TODO: .flat dict
+
+    Raises:
+        RuntimeError: when env variable missing api key & secret.
+
+    Returns:
+        dict: The comparison result, including the meta information of the two requests (method/url/traceid/payload).
+    """
     src_resp.encoding = "utf-8"
     url: str = src_resp.url  # contains query params
     parse_res = parse.urlparse(url)
     method = src_resp.request.method
     body = src_resp.request.body
     payload = json.loads(str(body)) if body else None
 
@@ -60,34 +73,32 @@
     else:
         src = src_resp.json()
         dst = dst_resp.json()
         src_retcode = src.get("retCode") or src.get("ret_code")
         dst_retcode = dst.get("retCode") or dst.get("ret_code")
 
         if src_retcode != dst_retcode:
+            res["result"] = False
             res["details"] = f"different ret code. src: {src_retcode}, dst: {dst_retcode}"
         else:
-            res["details"] = jsondiff(dst, dst, key_whitelist=key_whitelist)
-
-    res["result"] = True if len(res["details"]) == 0 else False
+            res.update(jsondiff(dst, dst, key_whitelist=key_whitelist))
 
     return res
 
 
-def jsondiff(src: dict, dst: dict, key_whitelist: Sequence[str] = None) -> List[dict]:
+def jsondiff(src: dict, dst: dict, key_whitelist: Sequence[str] = None) -> dict:
     assert all([type(src) == dict, type(dst) == dict]), "Unsupported parameter type."
 
     def _recursive_diff(l, r, details, path='/'):
         if type(l) != type(r):
             details.append({'replace': path, 'value': r, 'details': 'type', 'src': l})
             return
 
         delim = '/' if path != '/' else ''
 
-        # TODO: flat dict
         if key_whitelist and isinstance(l, dict) and isinstance(r, dict):
             for k in key_whitelist:
                 if k in l:
                     l.pop(k)
                 if k in r:
                     r.pop(k)
 
@@ -117,15 +128,19 @@
                     _recursive_diff(item, r[i], details, delim.join([path, str(i)]))
         else:
             if type(l) != type(r):
                 details.append({'replace': path, 'dst': r, 'src': l})
 
     details = []
     _recursive_diff(src, dst, details)
-    return details
+
+    res = {}
+    res["result"] = True if len(details) == 0 else False
+    res["details"] = details
+    return res
 
 
 def _get_traceid(resp: Response) -> str:
     return resp.headers.get("traceid", "")
 
 
 COIN_SYMBOL = {
```

### Comparing `pytest-wake-0.3.4/pytest_wake/signature.py` & `pytest-wake-0.3.5/pytest_wake/signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.api_key = api_key
         self.api_secret = bytes(api_secret, encoding="utf8")
         self.recv_window = recv_window
 
     def generate(self, method: str, url: str, params_or_body: dict, timestamp: int = None) -> str:
         self.now_timestamp = self.get_now_timestamp()
 
-        # TODO: 区分method
+        # TODO: Differentiate between methods
         if "/v2" in url:
             sign_str = ''
             for key in sorted(params_or_body.keys()):
                 v = str(params_or_body[key])
                 if isinstance(params_or_body[key], bool):
                     if params_or_body[key]:
                         v = 'true'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-wake-0.3.4/pytest_wake/utils.py` & `pytest-wake-0.3.5/pytest_wake/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-wake-0.3.4/pytest_wake.egg-info/PKG-INFO` & `pytest-wake-0.3.5/pytest_wake.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-wake
-Version: 0.3.4
+Version: 0.3.5
 Home-page: 
 Author: You can call me V
 Author-email: 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,8 +14,8 @@
 Classifier: Framework :: Pytest
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Info
-Now or Never.
+There are many things to do.
```

### Comparing `pytest-wake-0.3.4/setup.py` & `pytest-wake-0.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 #   $ pipenv install twine --dev
 
 import io
 import os
 import sys
 from shutil import rmtree
 
-from setuptools import Command, setup
+from setuptools import Command, find_packages, setup
 
 # Package meta-data.
-NAME = 'pytest-wake'
-DESCRIPTION = ''
-URL = ''
-EMAIL = ''
-AUTHOR = 'You can call me V'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.4'
+NAME = "pytest-wake"
+DESCRIPTION = ""
+URL = ""
+EMAIL = ""
+AUTHOR = "You can call me V"
+REQUIRES_PYTHON = ">=3.6.0"
+VERSION = "0.3.5"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "pytest",
 ]
 
 # What packages are optional?
@@ -36,96 +36,96 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
 else:
-    about['__version__'] = VERSION
+    about["__version__"] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
-    description = 'Build and publish the package.'
+    description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
+        print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
 
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    packages=["pytest_wake"],
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # packages=["pytest_wake"],
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['pytest_wake'],
     entry_points={"pytest11": ["pytest-wake = pytest_wake.core"]},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3',
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Pytest",
     ],
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        "upload": UploadCommand,
     },
     setup_requires=["setuptools_scm"],
 )
```

