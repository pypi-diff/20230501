# Comparing `tmp/ghananews-scraper-1.0.5.tar.gz` & `tmp/ghananews-scraper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghananews-scraper-1.0.5.tar", last modified: Wed Mar 15 23:51:07 2023, max compression
+gzip compressed data, was "dist/ghananews-scraper-1.0.6.tar", last modified: Mon May  1 20:24:22 2023, max compression
```

## Comparing `ghananews-scraper-1.0.5.tar` & `ghananews-scraper-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,39 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/
--rw-r--r--   0 tsiameh    (501) staff       (20)     5876 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     3732 2023-03-15 19:12:03.000000 ghananews-scraper-1.0.5/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     5876 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      349 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       21 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghananews_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/ghanaweb/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.5/ghanaweb/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5288 2023-03-15 23:47:28.000000 ghananews-scraper-1.0.5/ghanaweb/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      789 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.5/ghanaweb/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/myjoyonline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.5/myjoyonline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5419 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.5/myjoyonline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.5/myjoyonline/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-03-15 23:51:07.000000 ghananews-scraper-1.0.5/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1767 2023-03-15 23:51:00.000000 ghananews-scraper-1.0.5/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/3news/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 16:57:53.000000 ghananews-scraper-1.0.6/3news/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2931 2023-04-30 16:59:02.000000 ghananews-scraper-1.0.6/3news/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/3news/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     8910 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     6198 2023-05-01 07:17:09.000000 ghananews-scraper-1.0.6/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/citionline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-29 20:41:04.000000 ghananews-scraper-1.0.6/citionline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3283 2023-05-01 07:08:18.000000 ghananews-scraper-1.0.6/citionline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/citionline/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     8910 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      650 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       68 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghananews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/ghanaweb/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.6/ghanaweb/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4109 2023-05-01 07:08:47.000000 ghananews-scraper-1.0.6/ghanaweb/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-16 02:31:26.000000 ghananews-scraper-1.0.6/ghanaweb/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/graphiconline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 14:50:37.000000 ghananews-scraper-1.0.6/graphiconline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3522 2023-05-01 20:13:19.000000 ghananews-scraper-1.0.6/graphiconline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/graphiconline/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/modernghana/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-01 18:28:50.000000 ghananews-scraper-1.0.6/modernghana/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3273 2023-05-01 18:29:39.000000 ghananews-scraper-1.0.6/modernghana/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/modernghana/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/myjoyonline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.6/myjoyonline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     6216 2023-05-01 07:08:56.000000 ghananews-scraper-1.0.6/myjoyonline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/myjoyonline/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1767 2023-05-01 20:15:31.000000 ghananews-scraper-1.0.6/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:24:22.000000 ghananews-scraper-1.0.6/yen/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 18:14:26.000000 ghananews-scraper-1.0.6/yen/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4163 2023-05-01 07:09:06.000000 ghananews-scraper-1.0.6/yen/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.6/yen/utils.py
```

### Comparing `ghananews-scraper-1.0.5/ghanaweb/scraper.py` & `ghananews-scraper-1.0.6/ghanaweb/scraper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,94 @@
 import csv
 import os
-import urllib
+from datetime import datetime
+from urllib.parse import unquote
+
 import requests
 from bs4 import BeautifulSoup
-from .utils import SaveFile, HEADERS
+
+from .utils import HEADERS, SaveFile
 
 
 class GhanaWeb:
     def __init__(self, url, home_page="https://www.ghanaweb.com"):
         if not url.startswith(("http://", "https://")):
             raise ValueError("Invalid URL: must start with 'http://' or 'https://'")
         self.url = url
         self.home_page = home_page
-        self.file_name = urllib.parse.unquote(
+        self.file_name = unquote(
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
         self.response = None
         self.soup = None
 
     def download(self, output_dir=None):
         """scrape data"""
-        self.response = self.response or requests.request(
+        self.response = requests.request(
             "GET", self.url, headers=HEADERS
         )
-        self.soup = self.soup or BeautifulSoup(self.response.text, "html.parser")
+        self.soup = BeautifulSoup(self.response.text, "html.parser")
         lst_pages = [
             a for a in self.soup.find("div", {"class": "afcon-news list"}).find_all("a")
         ]
 
         try:
             print("saving results to csv...")
             output_dir = output_dir or os.getcwd()
             SaveFile.mkdir(output_dir)
             if not os.path.isdir(output_dir):
                 raise ValueError(
                     f"Invalid output directory: {output_dir} is not a directory"
                 )
             print(f"File will be saved to: {output_dir}")
+
+            stamp = datetime.strftime(datetime.utcnow(), "%Y-%m-%d")
             with open(
-                os.path.join(output_dir, self.file_name + ".csv"), mode="w", newline=""
+                    os.path.join(output_dir, self.file_name + f"_{stamp}.csv"), mode="w", newline=""
             ) as csv_file:
-                fieldnames = ["title", "content", "page_url"]
+                fieldnames = ["title", "content", "author", "published_date", "page_url"]
                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
                 writer.writeheader()
                 for page in lst_pages:
                     try:
-                        page_url = self.home_page + page.get("href", "")
+                        page_url = self.home_page + page["href"]  # get("href", "")
                         if page_url:
-                            response_page = requests.request("GET", page_url, headers=HEADERS)
+                            with requests.Session() as session:
+                                response_page = session.get(page_url, headers=HEADERS)
+                            # response_page = requests.request("GET", page_url, headers=HEADERS)
                             soup_page = BeautifulSoup(response_page.text, "html.parser")
                             try:
                                 title = soup_page.find("h1", {"style": "clear: both;"}).text.strip()
+                                # title = title.text.strip if title else ""
                             except Exception:
                                 title = ""
                             try:
                                 content = soup_page.find("p", {"style": "clear:right"}).text.strip()
+                                # content = content.text.strip() if content else ""
                             except Exception:
                                 content = ""
+                            try:
+                                published_date = soup_page.find("p", class_="floatLeft").text.split(",")[-1]
+                            except Exception:
+                                published_date = ""
+                            try:
+                                author = soup_page.find("p", class_="floatRight").text.split(":")[-1].split(",")[-2]
+                            except Exception:
+                                author = ""
+
                             writer.writerow(
-                                    {"title": title, "content": content, "page_url": page_url}
+                                {
+                                    "title": title,
+                                    "content": content,
+                                    "author": author,
+                                    "published_date": published_date,
+                                    "page_url": page_url,
+                                }
                             )
                     except Exception:
                         continue
                 print("Writing data to file...")
         except Exception as e:
             print(f"error: {e}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Done!")
-
-
-# class GhanaWeb:
-#     def __init__(self, url, home_page="https://www.ghanaweb.com"):
-#         self.url = url
-#         self.home_page = home_page
-#         self.file_name = url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
-#
-#     def download(self, output_dir=None):
-#         """scrape data"""
-#         response = requests.request('GET', self.url, headers=headers)
-#         soup = BeautifulSoup(response.text, 'html.parser')
-#         lst_pages = soup.find('div', {'class': 'afcon-news list'}).find_all('a')
-#
-#         try:
-#             print("saving results to csv...")
-#             if output_dir is None:
-#                 output_dir = os.getcwd()
-#                 SaveFile.mkdir(output_dir)
-#             print(f"File will be saved to: {output_dir}")
-#             with open(f"{output_dir}/{self.file_name}" + ".csv", mode='w', newline='') as csv_file:
-#                 fieldnames = ['title', 'content', 'page_url']
-#                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
-#                 print("Writing column names...")
-#                 writer.writeheader()
-#                 for page in lst_pages:
-#                     try:
-#                         page_url = self.home_page + page.attrs['href']
-#                         response_page = requests.request('GET', page_url, headers=headers)
-#                         soup_page = BeautifulSoup(response_page.text, 'html.parser')
-#                         try:
-#                             title = soup_page.find('h1', {'style': 'clear: both;'}).text.strip()
-#                         except Exception:
-#                             title = ""
-#                         try:
-#                             content = soup_page.find('p', {'style': 'clear:right'}).text.strip()
-#                         except Exception:
-#                             content = ""
-#
-#                         writer.writerow({'title': title, 'content': content, 'page_url': page_url})
-#                     except Exception:
-#                         continue
-#                 print("Writing artitle titles...")
-#                 print("Writing article content...")
-#                 print("Writing data to file...")
-#         except Exception as e:
-#             print(f"error: {e}")
-#
-#         print(f"All file(s) saved to: {output_dir} successfully!")
-#         print("Done!")
```

### Comparing `ghananews-scraper-1.0.5/ghanaweb/utils.py` & `ghananews-scraper-1.0.6/3news/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "Upgrade-Insecure-Requests": "1",
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
     "Cache-Control": "max-age=0",
     "Connection": "keep-alive",
 }
 
+
 class SaveFile:
     """a class to save file"""
 
     @staticmethod
     def mkdir(path):
         """Create directory"""
         try:
```

### Comparing `ghananews-scraper-1.0.5/myjoyonline/scraper.py` & `ghananews-scraper-1.0.6/myjoyonline/scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import csv
 import os
-import urllib
+from datetime import datetime
+from urllib.parse import unquote
+
 import requests
 from bs4 import BeautifulSoup
-from .utils import SaveFile, HEADERS
+
+from .utils import HEADERS, SaveFile
 
 
 class MyJoyOnline:
     def __init__(self, url):
         if not url.startswith(("http://", "https://")):
             raise ValueError("Invalid URL: must start with 'http://' or 'https://'")
         self.url = url
-        self.file_name = urllib.parse.unquote(
+        self.file_name = unquote(
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
 
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
@@ -41,36 +44,55 @@
                 output_dir = os.getcwd()
                 SaveFile.mkdir(output_dir)
             if not os.path.isdir(output_dir):
                 raise ValueError(
                     f"Invalid output directory: {output_dir} is not a directory"
                 )
             print(f"File will be saved to: {output_dir}")
+
+            stamp = datetime.strftime(datetime.utcnow(), "%Y-%m-%d")
             with open(
-                os.path.join(output_dir, self.file_name + ".csv"), mode="w", newline=""
+                os.path.join(output_dir, self.file_name + f"_{stamp}.csv"),
+                    mode="w",
+                    newline="",
+                    encoding='utf-8'
             ) as csv_file:
-                fieldnames = ["title", "content", "page_url"]
+                fieldnames = ["title", "content", "author", "published_date", "page_url"]
                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
                 writer.writeheader()
                 for page in lst_pages:
                     page_url = page.find("a").attrs.get("href")
                     if page_url:
                         with requests.Session() as session:
                             response_page = session.get(page_url, headers=HEADERS)
                         soup_page = BeautifulSoup(response_page.text, "html.parser")
+
                         title = soup_page.find("div", {"class": "article-title"})
                         title = title.text.strip() if title else ""
+
                         content = soup_page.find("div", {"id": "article-text"})
                         content = content.text.strip() if content else ""
+
+                        published_date = soup_page.find("div", class_="article-meta").find("div")
+                        published_date = published_date.text.strip() if published_date else ""
+
+                        author = soup_page.find("div", class_="article-meta").find("a")
+                        author = author.text.strip().split(":")[-1] if author else ""
+
                         writer.writerow(
-                            {"title": title, "content": content, "page_url": page_url}
+                            {"title": title,
+                             "content": content,
+                             "author": author,
+                             "published_date": published_date,
+                             "page_url": page_url
+                             }
                         )
                 print("Writing data to file...")
-        except Exception as e:
-            print(f"error: {e}")
+        except Exception as err:
+            print(f"error: {err}")
 
         print(f"All file(s) saved to: {output_dir} successfully!")
         print("Done!")
 
 
 # class MyJoyOnline:
 #     def __init__(self, url):
```

### Comparing `ghananews-scraper-1.0.5/myjoyonline/utils.py` & `ghananews-scraper-1.0.6/citionline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.5/setup.py` & `ghananews-scraper-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghananews-scraper',
     py_modules=['ghanaweb', 'myjoyonline'],
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghananews-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
@@ -34,11 +34,11 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
-    keywords="Scraper, Data, GhanaNews, GhanaWeb, JoyNews, MyJoyonline, News, Web Scraper, Ghana Scraper",
+    keywords="Scraper, Data, GhanaNews, GhanaWeb, JoyNews, MyJoyOnline, News, Web Scraper, Ghana Scraper",
     platforms=["any"],
     python_requires=">=3.7",
 )
```

