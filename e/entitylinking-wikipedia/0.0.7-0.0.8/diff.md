# Comparing `tmp/entitylinking_wikipedia-0.0.7.tar.gz` & `tmp/entitylinking_wikipedia-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entitylinking_wikipedia-0.0.7.tar", last modified: Mon May  1 20:41:07 2023, max compression
+gzip compressed data, was "entitylinking_wikipedia-0.0.8.tar", last modified: Mon May  1 21:06:17 2023, max compression
```

## Comparing `entitylinking_wikipedia-0.0.7.tar` & `entitylinking_wikipedia-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.154068 entitylinking_wikipedia-0.0.7/
--rw-rw-rw-   0        0        0     1165 2023-05-01 20:41:07.150064 entitylinking_wikipedia-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-05-01 19:28:26.000000 entitylinking_wikipedia-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.104998 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/
--rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:41:07.144986 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/
--rw-rw-rw-   0        0        0     1165 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-01 20:41:07.000000 entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 20:41:07.155067 entitylinking_wikipedia-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-01 20:07:35.000000 entitylinking_wikipedia-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:17.733582 entitylinking_wikipedia-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2023-05-01 21:00:41.000000 entitylinking_wikipedia-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1250 2023-05-01 21:06:17.732580 entitylinking_wikipedia-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-05-01 21:03:19.000000 entitylinking_wikipedia-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:17.714655 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia/
+-rw-rw-rw-   0        0        0     2009 2023-05-01 18:42:43.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 21:06:17.729584 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/
+-rw-rw-rw-   0        0        0     1250 2023-05-01 21:06:17.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-01 21:06:17.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 21:06:17.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-01 21:06:17.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-01 21:06:17.000000 entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 21:06:17.733582 entitylinking_wikipedia-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-05-01 21:05:54.000000 entitylinking_wikipedia-0.0.8/setup.py
```

### Comparing `entitylinking_wikipedia-0.0.7/PKG-INFO` & `entitylinking_wikipedia-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: entitylinking_wikipedia
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for Entity Linking using WikiPedia
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://github.com/Soumyadipta-Maiti/Package-Creation
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <h3>Entity Linking via WikiPedia </h3>
 
 This package is used to perform Entity Linking based on Wikipedia based on user's input sentence.
 
 Check out below github page for more details:
-https://github.com/pypa/sampleproject
+https://github.com/Soumyadipta-Maiti/Package-Creation
 
 <h3>Installation of Package</h3>
 
 pip install entitylinking-wikipedia
 
 
 <h3>Sample Coding using this Package</h3>
 
-from  import * <br>
+from entitylinking_wikipedia import * <br>
 import pandas as pd <br>
 final_out = pd.DataFrame() <br>
-final_out = Entity_Linking_via_Wikipedia('I stay in Kolkata in India.') <br>
+final_out = Entity_Linking_via_Wikipedia('I work at IBM in Kolkata in India.') <br>
 print(final_out) <br>
```

### Comparing `entitylinking_wikipedia-0.0.7/README.md` & `entitylinking_wikipedia-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <h3>Entity Linking via WikiPedia </h3>
 
 This package is used to perform Entity Linking based on Wikipedia based on user's input sentence.
 
 Check out below github page for more details:
-https://github.com/pypa/sampleproject
+https://github.com/Soumyadipta-Maiti/Package-Creation
 
 <h3>Installation of Package</h3>
 
 pip install entitylinking-wikipedia
 
 
 <h3>Sample Coding using this Package</h3>
 
-from  import * <br>
+from entitylinking_wikipedia import * <br>
 import pandas as pd <br>
 final_out = pd.DataFrame() <br>
-final_out = Entity_Linking_via_Wikipedia('I stay in Kolkata in India.') <br>
+final_out = Entity_Linking_via_Wikipedia('I work at IBM in Kolkata in India.') <br>
 print(final_out) <br>
```

### Comparing `entitylinking_wikipedia-0.0.7/entitylinking_wikipedia/__init__.py` & `entitylinking_wikipedia-0.0.8/entitylinking_wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `entitylinking_wikipedia-0.0.7/entitylinking_wikipedia.egg-info/PKG-INFO` & `entitylinking_wikipedia-0.0.8/entitylinking_wikipedia.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: entitylinking-wikipedia
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for Entity Linking using WikiPedia
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://github.com/Soumyadipta-Maiti/Package-Creation
 Author: Soumyadipta Maiti
 Author-email: soumya55555@gmail.com
 Keywords: Python,Entity Linking,NER,WikiPedia
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <h3>Entity Linking via WikiPedia </h3>
 
 This package is used to perform Entity Linking based on Wikipedia based on user's input sentence.
 
 Check out below github page for more details:
-https://github.com/pypa/sampleproject
+https://github.com/Soumyadipta-Maiti/Package-Creation
 
 <h3>Installation of Package</h3>
 
 pip install entitylinking-wikipedia
 
 
 <h3>Sample Coding using this Package</h3>
 
-from  import * <br>
+from entitylinking_wikipedia import * <br>
 import pandas as pd <br>
 final_out = pd.DataFrame() <br>
-final_out = Entity_Linking_via_Wikipedia('I stay in Kolkata in India.') <br>
+final_out = Entity_Linking_via_Wikipedia('I work at IBM in Kolkata in India.') <br>
 print(final_out) <br>
```

### Comparing `entitylinking_wikipedia-0.0.7/setup.py` & `entitylinking_wikipedia-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION_FILE = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION='Package for Entity Linking using WikiPedia'
 # LONG_DESCRIPTION = file:README.md
-URL = 'https://github.com/pypa/sampleproject'
+URL = 'https://github.com/Soumyadipta-Maiti/Package-Creation'
 
 #Setting Up
 setup(
     name='entitylinking_wikipedia',
     version=VERSION,
     author='Soumyadipta Maiti',
     author_email='soumya55555@gmail.com',
```

