# Comparing `tmp/ezregex-1.0.0.tar.gz` & `tmp/ezregex-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezregex-1.0.0.tar", last modified: Thu Apr 20 22:22:04 2023, max compression
+gzip compressed data, was "ezregex-1.1.0.tar", last modified: Mon May  1 20:56:02 2023, max compression
```

## Comparing `ezregex-1.0.0.tar` & `ezregex-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 22:22:04.966579 ezregex-1.0.0/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1059 2023-01-01 23:18:10.000000 ezregex-1.0.0/LICENSE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 21:53:36.000000 ezregex-1.0.0/LICENSE-APACHE
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 21:53:36.000000 ezregex-1.0.0/LICENSE-MIT
--rw-r--r--   0 leonard   (1000) leonard   (1000)       77 2023-04-20 21:53:36.000000 ezregex-1.0.0/MANIFEST.in
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4075 2023-04-20 22:22:04.966579 ezregex-1.0.0/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3024 2023-04-20 22:19:31.000000 ezregex-1.0.0/README.md
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 22:22:04.966579 ezregex-1.0.0/ezregex/
--rw-r--r--   0 leonard   (1000) leonard   (1000)      794 2022-06-23 20:20:47.000000 ezregex-1.0.0/ezregex/EasyRegexFunctionCall.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     6198 2023-04-19 21:55:00.000000 ezregex-1.0.0/ezregex/EasyRegexMember.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     1276 2023-04-19 21:35:33.000000 ezregex-1.0.0/ezregex/EasyRegexSingleton.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)      180 2022-06-23 20:21:19.000000 ezregex-1.0.0/ezregex/RegexDialect.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)     7458 2023-04-20 21:59:20.000000 ezregex-1.0.0/ezregex/__init__.py
--rw-r--r--   0 leonard   (1000) leonard   (1000)    11236 2023-04-19 21:55:23.000000 ezregex-1.0.0/ezregex/invert.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 22:22:04.966579 ezregex-1.0.0/ezregex.egg-info/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     4075 2023-04-20 22:22:04.000000 ezregex-1.0.0/ezregex.egg-info/PKG-INFO
--rw-r--r--   0 leonard   (1000) leonard   (1000)      371 2023-04-20 22:22:04.000000 ezregex-1.0.0/ezregex.egg-info/SOURCES.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-04-20 22:22:04.000000 ezregex-1.0.0/ezregex.egg-info/dependency_links.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)        8 2023-04-20 22:22:04.000000 ezregex-1.0.0/ezregex.egg-info/top_level.txt
--rw-r--r--   0 leonard   (1000) leonard   (1000)      448 2023-04-20 22:15:02.000000 ezregex-1.0.0/pyproject.toml
--rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-04-20 22:22:04.966579 ezregex-1.0.0/setup.cfg
--rw-r--r--   0 leonard   (1000) leonard   (1000)     2136 2023-04-20 22:21:57.000000 ezregex-1.0.0/setup.py
-drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-04-20 22:22:04.966579 ezregex-1.0.0/tests/
--rw-r--r--   0 leonard   (1000) leonard   (1000)     3869 2023-03-17 20:44:22.000000 ezregex-1.0.0/tests/tests.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1059 2023-01-01 23:18:10.000000 ezregex-1.1.0/LICENSE
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     9755 2023-04-20 21:53:36.000000 ezregex-1.1.0/LICENSE-APACHE
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     1072 2023-04-20 21:53:36.000000 ezregex-1.1.0/LICENSE-MIT
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       77 2023-04-20 21:53:36.000000 ezregex-1.1.0/MANIFEST.in
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     4215 2023-05-01 20:56:02.082066 ezregex-1.1.0/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     3164 2023-04-21 23:10:33.000000 ezregex-1.1.0/README.md
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/ezregex/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      277 2023-04-21 00:07:40.000000 ezregex-1.1.0/ezregex/EZRegexFunctionCall.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     7433 2023-04-21 23:16:41.000000 ezregex-1.1.0/ezregex/EZRegexMember.py
+-rw-------   0 leonard   (1000) leonard   (1000)     6928 2023-05-01 20:54:57.000000 ezregex-1.1.0/ezregex/__init__.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      152 2023-04-21 23:14:52.000000 ezregex-1.1.0/ezregex/_escapeChars.py
+-rw-r--r--   0 leonard   (1000) leonard   (1000)    11233 2023-04-21 23:15:12.000000 ezregex-1.1.0/ezregex/invert.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/ezregex.egg-info/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     4215 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/PKG-INFO
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      337 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/SOURCES.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        1 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/dependency_links.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)        8 2023-05-01 20:56:02.000000 ezregex-1.1.0/ezregex.egg-info/top_level.txt
+-rw-r--r--   0 leonard   (1000) leonard   (1000)      448 2023-05-01 20:55:15.000000 ezregex-1.1.0/pyproject.toml
+-rw-r--r--   0 leonard   (1000) leonard   (1000)       38 2023-05-01 20:56:02.082066 ezregex-1.1.0/setup.cfg
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     2136 2023-04-20 22:21:57.000000 ezregex-1.1.0/setup.py
+drwxr-xr-x   0 leonard   (1000) leonard   (1000)        0 2023-05-01 20:56:02.082066 ezregex-1.1.0/tests/
+-rw-r--r--   0 leonard   (1000) leonard   (1000)     3537 2023-04-21 23:01:44.000000 ezregex-1.1.0/tests/tests.py
```

### Comparing `ezregex-1.0.0/LICENSE` & `ezregex-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.0.0/LICENSE-APACHE` & `ezregex-1.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ezregex-1.0.0/LICENSE-MIT` & `ezregex-1.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `ezregex-1.0.0/PKG-INFO` & `ezregex-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezregex
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/smartycope/EasyRegex
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
 Classifier: Development Status :: 4 - Beta
@@ -34,32 +34,34 @@
 **Table of Contents**
 
 * [Installation](#installation)
 * [License](#license)
 
 ## Usage:
 ```
-    optionalParams = multiOptional(match(',') + whitechunk() + chunk())
-    regex = stuff() + 'test(' + ifFollowedBy(match('ing') + optionalParams)
-    regex.test('Testing test(ing, ?) + test-ing!')
+    import ezregex as er
+    optW = er.optional(er.whitechunk)
+    optionalParams = er.multiOptional(optW + er.group(er.optional(er.chunk)) + optW + er.match(','))
+    function = er.stuff + 'func(' + er.ifFollowedBy(optionalParams) + ')'
+    function.test('this should match only the func(param1, param2 ) part of this string')
 ```
 
 ## Current limitations
 - inverse() doesn't work well with broken up chains. A large code refactoring would be required. So to get proper
     inverting on broken up functions, you have to put .inverse() at the end of every chain, before it enters the main chain.
     This will mess up your end result however, so use only for debugging purposes.
 - inverse() is also not totally function yet? It's closish, but currently only works on simple regex expressions
 - The "not" operator doesn't currently work. Another large code refactoring would be required.
 - Everything is kinda just mushed together as generic dialect. Separating of python and generic dialects would be helpful.
 - The Perl dialect isn't implemented at all. I don't know any perl, but this is meant to be a cross-platform solution.
 
 ## Explination of How it Works
 This is version 2. The original version just had an EasyRegex class with a bunch of members that returned self, then you chained together member function calls.
 
-This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in this file, specifying lambdas (or strings, for convenience) describing how they interact with the regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialog lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
+This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in __init__.py, specifying lambdas (or strings, for convenience) describing how they interact with the current regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialect lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
 
 
 ## Installation
 
 ezregex is distributed on [PyPI](https://pypi.org) as a universal
 wheel and is available on Linux/macOS and Windows and supports
 Python 3.10+ and PyPy.
```

### Comparing `ezregex-1.0.0/README.md` & `ezregex-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 **Table of Contents**
 
 * [Installation](#installation)
 * [License](#license)
 
 ## Usage:
 ```
-    optionalParams = multiOptional(match(',') + whitechunk() + chunk())
-    regex = stuff() + 'test(' + ifFollowedBy(match('ing') + optionalParams)
-    regex.test('Testing test(ing, ?) + test-ing!')
+    import ezregex as er
+    optW = er.optional(er.whitechunk)
+    optionalParams = er.multiOptional(optW + er.group(er.optional(er.chunk)) + optW + er.match(','))
+    function = er.stuff + 'func(' + er.ifFollowedBy(optionalParams) + ')'
+    function.test('this should match only the func(param1, param2 ) part of this string')
 ```
 
 ## Current limitations
 - inverse() doesn't work well with broken up chains. A large code refactoring would be required. So to get proper
     inverting on broken up functions, you have to put .inverse() at the end of every chain, before it enters the main chain.
     This will mess up your end result however, so use only for debugging purposes.
 - inverse() is also not totally function yet? It's closish, but currently only works on simple regex expressions
 - The "not" operator doesn't currently work. Another large code refactoring would be required.
 - Everything is kinda just mushed together as generic dialect. Separating of python and generic dialects would be helpful.
 - The Perl dialect isn't implemented at all. I don't know any perl, but this is meant to be a cross-platform solution.
 
 ## Explination of How it Works
 This is version 2. The original version just had an EasyRegex class with a bunch of members that returned self, then you chained together member function calls.
 
-This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in this file, specifying lambdas (or strings, for convenience) describing how they interact with the regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialog lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
+This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in __init__.py, specifying lambdas (or strings, for convenience) describing how they interact with the current regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialect lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
 
 
 ## Installation
 
 ezregex is distributed on [PyPI](https://pypi.org) as a universal
 wheel and is available on Linux/macOS and Windows and supports
 Python 3.10+ and PyPy.
```

### Comparing `ezregex-1.0.0/ezregex/invert.py` & `ezregex-1.1.0/ezregex/invert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from random import randint, choice, choices
 import re
-from .EasyRegexMember import escapeChars
+from ._escapeChars import escapeChars
 
 # from Cope import debug, todo, percent; todo('remove this')
 
 def unsanitize(string):
     for part in escapeChars:
         string = re.sub(r'\\' + part, part[1], string)
     return string
```

### Comparing `ezregex-1.0.0/ezregex.egg-info/PKG-INFO` & `ezregex-1.1.0/ezregex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezregex
-Version: 1.0.0
+Version: 1.1.0
 Home-page: https://github.com/smartycope/EasyRegex
 Author: Copeland Carter
 Author-email: smartycope@gmail.com
 Maintainer: Copeland Carter
 Maintainer-email: smartycope@gmail.com
 License: MIT/Apache-2.0
 Classifier: Development Status :: 4 - Beta
@@ -34,32 +34,34 @@
 **Table of Contents**
 
 * [Installation](#installation)
 * [License](#license)
 
 ## Usage:
 ```
-    optionalParams = multiOptional(match(',') + whitechunk() + chunk())
-    regex = stuff() + 'test(' + ifFollowedBy(match('ing') + optionalParams)
-    regex.test('Testing test(ing, ?) + test-ing!')
+    import ezregex as er
+    optW = er.optional(er.whitechunk)
+    optionalParams = er.multiOptional(optW + er.group(er.optional(er.chunk)) + optW + er.match(','))
+    function = er.stuff + 'func(' + er.ifFollowedBy(optionalParams) + ')'
+    function.test('this should match only the func(param1, param2 ) part of this string')
 ```
 
 ## Current limitations
 - inverse() doesn't work well with broken up chains. A large code refactoring would be required. So to get proper
     inverting on broken up functions, you have to put .inverse() at the end of every chain, before it enters the main chain.
     This will mess up your end result however, so use only for debugging purposes.
 - inverse() is also not totally function yet? It's closish, but currently only works on simple regex expressions
 - The "not" operator doesn't currently work. Another large code refactoring would be required.
 - Everything is kinda just mushed together as generic dialect. Separating of python and generic dialects would be helpful.
 - The Perl dialect isn't implemented at all. I don't know any perl, but this is meant to be a cross-platform solution.
 
 ## Explination of How it Works
 This is version 2. The original version just had an EasyRegex class with a bunch of members that returned self, then you chained together member function calls.
 
-This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in this file, specifying lambdas (or strings, for convenience) describing how they interact with the regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialog lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
+This version uses a bunch of constant singletons (of type EasyRegexSingleton) that have the __call__() dunder function overridden to return a separate class (EasyRegexMember) which override the __add__() and __str__() dunder functions. What happens is you have all the singletons created in __init__.py, specifying lambdas (or strings, for convenience) describing how they interact with the current regex expression, and then optional inverted lambdas (get to that in a moment) and separate dialect lambdas. When those are called later on by the user, (they can be treated like regular functions) they initialize a EasyRegexMember, and give it the function they hold. Then, EasyRegexMembers are chained together with +'s (or <<'s). EasyRegexMembers all have internal ordered lists of functions that get added to when +'ed. If you assign the chain (or chains!) to a varaible or put in ()'s, what you end up with is one EasyRegexMember that has an ordered list of all the functions from all the EasyRegexMembers in that chain. When you then cast that to a string (or call .str() or .compile()), it finally goes through and calls all those functions, which results in the final regex string.
 
 
 ## Installation
 
 ezregex is distributed on [PyPI](https://pypi.org) as a universal
 wheel and is available on Linux/macOS and Windows and supports
 Python 3.10+ and PyPy.
```

### Comparing `ezregex-1.0.0/setup.py` & `ezregex-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.0.0/tests/tests.py` & `ezregex-1.1.0/tests/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-from EasyRegex import *
-from EasyRegex.invert import *
-# from .invert import *
-# from .__init__ import *
+from ezregex import *
+from ezregex.invert import *
 import re
 # from Cope import *
 
 # todo('test invert of (stuff)? some more (it might be always removing it)')
 # todo('invert notAnyCha/rs ([^s,t]) failed, it selected a char specified')
 # todo('invert [:punct:]')
 # todo('invert colors dont work')
 # todo('add a letter singleton')
 
-
 def runTests(singletons=True, invert=True, unsanitize_=False, unitTests=False, strictness=20):
-    # test = word() + whitespace() # + whiteChunk()
-    # test = wordChar() + whitespace()
-    # test = wordChar()
-    # str(test)
-    # debug()
-    # return
-
-    ow = optional(whitechunk())
-    # debug()
-    w = whitechunk()
+    ow = optional(whitechunk)
+    w = whitechunk
     regexs = [
-        'stuff' + anyof('a', 'b', 'c') + ' ' + optional(comma()) + space() + ifFollowedBy('*'),
-        optional(word() + ow + ':' + ow) + group(word()) + optional(',') + ow,
-        optional(w + 'as' + word()),
-        group(optional(matchMax(match('.') + word()))),
+        'stuff' + anyof('a', 'b', 'c') + ' ' + optional(comma) + space + ifFollowedBy('*'),
+        optional(word + ow + ':' + ow) + group(word) + optional(',') + ow,
+        optional(w + 'as' + word),
+        group(optional(matchMax(match('.') + word))),
         matchNum(3, either("'", '"')),
         raw(r'\A'),
         raw(r'\Z'),
         exactly('test'),
         raw(r'(test)+'),
         raw(r'test+'),
         raw(r'(test){3}'),
@@ -64,38 +53,36 @@
         raw(r'(?!stuff)'),
         raw(r'(stuff)'),
         raw(r'(?:stuff)'),
         raw(r'(?P<name>stuff)'),
         raw(r'(?<=stuff)'),
         raw(r'(?<!stuff)'),
         raw(r'(a|b|c|thing|st)uff'),
-        # ifEnclosedWith('(', namedGroup('stuff', word()), ')')
+        # ifEnclosedWith('(', namedGroup('stuff', word), ')')
     ]
 
     shouldMatch = [
         (
             'stuffa , *',
             'stuffb  *',
         ),
     ]
 
     if singletons:
-        # debug("Testing EasyRegex Singletons:", color=2)
         print("Testing EasyRegex Singletons:")
 
-        test = word() + whiteChunk()
+        test = word + whiteChunk
         assert str(test) == '\w+\s+'
         # debug(test)
         print(test)
         # str(test)
         # debug()
         # return
 
         for cnt, r in enumerate(regexs):
-            # r.debug()
             if cnt < len(shouldMatch):
                 for should in shouldMatch[cnt]:
                     assert r.test(should)
 
     if unsanitize_:
         print("Testing unsantize:")
         # debug("Testing unsantize:", color=2)
```

