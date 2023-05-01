# Comparing `tmp/gpt4free-0.1.3.tar.gz` & `tmp/gpt4free-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-spsifcfe\gpt4free-0.1.3.tar", last modified: Mon May  1 02:38:30 2023, max compression
+gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-4bzp4iut\gpt4free-0.1.4.tar", last modified: Mon May  1 06:24:58 2023, max compression
```

## Comparing `gpt4free-0.1.3.tar` & `gpt4free-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.378336 gpt4free-0.1.3/
--rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.3/AUTHORS.md
--rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.3/HISTORY.md
--rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1440 2023-05-01 02:38:30.378336 gpt4free-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.353337 gpt4free-0.1.3/gpt4free/
--rw-rw-rw-   0        0        0     2659 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.363329 gpt4free-0.1.3/gpt4free/cocalc/
--rw-rw-rw-   0        0        0     2461 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/cocalc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.366330 gpt4free-0.1.3/gpt4free/forefront/
--rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/forefront/__init__.py
--rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/forefront/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.370332 gpt4free-0.1.3/gpt4free/quora/
--rw-rw-rw-   0        0        0    21139 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/__init__.py
--rw-rw-rw-   0        0        0    19700 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/api.py
--rw-rw-rw-   0        0        0     1464 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/backup-mail.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.372333 gpt4free-0.1.3/gpt4free/quora/graphql/
--rw-rw-rw-   0        0        0        0 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/graphql/__init__.py
--rw-rw-rw-   0        0        0     2359 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/quora/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.375333 gpt4free-0.1.3/gpt4free/theb/
--rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/theb/__init__.py
--rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/theb/theb_test.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.376333 gpt4free-0.1.3/gpt4free/usesless/
--rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/usesless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.377335 gpt4free-0.1.3/gpt4free/you/
--rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-0.1.3/gpt4free/you/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:30.362341 gpt4free-0.1.3/gpt4free.egg-info/
--rw-rw-rw-   0        0        0     1440 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 02:38:29.000000 gpt4free-0.1.3/gpt4free.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 02:38:30.000000 gpt4free-0.1.3/gpt4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-01 02:38:30.379330 gpt4free-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2147 2023-05-01 02:37:59.000000 gpt4free-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.356054 gpt4free-0.1.4/
+-rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.4/AUTHORS.md
+-rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.4/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.4/HISTORY.md
+-rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1440 2023-05-01 06:24:58.356054 gpt4free-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.334844 gpt4free-0.1.4/gpt4free/
+-rw-rw-rw-   0        0        0     2391 2023-05-01 06:22:16.000000 gpt4free-0.1.4/gpt4free/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.345048 gpt4free-0.1.4/gpt4free/cocalc/
+-rw-rw-rw-   0        0        0     2461 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/cocalc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.348048 gpt4free-0.1.4/gpt4free/forefront/
+-rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/forefront/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/forefront/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.351052 gpt4free-0.1.4/gpt4free/theb/
+-rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/theb/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/theb/theb_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.353051 gpt4free-0.1.4/gpt4free/usesless/
+-rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/usesless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.354048 gpt4free-0.1.4/gpt4free/you/
+-rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-0.1.4/gpt4free/you/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 06:24:58.344052 gpt4free-0.1.4/gpt4free.egg-info/
+-rw-rw-rw-   0        0        0     1440 2023-05-01 06:24:58.000000 gpt4free-0.1.4/gpt4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-05-01 06:24:58.000000 gpt4free-0.1.4/gpt4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 06:24:58.000000 gpt4free-0.1.4/gpt4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 06:24:57.000000 gpt4free-0.1.4/gpt4free.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-05-01 06:24:58.000000 gpt4free-0.1.4/gpt4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 06:24:58.000000 gpt4free-0.1.4/gpt4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-05-01 06:24:58.358048 gpt4free-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2147 2023-05-01 06:06:17.000000 gpt4free-0.1.4/setup.py
```

### Comparing `gpt4free-0.1.3/CONTRIBUTING.md` & `gpt4free-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/LICENSE` & `gpt4free-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/PKG-INFO` & `gpt4free-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.3
+Version: 0.1.4
 Summary: decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
```

### Comparing `gpt4free-0.1.3/gpt4free/__init__.py` & `gpt4free-0.1.4/gpt4free/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,70 @@
-from enum import Enum
-
-from gpt4free import cocalc
-from gpt4free import forefront
-from gpt4free import quora
-from gpt4free import theb
-from gpt4free import you
-from gpt4free import usesless
-
-
-class Provider(Enum):
-    """An enum representing  different providers."""
-
-    You = 'you'
-    Poe = 'poe'
-    ForeFront = 'fore_front'
-    Theb = 'theb'
-    CoCalc = 'cocalc'
-    UseLess = 'useless'
-
-
-class Completion:
-    """This class will be used for invoking the given provider"""
-
-    @staticmethod
-    def create(provider: Provider, prompt: str, **kwargs) -> str:
-        
-        """
-        Invokes the given provider with given prompt and addition arguments and returns the string response
-
-        :param provider: an enum representing the provider to use while invoking
-        :param prompt: input provided by the user
-        :param kwargs:  Additional keyword arguments to pass to the provider while invoking
-        :return: A string representing the response from the provider
-        """
-        if provider == Provider.Poe:
-            return Completion.__poe_service(prompt, **kwargs)
-        elif provider == Provider.You:
-            return Completion.__you_service(prompt, **kwargs)
-        elif provider == Provider.ForeFront:
-            return Completion.__fore_front_service(prompt, **kwargs)
-        elif provider == Provider.Theb:
-            return Completion.__theb_service(prompt, **kwargs)
-        elif provider == Provider.CoCalc:
-            return Completion.__cocalc_service(prompt, **kwargs)
-        elif provider == Provider.UseLess:
-            return Completion.__useless_service(prompt, **kwargs)
-        else:
-            raise Exception('Provider not exist, Please try again')
-        
-    @staticmethod
-    def __useless_service(prompt: str, **kwargs) -> str:
-        return usesless.Completion.create(prompt = prompt, **kwargs)
-
-    @staticmethod
-    def __you_service(prompt: str, **kwargs) -> str:
-        return you.Completion.create(prompt, **kwargs).text
-
-    @staticmethod
-    def __poe_service(prompt: str, **kwargs) -> str:
-        return quora.Completion.create(prompt=prompt, **kwargs).text
-
-    @staticmethod
-    def __fore_front_service(prompt: str, **kwargs) -> str:
-        return forefront.Completion.create(prompt=prompt, **kwargs).text
-
-    @staticmethod
-    def __theb_service(prompt: str, **kwargs):
-        return ''.join(theb.Completion.create(prompt=prompt))
-
-    @staticmethod
-    def __cocalc_service(prompt: str, **kwargs):
-        return cocalc.Completion.create(prompt, cookie_input=kwargs.get('cookie_input', '')).text
+from enum import Enum
+
+from gpt4free import cocalc
+from gpt4free import forefront
+from gpt4free import theb
+from gpt4free import you
+from gpt4free import usesless
+
+__author__ = """Reza Shakeri"""
+__email__ = "rzashakeri@outlook.com"
+__version__ = "0.1.4"
+
+
+class Provider(Enum):
+    """An enum representing  different providers."""
+
+    You = 'you'
+    Poe = 'poe'
+    ForeFront = 'fore_front'
+    Theb = 'theb'
+    CoCalc = 'cocalc'
+    UseLess = 'useless'
+
+
+class Completion:
+    """This class will be used for invoking the given provider"""
+
+    @staticmethod
+    def create(provider: Provider, prompt: str, **kwargs) -> str:
+
+        """
+        Invokes the given provider with given prompt and addition arguments and returns the string response
+
+        :param provider: an enum representing the provider to use while invoking
+        :param prompt: input provided by the user
+        :param kwargs:  Additional keyword arguments to pass to the provider while invoking
+        :return: A string representing the response from the provider
+        """
+        if provider == Provider.You:
+            return Completion.__you_service(prompt, **kwargs)
+        elif provider == Provider.ForeFront:
+            return Completion.__fore_front_service(prompt, **kwargs)
+        elif provider == Provider.Theb:
+            return Completion.__theb_service(prompt, **kwargs)
+        elif provider == Provider.CoCalc:
+            return Completion.__cocalc_service(prompt, **kwargs)
+        elif provider == Provider.UseLess:
+            return Completion.__useless_service(prompt, **kwargs)
+        else:
+            raise Exception('Provider not exist, Please try again')
+
+    @staticmethod
+    def __useless_service(prompt: str, **kwargs) -> str:
+        return usesless.Completion.create(prompt=prompt, **kwargs)
+
+    @staticmethod
+    def __you_service(prompt: str, **kwargs) -> str:
+        return you.Completion.create(prompt, **kwargs).text
+
+    @staticmethod
+    def __fore_front_service(prompt: str, **kwargs) -> str:
+        return forefront.Completion.create(prompt=prompt, **kwargs).text
+
+    @staticmethod
+    def __theb_service(prompt: str, **kwargs):
+        return ''.join(theb.Completion.create(prompt=prompt))
+
+    @staticmethod
+    def __cocalc_service(prompt: str, **kwargs):
+        return cocalc.Completion.create(prompt, cookie_input=kwargs.get('cookie_input', '')).text
```

### Comparing `gpt4free-0.1.3/gpt4free/cocalc/__init__.py` & `gpt4free-0.1.4/gpt4free/cocalc/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/gpt4free/forefront/__init__.py` & `gpt4free-0.1.4/gpt4free/forefront/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/gpt4free/theb/__init__.py` & `gpt4free-0.1.4/gpt4free/theb/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/gpt4free/usesless/__init__.py` & `gpt4free-0.1.4/gpt4free/usesless/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/gpt4free/you/__init__.py` & `gpt4free-0.1.4/gpt4free/you/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.3/gpt4free.egg-info/PKG-INFO` & `gpt4free-0.1.4/gpt4free.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 0.1.3
+Version: 0.1.4
 Summary: decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's
 Home-page: https://github.com/rzashakeri/gpt4free
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free/issues
```

### Comparing `gpt4free-0.1.3/setup.py` & `gpt4free-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         "Ai"
     ],
     name='gpt4free',
     packages=find_packages(include=['gpt4free', 'gpt4free.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rzashakeri/gpt4free',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
     project_urls={
         "Homepage": "https://github.com/rzashakeri/gpt4free",
         "Issue tracker": "https://github.com/rzashakeri/gpt4free/issues",
         "Release notes": "https://github.com/rzashakeri/gpt4free/releases",
         "Source": "https://github.com/rzashakeri/gpt4free",
         "Discussions": "https://github.com/rzashakeri/gpt4free/discussions",
```

