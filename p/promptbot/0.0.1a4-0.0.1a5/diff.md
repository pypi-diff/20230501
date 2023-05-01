# Comparing `tmp/promptbot-0.0.1a4.tar.gz` & `tmp/promptbot-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptbot-0.0.1a4.tar", last modified: Sun Apr 30 16:24:25 2023, max compression
+gzip compressed data, was "promptbot-0.0.1a5.tar", last modified: Mon May  1 06:41:03 2023, max compression
```

## Comparing `promptbot-0.0.1a4.tar` & `promptbot-0.0.1a5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cbezui     (502) staff       (20)        0 2023-04-30 16:24:25.846793 promptbot-0.0.1a4/
--rw-r--r--   0 cbezui     (502) staff       (20)     1076 2023-04-30 10:31:49.000000 promptbot-0.0.1a4/LICENSE
--rw-r--r--   0 cbezui     (502) staff       (20)     3467 2023-04-30 16:24:25.846635 promptbot-0.0.1a4/PKG-INFO
--rw-r--r--   0 cbezui     (502) staff       (20)     3000 2023-04-30 15:38:08.000000 promptbot-0.0.1a4/README.md
-drwxr-xr-x   0 cbezui     (502) staff       (20)        0 2023-04-30 16:24:25.845123 promptbot-0.0.1a4/promptbot/
--rw-r--r--   0 cbezui     (502) staff       (20)       29 2023-04-30 15:38:08.000000 promptbot-0.0.1a4/promptbot/__init__.py
--rw-r--r--   0 cbezui     (502) staff       (20)     1031 2023-04-30 15:38:08.000000 promptbot-0.0.1a4/promptbot/api.py
--rw-r--r--   0 cbezui     (502) staff       (20)     1471 2023-04-30 15:38:08.000000 promptbot-0.0.1a4/promptbot/classes.py
--rw-r--r--   0 cbezui     (502) staff       (20)     8573 2023-04-30 15:38:08.000000 promptbot-0.0.1a4/promptbot/prompt.py
-drwxr-xr-x   0 cbezui     (502) staff       (20)        0 2023-04-30 16:24:25.846369 promptbot-0.0.1a4/promptbot.egg-info/
--rw-r--r--   0 cbezui     (502) staff       (20)     3467 2023-04-30 16:24:25.000000 promptbot-0.0.1a4/promptbot.egg-info/PKG-INFO
--rw-r--r--   0 cbezui     (502) staff       (20)      270 2023-04-30 16:24:25.000000 promptbot-0.0.1a4/promptbot.egg-info/SOURCES.txt
--rw-r--r--   0 cbezui     (502) staff       (20)        1 2023-04-30 16:24:25.000000 promptbot-0.0.1a4/promptbot.egg-info/dependency_links.txt
--rw-r--r--   0 cbezui     (502) staff       (20)       44 2023-04-30 16:24:25.000000 promptbot-0.0.1a4/promptbot.egg-info/requires.txt
--rw-r--r--   0 cbezui     (502) staff       (20)       10 2023-04-30 16:24:25.000000 promptbot-0.0.1a4/promptbot.egg-info/top_level.txt
--rw-r--r--   0 cbezui     (502) staff       (20)       38 2023-04-30 16:24:25.846854 promptbot-0.0.1a4/setup.cfg
--rw-r--r--   0 cbezui     (502) staff       (20)      838 2023-04-30 16:24:18.000000 promptbot-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/promptbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/promptbot/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/promptbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 06:41:03.000000 promptbot-0.0.1a5/promptbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:41:03.864810 promptbot-0.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 06:40:46.000000 promptbot-0.0.1a5/setup.py
```

### Comparing `promptbot-0.0.1a4/LICENSE` & `promptbot-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a4/PKG-INFO` & `promptbot-0.0.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
-Home-page: UNKNOWN
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # promptbot
@@ -97,7 +94,10 @@
                             f'{{ "step": "2", "task": "The 2nd task I create"}}]')
 
     def start(self, text):
         self.set_goal(text)
         return self.run_ai()
 ```
 
+## Documentation
+
+You can find the documentation for promptbot in the `/docs` directory.
```

### Comparing `promptbot-0.0.1a4/README.md` & `promptbot-0.0.1a5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,8 +80,12 @@
         self.add_rule("I must output only in the example format.")
         self.set_example_output(f'[{{ "step": "1", "task": "The 1st task I create"}},'
                             f'{{ "step": "2", "task": "The 2nd task I create"}}]')
 
     def start(self, text):
         self.set_goal(text)
         return self.run_ai()
-```
+```
+
+## Documentation
+
+You can find the documentation for promptbot in the `/docs` directory.
```

### Comparing `promptbot-0.0.1a4/promptbot/api.py` & `promptbot-0.0.1a5/promptbot/api.py`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a4/promptbot/classes.py` & `promptbot-0.0.1a5/promptbot/classes.py`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a4/promptbot/prompt.py` & `promptbot-0.0.1a5/promptbot/prompt.py`

 * *Files identical despite different names*

### Comparing `promptbot-0.0.1a4/promptbot.egg-info/PKG-INFO` & `promptbot-0.0.1a5/promptbot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: promptbot
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: A Python package for generating prompt bots on top of OpenAI GTP Apis.
-Home-page: UNKNOWN
 Author: Clayton Bezuidenhout
 Author-email: claytonbez.nl@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # promptbot
@@ -97,7 +94,10 @@
                             f'{{ "step": "2", "task": "The 2nd task I create"}}]')
 
     def start(self, text):
         self.set_goal(text)
         return self.run_ai()
 ```
 
+## Documentation
+
+You can find the documentation for promptbot in the `/docs` directory.
```

### Comparing `promptbot-0.0.1a4/setup.py` & `promptbot-0.0.1a5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 import os
 
 from setuptools import setup
 
-requirements = [
-    "toml==0.10.2",
-    "openai==0.27.5",
-    "colorama==0.4.6",
-]
-
-curdir = os.path.dirname(__file__)
-
-requirements = open(os.path.join(curdir, 'requirements.txt')).read()
-
-readme = open(os.path.join(curdir, 'README.md')).read()
+cwd = os.path.dirname(__file__)
+requirements = open(os.path.join(cwd, 'requirements.txt')).read()
+readme = open(os.path.join(cwd, 'README.md')).read()
 
 setup(
     name='promptbot',
-    version='0.0.1-alpha.4',
+    version='0.0.1-alpha.5',
     author='Clayton Bezuidenhout',
     author_email='claytonbez.nl@gmail.com',
     description='A Python package for generating prompt bots on top of OpenAI GTP Apis.',
     long_description=f"""{readme}""",
     long_description_content_type='text/markdown',
     packages=['promptbot'],
     install_requires=requirements,
```

