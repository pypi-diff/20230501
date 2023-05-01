# Comparing `tmp/gsearch-nyaa-0.1.tar.gz` & `tmp/gsearch-nyaa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsearch-nyaa-0.1.tar", last modified: Mon May  1 20:23:43 2023, max compression
+gzip compressed data, was "gsearch-nyaa-0.1.1.tar", last modified: Mon May  1 20:24:23 2023, max compression
```

## Comparing `gsearch-nyaa-0.1.tar` & `gsearch-nyaa-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:23:43.224597 gsearch-nyaa-0.1/
--rw-rw-rw-   0        0        0     2430 2023-05-01 20:23:43.223600 gsearch-nyaa-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2128 2023-05-01 20:22:17.000000 gsearch-nyaa-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 20:23:43.209648 gsearch-nyaa-0.1/gsearch/
--rw-rw-rw-   0        0        0     1634 2023-05-01 20:06:24.000000 gsearch-nyaa-0.1/gsearch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:23:43.222607 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/
--rw-rw-rw-   0        0        0     2430 2023-05-01 20:23:43.000000 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-01 20:23:43.000000 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:23:43.000000 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 20:23:43.000000 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 20:23:43.000000 gsearch-nyaa-0.1/gsearch_nyaa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 20:23:43.225595 gsearch-nyaa-0.1/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-05-01 20:23:01.000000 gsearch-nyaa-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:24:23.110169 gsearch-nyaa-0.1.1/
+-rw-rw-rw-   0        0        0     2437 2023-05-01 20:24:23.108764 gsearch-nyaa-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2128 2023-05-01 20:22:17.000000 gsearch-nyaa-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 20:24:23.087829 gsearch-nyaa-0.1.1/gsearch/
+-rw-rw-rw-   0        0        0     1634 2023-05-01 20:06:24.000000 gsearch-nyaa-0.1.1/gsearch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:24:23.107767 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/
+-rw-rw-rw-   0        0        0     2437 2023-05-01 20:24:22.000000 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-01 20:24:23.000000 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:24:22.000000 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-01 20:24:22.000000 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 20:24:22.000000 gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:24:23.111165 gsearch-nyaa-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-05-01 20:24:19.000000 gsearch-nyaa-0.1.1/setup.py
```

### Comparing `gsearch-nyaa-0.1/PKG-INFO` & `gsearch-nyaa-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1
+Version: 0.1.1
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
-Home-page: https://github.com/praveensenpai/gsearch
+Home-page: https://github.com/praveensenpai/gsearch-nyaa
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
 
 Introduction: gsearch is a Python package that allows users to perform automated Google searches and extract information from the search results using Python code. The package uses the Playwright and Selectolax libraries to scrape search results and provides a convenient way to automate and extract information from Google searches.
```

### Comparing `gsearch-nyaa-0.1/README.md` & `gsearch-nyaa-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gsearch-nyaa-0.1/gsearch/__init__.py` & `gsearch-nyaa-0.1.1/gsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `gsearch-nyaa-0.1/gsearch_nyaa.egg-info/PKG-INFO` & `gsearch-nyaa-0.1.1/gsearch_nyaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1
+Version: 0.1.1
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
-Home-page: https://github.com/praveensenpai/gsearch
+Home-page: https://github.com/praveensenpai/gsearch-nyaa
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
 
 Introduction: gsearch is a Python package that allows users to perform automated Google searches and extract information from the search results using Python code. The package uses the Playwright and Selectolax libraries to scrape search results and provides a convenient way to automate and extract information from Google searches.
```

### Comparing `gsearch-nyaa-0.1/setup.py` & `gsearch-nyaa-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     def run(self):
         install.run(self)
         subprocess.call(["playwright", "install", "chromium"])
 
 
 setup(
     name="gsearch-nyaa",
-    version="0.1",
+    version="0.1.1",
     author="Praveen Senpai",
     author_email="pvnt20@gmail.com",
     description="A Python Package for Automated Google Searches and Scraping of Search Results",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/praveensenpai/gsearch",
+    url="https://github.com/praveensenpai/gsearch-nyaa",
     packages=find_packages(),
     install_requires=[
         "playwright",
         "selectolax",
     ],
     cmdclass={
         "install": CustomInstallCommand,
```

