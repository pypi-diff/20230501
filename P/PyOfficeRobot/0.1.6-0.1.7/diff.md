# Comparing `tmp/PyOfficeRobot-0.1.6.tar.gz` & `tmp/PyOfficeRobot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.6.tar", last modified: Sat Apr 29 11:49:44 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.7.tar", last modified: Mon May  1 08:17:54 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.6.tar` & `PyOfficeRobot-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.363536 PyOfficeRobot-0.1.6/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     8068 2023-04-29 11:49:44.363536 PyOfficeRobot-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.302373 PyOfficeRobot-0.1.6/PyOfficeRobot/
--rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.330943 PyOfficeRobot-0.1.6/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/friend.py
--rw-rw-rw-   0        0        0      640 2023-04-27 14:44:49.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/api/group.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.334940 PyOfficeRobot-0.1.6/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.338955 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.345495 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.352013 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.317888 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     8068 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      757 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 13:31:57.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-29 11:49:44.000000 PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7488 2023-04-26 16:01:49.000000 PyOfficeRobot-0.1.6/README.md
--rw-rw-rw-   0        0        0      838 2023-04-29 11:49:44.365540 PyOfficeRobot-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 11:49:44.360013 PyOfficeRobot-0.1.6/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.6/tests/chat.py
--rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.6/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.854141 PyOfficeRobot-0.1.7/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     8321 2023-05-01 08:17:54.854141 PyOfficeRobot-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.747140 PyOfficeRobot-0.1.7/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      195 2023-04-27 13:53:55.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.800153 PyOfficeRobot-0.1.7/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     9379 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/friend.py
+-rw-rw-rw-   0        0        0      640 2023-04-27 14:44:49.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/api/group.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.814148 PyOfficeRobot-0.1.7/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13556 2023-04-26 14:23:30.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.825141 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/
+-rw-rw-rw-   0        0        0     3880 2023-04-27 14:56:15.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/Start.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-16 14:37:30.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/core/group/ui_file_py.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.831152 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.836140 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.842140 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-27 13:42:29.000000 PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.780140 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     8321 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 08:16:52.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-01 08:17:54.000000 PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7741 2023-04-29 12:53:26.000000 PyOfficeRobot-0.1.7/README.md
+-rw-rw-rw-   0        0        0      838 2023-05-01 08:17:54.857142 PyOfficeRobot-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:17:54.852146 PyOfficeRobot-0.1.7/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.7/tests/chat.py
+-rw-rw-rw-   0        0        0     1293 2023-05-01 08:14:58.000000 PyOfficeRobot-0.1.7/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.6/LICENSE` & `PyOfficeRobot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PKG-INFO` & `PyOfficeRobot-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.6
+Version: 0.1.7
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -81,14 +81,16 @@
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
 | 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 | 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
+| 11-定时群发 | [点我直达](https://www.bilibili.com/video/BV1Nm4y1C7N7)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py)     |
+
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.6 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.7 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -46,25 +46,29 @@
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
 blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
 (http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
 6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
-PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
-æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
-wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
-|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
-[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
-ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | | 11-å®æ¶ç¾¤å |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Nm4y1C7N7) |[ç¹æç´è¾¾]
+(https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼
+[ç¹æå å¥](http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
+å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
+- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
+(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
+3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/api/file.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/api/friend.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/api/friend.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/api/group.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/api/group.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/core/WeChatType.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.7/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.6
+Version: 0.1.7
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
@@ -81,14 +81,16 @@
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
 | 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 | 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
+| 11-定时群发 | [点我直达](https://www.bilibili.com/video/BV1Nm4y1C7N7)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py)     |
+
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.6 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.7 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
@@ -46,25 +46,29 @@
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
 blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
 (http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
 6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
-PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
-æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
-wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
-|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
-[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
-ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | | 11-å®æ¶ç¾¤å |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Nm4y1C7N7) |[ç¹æç´è¾¾]
+(https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼
+[ç¹æå å¥](http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
+å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
+- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
+(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
+3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.6/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.7/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 PyOfficeRobot/api/__init__.py
 PyOfficeRobot/api/chat.py
 PyOfficeRobot/api/file.py
 PyOfficeRobot/api/friend.py
 PyOfficeRobot/api/group.py
 PyOfficeRobot/core/WeChatType.py
 PyOfficeRobot/core/__init__.py
+PyOfficeRobot/core/group/Start.py
+PyOfficeRobot/core/group/__init__.py
+PyOfficeRobot/core/group/ui_file_py.py
 PyOfficeRobot/lib/CONST.py
 PyOfficeRobot/lib/__init__.py
 PyOfficeRobot/lib/dec/__init__.py
 PyOfficeRobot/lib/dec/act_dec.py
 PyOfficeRobot/lib/decorator_utils/__init__.py
 PyOfficeRobot/lib/decorator_utils/instruction_url.py
 tests/__init__.py
```

### Comparing `PyOfficeRobot-0.1.6/README.md` & `PyOfficeRobot-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 | ⌚005-定时自动发消息 | [点我直达](https://www.bilibili.com/video/BV1m8411b7LZ/)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/06-%E5%AE%9A%E6%97%B6.py)     |
 | 006-自己加功能 | [点我直达](https://www.bilibili.com/video/BV14R4y127h6)     |     |
 | ⭐007-独立使用 | [点我直达](https://www.bilibili.com/video/BV1SY411y7Uh)     |[点我直达](https://github.com/CoderWanFeng/PyOfficeRobot)     |
 | 08-收集群信息 | [点我直达](https://www.bilibili.com/video/BV1eD4y1g7yZ)     |[点我直达](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw)     |
 | 09-发消息如何换行？ | [点我直达](https://www.bilibili.com/video/BV1Xg4y1s79z/)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/08-new_line.py)     |
 | 特别篇-微信 + ChatGPT | [点我直达](http://xhslink.com/zXZAeo)     |[点我直达](https://blog.51cto.com/u_15493782/6131326)     |
 | 10-批量加好友 | [点我直达](https://www.bilibili.com/video/BV1DV4y1o7t2)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py)     |
+| 11-定时群发 | [点我直达](https://www.bilibili.com/video/BV1Nm4y1C7N7)     |[点我直达](https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py)     |
+
 > 持续更新中，交流群：[点我加入](http://www.python4office.cn/wechat-group/)
 #### 微信机器人-其它实现方式
 
 
 | 功能说明       | 视频 |代码 |
 | -------------- | -------- |-------- |
 | 机器人.exe | [点我直达](https://www.bilibili.com/video/BV1Q64y1Z7TB/)     |     |
```

#### html2text {}

```diff
@@ -38,25 +38,29 @@
 [ç¹æç´è¾¾](https://mp.weixin.qq.com/s/crjGYUzyQ3iIN3Sx2UUucw) | | 09-
 åæ¶æ¯å¦ä½æ¢è¡ï¼ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
 BV1Xg4y1s79z/) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/PyOfficeRobot/
 blob/main/demo/08-new_line.py) | | ç¹å«ç¯-å¾®ä¿¡ + ChatGPT | [ç¹æç´è¾¾]
 (http://xhslink.com/zXZAeo) |[ç¹æç´è¾¾](https://blog.51cto.com/u_15493782/
 6131326) | | 10-æ¹éå å¥½å | [ç¹æç´è¾¾](https://www.bilibili.com/
 video/BV1DV4y1o7t2) |[ç¹æç´è¾¾](https://gitee.com/CoderWanFeng/
-PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | >
-æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼[ç¹æå å¥](http://www.python4office.cn/
-wechat-group/) #### å¾®ä¿¡æºå¨äºº-å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢
-|ä»£ç  | | -------------- | -------- |-------- | | æºå¨äºº.exe |
-[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Q64y1Z7TB/) | | |
-ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Dx4y157qy) |
-[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-
-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾](https://www.bilibili.com/video/
-BV11L411L7oi/) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |[ç¹æç´è¾¾](https://
-mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ## 3ãåè½Demo
+PyOfficeRobot/blob/main/PyOfficeRobot/api/friend.py) | | 11-å®æ¶ç¾¤å |
+[ç¹æç´è¾¾](https://www.bilibili.com/video/BV1Nm4y1C7N7) |[ç¹æç´è¾¾]
+(https://gitee.com/CoderWanFeng/PyOfficeRobot/blob/main/demo/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91/11-
+%E5%AE%9A%E6%97%B6%E7%BE%A4%E5%8F%91.py) | > æç»­æ´æ°ä¸­ï¼äº¤æµç¾¤ï¼
+[ç¹æå å¥](http://www.python4office.cn/wechat-group/) #### å¾®ä¿¡æºå¨äºº-
+å¶å®å®ç°æ¹å¼ | åè½è¯´æ | è§é¢ |ä»£ç  | | -------------- | -------
+- |-------- | | æºå¨äºº.exe | [ç¹æç´è¾¾](https://www.bilibili.com/video/
+BV1Q64y1Z7TB/) | | | ChatGPTçæ¬ | [ç¹æç´è¾¾](https://www.bilibili.com/
+video/BV1Dx4y157qy) |[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
+HJfLZILUOWn4TK8qk3DL9w) | | âwxpy-24å°æ¶ï¼åå°è¿è¡ | [ç¹æç´è¾¾]
+(https://www.bilibili.com/video/BV11L411L7oi/) |[ç¹æç´è¾¾](https://
+mp.weixin.qq.com/s/ubJ1OhOFVKfFVT8sBNZ0pg) | | ä¼ä¸å¾®ä¿¡æºå¨äºº | |
+[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/mt-ONvz0DdhbMB96eTZDKA) | ##
+3ãåè½Demo
 ææè¿å¼æºäºè¿ä¸ªåºçå¨é¨æºä»£ç ï¼åè½æ­£å¨å¼åä¸­ï¼æ¬¢è¿å¤§å®¶åä¸å¼å~
 - [æ¼ç¤ºä»£ç ](https://github.com/CoderWanFeng/PyOfficeRobot/tree/main/demo)
 --- ![](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-
 office-qr.jpg) ## â­Star [![Stargazers over time](https://starchart.cc/
 CoderWanFeng/PyOfficeRobot.svg)](https://starchart.cc/CoderWanFeng/
 PyOfficeRobot) ## ðæå±èµæ
         [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/
```

### Comparing `PyOfficeRobot-0.1.6/setup.cfg` & `PyOfficeRobot-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
+00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `PyOfficeRobot-0.1.6/tests/test_file.py` & `PyOfficeRobot-0.1.7/tests/test_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from PyOfficeRobot.api import file
+from PyOfficeRobot.api import file, group
 
 from PyOfficeRobot.api.chat import *
 from PyOfficeRobot.api.file import *
 
 keywords = {
     '你好': "在干嘛？"
 }
@@ -29,7 +29,10 @@
     def test_weixin_file(self):
         who = '每天进步一点点'
         file_path = r'./dfasd.py'
         # file_path = r'D:\workplace\code\github\PyOfficeRobot\tests\chat.py'
         # PyOfficeRobot.file.send_file(who, file)
         file.send_file(who, file_path)
         # file.send_file(who='每天进步一点点', file=r'D:\workplace\code\github\PyOfficeRobot\dev\contributor\gen\自动加好友\Excel_File\【企查查】查企业-高级搜索“涂料”(202302030683).xls')
+
+    def test_group_send(self):
+        group.send()
```

