# Comparing `tmp/nonebot-plugin-watermarker-0.1.0.tar.gz` & `tmp/nonebot-plugin-watermarker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-watermarker-0.1.0.tar", last modified: Mon May  1 12:33:39 2023, max compression
+gzip compressed data, was "nonebot-plugin-watermarker-0.1.1.tar", last modified: Mon May  1 13:08:35 2023, max compression
```

## Comparing `nonebot-plugin-watermarker-0.1.0.tar` & `nonebot-plugin-watermarker-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:33:39.142888 nonebot-plugin-watermarker-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot-plugin-watermarker-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4000 2023-05-01 12:33:39.140894 nonebot-plugin-watermarker-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3644 2023-05-01 12:31:50.000000 nonebot-plugin-watermarker-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 12:33:39.130919 nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/
--rw-rw-rw-   0        0        0     2081 2023-05-01 09:27:24.000000 nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/config.py
--rw-rw-rw-   0        0        0     2009 2023-05-01 08:46:06.000000 nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/fuctions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:33:39.138897 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/
--rw-rw-rw-   0        0        0     4000 2023-05-01 12:33:39.000000 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-01 12:33:39.000000 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:33:39.000000 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 12:33:39.000000 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 12:33:39.000000 nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 12:33:39.142888 nonebot-plugin-watermarker-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4174 2023-05-01 12:33:23.000000 nonebot-plugin-watermarker-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:08:35.481809 nonebot-plugin-watermarker-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot-plugin-watermarker-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4000 2023-05-01 13:08:35.480813 nonebot-plugin-watermarker-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3644 2023-05-01 12:31:50.000000 nonebot-plugin-watermarker-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 13:08:35.470838 nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/
+-rw-rw-rw-   0        0        0     2081 2023-05-01 09:27:24.000000 nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/config.py
+-rw-rw-rw-   0        0        0     2009 2023-05-01 08:46:06.000000 nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/fuctions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:08:35.479843 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/
+-rw-rw-rw-   0        0        0     4000 2023-05-01 13:08:35.000000 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-01 13:08:35.000000 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:08:35.000000 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-01 13:08:35.000000 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 13:08:35.000000 nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:08:35.481809 nonebot-plugin-watermarker-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4195 2023-05-01 13:08:29.000000 nonebot-plugin-watermarker-0.1.1/setup.py
```

### Comparing `nonebot-plugin-watermarker-0.1.0/LICENSE` & `nonebot-plugin-watermarker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.0/PKG-INFO` & `nonebot-plugin-watermarker-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-watermarker
-Version: 0.1.0
+Version: 0.1.1
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.1 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-watermarker-0.1.0/README.md` & `nonebot-plugin-watermarker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/__init__.py` & `nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/config.py` & `nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.0/nonebot-plugin-watermarker/fuctions.py` & `nonebot-plugin-watermarker-0.1.1/nonebot-plugin-watermarker/fuctions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.0/nonebot_plugin_watermarker.egg-info/PKG-INFO` & `nonebot-plugin-watermarker-0.1.1/nonebot_plugin_watermarker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-watermarker
-Version: 0.1.0
+Version: 0.1.1
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.1 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-watermarker-0.1.0/setup.py` & `nonebot-plugin-watermarker-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
     
 setup(
     name='nonebot-plugin-watermarker',
 
-    version="0.1.0",
+    version="0.1.1",
     description=(
         '为nonebot机器人发送的图片加上水印'
 
     ),
     long_description="""<div align="center">
   <p><img src="https://user-images.githubusercontent.com/91937041/235443858-85949be1-08d6-4d7a-b132-b1aed71ab943.png" width="560" alt="PoweredByNonebotLogo"></p>
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -123,10 +123,11 @@
     long_description_content_type="text/markdown",
     author='XU',
     author_email='Woyerpa@outlook.com',
     license='MIT License',
     packages=find_packages(),
     url='https://github.com/X-Skirt-X/nonebot-plugin-watermarker',
     install_requires=[
-        "nb-cli"
+        "nb-cli",
+        "nonebot2"
     ]
 )
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages setup( name='nonebot-plugin-
-watermarker', version="0.1.0", description=
+watermarker', version="0.1.1", description=
 ( 'ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å°' ), long_description="""
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
@@ -35,8 +35,8 @@
 æ°´å°å°æ¦çè´´ä¸ä¸,åºè¯¥æ¯base64çåå ,ä½æ¯æä¸ç´æ¾ä¸å°çæ­£çé®é¢æº,å ä¸ºææ¶åè´´çä¸ææ¶åè´´ä¸ä¸
 ( # ð¥é¸£è°¢ [Nonebot2](https://github.com/nonebot/
 nonebot2),ä¸ç¨è¯´,æ²¡æNonebotå°±æ²¡æè¿ä¸ªæä»¶ ~~[æèªå·±](https://
 github.com/X-Skirt-X),å ä¸ºæåçPoweredByNonebotçLogo~~ # ð¦å¶ä»
 æ²¡æå¶ä»,æ³å°åè¡¥ """, long_description_content_type="text/markdown",
 author='XU', author_email='Woyerpa@outlook.com', license='MIT License',
 packages=find_packages(), url='https://github.com/X-Skirt-X/nonebot-plugin-
-watermarker', install_requires=[ "nb-cli" ] )
+watermarker', install_requires=[ "nb-cli", "nonebot2" ] )
```

