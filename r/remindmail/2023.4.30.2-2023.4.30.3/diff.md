# Comparing `tmp/remindmail-2023.4.30.2.tar.gz` & `tmp/remindmail-2023.4.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.4.30.2.tar", last modified: Mon May  1 03:49:41 2023, max compression
+gzip compressed data, was "remindmail-2023.4.30.3.tar", last modified: Mon May  1 04:22:23 2023, max compression
```

## Comparing `remindmail-2023.4.30.2.tar` & `remindmail-2023.4.30.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.30.2/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.4.30.2/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.30.2/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.4.30.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.4.30.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.4.30.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    24834 2023-05-01 03:48:08.000000 remindmail-2023.4.30.2/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.4.30.2/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 03:49:41.625120 remindmail-2023.4.30.2/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 03:49:41.000000 remindmail-2023.4.30.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-01 03:49:41.000000 remindmail-2023.4.30.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-01 03:49:41.000000 remindmail-2023.4.30.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-01 03:49:41.000000 remindmail-2023.4.30.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-01 03:49:41.000000 remindmail-2023.4.30.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 04:22:23.046567 remindmail-2023.4.30.3/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.4.30.3/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 04:22:23.046567 remindmail-2023.4.30.3/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11649 2023-04-19 21:19:01.000000 remindmail-2023.4.30.3/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.4.30.3/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-05-01 04:22:23.046567 remindmail-2023.4.30.3/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 04:22:23.042567 remindmail-2023.4.30.3/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 04:22:23.046567 remindmail-2023.4.30.3/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.4.30.3/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3323 2023-04-30 04:24:17.000000 remindmail-2023.4.30.3/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.4.30.3/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    24974 2023-05-01 04:18:45.000000 remindmail-2023.4.30.3/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     8189 2023-04-30 04:24:17.000000 remindmail-2023.4.30.3/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-01 04:22:23.046567 remindmail-2023.4.30.3/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11998 2023-05-01 04:22:23.000000 remindmail-2023.4.30.3/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-05-01 04:22:23.000000 remindmail-2023.4.30.3/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-01 04:22:23.000000 remindmail-2023.4.30.3/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-05-01 04:22:23.000000 remindmail-2023.4.30.3/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-05-01 04:22:23.000000 remindmail-2023.4.30.3/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.4.30.2/LICENSE.md` & `remindmail-2023.4.30.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.30.2/PKG-INFO` & `remindmail-2023.4.30.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.30.2
+Version: 2023.4.30.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2023.4.30.2/README.md` & `remindmail-2023.4.30.3/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.30.2/setup.cfg` & `remindmail-2023.4.30.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.04.30.2
+version = 2023.04.30.3
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.4.30.2/src/remind/__main__.py` & `remindmail-2023.4.30.3/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.30.2/src/remind/reminder.py` & `remindmail-2023.4.30.3/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.30.2/src/remind/remindmail.py` & `remindmail-2023.4.30.3/src/remind/remindmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,16 @@
                 token_after = int(token_after)
             else:
                 token_after = -1
 
             parsed_date = ""
             if not "%" in token and not "any" in token:
                 try:
-                    parsed_date = parse(token, fuzzy_with_tokens=True)
+                    parsed_date = parse(
+                        token, fuzzy_with_tokens=True, default=generate_date)
                 except ValueError:
                     try:
                         parsed_date = parse(
                             f"{token}day", fuzzy_with_tokens=True)
                     except ValueError as error:
                         RemindMail().log_msg(
                             f"Could not parse token: {token}; {error}", level="error")
@@ -171,15 +172,14 @@
                         is_match = True
                     elif (split_type in ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat']
                           and today_dayw.lower() == split_type):
                         is_match = True
 
             # handle deletion and decrementing
             if is_match:
-
                 if not is_command:
                     if generate_type == GenerateType.EMAIL and not dry_run:
                         RemindMailUtils().send_email(item.split(' ', 1)[1],
                                                      item_notes, "remind.md")
                     if dry_run and generate_type == GenerateType.EMAIL:
                         RemindMail().log_msg(
                             f"Test Mode. Not Sending: {item.split(' ', 1)[1]}", level="debug")
@@ -248,14 +248,17 @@
 
         tomorrow = datetime.today() + timedelta(days=1)
 
         # 'tomorrow' is 'today' if between 12AM and 3AM
         if datetime.now().hour < 3:
             tomorrow = datetime.today()
 
+        tomorrow = tomorrow.replace(
+            hour=0, minute=0, second=0, microsecond=0)
+
         RemindMail().generate(force=True, dry_run=True, generate_date=tomorrow,
                               generate_type=GenerateType.LIST)
 
     def parse_query(self, query=None, manual_message='', manual_date='', noconfirm=False):
         """
         Parses arguments to determine what to email or what to write to a file for later.
```

### Comparing `remindmail-2023.4.30.2/src/remind/remindmail_utils.py` & `remindmail-2023.4.30.3/src/remind/remindmail_utils.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.4.30.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.4.30.3/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.4.30.2
+Version: 2023.4.30.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

