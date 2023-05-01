# Comparing `tmp/gsearch-nyaa-0.1.3.tar.gz` & `tmp/gsearch-nyaa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsearch-nyaa-0.1.3.tar", last modified: Mon May  1 20:37:29 2023, max compression
+gzip compressed data, was "gsearch-nyaa-0.1.4.tar", last modified: Mon May  1 20:39:59 2023, max compression
```

## Comparing `gsearch-nyaa-0.1.3.tar` & `gsearch-nyaa-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:37:29.069097 gsearch-nyaa-0.1.3/
--rw-rw-rw-   0        0        0     2434 2023-05-01 20:37:29.068101 gsearch-nyaa-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2188 2023-05-01 20:37:11.000000 gsearch-nyaa-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 20:37:29.037541 gsearch-nyaa-0.1.3/gsearch/
--rw-rw-rw-   0        0        0     1634 2023-05-01 20:06:24.000000 gsearch-nyaa-0.1.3/gsearch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:37:29.066764 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/
--rw-rw-rw-   0        0        0     2434 2023-05-01 20:37:28.000000 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-01 20:37:28.000000 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:37:28.000000 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 20:37:28.000000 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 20:37:28.000000 gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 20:37:29.069097 gsearch-nyaa-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-05-01 20:37:23.000000 gsearch-nyaa-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.026022 gsearch-nyaa-0.1.4/
+-rw-rw-rw-   0        0        0     2427 2023-05-01 20:39:59.026022 gsearch-nyaa-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2181 2023-05-01 20:39:45.000000 gsearch-nyaa-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.003642 gsearch-nyaa-0.1.4/gsearch/
+-rw-rw-rw-   0        0        0     1634 2023-05-01 20:06:24.000000 gsearch-nyaa-0.1.4/gsearch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.024855 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/
+-rw-rw-rw-   0        0        0     2427 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 20:39:59.027155 gsearch-nyaa-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-05-01 20:39:52.000000 gsearch-nyaa-0.1.4/setup.py
```

### Comparing `gsearch-nyaa-0.1.3/PKG-INFO` & `gsearch-nyaa-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
 
@@ -35,15 +35,15 @@
     print(f"Title: {result.title}")
     print(f"URL: {result.url}")
     print(f"Description: {result.description}\n")
 ```
 
 Here is an example of using gsearch to perform a Google search for "how to use Python":
 
-````
+```
 from gsearch import Google
 with Google() as google:
     results = google.search("how to use Python")
     for result in results:
         print(f"Title: {result.title}")
         print(f"URL: {result.url}")
         print(f"Description: {result.description}\n")
@@ -56,8 +56,7 @@
 If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 
 gsearch is released under the MIT License. See `LICENSE` for more information.
 
 Conclusion: gsearch is a powerful Python package that makes it easy to automate Google searches and extract information from the search results. Whether you need to perform a one-time search or automate a search process, gsearch is a great tool to have in your Python toolbox.
-````
```

### Comparing `gsearch-nyaa-0.1.3/README.md` & `gsearch-nyaa-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     print(f"Title: {result.title}")
     print(f"URL: {result.url}")
     print(f"Description: {result.description}\n")
 ```
 
 Here is an example of using gsearch to perform a Google search for "how to use Python":
 
-````
+```
 from gsearch import Google
 with Google() as google:
     results = google.search("how to use Python")
     for result in results:
         print(f"Title: {result.title}")
         print(f"URL: {result.url}")
         print(f"Description: {result.description}\n")
@@ -48,8 +48,7 @@
 If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 
 gsearch is released under the MIT License. See `LICENSE` for more information.
 
 Conclusion: gsearch is a powerful Python package that makes it easy to automate Google searches and extract information from the search results. Whether you need to perform a one-time search or automate a search process, gsearch is a great tool to have in your Python toolbox.
-````
```

### Comparing `gsearch-nyaa-0.1.3/gsearch/__init__.py` & `gsearch-nyaa-0.1.4/gsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `gsearch-nyaa-0.1.3/gsearch_nyaa.egg-info/PKG-INFO` & `gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
 
@@ -35,15 +35,15 @@
     print(f"Title: {result.title}")
     print(f"URL: {result.url}")
     print(f"Description: {result.description}\n")
 ```
 
 Here is an example of using gsearch to perform a Google search for "how to use Python":
 
-````
+```
 from gsearch import Google
 with Google() as google:
     results = google.search("how to use Python")
     for result in results:
         print(f"Title: {result.title}")
         print(f"URL: {result.url}")
         print(f"Description: {result.description}\n")
@@ -56,8 +56,7 @@
 If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 
 gsearch is released under the MIT License. See `LICENSE` for more information.
 
 Conclusion: gsearch is a powerful Python package that makes it easy to automate Google searches and extract information from the search results. Whether you need to perform a one-time search or automate a search process, gsearch is a great tool to have in your Python toolbox.
-````
```

### Comparing `gsearch-nyaa-0.1.3/setup.py` & `gsearch-nyaa-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def run(self):
         install.run(self)
         subprocess.call(["playwright", "install", "chromium"])
 
 
 setup(
     name="gsearch-nyaa",
-    version="0.1.3",
+    version="0.1.4",
     author="Praveen Senpai",
     author_email="pvnt20@gmail.com",
     description="A Python Package for Automated Google Searches and Scraping of Search Results",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

