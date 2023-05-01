# Comparing `tmp/PyOfficeRobot-0.1.7.tar.gz` & `tmp/PyOfficeRobot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.7.tar", last modified: Mon May  1 08:17:54 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.8.tar", last modified: Mon May  1 08:24:22 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.7.tar` & `PyOfficeRobot-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.854141 PyOfficeRobot-0.1.7/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     8321 2023-05-01 08:17:54.854141 PyOfficeRobot-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.747140 PyOfficeRobot-0.1.7/PyOfficeRobot/
--rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.800153 PyOfficeRobot-0.1.7/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/friend.py
--rw-rw-rw-   0        0        0      640 2023-04-27 14:44:49.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/group.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.814148 PyOfficeRobot-0.1.7/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.825141 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/
--rw-rw-rw-   0        0        0     3880 2023-04-27 14:56:15.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/Start.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-16 14:37:30.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/ui_file_py.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.831152 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.836140 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.842140 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.780140 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     8321 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      867 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 08:16:52.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7741 2023-04-29 12:53:26.000000 PyOfficeRobot-0.1.7/README.md
--rw-rw-rw-   0        0        0      838 2023-05-01 08:17:54.857142 PyOfficeRobot-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.852146 PyOfficeRobot-0.1.7/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.7/tests/chat.py
--rw-rw-rw-   0        0        0     1293 2023-05-01 08:14:58.000000 PyOfficeRobot-0.1.7/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.552180 PyOfficeRobot-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     8321 2023-05-01 08:24:22.553178 PyOfficeRobot-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.466407 PyOfficeRobot-0.1.8/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.512179 PyOfficeRobot-0.1.8/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/friend.py
+-rw-rw-rw-   0        0        0      727 2023-05-01 08:21:55.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/api/group.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.518181 PyOfficeRobot-0.1.8/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.526179 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/
+-rw-rw-rw-   0        0        0     3880 2023-04-27 14:56:15.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/Start.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-16 14:37:30.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/ui_file_py.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.531180 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.538175 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.542179 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2523 2023-05-01 08:22:39.000000 PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.497179 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     8321 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 08:16:52.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-01 08:24:22.000000 PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7741 2023-04-29 12:53:26.000000 PyOfficeRobot-0.1.8/README.md
+-rw-rw-rw-   0        0        0      838 2023-05-01 08:24:22.556173 PyOfficeRobot-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:22.550176 PyOfficeRobot-0.1.8/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.8/tests/chat.py
+-rw-rw-rw-   0        0        0     1293 2023-05-01 08:14:58.000000 PyOfficeRobot-0.1.8/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.7/LICENSE` & `PyOfficeRobot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PKG-INFO` & `PyOfficeRobot-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.7 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.8 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/api/file.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/api/friend.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/api/friend.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/api/group.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/api/group.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 @Blog      ：www.python-office.com
 @Date    ：2023/4/27 21:50 
 @Description     ：
 '''
 
 import sys
 
+from PyOfficeRobot.lib.decorator_utils.instruction_url import instruction
 from PySide6.QtWidgets import QApplication
 
 from PyOfficeRobot.core.group.Start import MyWidget
 
-
+@instruction
 def send():
     app = QApplication(sys.argv)
     # 初始化QApplication，界面展示要包含在QApplication初始化之后，结束之前
     window = MyWidget()
     window.show()
     # 初始化并展示我们的界面组件
     sys.exit(app.exec_())
```

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/core/WeChatType.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/Start.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/Start.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/ui_file_py.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/core/group/ui_file_py.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.8/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,24 @@
 }
 
 friend_dict = {
     "add": "https://www.bilibili.com/video/BV1DV4y1o7t2",
 
 }
 
+group_dict = {
+    "send": "https://www.bilibili.com/video/BV1Nm4y1C7N7",
+}
+
 # 有多少文件需要说明
 instruction_file_dict = {
     "chat.py": chat_dict,
     "file.py": file_dict,
     "friend.py": friend_dict,
+    "group.py": group_dict,
 }
 
 
 def instruction(func):
     @wraps(func)
     def instruction_wrapper(*args, **kwargs):
         func_filename = os.path.basename(func.__code__.co_filename)  # 取出方法所在的文件名
```

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.7
+Version: 0.1.8
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.7 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.8 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.8/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/README.md` & `PyOfficeRobot-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.7/setup.cfg` & `PyOfficeRobot-0.1.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `PyOfficeRobot-0.1.7/tests/test_file.py` & `PyOfficeRobot-0.1.8/tests/test_file.py`

 * *Files identical despite different names*

