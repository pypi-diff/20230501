# Comparing `tmp/remindmail-2023.4.29.1.tar.gz` & `tmp/remindmail-2023.4.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.4.29.1.tar", last modified: Sat Apr 29 19:31:28 2023, max compression
+gzip compressed data, was "remindmail-2023.4.30.1.tar", last modified: Mon May  1 00:04:16 2023, max compression
```

## Comparing `remindmail-2023.4.29.1.tar` & `remindmail-2023.4.30.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-29 19:31:28.484501 remindmail-2023.4.29.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.29.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-04-29 19:31:28.484501 remindmail-2023.4.29.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.4.29.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.29.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-04-29 19:31:28.484501 remindmail-2023.4.29.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-29 19:31:28.480502 remindmail-2023.4.29.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-29 19:31:28.484501 remindmail-2023.4.29.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-20 02:01:45.000000 remindmail-2023.4.29.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-29 19:29:52.000000 remindmail-2023.4.29.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-19 23:29:29.000000 remindmail-2023.4.29.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    22975 2023-04-20 03:52:43.000000 remindmail-2023.4.29.1/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     7868 2023-04-20 03:40:50.000000 remindmail-2023.4.29.1/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-04-29 19:31:28.484501 remindmail-2023.4.29.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-04-29 19:31:28.000000 remindmail-2023.4.29.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-04-29 19:31:28.000000 remindmail-2023.4.29.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-04-29 19:31:28.000000 remindmail-2023.4.29.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-04-29 19:31:28.000000 remindmail-2023.4.29.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-04-29 19:31:28.000000 remindmail-2023.4.29.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 00:04:16.740718 remindmail-2023.4.30.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.30.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 00:04:16.740718 remindmail-2023.4.30.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.4.30.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.30.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-01 00:04:16.740718 remindmail-2023.4.30.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 00:04:16.736718 remindmail-2023.4.30.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 00:04:16.736718 remindmail-2023.4.30.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.4.30.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.4.30.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.4.30.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    24662 2023-04-30 22:58:45.000000 remindmail-2023.4.30.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.4.30.1/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 00:04:16.736718 remindmail-2023.4.30.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 00:04:16.000000 remindmail-2023.4.30.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-01 00:04:16.000000 remindmail-2023.4.30.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-01 00:04:16.000000 remindmail-2023.4.30.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-01 00:04:16.000000 remindmail-2023.4.30.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-01 00:04:16.000000 remindmail-2023.4.30.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.4.29.1/LICENSE.md` & `remindmail-2023.4.30.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.29.1/PKG-INFO` & `remindmail-2023.4.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.29.1
+Version: 2023.4.30.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2023.4.29.1/README.md` & `remindmail-2023.4.30.1/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.29.1/setup.cfg` & `remindmail-2023.4.30.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.04.29.1
+version = 2023.04.30.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.4.29.1/src/remind/__main__.py` & `remindmail-2023.4.30.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.29.1/src/remind/reminder.py` & `remindmail-2023.4.30.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.29.1/src/remind/remindmail.py` & `remindmail-2023.4.30.1/src/remind/remindmail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 The main class
 """
 
 import os
 import re
+import subprocess
 from enum import Enum
 from datetime import datetime
 from datetime import timedelta
 from dateutil.relativedelta import relativedelta
 from dateutil.parser import parse
 from .remindmail_utils import RemindMailUtils
 
+
 class GenerateType(Enum):
     """
     The options available for the `generate` function
 
     EMAIL will send each matching reminder
     LIST will print each matching reminder to the console
     """
     EMAIL = 'email'
     LIST = 'list'
 
+
 class RemindMail:
     """
     Contains the logic for parsing, generating, and sending reminders
     """
 
     def log_msg(self, message, level="info", path=None, print_msg=False):
         """A wrapper for cab.log to handle the remindmail log setting"""
@@ -172,23 +175,23 @@
 
             # handle deletion and decrementing
             if is_match:
 
                 if not is_command:
                     if generate_type == GenerateType.EMAIL and not dry_run:
                         RemindMailUtils().send_email(item.split(' ', 1)[1],
-                                                item_notes, "remind.md")
+                                                     item_notes, "remind.md")
                     if dry_run and generate_type == GenerateType.EMAIL:
                         RemindMail().log_msg(
                             f"Test Mode. Not Sending: {item.split(' ', 1)[1]}", level="debug")
                     elif generate_type == GenerateType.LIST:
                         print(item)
                 if token_after == 1:
                     RemindMail().log_msg(
-                        f"Deleting item from remind.md: {item}")
+                        f"Deleting item from remind.md: {item}", level="debug")
                     if not dry_run:
                         try:
                             remindmd_file.remove(_item)
                         except ValueError as err:
                             RemindMail().log_msg(
                                 f"Could not remove from remind.md: {err}", level="error")
                     elif generate_type != GenerateType.LIST:
@@ -196,18 +199,34 @@
                                              level="debug")
                 elif token_after > 1:
                     remindmd_file[index] = (item.replace(
                         f"]{token_after} ", f"]{token_after-1} "))
 
                 if is_command:
                     if not dry_run:
-                        print("Executing command:\n", command)
-                        os.system(command)
+                        RemindMail().log_msg(
+                            f"Executing command: {command}", level="debug")
+                        try:
+                            # add path so things like `cabinet` calls work from crontab
+                            home_dir = os.path.expanduser("~")
+                            path_local_bin = os.path.join(
+                                home_dir, ".local/bin")
+                            os.environ['PATH'] = f"{path_local_bin}:{os.environ['PATH']}"
+
+                            cmd_output = subprocess.check_output(
+                                command, shell=True, universal_newlines=True)
+                            RemindMail().log_msg(
+                                f"Results: {cmd_output}", level="debug")
+                        except subprocess.CalledProcessError as error:
+                            RemindMail().log_msg(
+                                f"Command execution failed with exit code: {error.returncode}", level="error")
+                            RemindMail().log_msg(
+                                f"Error output: {error.output}", level="error")
                     else:
-                        RemindMail().log_msg(f"Test Mode. Not executing {item})",
+                        RemindMail().log_msg(f"Test Mode. Not executing {command})",
                                              level="debug")
 
         RemindMailUtils.cab.write_file("remind.md", "notes",
                                        '\n'.join(remindmd_file), is_quiet=True)
 
         if not dry_run:
             RemindMail().log_msg(
@@ -242,29 +261,43 @@
         """
 
         today = str(datetime.today().strftime('%Y-%m-%d'))
         weekdays = ['sunday', 'monday', 'tuesday',
                     'wednesday', 'thursday', 'friday', 'saturday']
 
         # helper functions
-        def get_larger(string_a, string_b):
+        def get_larger(string_a: str, string_b: str):
             """A helper function to return the larger string between string_a and string_b"""
 
             return string_a if len(string_a) > len(string_b) else string_b
 
         def strip_to(query):
             """A helper function to remove the portion after 'to' or 'day to'"""
             if query.startswith(' to ') or query.startswith('to ') or query.startswith('day to '):
                 return ''.join(query.split('to')[1:]).strip()
 
             return query.strip()
 
-        def parse_date(query):
+        def parse_date(query: str):
             """
-            Parses a date from the input query
+            Parses a date from the input query.
+
+            Args:
+                query (str): The input query containing the date information.
+
+            Returns:
+                tuple or bool: A tuple containing the parsed date/tokens, or False if parsing fails.
+
+            Raises:
+                ValueError: If an error occurs during date parsing.
+
+            Notes:
+                - The function supports parsing various date formats.
+                - If the query contains the word 'tomorrow', it returns the date for the next day.
+                - If a date is parsed into before 90 days ago, it is returns a date for next year.
             """
 
             # handle 'tomorrow'
             if 'tomorrow' in query:
                 _days = 0 if datetime.today().hour < 3 else 1
                 query = (datetime.now() + timedelta(days=_days)).strftime('%F')
```

### Comparing `remindmail-2023.4.29.1/src/remind/remindmail_utils.py` & `remindmail-2023.4.30.1/src/remind/remindmail_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,57 +10,66 @@
 import requests
 import pytz
 from cabinet import Cabinet, Mail
 
 
 class RemindMailUtils:
     """
-    Contains standalone helper functions
+    A utility class for handling reminders and email operations.
     """
 
+    # instance of the Cabinet class for configuration management
     cab = Cabinet()
-    path_remind_file = cab.get(
-        'path', 'remindmail', 'file')
+
+    # file path for reminders
+    path_remind_file = cab.get('path', 'remindmail', 'file')
+
+    # for sending emails
     mail = Mail()
+
+    # to store query trace information
     query_trace: List[str] = []
 
     def get_user_time(self):
         """
-        A helper function to return the epoch seconds based on the user's timezone
+        A helper function to return the epoch seconds based on the user's timezone.
+
+        Returns:
+            int: The epoch seconds representing the current time in the user's timezone.
         """
 
         user_timezone = self.cab.get("remindmail", "timezone")
         if user_timezone is None:
-            # get timezone based on IP
+            # user's timezone not saved in `cab`; get timezone based on IP
             print("Checking timezone...")
             response = requests.get('https://ipapi.co/json/', timeout=10)
 
-            # Parse the response JSON to get the user's timezone
+            # parse the response JSON to get the user's timezone
             if response.status_code == 200:
                 data = response.json()
                 user_timezone = self.cab.put("remindmail", "timezone", data.get('timezone'))
                 print(f"Set timezone: {user_timezone}")
             else:
                 print("Could not parse timezone; using UTC")
                 return datetime.datetime.utcnow()
 
         timezone = pytz.timezone(user_timezone)
 
         now = datetime.datetime.now(timezone)
 
-        # Get the UTC time
+        # get the UTC time
         utc_now = datetime.datetime.utcnow()
 
-        # Calculate the time difference between the specified timezone and UTC
+        # calculate the time difference between the specified timezone and UTC
         offset = timezone.utcoffset(utc_now).total_seconds()
 
-        # Subtract the offset from the current time
+        # subtract the offset from the current time
         utc_time = now + datetime.timedelta(seconds=offset)
 
-        # Convert the UTC time to the number of seconds since January 1, 1970
+        # convert the UTC time to the number of seconds since January 1, 1970
         unix_time = int(utc_time.timestamp())
 
         return unix_time
 
 
     def print_reminders_file(self, param=None):
         """
```

### Comparing `remindmail-2023.4.29.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.4.30.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.29.1
+Version: 2023.4.30.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

