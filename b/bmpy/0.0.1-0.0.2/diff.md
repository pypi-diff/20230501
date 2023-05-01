# Comparing `tmp/bmpy-0.0.1.tar.gz` & `tmp/bmpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmpy-0.0.1.tar", last modified: Mon May  1 08:46:59 2023, max compression
+gzip compressed data, was "bmpy-0.0.2.tar", last modified: Mon May  1 10:39:54 2023, max compression
```

## Comparing `bmpy-0.0.1.tar` & `bmpy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:46:59.854033 bmpy-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-01 08:46:59.854033 bmpy-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3290 2023-05-01 08:28:13.000000 bmpy-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:46:59.854033 bmpy-0.0.1/bmpy/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-01 08:36:11.000000 bmpy-0.0.1/bmpy/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9001 2023-04-17 19:30:13.000000 bmpy-0.0.1/bmpy/bmpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 08:46:59.854033 bmpy-0.0.1/bmpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-01 08:46:59.000000 bmpy-0.0.1/bmpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 08:46:59.854033 bmpy-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1400 2023-05-01 08:46:54.000000 bmpy-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 10:39:54.265967 bmpy-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-01 10:39:54.265967 bmpy-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-05-01 08:28:13.000000 bmpy-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 10:39:54.265967 bmpy-0.0.2/bmpy/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-01 10:37:44.000000 bmpy-0.0.2/bmpy/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9011 2023-05-01 10:34:20.000000 bmpy-0.0.2/bmpy/bmpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 10:39:54.265967 bmpy-0.0.2/bmpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-01 10:39:54.000000 bmpy-0.0.2/bmpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 10:39:54.265967 bmpy-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-01 09:05:33.000000 bmpy-0.0.2/setup.py
```

### Comparing `bmpy-0.0.1/PKG-INFO` & `bmpy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bmpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bounty Meter is a command-line utility tool designed for bug bounty hunters to define their bounty target for a year, maintain and keep record of their bounties on a monthly basis, and track their progress throughout the year. With Bounty Meter, you can add and subtract bounties, view your total bounties earned this year, and display an interactive stats card to visualize your progress.
 Home-page: https://github.com/720922/bountymeterPY
-Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.1.zip
+Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.2.zip
 Author: 720922
 License: GNU Affero General Public License v3.0
 Keywords: recon,bugbounty,pentesting,utility,hacking
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bmpy-0.0.1/README.md` & `bmpy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bmpy-0.0.1/bmpy/bmpy.py` & `bmpy-0.0.2/bmpy/bmpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,12 +204,12 @@
                 stats() 
             case default:
                 usage()
     else:
         usage()
 
 
-#########################################################
-#                   Script Start                        #
-#########################################################
-if __name__ == "__main__":
-    main()
+# #########################################################
+# #                   Script Start                        #
+# #########################################################
+# if __name__ == "__main__":
+#     main()
```

### Comparing `bmpy-0.0.1/bmpy.egg-info/PKG-INFO` & `bmpy-0.0.2/bmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bmpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bounty Meter is a command-line utility tool designed for bug bounty hunters to define their bounty target for a year, maintain and keep record of their bounties on a monthly basis, and track their progress throughout the year. With Bounty Meter, you can add and subtract bounties, view your total bounties earned this year, and display an interactive stats card to visualize your progress.
 Home-page: https://github.com/720922/bountymeterPY
-Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.1.zip
+Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.2.zip
 Author: 720922
 License: GNU Affero General Public License v3.0
 Keywords: recon,bugbounty,pentesting,utility,hacking
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bmpy-0.0.1/setup.py` & `bmpy-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type='text/markdown',
     author='720922',
     license='GNU Affero General Public License v3.0',
     url='https://github.com/720922/bountymeterPY',
     download_url='https://github.com/720922/bountymeterPY/archive/v%s.zip' % __import__(
         'bmpy').__version__,
     packages=find_packages(),
-    install_requires=['progress'],
+    install_requires=['progress','sys','os'],
     classifiers=[
         'Topic :: Security',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
     ],
     entry_points={
         'console_scripts': [
```

