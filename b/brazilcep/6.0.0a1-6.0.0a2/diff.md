# Comparing `tmp/brazilcep-6.0.0a1.tar.gz` & `tmp/brazilcep-6.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brazilcep-6.0.0a1.tar", max compression
+gzip compressed data, was "brazilcep-6.0.0a2.tar", max compression
```

## Comparing `brazilcep-6.0.0a1.tar` & `brazilcep-6.0.0a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     5935 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-20 23:13:05.854496 brazilcep-6.0.0a1/LICENSE
--rw-r--r--   0        0        0     3669 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/README.md
--rw-r--r--   0        0        0      497 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/brazilcep/__init__.py
--rw-r--r--   0        0        0     1543 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/brazilcep/apicep.py
--rw-r--r--   0        0        0     2025 2023-04-30 22:04:21.247217 brazilcep-6.0.0a1/brazilcep/client.py
--rw-r--r--   0        0        0     1129 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/brazilcep/correios.py
--rw-r--r--   0        0        0      543 2023-04-30 22:04:21.247217 brazilcep-6.0.0a1/brazilcep/exceptions.py
--rw-r--r--   0        0        0     1326 2023-04-30 22:04:21.251217 brazilcep-6.0.0a1/brazilcep/viacep.py
--rw-r--r--   0        0        0     1328 2023-04-30 22:11:57.397481 brazilcep-6.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4573 1970-01-01 00:00:00.000000 brazilcep-6.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     5935 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-20 23:13:05.854496 brazilcep-6.0.0a2/LICENSE
+-rw-r--r--   0        0        0     3663 2023-05-01 02:07:05.152294 brazilcep-6.0.0a2/README.md
+-rw-r--r--   0        0        0      497 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/__init__.py
+-rw-r--r--   0        0        0     1543 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/apicep.py
+-rw-r--r--   0        0        0     2025 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/client.py
+-rw-r--r--   0        0        0     1129 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/correios.py
+-rw-r--r--   0        0        0      543 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/exceptions.py
+-rw-r--r--   0        0        0     1326 2023-04-30 22:23:02.754880 brazilcep-6.0.0a2/brazilcep/viacep.py
+-rw-r--r--   0        0        0     2209 2023-05-01 02:21:38.821282 brazilcep-6.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 brazilcep-6.0.0a2/PKG-INFO
```

### Comparing `brazilcep-6.0.0a1/CHANGELOG.md` & `brazilcep-6.0.0a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/LICENSE` & `brazilcep-6.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/README.md` & `brazilcep-6.0.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Install
 
 The recommended way to get BrazilCEP is to **install the latest stable release**
 via [pip](http://pip-installer.org>):
 
 ```sh
-$ pip install brazilcep
+pip install brazilcep
 ```
 
 We currently support **Python 3.8+ only**. Users on older interpreter versions
 are urged to upgrade.
 
 ## How to Use
 
@@ -71,15 +71,15 @@
 ```python
 >>> import brazilcep
 ```
 
 Now, call the `get_address_from_cep` to query any CEP:
 
 ```python
->>> address = requests.get_address_from_cep('37503-130')
+>>> address = brazilcep.get_address_from_cep('37503-130')
 ```
 
 Now, we have a *dict* object called ``address``. We can
 get all the address information we need from this object:
 
 ```python
  >>> address
@@ -93,15 +93,15 @@
 }
 ```
 
 The CEP always must be a string.
 
 ## Documentation
 
-Documentation for the current version of BrazilCEP is available from the official docs [here](https://mstuttgart.github.io/brazilcep).
+Documentation for the current version of BrazilCEP is available from the official docs [here](https://brazilcep.readthedocs.io/).
 
 ## Contribute
 
 See this *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md).
 
 ## Credits
```

#### html2text {}

```diff
@@ -14,21 +14,21 @@
 supports several CEP API's: * [ViaCEP](https://viacep.com.br) * [ApiCEP
 (WideNet)](https://apicep.com) * [Correios (SIGEPWeb)](http://
 www.corporativo.correios.com.br/encomendas/sigepweb/doc/
 Manual_de_Implementacao_do_Web_Service_SIGEP_WEB.pdf) BrazilCEP started as a
 personal study project and evolved into a serious and open source project that
 is used by many developers on a daily basis. ## Install The recommended way to
 get BrazilCEP is to **install the latest stable release** via [pip](http://pip-
-installer.org>): ```sh $ pip install brazilcep ``` We currently support
-**Python 3.8+ only**. Users on older interpreter versions are urged to upgrade.
-## How to Use Making a request is very simple. Begin by importing the BrazilCEP
+installer.org>): ```sh pip install brazilcep ``` We currently support **Python
+3.8+ only**. Users on older interpreter versions are urged to upgrade. ## How
+to Use Making a request is very simple. Begin by importing the BrazilCEP
 module: ```python >>> import brazilcep ``` Now, call the `get_address_from_cep`
-to query any CEP: ```python >>> address = requests.get_address_from_cep('37503-
-130') ``` Now, we have a *dict* object called ``address``. We can get all the
-address information we need from this object: ```python >>> address
+to query any CEP: ```python >>> address = brazilcep.get_address_from_cep
+('37503-130') ``` Now, we have a *dict* object called ``address``. We can get
+all the address information we need from this object: ```python >>> address
 { 'district': 'rua abc', 'cep': '37503130', 'city': 'city ABC', 'street':
 'str', 'uf': 'str', 'complement': 'str', } ``` The CEP always must be a string.
 ## Documentation Documentation for the current version of BrazilCEP is
-available from the official docs [here](https://mstuttgart.github.io/
-brazilcep). ## Contribute See this *guideline* [here](https://github.com/
-mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md). ## Credits Copyright (C)
-2016-2023 by Michell Stuttgart
+available from the official docs [here](https://brazilcep.readthedocs.io/). ##
+Contribute See this *guideline* [here](https://github.com/mstuttgart/brazilcep/
+blob/develop/CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell
+Stuttgart
```

### Comparing `brazilcep-6.0.0a1/brazilcep/apicep.py` & `brazilcep-6.0.0a2/brazilcep/apicep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/brazilcep/client.py` & `brazilcep-6.0.0a2/brazilcep/client.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/brazilcep/correios.py` & `brazilcep-6.0.0a2/brazilcep/correios.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/brazilcep/exceptions.py` & `brazilcep-6.0.0a2/brazilcep/exceptions.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/brazilcep/viacep.py` & `brazilcep-6.0.0a2/brazilcep/viacep.py`

 * *Files identical despite different names*

### Comparing `brazilcep-6.0.0a1/PKG-INFO` & `brazilcep-6.0.0a2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 Metadata-Version: 2.1
 Name: brazilcep
-Version: 6.0.0a1
-Summary: Python library to search brazilian CEP (brazilian zip codes)
-Home-page: https://github.com/mstuttgart/brazilcep
+Version: 6.0.0a2
+Summary: Python library to query brazilian CEP (brazilian zip codes) data
 License: MIT
 Keywords: correios,viacep,apicep,cep,brazil
 Author: Michell Stuttgart
 Author-email: michellstut@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Natural Language :: Portuguese (Brazilian)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: zeep (>=4.2.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/mstuttgart/brazilcep/issues
-Project-URL: Documentation, https://mstuttgart.github.io/brazilcep
+Project-URL: Documentation, https://brazilcep.readthedocs.io/en/latest/
+Project-URL: Donation, https://ko-fi.com/mstuttgart
 Project-URL: Repository, https://github.com/mstuttgart/brazilcep
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <a href="https://pypi.org/project/brazilcep/">
     <img src="https://raw.githubusercontent.com/mstuttgart/brazilcep/develop/docs/static/logo.png" width="30%">
@@ -76,15 +93,15 @@
 
 ## Install
 
 The recommended way to get BrazilCEP is to **install the latest stable release**
 via [pip](http://pip-installer.org>):
 
 ```sh
-$ pip install brazilcep
+pip install brazilcep
 ```
 
 We currently support **Python 3.8+ only**. Users on older interpreter versions
 are urged to upgrade.
 
 ## How to Use
 
@@ -93,15 +110,15 @@
 ```python
 >>> import brazilcep
 ```
 
 Now, call the `get_address_from_cep` to query any CEP:
 
 ```python
->>> address = requests.get_address_from_cep('37503-130')
+>>> address = brazilcep.get_address_from_cep('37503-130')
 ```
 
 Now, we have a *dict* object called ``address``. We can
 get all the address information we need from this object:
 
 ```python
  >>> address
@@ -115,15 +132,15 @@
 }
 ```
 
 The CEP always must be a string.
 
 ## Documentation
 
-Documentation for the current version of BrazilCEP is available from the official docs [here](https://mstuttgart.github.io/brazilcep).
+Documentation for the current version of BrazilCEP is available from the official docs [here](https://brazilcep.readthedocs.io/).
 
 ## Contribute
 
 See this *guideline* [here](https://github.com/mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md).
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,19 +1,31 @@
-Metadata-Version: 2.1 Name: brazilcep Version: 6.0.0a1 Summary: Python library
-to search brazilian CEP (brazilian zip codes) Home-page: https://github.com/
-mstuttgart/brazilcep License: MIT Keywords: correios,viacep,apicep,cep,brazil
-Author: Michell Stuttgart Author-email: michellstut@gmail.com Requires-Python:
->=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Metadata-Version: 2.1 Name: brazilcep Version: 6.0.0a2 Summary: Python library
+to query brazilian CEP (brazilian zip codes) data License: MIT Keywords:
+correios,viacep,apicep,cep,brazil Author: Michell Stuttgart Author-email:
+michellstut@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Natural Language :: Portuguese (Brazilian) Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: requests
-(>=2.28.2,<3.0.0) Requires-Dist: zeep (>=4.2.1,<5.0.0) Project-URL: Bug
-Tracker, https://github.com/mstuttgart/brazilcep/issues Project-URL:
-Documentation, https://mstuttgart.github.io/brazilcep Project-URL: Repository,
-https://github.com/mstuttgart/brazilcep Description-Content-Type: text/markdown
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development :: Build Tools Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
+Dist: zeep (>=4.2.1,<5.0.0) Project-URL: Bug Tracker, https://github.com/
+mstuttgart/brazilcep/issues Project-URL: Documentation, https://
+brazilcep.readthedocs.io/en/latest/ Project-URL: Donation, https://ko-fi.com/
+mstuttgart Project-URL: Repository, https://github.com/mstuttgart/brazilcep
+Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/mstuttgart/brazilcep/develop/docs/static/
                                    logo.png]
                               **** BrazilCEP ****
 *** Minimalist and easy-to-use python library designed to query CEP (brazilian
                              zip codes) data. ***
 [GitHub_Workflow_Status_(with_branch)] [Coveralls_github] [Status] [Downloads]
                               [Ratings] [Version]
@@ -26,21 +38,21 @@
 supports several CEP API's: * [ViaCEP](https://viacep.com.br) * [ApiCEP
 (WideNet)](https://apicep.com) * [Correios (SIGEPWeb)](http://
 www.corporativo.correios.com.br/encomendas/sigepweb/doc/
 Manual_de_Implementacao_do_Web_Service_SIGEP_WEB.pdf) BrazilCEP started as a
 personal study project and evolved into a serious and open source project that
 is used by many developers on a daily basis. ## Install The recommended way to
 get BrazilCEP is to **install the latest stable release** via [pip](http://pip-
-installer.org>): ```sh $ pip install brazilcep ``` We currently support
-**Python 3.8+ only**. Users on older interpreter versions are urged to upgrade.
-## How to Use Making a request is very simple. Begin by importing the BrazilCEP
+installer.org>): ```sh pip install brazilcep ``` We currently support **Python
+3.8+ only**. Users on older interpreter versions are urged to upgrade. ## How
+to Use Making a request is very simple. Begin by importing the BrazilCEP
 module: ```python >>> import brazilcep ``` Now, call the `get_address_from_cep`
-to query any CEP: ```python >>> address = requests.get_address_from_cep('37503-
-130') ``` Now, we have a *dict* object called ``address``. We can get all the
-address information we need from this object: ```python >>> address
+to query any CEP: ```python >>> address = brazilcep.get_address_from_cep
+('37503-130') ``` Now, we have a *dict* object called ``address``. We can get
+all the address information we need from this object: ```python >>> address
 { 'district': 'rua abc', 'cep': '37503130', 'city': 'city ABC', 'street':
 'str', 'uf': 'str', 'complement': 'str', } ``` The CEP always must be a string.
 ## Documentation Documentation for the current version of BrazilCEP is
-available from the official docs [here](https://mstuttgart.github.io/
-brazilcep). ## Contribute See this *guideline* [here](https://github.com/
-mstuttgart/brazilcep/blob/develop/CONTRIBUTING.md). ## Credits Copyright (C)
-2016-2023 by Michell Stuttgart
+available from the official docs [here](https://brazilcep.readthedocs.io/). ##
+Contribute See this *guideline* [here](https://github.com/mstuttgart/brazilcep/
+blob/develop/CONTRIBUTING.md). ## Credits Copyright (C) 2016-2023 by Michell
+Stuttgart
```

