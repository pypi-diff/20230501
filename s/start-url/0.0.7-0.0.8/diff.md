# Comparing `tmp/start_url-0.0.7.tar.gz` & `tmp/start_url-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_url-0.0.7.tar", max compression
+gzip compressed data, was "start_url-0.0.8.tar", max compression
```

## Comparing `start_url-0.0.7.tar` & `start_url-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.7/README.md
--rw-r--r--   0        0        0     1558 2023-05-01 16:50:15.455095 start_url-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      152 2023-05-01 16:50:18.443961 start_url-0.0.7/start_url/__init__.py
--rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.7/start_url/headers.py
--rw-r--r--   0        0        0     1920 2023-05-01 16:47:18.833042 start_url-0.0.7/start_url/main.py
--rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.7/start_url/meta.py
--rw-r--r--   0        0        0     1050 2023-05-01 16:49:28.441557 start_url-0.0.7/start_url/url.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 start_url-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.8/README.md
+-rw-r--r--   0        0        0     1558 2023-05-01 17:05:15.282897 start_url-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-05-01 17:05:21.573489 start_url-0.0.8/start_url/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.8/start_url/headers.py
+-rw-r--r--   0        0        0     1871 2023-05-01 17:07:59.006241 start_url-0.0.8/start_url/main.py
+-rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.8/start_url/meta.py
+-rw-r--r--   0        0        0     1050 2023-05-01 16:49:28.441557 start_url-0.0.8/start_url/url.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 start_url-0.0.8/PKG-INFO
```

### Comparing `start_url-0.0.7/pyproject.toml` & `start_url-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-url"
 description = "httpx.get URL metadata with BeautifulSoup"
-version = "0.0.7"
+version = "0.0.8"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-url"
 documentation = "https://mv3.dev/start-url"
 classifiers = [
```

### Comparing `start_url-0.0.7/start_url/headers.py` & `start_url-0.0.8/start_url/headers.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.7/start_url/main.py` & `start_url-0.0.8/start_url/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,25 @@
 @dataclass
 class InspectedURL:
     url: str
     head: httpx.Headers | None = None
     content: bytes | None = None
 
     def __post_init__(self):
-        if not url(
-            value=self.url,  # type: ignore
-            may_have_port=False,
-            simple_host=True,
-            skip_ipv6_addr=True,
-            skip_ipv4_addr=True,
-        ):
+        if not url(self.url):  # type: ignore
             raise Exception(f"Invalid {self.url}")
         r = httpx.get(self.url, follow_redirects=True)
         if not r.status_code == HTTPStatus.OK:
             raise Exception(f"Bad {self.url}: {r.status_code}")
         self.head = r.headers
         self.content = r.content
 
+    def __repr__(self) -> str:
+        return f"{self.site_url.id['domain']=} {self.site_url.id['route']=}"
+
     @property
     def site_url(self) -> ParsedURL:
         """Wrapper over urlparse.ParsedResult to conform with headers / meta.
 
         Returns:
             ParsedURL: Fields are from urlparse.ParsedResult
         """
```

### Comparing `start_url-0.0.7/start_url/meta.py` & `start_url-0.0.8/start_url/meta.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.7/start_url/url.py` & `start_url-0.0.8/start_url/url.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.7/PKG-INFO` & `start_url-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-url
-Version: 0.0.7
+Version: 0.0.8
 Summary: httpx.get URL metadata with BeautifulSoup
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

