# Comparing `tmp/amarps-0.18.0.tar.gz` & `tmp/amarps-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarps-0.18.0.tar", max compression
+gzip compressed data, was "amarps-0.19.0.tar", max compression
```

## Comparing `amarps-0.18.0.tar` & `amarps-0.19.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3286 2023-04-17 21:27:27.368943 amarps-0.18.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-04-17 21:27:27.368943 amarps-0.18.0/LICENSE
--rw-r--r--   0        0        0     1001 2023-04-17 21:27:27.368943 amarps-0.18.0/README.md
--rw-r--r--   0        0        0     1111 2023-04-17 21:27:27.368943 amarps-0.18.0/pyproject.toml
--rw-r--r--   0        0        0       79 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/__init__.py
--rw-r--r--   0        0        0       32 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/__main__.py
--rw-r--r--   0        0        0     3466 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/main.py
--rw-r--r--   0        0        0     1314 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/profile_page_selectors.yml
--rw-r--r--   0        0        0     1044 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/review_page_selectors.yml
--rw-r--r--   0        0        0    10807 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/scraper.py
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 amarps-0.18.0/setup.py
--rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 amarps-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0     3684 2023-05-01 20:21:39.207119 amarps-0.19.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-05-01 20:21:39.207119 amarps-0.19.0/LICENSE
+-rw-r--r--   0        0        0     1001 2023-05-01 20:21:39.207119 amarps-0.19.0/README.md
+-rw-r--r--   0        0        0     1111 2023-05-01 20:21:39.207119 amarps-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/__main__.py
+-rw-r--r--   0        0        0      476 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/events.py
+-rw-r--r--   0        0        0     3771 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/main.py
+-rw-r--r--   0        0        0     1314 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/profile_page_selectors.yml
+-rw-r--r--   0        0        0     1044 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/review_page_selectors.yml
+-rw-r--r--   0        0        0    11142 2023-05-01 20:21:39.207119 amarps-0.19.0/src/amarps/scraper.py
+-rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 amarps-0.19.0/PKG-INFO
```

### Comparing `amarps-0.18.0/CHANGELOG.md` & `amarps-0.19.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+## v0.19.0 (2023-05-01)
+
+### Feat
+
+- Allow to stop waiting with SIGINT
+- Delete all cookies before each request
+- **log**: Improve wording
+- **log**: Improve wording
+- Abort early when error occurs
+- **log**: Log when HTTP status code is checked
+- **log**: Log when html page will be saved
+- Log CLI options and arguments
+
+### Fix
+
+- Fix bug
+
+### Refactor
+
+- Make typing information more specific
+
 ## v0.18.0 (2023-04-17)
 
 ### Feat
 
 - Sleep shortly after scrolling
 - Increase scrolling and make it configurable
 - Add debug log initializing browser
```

### Comparing `amarps-0.18.0/LICENSE` & `amarps-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amarps-0.18.0/README.md` & `amarps-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `amarps-0.18.0/pyproject.toml` & `amarps-0.19.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Joris Clement <joclement@posteo.net>"]
 description = "Download amazon product reviews and the reviewers profile information"
 license = "MIT"
 name = "amarps"
 readme = "README.md"
 repository = "https://github.com/joclement/amarps"
-version = "0.18.0"
+version = "0.19.0"
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click= "^8"
 selectorlib = "~0.16"
 selenium = "^4"
@@ -23,27 +23,27 @@
 pytest = "^7"
 pytest-cov = "^4"
 pytest-httpserver = "^1"
 pytest-random-order = "^1"
 pytest-rerunfailures = "^11"
 pytest-xdist = "^3"
 flake8 = {version = "^6", python = ">=3.8.1"}
-mypy = ">=0.931,<=1.1.1"
+mypy = ">=0.931,<=1.2.0"
 flake8-import-order = "^0.18"
 
 [tool.poetry.scripts]
 amarps = "amarps.main:main"
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 85
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.18.0"
+version = "0.19.0"
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `amarps-0.18.0/src/amarps/main.py` & `amarps-0.19.0/src/amarps/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import json
+import logging
 import sys
-from typing import Any, Dict, Optional
+from typing import Dict, Optional
 
 import click
 import click_log
 
 from . import __version__
 from .scraper import (
     BROWSER,
     HAVE_BROWSER_HEADLESS,
-    logger,
+    logger as scrapper_logger,
     Scraper,
     SCROLL_DEPTH_PROFILE_PAGE,
     SCROLL_DEPTH_REVIEWS_PAGE,
 )
 
+main_logger = logging.getLogger(__name__)
 
-click_log.basic_config(logger)
+click_log.basic_config(scrapper_logger)
+click_log.basic_config(main_logger)
 
 
-def _get_command_parameters() -> Dict[str, Any]:
-    params = click.get_current_context().params
-    params["output"] = str(params["output"])
-    return params
+def _get_command_parameters() -> Dict[str, str]:
+    return {k: str(v) for k, v in click.get_current_context().params.items()}
 
 
 @click.command()
-@click_log.simple_verbosity_option(logger, show_default=True)
+@click_log.simple_verbosity_option(scrapper_logger, show_default=True)
+@click_log.simple_verbosity_option(main_logger, show_default=True)
 @click.version_option(version=__version__)
 @click.argument(
     "link",
     type=str,
 )
 @click.option(
     "--profiles/--no-profiles",
@@ -86,15 +88,18 @@
     "have_browser_headless",
     help="Run browser in background making it more easily detectable as a web scraper",
     default=HAVE_BROWSER_HEADLESS,
     show_default=True,
 )
 @click.option(
     "--sleep-time",
-    help="Time to wait for user input when the 1st request fails",
+    help=(
+        "Time to wait for user input when the 1st request fails, "
+        "use SIGINT to interrupt the waiting"
+    ),
     type=int,
     default=60,
     show_default=True,
 )
 @click.option(
     "--scroll-depth-profile",
     help="Scroll depth for the profile pages",
@@ -126,14 +131,15 @@
     """Download amazon product reviews and reviewers profile information
 
     LINK is an URL to the reviews of an amazon product or to an amazon profile.
     Link must be of the form 'https://www.amazon.com/product-reviews/ID123ABC/' and
     must end with a '/'."
     """
     data = {"python_command_parameters": _get_command_parameters()}
+    main_logger.debug(f"command parameters: {data['python_command_parameters']}")
 
     arr = Scraper(
         html_page,
         browser,
         have_browser_headless,
         scroll_depth_profile,
         scroll_depth_reviews,
```

### Comparing `amarps-0.18.0/src/amarps/profile_page_selectors.yml` & `amarps-0.19.0/src/amarps/profile_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.18.0/src/amarps/review_page_selectors.yml` & `amarps-0.19.0/src/amarps/review_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.18.0/src/amarps/scraper.py` & `amarps-0.19.0/src/amarps/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from click import File
 import dateparser
 import requests
 from selectorlib import Extractor
 from selectorlib.formatter import Formatter
 from seleniumwire import webdriver
 
+from .events import WaitHandler
+
 
 BROWSER: Final = "chrome"
 HAVE_BROWSER_HEADLESS: Final = False
 SCROLL_DEPTH_PROFILE_PAGE: Final = 2000
 SCROLL_DEPTH_REVIEWS_PAGE: Final = 2000
 
 
@@ -227,24 +229,27 @@
             logger.warning("Failed to get HTTP status code")
 
     def _get_html_data(
         self, url: str, scroll_depth: int, check_status: bool = True
     ) -> str:
         logger.info(f"Download {url}")
 
+        self._webdriver.delete_all_cookies()
         self._webdriver.get(url)
         self._webdriver.execute_script(f"window.scrollTo(0,{scroll_depth})")
 
         sleep(random.random())
 
         html_page = self._webdriver.page_source
         if self._html_page_writer is not None:
+            logger.debug("Write HTML page")
             self._html_page_writer.write(html_page)
 
         if check_status:
+            logger.debug("Check HTTP status")
             self._raise_for_status()
 
         return html_page
 
     def _get_data(self, url: str) -> Dict[str, Any]:
         return self._review_extractor.extract(
             self._get_html_data(url, self.scroll_depth_reviews_page), base_url=url
@@ -314,26 +319,30 @@
 
     def extract(
         self,
         base_url: str,
         download_profiles: bool,
         start_page: int,
         stop_page: Optional[int],
-        sleep_time: int,
+        wait_time: int,
     ) -> Dict[str, Any]:
         data = self._get_data(_get_page_url(base_url, start_page))
 
         if data["reviews"] is None or len(data["reviews"]) == 0:
-            logger.warning("Failed to extract review data")
-            if not self.have_browser_headless:
-                logger.warning(
-                    f"The query will be retried in {sleep_time} seconds, "
-                    "please try to solve a CAPTCHA or login if possible"
+            logger.error("Failed to extract review data on 1st attempt")
+            if self.have_browser_headless:
+                raise RuntimeError(
+                    "Browser is headless: there is no way to solve a CAPTCHA or login"
                 )
-                sleep(sleep_time)
-                data = self._get_data(_get_page_url(base_url, start_page))
+
+            logger.warning(
+                f"The query will be retried after {wait_time} seconds or when SIGINT "
+                "is signaled, please try to solve a CAPTCHA or login if possible"
+            )
+            WaitHandler().wait(wait_time)
+            data = self._get_data(_get_page_url(base_url, start_page))
 
         data["reviews"] = self._get_reviews(
             base_url, data, start_page, stop_page, download_profiles
         )
 
         return data
```

### Comparing `amarps-0.18.0/PKG-INFO` & `amarps-0.19.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarps
-Version: 0.18.0
+Version: 0.19.0
 Summary: Download amazon product reviews and the reviewers profile information
 Home-page: https://github.com/joclement/amarps
 License: MIT
 Author: Joris Clement
 Author-email: joclement@posteo.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

