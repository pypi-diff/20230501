# Comparing `tmp/HTTP-PyServer-0.0.4.tar.gz` & `tmp/HTTP-PyServer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.0.4.tar", last modified: Mon Apr 17 15:25:24 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.0.7.tar", last modified: Mon May  1 16:48:57 2023, max compression
```

## Comparing `HTTP-PyServer-0.0.4.tar` & `HTTP-PyServer-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.243085 HTTP-PyServer-0.0.4/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2036 2023-04-17 15:25:24.242087 HTTP-PyServer-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1473 2023-04-13 03:09:58.000000 HTTP-PyServer-0.0.4/README.md
--rw-rw-rw-   0        0        0      641 2023-04-17 15:21:34.000000 HTTP-PyServer-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 15:25:24.244083 HTTP-PyServer-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.165295 HTTP-PyServer-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.219152 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2036 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-17 15:25:24.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.239095 HTTP-PyServer-0.0.4/src/server/
--rw-rw-rw-   0        0        0      191 2023-04-13 02:01:27.000000 HTTP-PyServer-0.0.4/src/server/__init__.py
--rw-rw-rw-   0        0        0     5364 2023-04-13 03:02:53.000000 HTTP-PyServer-0.0.4/src/server/render.py
--rw-rw-rw-   0        0        0     2347 2023-04-17 15:20:32.000000 HTTP-PyServer-0.0.4/src/server/request.py
--rw-rw-rw-   0        0        0     3930 2023-04-13 01:37:40.000000 HTTP-PyServer-0.0.4/src/server/responses.py
--rw-rw-rw-   0        0        0     3656 2023-04-13 02:47:16.000000 HTTP-PyServer-0.0.4/src/server/routes.py
--rw-rw-rw-   0        0        0     4387 2023-04-17 15:21:28.000000 HTTP-PyServer-0.0.4/src/server/server.py
+drwxrwxrwx   0        0        0        0 2023-05-01 16:48:57.704808 HTTP-PyServer-0.0.7/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2019 2023-05-01 16:48:57.703809 HTTP-PyServer-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-05-01 16:32:34.000000 HTTP-PyServer-0.0.7/README.md
+-rw-rw-rw-   0        0        0      641 2023-05-01 16:48:30.000000 HTTP-PyServer-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 16:48:57.704808 HTTP-PyServer-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 16:48:57.670125 HTTP-PyServer-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 16:48:57.684856 HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-05-01 16:48:57.000000 HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-05-01 16:48:57.000000 HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 16:48:57.000000 HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-01 16:48:57.000000 HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 16:48:57.701814 HTTP-PyServer-0.0.7/src/server/
+-rw-rw-rw-   0        0        0      318 2023-05-01 16:28:05.000000 HTTP-PyServer-0.0.7/src/server/__init__.py
+-rw-rw-rw-   0        0        0     5344 2023-04-30 04:44:01.000000 HTTP-PyServer-0.0.7/src/server/render.py
+-rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.0.7/src/server/request.py
+-rw-rw-rw-   0        0        0     2122 2023-05-01 16:34:09.000000 HTTP-PyServer-0.0.7/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.0.7/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.0.7/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     4265 2023-05-01 16:35:52.000000 HTTP-PyServer-0.0.7/src/server/routes.py
+-rw-rw-rw-   0        0        0     5690 2023-05-01 16:37:33.000000 HTTP-PyServer-0.0.7/src/server/server.py
```

### Comparing `HTTP-PyServer-0.0.4/LICENSE` & `HTTP-PyServer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.4/PKG-INFO` & `HTTP-PyServer-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.0.4
+Version: 0.0.7
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,41 +26,44 @@
 python -m pip install HTTP-PyServer
 ```
 
 # Simple Example
 
 ```
 # Saved as "main.py"
-from server import Routes, text, run
+import server
 
-@Routes.route(path = '/')
-def home(request):
+app = server.Server()
 
-    return text(text = 'Hello, world!')
+@app.route('/')
+def _(request):
 
-if __name__ == '__main__':
+    return 'Hello, world!'
 
-    run()
+with app:
+    
+    app.wait()
 ```
 
 ```
 $ python main.py
 Press enter to exit...
 
 ```
 
 # Contributing
 
 Look on github, and create a fork of HTTP-PyServer. Submit, pull requests, and any features will be looked at, and potentially implemented.
 
 # Used Packages
 
-Although, no external packages were used, the following packages were imported. All packages are native in Python 3.11.2. Not tested on any other versions, however it should work.
+Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
-- `sys`
+- `typing`
 - `logging`
 - `os`
+- `json`
 - `urllib`
 - `mimetypes`
 - `enum`
```

### Comparing `HTTP-PyServer-0.0.4/README.md` & `HTTP-PyServer-0.0.7/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: HTTP-PyServer
+Version: 0.0.7
+Summary: Simple way to make complex HTTP servers with python
+Author-email: Alex-Jando <alexjando2007@outlook.com>
+Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
+Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Project Description
 
 HTTP-PyServer is a simple, and extremly light-weight solution to create powerful projects relying on the web with few lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
 
 HTTP-PyServer is also very flexible on your project layout. It ensures security by allowing you to specify which files to send, and to where. HTTP-PyServer allows you to do everything you need whilst keeping hands relaxed with as few lines of code as possible.
 
 # Installing
@@ -12,41 +26,44 @@
 python -m pip install HTTP-PyServer
 ```
 
 # Simple Example
 
 ```
 # Saved as "main.py"
-from server import Routes, text, run
+import server
 
-@Routes.route(path = '/')
-def home(request):
+app = server.Server()
 
-    return text(text = 'Hello, world!')
+@app.route('/')
+def _(request):
 
-if __name__ == '__main__':
+    return 'Hello, world!'
 
-    run()
+with app:
+    
+    app.wait()
 ```
 
 ```
 $ python main.py
 Press enter to exit...
 
 ```
 
 # Contributing
 
 Look on github, and create a fork of HTTP-PyServer. Submit, pull requests, and any features will be looked at, and potentially implemented.
 
 # Used Packages
 
-Although, no external packages were used, the following packages were imported. All packages are native in Python 3.11.2. Not tested on any other versions, however it should work.
+Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
-- `sys`
+- `typing`
 - `logging`
 - `os`
+- `json`
 - `urllib`
 - `mimetypes`
-- `enum`
+- `enum`
```

### Comparing `HTTP-PyServer-0.0.4/pyproject.toml` & `HTTP-PyServer-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.0.4"
+version = "0.0.7"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.0.4/src/server/render.py` & `HTTP-PyServer-0.0.7/src/server/render.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,161 @@
 import mimetypes
 import os
 
-from . import responses
+from . import response_codes
 from . import request
-from . import routes
+from . import response
+from . import response_messages
 
-def _get_template(*args,
-                  data: bytes = '',
+def _get_template(data: bytes,
                   **template_vars) -> str:
     '''Replaces all template variables in a data with their values.
     Template variables are defined as {{var_name}},
     and are replaced with the value of var_name in template_vars.'''
     
     for var_name, var_value in template_vars.items():
 
         data = data.replace(f'{{{{{var_name}}}}}'.encode(encoding = 'utf-8',
                                                          errors = 'ignore'),
                             var_value.encode(encoding = 'utf-8',
                                              errors = 'ignore'))
 
     return data
 
-def text(*args,
-         text: str = '',
+def text(text: str,
+         *,
          filetype: str = 'txt',
-         code: int | responses.ResponseCodes = 200,
-         message: str | responses.ResponseMessages = 'OK',
-         ) -> bytes:
+         code: int | response_codes.ResponseCodes = 200,
+         message: str | response_messages.ResponseMessages = 'OK',
+         ) -> response.Response:
     '''Returns a text response. Use this to return plain text, JSON, XML, etc.'''
 
-    if type(code) == responses.ResponseCodes:
+    if type(code) == response_codes.ResponseCodes:
 
         code = code.value
 
-    if type(message) == responses.ResponseMessages:
+    if type(message) == response_messages.ResponseMessages:
 
         message = message.value
 
     text = text.encode(encoding = 'utf-8',
                        errors = 'ignore')
 
     headers = {
 
         'Content-Type': mimetypes.guess_type(f'file.{filetype.strip(".")}')[0],
 
         'Content-Length': str(len(text)),
 
     }
 
-    return (f'HTTP/1.1 {code} {message}\r\n'\
-            + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
-            .encode(encoding = 'utf-8',
-            errors = 'ignore') \
-            + b'\r\n\r\n' \
-            + text
+    return response.Response(version = 1.1,
+                             code = code,
+                             message = message,
+                             headers = headers,
+                             body = text)
 
-def file(*args,
-         filepath: str = '',
+def file(filepath: str,
+         *,
          request: request.Request = request.Request(),
          templated_vars: dict = {},
-         code: int | responses.ResponseCodes = 200,
-         message: str | responses.ResponseMessages = 'OK'
-         ) -> bytes:
+         code: int | response_codes.ResponseCodes = 200,
+         message: str | response_messages.ResponseMessages = 'OK'
+         ) -> response.Response:
     '''Returns a file as a response. Use this to return HTML, CSS, JS, images, etc.'''
 
-    if type(code) == responses.ResponseCodes:
+    if type(code) == response_codes.ResponseCodes:
 
         code = code.value
 
-    if type(message) == responses.ResponseMessages:
+    if type(message) == response_messages.ResponseMessages:
 
         message = message.value
 
     if not filepath or not os.path.exists(filepath):
 
-        return text(text = routes.Routes.get_route('/404',
-                                                   request = request),
-                    code = responses.ResponseCodes.NOT_FOUND,
-                    message = responses.ResponseMessages.NOT_FOUND)
+        raise FileNotFoundError(f'File not found: {filepath}')
             
     else:
 
         with open(filepath, 'rb') as file:
 
             data = file.read()
 
     if templated_vars:
 
         data = _get_template(data = data,
                              **templated_vars)
 
     headers = {
 
-        'Content-Type': mimetypes.guess_type(os.path.basename(filepath))[0]\
+        'Content-Type': mimetypes.guess_type(filepath)[0]\
                         or 'application/octet-stream',
 
         'Content-Length': str(len(data)),
 
     }
 
-    return (f'HTTP/1.1 {code} {message}\r\n' \
-            + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
-            .encode(encoding = 'utf-8',
-            errors = 'ignore') \
-            + b'\r\n\r\n' \
-            + data
+    return response.Response(version = 1.1,
+                             code = code,
+                             message = message,
+                             headers = headers,
+                             body = data)
 
-def redirect(*args,
-             url: str = '') -> bytes:
+def redirect(url: str) -> response.Response:
     '''Returns a redirect request to the specified URL.'''
 
     redirect_request = f'HTTP/1.1 301 See Other\
         \r\nLocation: {url}\
         \r\nContent-Type: text/html\
         \r\n\r\n\
         <html>\
             <head>\
                 <meta http-equiv="refresh" content="0;URL={url}" />\
             </head>\
         </html>'
 
-    return redirect_request.encode(encoding = 'utf-8',
-                                   errors = 'ignore')
+    return response.Response(version = 1.1,
+                             code = response_codes.ResponseCodes.SEE_OTHER,
+                             message = response_messages.ResponseMessages.SEE_OTHER,
+                             headers = {'Location': url,
+                                        'Content-Type': 'text/html',
+                                        'Content-Length': str(len(redirect_request))},
+                             body = redirect_request)
 
-def attachment(*args,
-               filepath: str = '',
+def attachment(filepath: str = '',
+               *,
                is_download: bool = False,
                is_text: bool = False,
                filename: str = '',
-               request: request.Request = request.Request()) -> bytes:
+               request: request.Request = request.Request()) -> response.Response:
     '''Returns a file as an attachment.
     Use this to return files for download or viewing.
     Sometimes browsers will preview text files, so you can use is_text
     to force the browser to display the raw text instead of previewing it.'''
 
     if not filepath or not os.path.exists(filepath):
 
-        return text(text = routes.Routes.get_route('/404',
-                                                   request = request),
-                    code = responses.ResponseCodes.NOT_FOUND,
-                    message = responses.ResponseMessages.NOT_FOUND)
+        raise FileNotFoundError(f'File not found: {filepath}')
 
     with open(filepath, 'rb') as f:
 
         data = f.read()
 
     headers = {
 
         'Content-Type': 'text/plain' if is_text else\
-                        mimetypes.guess_type(os.path.basename(filepath))[0]\
+                        mimetypes.guess_type(filepath)[0]\
                         or 'application/octet-stream',
 
         'Content-Length': str(len(data)),
 
         'Content-Disposition': ('attachment' if is_download else 'inline')\
-                                + f'; filename="{filename}"' if filename else ''
+                                + (f'; filename="{filename}"' if filename else '')
 
     }
 
-    return ('HTTP/1.1 200 OK\r\n' \
-            + '\r\n'.join([f'{key}: {value}' for key, value in headers.items()])) \
-            .encode(encoding = 'utf-8',
-            errors = 'ignore') \
-            + b'\r\n\r\n' \
-            + data
+    return response.Response(version = 1.1,
+                             code = response_codes.ResponseCodes.OK,
+                             message = response_messages.ResponseMessages.OK,
+                             headers = headers,
+                             body = data)
```

### Comparing `HTTP-PyServer-0.0.4/src/server/request.py` & `HTTP-PyServer-0.0.7/src/server/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import urllib
+import json
 
 class Request:
+    '''Represents an HTTP request.'''
 
     def __init__(self,
-                 *args,
+                 *,
                  address: tuple = (),
                  method: str = '',
                  path: str = '',
                  version: str = '',
                  headers: dict = {},
                  body: str = '',
-                 query: dict = {},
-                 values: dict = {}):
+                 query: dict = {}):
         '''Initializes the request class.'''
 
         self.address = address
 
         self.method = method
 
         self.path = path
@@ -24,16 +25,14 @@
 
         self.headers = headers
 
         self.body = body
 
         self.query = query
 
-        self.values = values
-
     @classmethod
     def from_string(cls,
                     *args,
                     address: tuple = (),
                     request: str):
         '''Creates a request object from an HTTP request string.'''
 
@@ -55,45 +54,46 @@
 
         query = urllib.parse.parse_qs(query)
 
         for key, value in query.items():
 
             query[key] = value[0]
 
-        headers = dict()
+        headers = {}
 
         for line in lines[1:]:
 
             if line == '':
 
                 break
 
             key, value = line.split(': ')
 
             headers[key] = value
 
         body = '\r\n'.join(lines[lines.index('') + 1:])
 
-        if method == 'POST':
-
-            values = dict()
-
-            for key, value in urllib.parse.parse_qs(body).items():
-
-                values[key] = value[0]
-
-            return cls(address = address,
-                       method = method,
-                       path = path,
-                       version = version,
-                       headers = headers,
-                       body = body,
-                       query = query,
-                       values = values)
-
         return cls(address = address,
                    method = method,
                    path = path,
                    version = version,
                    headers = headers,
                    body = body,
-                   query = query)
+                   query = query)
+    
+    def __str__(self):
+        '''Returns the request as an HTTP request string.'''
+
+        return f'{self.method} {self.path} {self.version}\r\n' + \
+'\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) + \
+'\r\n\r\n' + \
+self.body
+
+    def json(self):
+        '''Returns the request body as a JSON object.'''
+
+        return json.loads(self.body)
+    
+    def form(self):
+        '''Returns the request body as parsed urlencoded form data.'''
+
+        return urllib.parse.parse_qs(self.body)
```

