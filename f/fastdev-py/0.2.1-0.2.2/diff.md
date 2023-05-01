# Comparing `tmp/fastdev-py-0.2.1.tar.gz` & `tmp/fastdev-py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-py-0.2.1.tar", last modified: Sun Apr 30 15:05:41 2023, max compression
+gzip compressed data, was "fastdev-py-0.2.2.tar", last modified: Mon May  1 03:25:47 2023, max compression
```

## Comparing `fastdev-py-0.2.1.tar` & `fastdev-py-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      677 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      748 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/.github/workflows/pypitest-publish.yml
--rw-r--r--   0        0        0      856 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/.gitignore
--rw-r--r--   0        0        0       51 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/license.md
--rw-r--r--   0        0        0     1231 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      302 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/readme.md
--rw-r--r--   0        0        0      154 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/__init__.py
--rw-r--r--   0        0        0      584 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/__main__.py
--rw-r--r--   0        0        0    11496 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/builders/deno_lts_esbuild.ts
--rw-r--r--   0        0        0     1015 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/config.py
--rw-r--r--   0        0        0     1786 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/fs_serving.py
--rw-r--r--   0        0        0     8133 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/preprocessor/temp.py.bak
--rw-r--r--   0        0        0     2401 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/router.py
--rw-r--r--   0        0        0     1364 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/ts_serving.py
--rw-r--r--   0        0        0     1476 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/src/fastdev/utils.py
--rw-r--r--   0        0        0      313 2023-04-30 15:05:31.448341 fastdev-py-0.2.1/tests/1/hello.ts
--rw-r--r--   0        0        0       40 2023-04-30 15:05:31.452341 fastdev-py-0.2.1/tests/1/temp.ts
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      677 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      748 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.github/workflows/pypitest-publish.yml
+-rw-r--r--   0        0        0      856 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/.gitignore
+-rw-r--r--   0        0        0       51 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/license.md
+-rw-r--r--   0        0        0     1231 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/readme.md
+-rw-r--r--   0        0        0      154 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/__main__.py
+-rw-r--r--   0        0        0    11496 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/builders/deno_lts_esbuild.ts
+-rw-r--r--   0        0        0     1015 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/config.py
+-rw-r--r--   0        0        0     1848 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/fs_serving.py
+-rw-r--r--   0        0        0     8133 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/preprocessor/temp.py.bak
+-rw-r--r--   0        0        0     2508 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/router.py
+-rw-r--r--   0        0        0     1364 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/ts_serving.py
+-rw-r--r--   0        0        0     1463 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/src/fastdev/utils.py
+-rw-r--r--   0        0        0      313 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/tests/1/hello.ts
+-rw-r--r--   0        0        0       40 2023-05-01 03:25:34.935001 fastdev-py-0.2.2/tests/1/temp.ts
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 fastdev-py-0.2.2/PKG-INFO
```

### Comparing `fastdev-py-0.2.1/.github/workflows/pypi-publish.yml` & `fastdev-py-0.2.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/.github/workflows/pypitest-publish.yml` & `fastdev-py-0.2.2/.github/workflows/pypitest-publish.yml`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/.gitignore` & `fastdev-py-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/pyproject.toml` & `fastdev-py-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fastdev-py"
-version = "0.2.1"
+version = "0.2.2"
 description = "FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files."
 readme = "readme.md"
 requires-python = ">=3.11"
 license = { file = "license.md" }
 authors = [{ name = "Omar Azmi" }]
 dependencies = ["fastapi"]
 keywords = [
```

### Comparing `fastdev-py-0.2.1/src/fastdev/__main__.py` & `fastdev-py-0.2.2/src/fastdev/__main__.py`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/src/fastdev/builders/deno_lts_esbuild.ts` & `fastdev-py-0.2.2/src/fastdev/builders/deno_lts_esbuild.ts`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/src/fastdev/config.py` & `fastdev-py-0.2.2/src/fastdev/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import mimetypes
 from pathlib import Path
 
-Port: int = 8000 
-ModDir: Path = Path(__file__).absolute().parent # this module's root directory
+Port: int = 8000
+ModDir: Path = Path(__file__).absolute().parent  # this module's root directory
 SWD: Path = Path.cwd()  # current working directory is where the server was invoked
 ESBuildConfig = {
 	"path": "./path/to/script.ts",
 	"config": {"minify": False},
 	"plugins": ["solid"],
 	"plugins_config": dict(),
 }
```

### Comparing `fastdev-py-0.2.1/src/fastdev/fs_serving.py` & `fastdev-py-0.2.2/src/fastdev/fs_serving.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 	directory_index = directory.joinpath("./index.html")
 	if directory_index.is_file():
 		index_html_url = "/" + str(directory_index.relative_to(SWD).as_posix())
 		print(f"index.html found. redirecting to:\n\t{index_html_url}")
 		return RedirectResponse(index_html_url)
 	dir_head = directory.relative_to(SWD)
 	dir_links: dict[str, str] = dict()  # key: href_path, value: title
-	dir_links[".."] = "./.."
+	dir_links["./.."] = ".."
 	for subpath in directory.iterdir():
 		rel_subpath = subpath.relative_to(directory)
-		href = str(rel_subpath)
-		title = href + ("" if subpath.is_file() else "/")
+		prefix = "./"
+		suffix = "" if subpath.is_file() else "/"
+		href = prefix + str(rel_subpath) + suffix
+		title = str(rel_subpath) + suffix
 		dir_links[href] = title
 	dir_links_html_li: list[str] = [f"""
 	<li><a href={qoute(href)}>{title}</a></li>
 	""" for href, title in dir_links.items()]
 	html = f"""
 	<html lang="en">
 	<head>
```

#### html2text {}

```diff
@@ -8,18 +8,19 @@
 media_type=mime) """ return FileResponse(file) async def serve_dir(directory:
 Path): if not directory.is_dir(): return PlainTextResponse( f"the following
 directory was not found:\n\t{directory}", status_code=404 ) directory_index =
 directory.joinpath("./index.html") if directory_index.is_file(): index_html_url
 = "/" + str(directory_index.relative_to(SWD).as_posix()) print(f"index.html
 found. redirecting to:\n\t{index_html_url}") return RedirectResponse
 (index_html_url) dir_head = directory.relative_to(SWD) dir_links: dict[str,
-str] = dict() # key: href_path, value: title dir_links[".."] = "./.." for
+str] = dict() # key: href_path, value: title dir_links["./.."] = ".." for
 subpath in directory.iterdir(): rel_subpath = subpath.relative_to(directory)
-href = str(rel_subpath) title = href + ("" if subpath.is_file() else "/")
-dir_links[href] = title dir_links_html_li: list[str] = [f"""
+prefix = "./" suffix = "" if subpath.is_file() else "/" href = prefix + str
+(rel_subpath) + suffix title = str(rel_subpath) + suffix dir_links[href] =
+title dir_links_html_li: list[str] = [f"""
 {title}
 """ for href, title in dir_links.items()] html = f"""
 ****** Directory listing for: {qoute(dir_head)} ******
 ===============================================================================
     * {"".join(dir_links_html_li)}
 ===============================================================================
 """ return HTMLResponse(html)
```

### Comparing `fastdev-py-0.2.1/src/fastdev/preprocessor/temp.py.bak` & `fastdev-py-0.2.2/src/fastdev/preprocessor/temp.py.bak`

 * *Files identical despite different names*

### Comparing `fastdev-py-0.2.1/src/fastdev/router.py` & `fastdev-py-0.2.2/src/fastdev/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Type, TypeVar
 from fastapi import APIRouter, FastAPI, Request, Response
-from fastapi.responses import PlainTextResponse
+from fastapi.responses import PlainTextResponse, RedirectResponse
 from .config import SWD
 from .fs_serving import serve_dir, serve_file
 from .ts_serving import (
 	build_server_callback_path, build_server_loaded_promise, serve_ts,
 )
 
 APP_OR_ROUTER = TypeVar("APP_OR_ROUTER", FastAPI, APIRouter)
@@ -49,15 +49,17 @@
 async def route_path(path: str):
 	abspath = SWD.joinpath(path)
 	if not abspath.exists():
 		return Response(status_code=404)
 	elif abspath.is_file():
 		return await serve_file(abspath)
 	elif abspath.is_dir():
-		return await serve_dir(abspath)
+		if path.endswith("/") or SWD.samefile(abspath):
+			return await serve_dir(abspath)
+		return RedirectResponse(path + "/")
 	else:
 		return PlainTextResponse(
 			f"the following request was uncaught by main router:\n\t{path}",
 			status_code=500
 		)
```

### Comparing `fastdev-py-0.2.1/src/fastdev/ts_serving.py` & `fastdev-py-0.2.2/src/fastdev/ts_serving.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asyncio import Future
 from subprocess import Popen
 from urllib.parse import urljoin
-from fastapi.responses import Response, PlainTextResponse
-from .config import SWD, Port, ModDir, ESBuildConfig
-from .utils import qoute, post_data
+from fastapi.responses import PlainTextResponse, Response
+from .config import SWD, ESBuildConfig, ModDir, Port
+from .utils import post_data, qoute
 
 BUILD_SERVER_PORT = 3000  # the port on which `deno_lts_esbuild.ts` listens for build requests
 build_server_loaded_promise = Future()
 build_server_path = ModDir.joinpath("./builders/deno_lts_esbuild.ts")
 build_server_callback_path = "/build_server_loaded"
 build_server_callback = f"http://localhost:{Port}{build_server_callback_path}"
 build_server_url = f"http://localhost:{BUILD_SERVER_PORT}"
```

### Comparing `fastdev-py-0.2.1/src/fastdev/utils.py` & `fastdev-py-0.2.2/src/fastdev/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import json
-from typing import Annotated, TypedDict, Optional, Literal
-from urllib.request import Request as urlRequest, urlopen
-from asyncio import gather, Future, run as async_run
+from typing import Annotated, Literal, Optional, TypedDict
+from urllib.request import Request, urlopen
 
 HTTPHeader = TypedDict("HTTPHeader", {
 	"content-type": Optional[Annotated[str, "mimetype"]],
 	"accept": Optional[Annotated[str, "accepted mimetype"]],
 })
 HTTPMethod = Literal["GET", "POST", "PUT", "DELETE"]
 HTTPResponse = TypedDict("HTTPResponse", {
-	"status_code": int,
 	"content": Optional[bytes],
+	"status_code": int,
 })
 HTTPResponseText = TypedDict("HTTPResponseText", {
-	"status_code": int,
 	"content": Optional[str],
+	"status_code": int,
 })
 
 
 def qoute(string: str | object) -> str:
 	if not isinstance(string, str):
 		string = str(string)
 	return "\"" + string + "\""
@@ -28,29 +27,32 @@
 	url: str,
 	content: bytes,
 	timeout=10_000,
 	*,
 	method: HTTPMethod = "GET",
 	headers: HTTPHeader = dict()
 ) -> HTTPResponse:
-	with urlopen(urlRequest(url, content, headers=headers, method=method), timeout=timeout) as response:
-		return {
-			"status_code": response.getcode(),
-			"content": response.read(),
-		}
+	with urlopen(Request(url, content, headers=headers, method=method), timeout=timeout) as response:
+		return HTTPResponse(
+			content=response.read(),
+			status_code=response.getcode(),
+		)
 
 
 def post_data(
 	url: str,
 	data: dict | list,
 	timeout=10_000,
 	*,
 	method: HTTPMethod = "POST",
 	headers: HTTPHeader = {"content-type": "application/json"}
 ) -> HTTPResponseText | None:
 	try:
 		response = fetch(url, json.dumps(data).encode("utf-8"), timeout, method=method, headers=headers)
-		if response["content"] is not None:
-			response["content"] = response["content"].decode("utf-8")
-		return response
+		if response["content"] is None:
+			return None
+		return HTTPResponseText(
+			content=response["content"].decode("utf-8"),
+			status_code=response["status_code"],
+		)
 	except:
 		return None
```

### Comparing `fastdev-py-0.2.1/PKG-INFO` & `fastdev-py-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdev-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: FastAPI development server that JIT preprocess TS, TSX, SCSS, etc... files.
 Keywords: devserver,dev-server,devtools,sever,liveserver,live-server
 Author: Omar Azmi
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Project-URL: Homepage, https://github.com/omar-azmi/fastdev_py
```

