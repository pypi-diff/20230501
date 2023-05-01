# Comparing `tmp/rssfixer-0.1.5.tar.gz` & `tmp/rssfixer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.1.5.tar", last modified: Fri Apr 28 10:54:14 2023, max compression
+gzip compressed data, was "rssfixer-0.1.6.tar", max compression
```

## Comparing `rssfixer-0.1.5.tar` & `rssfixer-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,6 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-28 10:54:14.688472 rssfixer-0.1.5/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.5/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)    11309 2023-04-28 10:54:14.688210 rssfixer-0.1.5/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)    10483 2023-04-28 10:38:40.000000 rssfixer-0.1.5/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1162 2023-04-28 10:11:12.000000 rssfixer-0.1.5/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-28 10:54:14.688537 rssfixer-0.1.5/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-28 10:54:14.683383 rssfixer-0.1.5/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-28 10:54:14.684821 rssfixer-0.1.5/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.5/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)    12428 2023-04-28 02:57:35.000000 rssfixer-0.1.5/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-28 10:54:14.686193 rssfixer-0.1.5/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)    11309 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      415 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      249 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-28 10:54:14.000000 rssfixer-0.1.5/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-28 10:54:14.687643 rssfixer-0.1.5/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)    14680 2023-04-26 16:32:08.000000 rssfixer-0.1.5/src/tests/test_rss.py
--rw-r--r--   0 reuteras   (501) staff       (20)     4983 2023-04-28 02:57:35.000000 rssfixer-0.1.5/src/tests/test_rss_args.py
--rw-r--r--   0 reuteras   (501) staff       (20)     2236 2023-04-28 02:57:35.000000 rssfixer-0.1.5/src/tests/test_rss_extract_links_release.py
--rw-r--r--   0 reuteras   (501) staff       (20)     1980 2023-04-26 16:34:02.000000 rssfixer-0.1.5/src/tests/test_rss_main.py
+-rw-r--r--   0        0        0     1059 2023-04-30 11:20:03.145292 rssfixer-0.1.6/LICENSE
+-rw-r--r--   0        0        0    10493 2023-05-01 06:44:43.555449 rssfixer-0.1.6/README.md
+-rw-r--r--   0        0        0     2865 2023-05-01 06:42:19.258554 rssfixer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-30 07:34:12.316893 rssfixer-0.1.6/src/rssfixer/__init__.py
+-rw-r--r--   0        0        0    12914 2023-04-30 11:38:07.420585 rssfixer-0.1.6/src/rssfixer/rss.py
+-rw-r--r--   0        0        0    11143 1970-01-01 00:00:00.000000 rssfixer-0.1.6/PKG-INFO
```

### Comparing `rssfixer-0.1.5/LICENSE` & `rssfixer-0.1.6/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `rssfixer-0.1.5/PKG-INFO` & `rssfixer-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.1.5
-Summary: Generate RSS feed for Wordpress blog without it.
-Author-email: Peter Reuterås <peter@reuteras.net>
-Project-URL: Homepage, https://github.com/reuteras/rssfixer
-Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
-Classifier: Programming Language :: Python :: 3
+Version: 0.1.6
+Summary: Generate RSS for blogs without a feed.
+License: MIT
+Author: Peter Reuterås
+Author-email: peter@reuteras.net
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Information Technology
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (==4.12.2)
+Requires-Dist: feedgen (==0.9.0)
+Requires-Dist: requests (==2.29.0)
 Description-Content-Type: text/markdown
-Provides-Extra: audit
-Provides-Extra: build
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: github
-Provides-Extra: dev
-License-File: LICENSE
 
 # rssfixer
 
 <!-- CODE:BASH:START -->
 <!-- echo '[![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)' -->
 <!-- echo '![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)' -->
 <!-- echo '[![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)' -->
@@ -112,15 +107,14 @@
 
 Pages with a more general HTML structure can be parsed with the `--html` option. You can specify the HTML tag for the entries, the URL and title of the blog entry.
 
 An example for [tripwire.com][tri]:
 
 ```bash
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
-
 ```
 
 ### Release
 
 Check for one entity on release pages like [SQLite][sql] (h3) and generate RSS feed with links to the download page (required argument `--release-url`). Easy way to get notified when a new version is released.
 
 ```bash
@@ -129,15 +123,15 @@
 
 ### Usage
 
 Command-line options (updated on commit by [markdown-code-runner][mcr]):
 
 <!-- CODE:BASH:START -->
 <!-- echo '```Text' -->
-<!-- rssfixer --help -->
+<!-- poetry run rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
 usage: rssfixer [-h] (--html | --json | --list | --release) [--version]
@@ -237,7 +231,8 @@
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
   [sql]: https://sqlite.org/changes.html
   [sue]: https://github.com/reuteras/rssfixer/discussions/categories/show-usage-examples
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
   [wor]: https://wordpress.org/
+
```

### Comparing `rssfixer-0.1.5/README.md` & `rssfixer-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
 Pages with a more general HTML structure can be parsed with the `--html` option. You can specify the HTML tag for the entries, the URL and title of the blog entry.
 
 An example for [tripwire.com][tri]:
 
 ```bash
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
-
 ```
 
 ### Release
 
 Check for one entity on release pages like [SQLite][sql] (h3) and generate RSS feed with links to the download page (required argument `--release-url`). Easy way to get notified when a new version is released.
 
 ```bash
@@ -105,15 +104,15 @@
 
 ### Usage
 
 Command-line options (updated on commit by [markdown-code-runner][mcr]):
 
 <!-- CODE:BASH:START -->
 <!-- echo '```Text' -->
-<!-- rssfixer --help -->
+<!-- poetry run rssfixer --help -->
 <!-- echo '```' -->
 <!-- CODE:END -->
 
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
 usage: rssfixer [-h] (--html | --json | --list | --release) [--version]
```

### Comparing `rssfixer-0.1.5/src/rssfixer/rss.py` & `rssfixer-0.1.6/src/rssfixer/rss.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 """Generate rss feed for "blogs" without rss feed."""
 import argparse
 import hashlib
 import importlib.metadata
 import json
 import re
 import sys
+from pathlib import Path
 
 import requests
 from bs4 import BeautifulSoup
 from feedgen.feed import FeedGenerator
 
 try:
     __version__ = "version " + importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "0.0.0"
 
 
 class CheckHtmlAction(argparse.Action):
+    """Class to validate argparse for --html options."""
+
     def __call__(self, parser, namespace, values, option_string=None):
+        """Validate the class."""
         if not namespace.html:
             parser.error(f"{option_string} requires --html to be specified.")
         setattr(namespace, self.dest, values)
 
 
 class CheckJsonAction(argparse.Action):
+    """Class to validate argparse for --json options."""
+
     def __call__(self, parser, namespace, values, option_string=None):
+        """Validate the class."""
         if not namespace.json:
             parser.error(f"{option_string} requires --json to be specified.")
         setattr(namespace, self.dest, values)
 
 
 class CheckReleaseAction(argparse.Action):
+    """Class to validate argparse for --release options."""
+
     def __call__(self, parser, namespace, values, option_string=None):
+        """Validate the class."""
         if not namespace.release:
             parser.error(f"{option_string} requires --release to be specified.")
         setattr(namespace, self.dest, values)
 
 
 def fetch_html(url):
     """Fetch HTML content from a URL."""
@@ -100,22 +110,24 @@
     unique_links = set()
 
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.html_entries):
         try:
             url = entry.findNext(arguments.html_url)["href"]
             title = entry.find(
-                arguments.html_title, re.compile(arguments.html_title_class)
+                arguments.html_title,
+                re.compile(arguments.html_title_class),
             ).text.strip()
         except (KeyError, AttributeError):
             print("ERROR: Unable to find URL or title in HTML element")
             sys.exit(1)
         try:
             description = entry.find(
-                arguments.html_description, re.compile(arguments.html_description_class)
+                arguments.html_description,
+                re.compile(arguments.html_description_class),
             ).text.strip()
         except (KeyError, AttributeError):
             # Ignore description if it's not found
             description = ""
         if url not in unique_links:
             unique_links.add(url)
             links.append((url, title, description))
@@ -168,15 +180,15 @@
     links = []
     unique_titles = set()
 
     # Iterate through all the elements of type html_entries in the page
     for entry in soup.find_all(arguments.release_entries):
         try:
             title = entry.text.strip()
-            if title == "":
+            if not title:
                 raise AttributeError
             title_bytes = title.encode("utf-8")
             title_hash = hashlib.sha256(title_bytes)
             title_sha256 = title_hash.hexdigest()
             url = arguments.release_url + "?" + title_sha256
         except (KeyError, AttributeError):
             print("ERROR: Unable to title in HTML element")
@@ -201,20 +213,22 @@
     fg.id(arguments.url)
     fg.title(arguments.title)
     fg.description(feed_description)
     fg.link(href=arguments.url, rel="alternate")
 
     # Add entries to the RSS feed
     for url, title, description in links:
-        if arguments.base_url:
-            url = arguments.base_url + url
         fe = fg.add_entry()
-        fe.id(url)
+        if arguments.base_url:
+            fe.link(href=arguments.base_url + url)
+            fe.id(arguments.base_url + url)
+        else:
+            fe.link(href=url)
+            fe.id(url)
         fe.title(title)
-        fe.link(href=url)
         if vars(arguments).get("atom", False):
             fe.summary(description)
             fe.content(content=description, src=url)
         else:
             fe.description(description)
 
     if vars(arguments).get("atom", False):
@@ -223,49 +237,56 @@
 
 
 def parse_arguments(arguments):
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description="""Generate RSS feed for blog that don't publish a feed.
         Default is to find links in a simple <ul>-list.
-        Options are available to find links in other HTML elements or JSON strings."""
+        Options are available to find links in other HTML elements or JSON strings.""",
     )
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("--html", action="store_true", help="Find entries in HTML")
     group.add_argument("--json", action="store_true", help="Find entries in JSON")
     group.add_argument(
-        "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
+        "--list",
+        action="store_true",
+        help="Find entries in HTML <ul>-list (default)",
     )
     group.add_argument("--release", action="store_true", help="Find releases in HTML")
 
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
     parser.add_argument("url", help="URL for the blog")
     parser.add_argument("--atom", action="store_true", help="Generate Atom feed")
     parser.add_argument("--base-url", help="Base URL for the blog")
     parser.add_argument(
-        "--release-url", action=CheckReleaseAction, help="Release URL for downloads"
+        "--release-url",
+        action=CheckReleaseAction,
+        help="Release URL for downloads",
     )
     parser.add_argument(
         "--release-entries",
         action=CheckReleaseAction,
         help="Release selector for entries",
     )
     parser.add_argument(
         "--html-entries",
         action=CheckHtmlAction,
         default="article",
         help="HTML selector for entries",
     )
     parser.add_argument(
-        "--html-url", action=CheckHtmlAction, default="a", help="HTML selector for URL"
+        "--html-url",
+        action=CheckHtmlAction,
+        default="a",
+        help="HTML selector for URL",
     )
     parser.add_argument(
         "--html-title",
         action=CheckHtmlAction,
         default="h3",
         help="HTML selector for title",
     )
@@ -326,29 +347,29 @@
 
     return parser.parse_args(arguments)
 
 
 def save_rss_feed(rss_feed, arguments):
     """Save the RSS feed to a file."""
     try:
-        with open(arguments.output, "w", encoding="utf-8") as f:
+        with Path.open(arguments.output, "w", encoding="utf-8") as f:
             f.write(rss_feed)
-    except IOError:
+    except OSError:
         print("ERROR: Unable to write to file")
         sys.exit(1)
 
     if not arguments.quiet:
         if arguments.atom:
             print(f"Atom feed created: {arguments.output}")
         else:
             print(f"RSS feed created: {arguments.output}")
 
 
 def main(args=None):
-    """Main function."""
+    """Handle program arguments."""
     if args is None:
         args = sys.argv[1:]
 
     args = parse_arguments(args)
 
     if vars(args).get("version"):
         print(__version__)
```

