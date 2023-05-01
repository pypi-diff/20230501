# Comparing `tmp/start_url-0.0.3.tar.gz` & `tmp/start_url-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_url-0.0.3.tar", max compression
+gzip compressed data, was "start_url-0.0.4.tar", max compression
```

## Comparing `start_url-0.0.3.tar` & `start_url-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.3/README.md
--rw-r--r--   0        0        0     1559 2023-04-30 15:36:47.331278 start_url-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      152 2023-04-30 15:31:07.695931 start_url-0.0.3/start_url/__init__.py
--rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.3/start_url/headers.py
--rw-r--r--   0        0        0     2001 2023-04-30 15:30:53.449715 start_url-0.0.3/start_url/main.py
--rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.3/start_url/meta.py
--rw-r--r--   0        0        0     2030 2023-04-30 13:19:26.255355 start_url-0.0.3/start_url/repo.py
--rw-r--r--   0        0        0      596 2023-04-30 15:25:08.484611 start_url-0.0.3/start_url/url.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 start_url-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      241 2023-04-30 13:19:26.253134 start_url-0.0.4/README.md
+-rw-r--r--   0        0        0     1559 2023-05-01 04:36:42.312109 start_url-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-05-01 04:34:26.114367 start_url-0.0.4/start_url/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-30 13:19:26.255016 start_url-0.0.4/start_url/headers.py
+-rw-r--r--   0        0        0     2098 2023-05-01 04:36:02.631836 start_url-0.0.4/start_url/main.py
+-rw-r--r--   0        0        0     3630 2023-04-30 13:19:26.255251 start_url-0.0.4/start_url/meta.py
+-rw-r--r--   0        0        0      596 2023-04-30 15:25:08.484611 start_url-0.0.4/start_url/url.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 start_url-0.0.4/PKG-INFO
```

### Comparing `start_url-0.0.3/pyproject.toml` & `start_url-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-url"
 description = "httpx.get URL metadata with BeautifulSoup"
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-url"
 documentation = "https://mv3.dev/start-url"
 classifiers = [
```

### Comparing `start_url-0.0.3/start_url/headers.py` & `start_url-0.0.4/start_url/headers.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.3/start_url/main.py` & `start_url-0.0.4/start_url/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import asdict, dataclass
 from http import HTTPStatus
+from typing import Any
 
 import httpx
 from bs4 import BeautifulSoup
 
 from .headers import SimpleResponseHeaders
 from .meta import SimpleMeta
-from .repo import GithubRepo
 from .url import ParsedURL
 
 
 @dataclass
 class InspectedURL:
     url: str
     head: httpx.Headers | None = None
@@ -19,43 +19,50 @@
     def __post_init__(self):
         r = httpx.get(self.url, follow_redirects=True)
         if not r.status_code == HTTPStatus.OK:
             raise Exception(f"Bad {self.url}: {r.status_code}")
         self.head = r.headers
         self.content = r.content
 
-    def prep(self, dc) -> dict:
-        """Must be a dataclass."""
-        return {dc.__class__.__name__: asdict(dc)} if dc is not None else {}
-
     @property
     def site_url(self) -> ParsedURL:
-        """Generates the parts of urlparse.ParsedResult as a dictionary."""
+        """Wrapper over urlparse.ParsedResult to conform with headers / meta.
+
+        Returns:
+            ParsedURL: Fields are from urlparse.ParsedResult
+        """
         return ParsedURL.from_url(url=self.url)
 
     @property
     def site_headers(self) -> SimpleResponseHeaders | None:
-        """Selected HTML headers, requires content-type to include `text/html`."""
+        """After an http request is made from the inspected url, extract selected
+        response headers. Requires content-type to include `text/html`.
+
+        Returns:
+            SimpleResponseHeaders | None: _description_
+        """
         if self.head:
             return SimpleResponseHeaders.from_raw_headers(data=self.head)
 
     @property
     def site_meta(self) -> SimpleMeta | None:
-        """Simplified summary of meta tags."""
-        if self.content:
-            html_soup = BeautifulSoup(self.content, "html.parser")
-            return SimpleMeta.from_soup(html_soup)
+        """Based on content of the url requested, extract meta tags.
 
-    @property
-    def repo_meta(self) -> GithubRepo | None:
-        """Usable fields from Github repository, requires Github token."""
-        if raw_data := GithubRepo.matches(self.url):
-            return GithubRepo(**raw_data)
-
-    @property
-    def export(self):
-        """Combine url, header, meta, repo key-value pairs."""
-        data = self.prep(self.site_url)
-        head = self.prep(self.site_headers) or {}
-        meta = self.prep(self.site_meta) or {}
-        repo = self.prep(self.repo_meta) or {}
-        return data | head | meta | repo
+        Returns:
+            SimpleMeta | None: e.g. title, author, meta tags from html page.
+        """
+        if self.content:
+            return SimpleMeta.from_soup(
+                BeautifulSoup(self.content, "html.parser")
+            )
+
+    def convert(self) -> dict[str, Any]:
+        """Convert url, header, meta dataclasses key-value into a single dict.
+
+        Returns:
+            dict[str, Any]: Compiled dict of dataclasses, each key is a classname
+        """
+        data = {}
+        for dc in [self.site_url, self.site_headers, self.site_meta]:
+            if dc is not None:
+                data[dc.__class__.__name__] = asdict(dc)
+        return data
```

### Comparing `start_url-0.0.3/start_url/meta.py` & `start_url-0.0.4/start_url/meta.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.3/start_url/url.py` & `start_url-0.0.4/start_url/url.py`

 * *Files identical despite different names*

### Comparing `start_url-0.0.3/PKG-INFO` & `start_url-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-url
-Version: 0.0.3
+Version: 0.0.4
 Summary: httpx.get URL metadata with BeautifulSoup
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

