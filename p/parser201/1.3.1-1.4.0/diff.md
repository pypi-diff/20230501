# Comparing `tmp/parser201-1.3.1.tar.gz` & `tmp/parser201-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parser201-1.3.1.tar", max compression
+gzip compressed data, was "parser201-1.4.0.tar", max compression
```

## Comparing `parser201-1.3.1.tar` & `parser201-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1074 2022-10-22 00:30:01.195716 parser201-1.3.1/LICENSE
--rw-r--r--   0        0        0     4094 2022-10-22 17:34:25.763016 parser201-1.3.1/README.md
--rw-r--r--   0        0        0     1549 2022-10-22 17:30:42.250088 parser201-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      399 2022-10-22 17:30:42.597926 parser201-1.3.1/src/parser201/__init__.py
--rw-r--r--   0        0        0    11492 2022-10-22 00:30:01.199712 parser201-1.3.1/src/parser201/classes.py
--rw-r--r--   0        0        0     4861 1970-01-01 00:00:00.000000 parser201-1.3.1/setup.py
--rw-r--r--   0        0        0     5698 1970-01-01 00:00:00.000000 parser201-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-30 20:20:31.148592 parser201-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4454 2023-04-30 22:23:05.969168 parser201-1.4.0/README.md
+-rw-r--r--   0        0        0     1657 2023-04-30 20:20:31.152590 parser201-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-04-30 20:20:31.156589 parser201-1.4.0/src/parser201/__init__.py
+-rw-r--r--   0        0        0    10446 2023-04-30 20:29:04.112043 parser201-1.4.0/src/parser201/classes.py
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 parser201-1.4.0/PKG-INFO
```

### Comparing `parser201-1.3.1/LICENSE` & `parser201-1.4.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022, Peter Nardi
+Copyright (c) 2020-2023, Peter Nardi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `parser201-1.3.1/README.md` & `parser201-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 
 <br>
 
 <img src="https://github.com/geozeke/parser201/blob/main/docs/logo.png?raw=true" width="120"/>
 
 ## Features
 
-The centerpiece of the parser201 module is the LogParser class. The class initializer takes a single line from an Apache access log file and extracts the individual fields into attributes within an object.
+The centerpiece of the parser201 module is the LogParser class. The class
+initializer takes a single line from an Apache access log file and extracts the
+individual fields into attributes within an object.
 
 ## Installation
 
 ```text
 pip3 install parser201
 ```
 
 ## Usage
 
-The most common use-case for parser201 is importing individual lines from an Apache access log file and creating LogParser objects, like this:
+The most common use-case for parser201 is importing individual lines from an
+Apache access log file and creating LogParser objects, like this:
 
 ```python
 from parser201 import LogParser
 
 with open('access.log', 'r') as f:
     for line in f:
         lp = LogParser(line)
@@ -36,62 +39,80 @@
 
 ## Documentation
 
 See: [parser201 Documentation](https://geozeke.github.io/parser201).
 
 ## Version History
 
+* 1.4.0 (2023-04-30)
+  * Strengthened regular expression parsing to handle log lines that
+    contain a wider array of malicious attacks.
+  * Added support for access logs that contain both IPv4 and IPv6
+    addresses.
+  * Minimum supported Python version is now 3.8 (^3.8).
+  * Miscellaneous optimizations.<br><br>
 * 1.3.1 (2022-10-22)
-  * Migrated dependency/build management to [poetry](https://python-poetry.org/).<br><br>
+  * Migrated dependency/build management to
+    [poetry](https://python-poetry.org/).<br><br>
 * 1.3.0 (2022-08-13)
   * Implemented `__eq__` magic method for the `LogParser` class. You can now
     perform equality checks on two `LogParser` objects.
   * Added test cases for `__eq__`
   * Migrated task runner to `make`
   * Documentation cleanup
   * Code linting and cleanup<br><br>
 * 1.2.0 (2022-07-17)
   * Implemented `__eq__` magic methods in the `FMT` and `TZ` classes.
   * Documentation cleanup.
-  * Testing improvements and pyproject.toml adjustments for better pytest compatability.
+  * Testing improvements and pyproject.toml adjustments for better pytest
+    compatability.
   * Code linting and cleanup.<br><br>
 * 1.1.5 (2022-01-17)
   * Code linting and cleanup.<br><br>
 * 1.1.4 (2021-12-23)
   * Documentation cleanup.<br><br>
 * 1.1.3 (2021-12-19)
   * Make file tuning.
   * Documentation cleanup.
   * Added site logo to README.md.<br><br>
 * 1.1.0 (2021-11-13)
-  * Implemented selectable timestamp conversion options {*original*, *local*, [*UTC*](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)}.
-  * Implemented selectable formatting options for timestamp attribute {*string*, *date_obj*}.
+  * Implemented selectable timestamp conversion options {*original*, *local*,
+    [*UTC*](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)}.
+  * Implemented selectable formatting options for timestamp attribute
+    {*string*, *date_obj*}.
   * Migrated API reference to GitHub pages.
   * Code cleanup.<br><br>
 * 1.0.2 (2021-11-05)
   * Documentation cleanup.<br><br>
 * 1.0.0 (2021-11-04)
   * Stable production release.
   * Migrated to a new development framework.
   * Implemented more robust and compartmentalized test cases.
   * Code tuning.<br><br>
 * 0.2.0 (2021-10-31)
-  * Changed behavior to gracefully fail for any malformed input line. If an input line cannot be successfully parsed, all attributes of the returned object are set to `None` and no messages are printed.
+  * Changed behavior to gracefully fail for any malformed input line. If an
+    input line cannot be successfully parsed, all attributes of the returned
+    object are set to `None` and no messages are printed.
   * Added additional pytest cases to verify failure behavior.<br><br>
 * 0.1.9 (2021-09-15)
   * Code cleanup for pep8 compliance.
-  * Cleaned up Makefiles and scripts to remove references to python (meaning python2) and replace it with python3.<br><br>
+  * Cleaned up Makefiles and scripts to remove references to python (meaning
+    python2) and replace it with python3.<br><br>
 * 0.1.7 (2021-06-05)
-  * Re-tooled testing scripts to use parameterized test data, and conduct more robust testing.<br><br>
+  * Re-tooled testing scripts to use parameterized test data, and conduct more
+    robust testing.<br><br>
 * 0.1.6 (2020-12-19)
-  * Addressed exception handling for initializer input not being a valid string data type.
+  * Addressed exception handling for initializer input not being a valid string
+    data type.
   * Documentation cleanup.<br><br>
 * 0.1.5 (2020-10-26)
-  * Enabled automatic deployment of tagged releases to pypi from travis using encrypted token.
-  * Converted references to the master branch in the git repository to main across the documentation set.
+  * Enabled automatic deployment of tagged releases to pypi from travis using
+    encrypted token.
+  * Converted references to the master branch in the git repository to main
+    across the documentation set.
   * Documentation cleanup.<br><br>
 * 0.1.4 (2020-10-24)
   * Initial pypi release.
   * Fixed test file filtering issue in .gitignore.
   * Dependency fix for travis tests.<br><br>
 * 0.1.1 (2020-10-22)
   * Follow-on testing on test.pypi.org.<br><br>
```

### Comparing `parser201-1.3.1/pyproject.toml` & `parser201-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 [tool.poetry]
 name = "parser201"
-version = "1.3.1"
+version = "1.4.0"
 description = "Extract individual fields from lines in Apache access logs"
 authors = ["Peter Nardi <pete@nardi.com>"]
 maintainers = ["Peter Nardi <pete@nardi.com>"]
 license = "MIT"
 readme = "README.md"
+packages = [{ include = "parser201", from = "src" }]
 homepage = "https://github.com/geozeke/parser201"
 keywords = [
 	"parser201",
 	"apache",
 	"log",
 	"parse",
 	"parser",
 	"scanner",
 	"web",
-	"server"
+	"server",
 ]
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Education",
 	"Intended Audience :: Developers",
 	"Intended Audience :: System Administrators",
 	"License :: OSI Approved :: MIT License",
 	"Natural Language :: English",
 	"Operating System :: OS Independent",
 	"Topic :: Education",
 	"Topic :: Internet :: Log Analysis",
 	"Topic :: Security",
 	"Topic :: System :: Logging",
 	"Topic :: System :: Systems Administration",
-	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+	"Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/geozeke/parser201"
 "Bug Tracker" = "https://github.com/geozeke/parser201/issues"
 "Documentation" = "https://geozeke.github.io/parser201"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 pytest = "^7.1.3"
 autopep8 = "^1.7.0"
 flake8 = "^5.0.4"
 flake8-docstrings = "^1.6.0"
 mypy = "^0.982"
 pdoc3 = "^0.10.0"
 
 [tool.pytest.ini_options]
-pythonpath = [
-    "src/parser201"
-]
+pythonpath = [".", "./src", "./src/parser201"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `parser201-1.3.1/src/parser201/classes.py` & `parser201-1.4.0/src/parser201/classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,99 +135,99 @@
     will be stored as a Python [datetime object](https:\
     //docs.python.org/3/library/datetime.html).
     >>> from parser201 import LogParser, TZ, FMT
     >>> line = # a line from an Apache access log
     >>> lp = LogParser(line, timezone=TZ.local, dts_format=FMT.date_obj)
     """
 
+    # Class variables
+
+    # Behold the power of generative AI. I provided the following query to
+    # ChatGPT: "Write a regular expression that recognizes a line from an
+    # apache access log". I had to have a "conversation" with ChatGPT to refine
+    # the regex with a few examples, but after a brief exchange, it produced
+    # what you see below. This regex cleaned up my previous solution and
+    # replace several lines of code. I split the regex into individual match
+    # groups here to make it easier to follow.
+    _ip = r'^([^ ]+)'
+    _ui = r'(\S+)'
+    _un = r'(\S+)'
+    _ts = r'\[([^\]]+)\]'
+    _rl = r'"(.*?)"'
+    _sc = r'(\d{3})'
+    _ds = r'(\S+)'
+    _re = r'"((?:[^"]|\")*?)"'
+    _ua = r'"((?:[^"]|\")*?|-)"'
+    _regex = fr'{_ip} {_ui} {_un} {_ts} {_rl} {_sc} {_ds} {_re} {_ua}'
+
+    # A list of labels (in the correct order) used to render string
+    # representations of LogParser objects. Also calculate the length of the
+    # longest label so we can use f-strings to right-justify all the labels.
+    _labels = [
+        'ipaddress',
+        'userid',
+        'username',
+        'timestamp',
+        'requestline',
+        'statuscode',
+        'datasize',
+        'referrer',
+        'useragent'
+    ]
+    _pad = len(max(_labels, key=len))
+
     def __init__(self, line, timezone=TZ.original, dts_format=FMT.string):
 
-        # Establish attributes
-        self.ipaddress = ''
-        self.userid = ''
-        self.username = ''
-        self.timestamp = ''
-        self.requestline = ''
-        self.referrer = ''
-        self.useragent = ''
-        self.statuscode = 0
-        self.datasize = 0
+        # Initialize data fields
+        self.ipaddress: str = ''
+        self.userid: str = ''
+        self.username: str = ''
+        self.timestamp: str = ''
+        self.requestline: str = ''
+        self.statuscode: int = 0
+        self.datasize: int = 0
+        self.referrer: str = ''
+        self.useragent: str = ''
 
-        # Initial check. If the line passed to the initializer is not a string
-        # (type == str), then return an empty LogParser object.
         if type(line) != str:
             self.__none_fields()
             return
 
-        # If a valid string is entered, then perform pre-processing. For some
-        # lines, an empty field is represented as two quotes back-to-back, like
-        # this: "". The regex to pull out agent strings between quotes will
-        # incorrectly ignore that field, rather than returning an empty string.
-        # Replace "" with "-" to prevent that.
-        clean = line.replace('\"\"', '\"-\"')
-
-        # agent_strings: This part of the regex:(?<!\\)\" is a negative
-        # lookbehind assertion. It says, "end with a quote mark, unless that
-        # quote mark is preceded by an escape character '\'"
-        agent_strings = re.findall(r'\"(.+?)(?<!\\)\"', clean)
-
-        # The next one's tricky. We're looking to extract the statuscode and
-        # datasize fields. For some entires, the datasize field is '-', but for
-        # all entries the returncode field is a reliable integer. If we split
-        # the log line on space, then the first purely isnumeric() item in the
-        # resulting list should be the returncode. If we capture the index of
-        # that code, and take that code and the one next to it from the list,
-        # we should have both fields. If the fields are valid integers, then
-        # cast to them int; else set them to 0. If any of this fails, then
-        # consider that we have a malformed log line and set all the properties
-        # to None.
-        try:
-            L = clean.split(' ')
-            i = [j for j in range(len(L)) if L[j].isnumeric()][0]
-            code_and_size = [int(n) if n.isnumeric() else 0 for n in L[i:i+2]]
-            # Splitting on '[' returns a list where item [0] contains the first
-            # three fields (ipaddress; userid; username), each separated by
-            # space.
-            first3 = clean.split('[')[0].split()
-        except Exception:
-            self.__none_fields()
-            return
-
-        # Set properties. If any of these fail, then consider that we have a
-        # malformed log line and set all the properties to None.
-        try:
-            self.ipaddress = first3[0]
-            self.userid = first3[1]
-            self.username = first3[2]
-            self.timestamp = re.search(
-                r'\[(.+?)\]', clean).group().strip('[]')
-            self.requestline = agent_strings[0]
-            self.referrer = agent_strings[1]
-            self.useragent = agent_strings[2]
-            self.statuscode = code_and_size[0]
-            self.datasize = code_and_size[1]
-        except Exception:
+        if (groups := re.match(LogParser._regex, line)):
+            self.ipaddress = groups.group(1)
+            self.userid = groups.group(2)
+            self.username = groups.group(3)
+            self.timestamp = groups.group(4)
+            self.requestline = groups.group(5)
+            self.statuscode = int(groups.group(6))
+            try:
+                self.datasize = int(groups.group(7))
+            except ValueError:
+                self.datasize = 0
+            self.referrer = groups.group(8)
+            self.useragent = groups.group(9)
+        else:
             self.__none_fields()
             return
 
-        # Process date/time stamp and adjust timezone/dts_format as indicated
-        if timezone == TZ.original and dts_format == FMT.string:
-            return
-
+        # This takes the work of ensuring valid date-time stamps from the regex
+        # and guarantees things like "Feb 31" will be handled as an invalid
+        # date.
         try:
             date_obj = dt.datetime.strptime(self.timestamp,
                                             '%d/%b/%Y:%H:%M:%S %z')
         except ValueError:
             self.__none_fields()
             return
 
+        # Process date/time stamp and adjust timezone/dts_format as indicated
         sign, hh, mm = self.__decomposeTZ(self.timestamp)
-
         if timezone == TZ.original:
-            pass
+            if dts_format == FMT.string:
+                return
         elif timezone == TZ.local:
             zone_str = time.strftime('%z')
             # First convert to GMT
             date_obj = date_obj + (-1*sign*dt.timedelta(hours=hh, minutes=mm))
             # Now convert to local time and replace tzinfo
             sign, hh, mm = self.__decomposeTZ(zone_str)
             zone_obj = dt.timezone(dt.timedelta(hours=hh*sign, minutes=mm))
@@ -244,16 +244,16 @@
         else:  # dts_format == FMT.date_obj
             self.timestamp = date_obj
 
         return
 
     def __none_fields(self):
         """Set all properties to None."""
-        for prop in [p for p in dir(self) if not p.startswith('_')]:
-            setattr(self, prop, None)
+        for key in vars(self):
+            setattr(self, key, None)
         return
 
     def __str__(self):
         """`LogParser` class str method.
 
         The class provides a `__str__` method which renders a
         `LogParser` object as string suitable for display.
@@ -275,24 +275,18 @@
           timestamp: 24/Mar/2009:18:07:16 +0100
         requestline: GET /images/puce.gif HTTP/1.1
          statuscode: 304
            datasize: 2454
            referrer: -
           useragent: Mozilla/4.0 compatible; MSIE 7.0; Windows NT 5.1;
         """
-        labels = ['ipaddress', 'userid', 'username', 'timestamp',
-                  'requestline', 'statuscode', 'datasize', 'referrer',
-                  'useragent']
-        pad = len(max(labels, key=len))
-        L = []
-
-        # Build the string in the same order as the labels.
-        for label in labels:
-            L.append(f'{label:>{pad}}: {getattr(self, label)}')
-        return '\n'.join(L)
+        lp_str = []
+        for label in LogParser._labels:
+            lp_str.append(f'{label:>{LogParser._pad}}: {getattr(self, label)}')
+        return '\n'.join(lp_str)
 
     def __eq__(self, other):
         """Determine if two `LogParser` objects are equal.
 
         The class provides a `__eq__` method to test for equality
         between two `LogParser` objects.
 
@@ -304,18 +298,15 @@
         Returns
         -------
         bool
             True it two `LogParser` objects are equal, False otherwise.
         """
         if type(self) != type(other):
             return False
-        for prop in [p for p in dir(self) if not p.startswith('_')]:
-            if getattr(self, prop) != getattr(other, prop):
-                return False
-        return True
+        return vars(self) == vars(other)
 
     def __decomposeTZ(self, zone):
         """Decompose a time zone into +/-, hrs, and mins."""
         leader, hrs, mins = zone[-5], zone[-4:-2], zone[-2:]
         sign = -1 if leader == '-' else 1
         return sign, int(hrs), int(mins)
```

### Comparing `parser201-1.3.1/PKG-INFO` & `parser201-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: parser201
-Version: 1.3.1
+Version: 1.4.0
 Summary: Extract individual fields from lines in Apache access logs
 Home-page: https://github.com/geozeke/parser201
 License: MIT
 Keywords: parser201,apache,log,parse,parser,scanner,web,server
 Author: Peter Nardi
 Author-email: pete@nardi.com
 Maintainer: Peter Nardi
 Maintainer-email: pete@nardi.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Systems Administration
@@ -47,25 +47,28 @@
 
 <br>
 
 <img src="https://github.com/geozeke/parser201/blob/main/docs/logo.png?raw=true" width="120"/>
 
 ## Features
 
-The centerpiece of the parser201 module is the LogParser class. The class initializer takes a single line from an Apache access log file and extracts the individual fields into attributes within an object.
+The centerpiece of the parser201 module is the LogParser class. The class
+initializer takes a single line from an Apache access log file and extracts the
+individual fields into attributes within an object.
 
 ## Installation
 
 ```text
 pip3 install parser201
 ```
 
 ## Usage
 
-The most common use-case for parser201 is importing individual lines from an Apache access log file and creating LogParser objects, like this:
+The most common use-case for parser201 is importing individual lines from an
+Apache access log file and creating LogParser objects, like this:
 
 ```python
 from parser201 import LogParser
 
 with open('access.log', 'r') as f:
     for line in f:
         lp = LogParser(line)
@@ -74,62 +77,80 @@
 
 ## Documentation
 
 See: [parser201 Documentation](https://geozeke.github.io/parser201).
 
 ## Version History
 
+* 1.4.0 (2023-04-30)
+  * Strengthened regular expression parsing to handle log lines that
+    contain a wider array of malicious attacks.
+  * Added support for access logs that contain both IPv4 and IPv6
+    addresses.
+  * Minimum supported Python version is now 3.8 (^3.8).
+  * Miscellaneous optimizations.<br><br>
 * 1.3.1 (2022-10-22)
-  * Migrated dependency/build management to [poetry](https://python-poetry.org/).<br><br>
+  * Migrated dependency/build management to
+    [poetry](https://python-poetry.org/).<br><br>
 * 1.3.0 (2022-08-13)
   * Implemented `__eq__` magic method for the `LogParser` class. You can now
     perform equality checks on two `LogParser` objects.
   * Added test cases for `__eq__`
   * Migrated task runner to `make`
   * Documentation cleanup
   * Code linting and cleanup<br><br>
 * 1.2.0 (2022-07-17)
   * Implemented `__eq__` magic methods in the `FMT` and `TZ` classes.
   * Documentation cleanup.
-  * Testing improvements and pyproject.toml adjustments for better pytest compatability.
+  * Testing improvements and pyproject.toml adjustments for better pytest
+    compatability.
   * Code linting and cleanup.<br><br>
 * 1.1.5 (2022-01-17)
   * Code linting and cleanup.<br><br>
 * 1.1.4 (2021-12-23)
   * Documentation cleanup.<br><br>
 * 1.1.3 (2021-12-19)
   * Make file tuning.
   * Documentation cleanup.
   * Added site logo to README.md.<br><br>
 * 1.1.0 (2021-11-13)
-  * Implemented selectable timestamp conversion options {*original*, *local*, [*UTC*](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)}.
-  * Implemented selectable formatting options for timestamp attribute {*string*, *date_obj*}.
+  * Implemented selectable timestamp conversion options {*original*, *local*,
+    [*UTC*](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)}.
+  * Implemented selectable formatting options for timestamp attribute
+    {*string*, *date_obj*}.
   * Migrated API reference to GitHub pages.
   * Code cleanup.<br><br>
 * 1.0.2 (2021-11-05)
   * Documentation cleanup.<br><br>
 * 1.0.0 (2021-11-04)
   * Stable production release.
   * Migrated to a new development framework.
   * Implemented more robust and compartmentalized test cases.
   * Code tuning.<br><br>
 * 0.2.0 (2021-10-31)
-  * Changed behavior to gracefully fail for any malformed input line. If an input line cannot be successfully parsed, all attributes of the returned object are set to `None` and no messages are printed.
+  * Changed behavior to gracefully fail for any malformed input line. If an
+    input line cannot be successfully parsed, all attributes of the returned
+    object are set to `None` and no messages are printed.
   * Added additional pytest cases to verify failure behavior.<br><br>
 * 0.1.9 (2021-09-15)
   * Code cleanup for pep8 compliance.
-  * Cleaned up Makefiles and scripts to remove references to python (meaning python2) and replace it with python3.<br><br>
+  * Cleaned up Makefiles and scripts to remove references to python (meaning
+    python2) and replace it with python3.<br><br>
 * 0.1.7 (2021-06-05)
-  * Re-tooled testing scripts to use parameterized test data, and conduct more robust testing.<br><br>
+  * Re-tooled testing scripts to use parameterized test data, and conduct more
+    robust testing.<br><br>
 * 0.1.6 (2020-12-19)
-  * Addressed exception handling for initializer input not being a valid string data type.
+  * Addressed exception handling for initializer input not being a valid string
+    data type.
   * Documentation cleanup.<br><br>
 * 0.1.5 (2020-10-26)
-  * Enabled automatic deployment of tagged releases to pypi from travis using encrypted token.
-  * Converted references to the master branch in the git repository to main across the documentation set.
+  * Enabled automatic deployment of tagged releases to pypi from travis using
+    encrypted token.
+  * Converted references to the master branch in the git repository to main
+    across the documentation set.
   * Documentation cleanup.<br><br>
 * 0.1.4 (2020-10-24)
   * Initial pypi release.
   * Fixed test file filtering issue in .gitignore.
   * Dependency fix for travis tests.<br><br>
 * 0.1.1 (2020-10-22)
   * Follow-on testing on test.pypi.org.<br><br>
```

