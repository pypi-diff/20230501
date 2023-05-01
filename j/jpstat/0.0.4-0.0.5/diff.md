# Comparing `tmp/jpstat-0.0.4.tar.gz` & `tmp/jpstat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpstat-0.0.4.tar", last modified: Tue Jan 19 18:29:02 2021, max compression
+gzip compressed data, was "jpstat-0.0.5.tar", last modified: Mon May  1 12:27:58 2023, max compression
```

## Comparing `jpstat-0.0.4.tar` & `jpstat-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1067 2020-09-28 13:46:28.861235 jpstat-0.0.4/LICENSE
--rw-r--r--   0        0        0     2604 2021-01-19 14:57:51.822581 jpstat-0.0.4/README.md
--rw-r--r--   0        0        0      213 2020-11-13 18:00:03.521780 jpstat-0.0.4/jpstat/__init__.py
--rw-r--r--   0        0        0     7670 2020-11-22 13:27:59.660779 jpstat-0.0.4/jpstat/config.py
--rw-r--r--   0        0        0      103 2020-11-09 07:37:31.232108 jpstat-0.0.4/jpstat/estat/__init__.py
--rwxr-xr-x   0        0        0     3638 2021-01-19 14:57:14.971599 jpstat-0.0.4/jpstat/estat/api.py
--rw-r--r--   0        0        0     2505 2021-01-19 18:25:52.184910 jpstat-0.0.4/jpstat/estat/core.py
--rwxr-xr-x   0        0        0      127 2020-11-08 19:41:48.494446 jpstat-0.0.4/jpstat/estat/menu.py
--rw-r--r--   0        0        0        0 2020-11-08 10:14:01.085976 jpstat-0.0.4/jpstat/estat/util/__init__.py
--rw-r--r--   0        0        0      194 2020-11-08 19:20:36.855822 jpstat-0.0.4/jpstat/estat/util/clean.py
--rw-r--r--   0        0        0     1926 2020-11-09 07:57:05.026518 jpstat-0.0.4/jpstat/estat/util/validate.py
--rw-r--r--   0        0        0      101 2020-11-13 20:24:30.617851 jpstat-0.0.4/jpstat/estatFile/__init__.py
--rw-r--r--   0        0        0     1564 2020-11-22 13:19:51.494181 jpstat-0.0.4/jpstat/estatFile/core.py
--rw-r--r--   0        0        0     3133 2020-11-30 15:11:14.978378 jpstat-0.0.4/jpstat/estatFile/scrape.py
--rw-r--r--   0        0        0        0 2020-11-13 18:41:20.016192 jpstat-0.0.4/jpstat/util/__init__.py
--rw-r--r--   0        0        0      911 2020-11-13 20:43:54.235627 jpstat-0.0.4/jpstat/util/download.py
--rw-r--r--   0        0        0      696 2020-11-22 13:06:30.157026 jpstat-0.0.4/jpstat/util/io.py
--rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 jpstat-0.0.4/jpstat/util/z2h.py
--rw-r--r--   0        0        0       22 2021-01-19 18:26:51.670859 jpstat-0.0.4/jpstat/version.py
--rw-r--r--   0        0        0      636 2021-01-19 18:26:59.336016 jpstat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3501 2021-01-19 18:29:02.505566 jpstat-0.0.4/setup.py
--rw-r--r--   0        0        0     3344 2021-01-19 18:29:02.506024 jpstat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-09-28 13:46:28.861235 jpstat-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2903 2023-05-01 12:22:57.338109 jpstat-0.0.5/README.md
+-rw-r--r--   0        0        0      213 2020-11-13 18:00:03.521780 jpstat-0.0.5/jpstat/__init__.py
+-rw-r--r--   0        0        0     7670 2020-11-22 13:27:59.660779 jpstat-0.0.5/jpstat/config.py
+-rw-r--r--   0        0        0      103 2020-11-09 07:37:31.232108 jpstat-0.0.5/jpstat/estat/__init__.py
+-rwxr-xr-x   0        0        0     3638 2021-01-19 14:57:14.971599 jpstat-0.0.5/jpstat/estat/api.py
+-rw-r--r--   0        0        0     2692 2023-05-01 12:15:38.467292 jpstat-0.0.5/jpstat/estat/core.py
+-rwxr-xr-x   0        0        0      127 2020-11-08 19:41:48.494446 jpstat-0.0.5/jpstat/estat/menu.py
+-rw-r--r--   0        0        0        0 2020-11-08 10:14:01.085976 jpstat-0.0.5/jpstat/estat/util/__init__.py
+-rw-r--r--   0        0        0      194 2020-11-08 19:20:36.855822 jpstat-0.0.5/jpstat/estat/util/clean.py
+-rw-r--r--   0        0        0     1926 2020-11-09 07:57:05.026518 jpstat-0.0.5/jpstat/estat/util/validate.py
+-rw-r--r--   0        0        0      101 2020-11-13 20:24:30.617851 jpstat-0.0.5/jpstat/estatFile/__init__.py
+-rw-r--r--   0        0        0     1564 2020-11-22 13:19:51.494181 jpstat-0.0.5/jpstat/estatFile/core.py
+-rw-r--r--   0        0        0     3133 2020-11-30 15:11:14.978378 jpstat-0.0.5/jpstat/estatFile/scrape.py
+-rw-r--r--   0        0        0        0 2020-11-13 18:41:20.016192 jpstat-0.0.5/jpstat/util/__init__.py
+-rw-r--r--   0        0        0      911 2020-11-13 20:43:54.235627 jpstat-0.0.5/jpstat/util/download.py
+-rw-r--r--   0        0        0      696 2020-11-22 13:06:30.157026 jpstat-0.0.5/jpstat/util/io.py
+-rw-r--r--   0        0        0     1452 2020-10-09 14:14:04.379726 jpstat-0.0.5/jpstat/util/z2h.py
+-rw-r--r--   0        0        0       22 2023-05-01 12:24:54.391235 jpstat-0.0.5/jpstat/version.py
+-rw-r--r--   0        0        0      636 2023-05-01 12:25:19.431588 jpstat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3807 2023-05-01 12:27:58.749992 jpstat-0.0.5/setup.py
+-rw-r--r--   0        0        0     3643 2023-05-01 12:27:58.750359 jpstat-0.0.5/PKG-INFO
```

### Comparing `jpstat-0.0.4/LICENSE` & `jpstat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/README.md` & `jpstat-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,60 +24,67 @@
 To see a list of statistics offered by estat api
 
 ```python
 import jpstat
 stat = jpstat.estat.get_stat(key=YOUR_API_KEY)
 ```
 
-To search data by either the code of a statistic or some key words
+To search data by either the code of a statistic or some keywords
 
 ```python
 data = jpstat.estat.get_list(statsCode="00400001")
 data = jpstat.estat.get_list(searchWord="企業")
 ```
 
-To download data
+To download data and data note
 
 ```python
 data, note = jpstat.estat.get_data(statsDataId="0000040001")
 ```
 
+If there is an error related to accessing the data note, one can simply suppress outputting it by
+
+```python
+data = jpstat.estat.get_data(statsDataId="0000040001", return_note=False)
+```
+
 ### Configuration
 
 You can pass the estat api key to each function. Or you can set a configuration
 
 ```python
 jpstat.options["estat.api_key"] = "MY_API_KEY"
 ```
 
 You can also set the language from Japanese (default, "J") to English
+(However it is strongly recommended to use "J" as it often returns more information about the data)
 
 ```python
 jpstat.options["estat.lang"] = "E"
 ```
 
 To see a list of valid configuration options
 
 ```python
 jpstat.config.describe_options()
 ```
 
 ## estat File
 
-Many statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrapes the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.
+Many statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrape the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.
 
 ### Functions
 
 To see a list of all statistics in estat that have downloadable files
 
 ```python
 data = jpstat.estatFile.get_stat()
 ```
 
-It will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force to scrape again by setting `update=True`.
+It will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force scraping again by setting `update=True`.
 
 To search data files by code of a statistic and the survey year (optional)
 
 ```python
 data = jpstat.estatFile.get_list(statsCode="00400001")
 data = jpstat.estatFile.get_list(statsCode="00400001", year="1950")
 ```
```

### Comparing `jpstat-0.0.4/jpstat/config.py` & `jpstat-0.0.5/jpstat/config.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/estat/api.py` & `jpstat-0.0.5/jpstat/estat/api.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/estat/core.py` & `jpstat-0.0.5/jpstat/estat/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,16 +56,19 @@
     cats = data['STATISTICAL_DATA']['CLASS_INF']['CLASS_OBJ']
     for cat in cats:
         col_name = '@' + cat['@id']
         _cat_map = cat['CLASS']
         if isinstance(_cat_map, dict):
             _cat_map = [_cat_map]
         cat_map = {m['@code']: m['@name'] for m in _cat_map}
-        df[cat['@name']] = df[col_name].map(cat_map)
-        df.drop(col_name, axis=1, inplace=True)
+        # when lang="E" there is no @name and thus adjust the code to use the original col_name
+        new_col_name = cat.get('@name', col_name)
+        df[new_col_name] = df[col_name].map(cat_map)
+        if new_col_name != col_name:
+            df.drop(col_name, axis=1, inplace=True)
     df['Value'] = df['$']
     df.drop('$', axis=1, inplace=True)
     df = df.applymap(str_z2h)
     if return_note:
         try:
             note = pd.DataFrame(data['STATISTICAL_DATA']['DATA_INF']['NOTE'])
             note = note.rename(columns={"$": "EXPLAIN"})
```

### Comparing `jpstat-0.0.4/jpstat/estat/util/validate.py` & `jpstat-0.0.5/jpstat/estat/util/validate.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/estatFile/core.py` & `jpstat-0.0.5/jpstat/estatFile/core.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/estatFile/scrape.py` & `jpstat-0.0.5/jpstat/estatFile/scrape.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/util/download.py` & `jpstat-0.0.5/jpstat/util/download.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/util/io.py` & `jpstat-0.0.5/jpstat/util/io.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/jpstat/util/z2h.py` & `jpstat-0.0.5/jpstat/util/z2h.py`

 * *Files identical despite different names*

### Comparing `jpstat-0.0.4/pyproject.toml` & `jpstat-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jpstat"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python library for accessing official statistics of Japan."
 authors = ["Xuanli Zhu <akaguro.koyomi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alalalalaki/jpstat"
 repository = "https://github.com/alalalalaki/jpstat"
 keywords = ["estat", "japan", "statistics", "economics", "data"]
```

### Comparing `jpstat-0.0.4/setup.py` & `jpstat-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.0,<2.0', 'requests>=2.0,<3.0', 'requests_html>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'jpstat',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'A python library for accessing official statistics of Japan.',
-    'long_description': '# jpstat\n\nA python package for accessing the official statistics of Japan.\n\n## Features\n\n- [estat api](#estat-api)\n- [estat file](#estat-file)\n\n## Install\n\n```sh\npip install jpstat\n```\n\n## estat API\n\n[estat](https://www.e-stat.go.jp/) is the official site for government statistics in Japan. Its api service offers data of over 250+ statistics in Japan. You need to register an api key to access to the statistics.\n\n### Functions\n\nAll functions return one or multiple pandas DataFrames.\n\nTo see a list of statistics offered by estat api\n\n```python\nimport jpstat\nstat = jpstat.estat.get_stat(key=YOUR_API_KEY)\n```\n\nTo search data by either the code of a statistic or some key words\n\n```python\ndata = jpstat.estat.get_list(statsCode="00400001")\ndata = jpstat.estat.get_list(searchWord="企業")\n```\n\nTo download data\n\n```python\ndata, note = jpstat.estat.get_data(statsDataId="0000040001")\n```\n\n### Configuration\n\nYou can pass the estat api key to each function. Or you can set a configuration\n\n```python\njpstat.options["estat.api_key"] = "MY_API_KEY"\n```\n\nYou can also set the language from Japanese (default, "J") to English\n\n```python\njpstat.options["estat.lang"] = "E"\n```\n\nTo see a list of valid configuration options\n\n```python\njpstat.config.describe_options()\n```\n\n## estat File\n\nMany statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrapes the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.\n\n### Functions\n\nTo see a list of all statistics in estat that have downloadable files\n\n```python\ndata = jpstat.estatFile.get_stat()\n```\n\nIt will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force to scrape again by setting `update=True`.\n\nTo search data files by code of a statistic and the survey year (optional)\n\n```python\ndata = jpstat.estatFile.get_list(statsCode="00400001")\ndata = jpstat.estatFile.get_list(statsCode="00400001", year="1950")\n```\n\nAgain, you can save the result by setting `save=True`, and from next time jpstat would first check if the result already exists.\n\nTo download the file by using the information of data id and file type ("EXCEL"/"CSV"/"PDF") gotten from the result of `estatFile.get_list`\n\n```python\njpstat.estatFile.get_file(statsDataId="000029094935", file_type="EXCEL")\n```\n\nThe file would be downloaded to current folder by default.\n',
+    'long_description': '# jpstat\n\nA python package for accessing the official statistics of Japan.\n\n## Features\n\n- [estat api](#estat-api)\n- [estat file](#estat-file)\n\n## Install\n\n```sh\npip install jpstat\n```\n\n## estat API\n\n[estat](https://www.e-stat.go.jp/) is the official site for government statistics in Japan. Its api service offers data of over 250+ statistics in Japan. You need to register an api key to access to the statistics.\n\n### Functions\n\nAll functions return one or multiple pandas DataFrames.\n\nTo see a list of statistics offered by estat api\n\n```python\nimport jpstat\nstat = jpstat.estat.get_stat(key=YOUR_API_KEY)\n```\n\nTo search data by either the code of a statistic or some keywords\n\n```python\ndata = jpstat.estat.get_list(statsCode="00400001")\ndata = jpstat.estat.get_list(searchWord="企業")\n```\n\nTo download data and data note\n\n```python\ndata, note = jpstat.estat.get_data(statsDataId="0000040001")\n```\n\nIf there is an error related to accessing the data note, one can simply suppress outputting it by\n\n```python\ndata = jpstat.estat.get_data(statsDataId="0000040001", return_note=False)\n```\n\n### Configuration\n\nYou can pass the estat api key to each function. Or you can set a configuration\n\n```python\njpstat.options["estat.api_key"] = "MY_API_KEY"\n```\n\nYou can also set the language from Japanese (default, "J") to English\n(However it is strongly recommended to use "J" as it often returns more information about the data)\n\n```python\njpstat.options["estat.lang"] = "E"\n```\n\nTo see a list of valid configuration options\n\n```python\njpstat.config.describe_options()\n```\n\n## estat File\n\nMany statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrape the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.\n\n### Functions\n\nTo see a list of all statistics in estat that have downloadable files\n\n```python\ndata = jpstat.estatFile.get_stat()\n```\n\nIt will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force scraping again by setting `update=True`.\n\nTo search data files by code of a statistic and the survey year (optional)\n\n```python\ndata = jpstat.estatFile.get_list(statsCode="00400001")\ndata = jpstat.estatFile.get_list(statsCode="00400001", year="1950")\n```\n\nAgain, you can save the result by setting `save=True`, and from next time jpstat would first check if the result already exists.\n\nTo download the file by using the information of data id and file type ("EXCEL"/"CSV"/"PDF") gotten from the result of `estatFile.get_list`\n\n```python\njpstat.estatFile.get_file(statsDataId="000029094935", file_type="EXCEL")\n```\n\nThe file would be downloaded to current folder by default.\n',
     'author': 'Xuanli Zhu',
     'author_email': 'akaguro.koyomi@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alalalalaki/jpstat',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jpstat-0.0.4/PKG-INFO` & `jpstat-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpstat
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for accessing official statistics of Japan.
 Home-page: https://github.com/alalalalaki/jpstat
 License: MIT
 Keywords: estat,japan,statistics,economics,data
 Author: Xuanli Zhu
 Author-email: akaguro.koyomi@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -44,60 +44,67 @@
 To see a list of statistics offered by estat api
 
 ```python
 import jpstat
 stat = jpstat.estat.get_stat(key=YOUR_API_KEY)
 ```
 
-To search data by either the code of a statistic or some key words
+To search data by either the code of a statistic or some keywords
 
 ```python
 data = jpstat.estat.get_list(statsCode="00400001")
 data = jpstat.estat.get_list(searchWord="企業")
 ```
 
-To download data
+To download data and data note
 
 ```python
 data, note = jpstat.estat.get_data(statsDataId="0000040001")
 ```
 
+If there is an error related to accessing the data note, one can simply suppress outputting it by
+
+```python
+data = jpstat.estat.get_data(statsDataId="0000040001", return_note=False)
+```
+
 ### Configuration
 
 You can pass the estat api key to each function. Or you can set a configuration
 
 ```python
 jpstat.options["estat.api_key"] = "MY_API_KEY"
 ```
 
 You can also set the language from Japanese (default, "J") to English
+(However it is strongly recommended to use "J" as it often returns more information about the data)
 
 ```python
 jpstat.options["estat.lang"] = "E"
 ```
 
 To see a list of valid configuration options
 
 ```python
 jpstat.config.describe_options()
 ```
 
 ## estat File
 
-Many statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrapes the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.
+Many statistics and datasets in estat can not be accessed through API, but are excel, csv, or pdf files and can be downloaded. Here jpstat provides the functions that scrape the information of statistics and download the files. Api key for estat is not needed, and the result is in Japanese only.
 
 ### Functions
 
 To see a list of all statistics in estat that have downloadable files
 
 ```python
 data = jpstat.estatFile.get_stat()
 ```
 
-It will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force to scrape again by setting `update=True`.
+It will take some time to scraping the website of estat at the first time and then save the list to `options["estat.data_dir"]`. From then on, the function would first try to read the local file. You can force scraping again by setting `update=True`.
 
 To search data files by code of a statistic and the survey year (optional)
 
 ```python
 data = jpstat.estatFile.get_list(statsCode="00400001")
 data = jpstat.estatFile.get_list(statsCode="00400001", year="1950")
 ```
```

