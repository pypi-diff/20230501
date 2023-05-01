# Comparing `tmp/bmpy-0.0.3.tar.gz` & `tmp/bmpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmpy-0.0.3.tar", last modified: Mon May  1 11:02:11 2023, max compression
+gzip compressed data, was "bmpy-0.0.4.tar", last modified: Mon May  1 11:06:38 2023, max compression
```

## Comparing `bmpy-0.0.3.tar` & `bmpy-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:02:11.145954 bmpy-0.0.3/
--rw-r--r--   0 root         (0) root         (0)    34522 2023-05-01 10:57:01.000000 bmpy-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-01 11:02:11.145954 bmpy-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3290 2023-05-01 08:28:13.000000 bmpy-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:02:11.145954 bmpy-0.0.3/bmpy/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-01 11:02:02.000000 bmpy-0.0.3/bmpy/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9019 2023-05-01 11:01:54.000000 bmpy-0.0.3/bmpy/bmpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:02:11.145954 bmpy-0.0.3/bmpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-01 11:02:11.000000 bmpy-0.0.3/bmpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 11:02:11.145954 bmpy-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1400 2023-05-01 10:44:00.000000 bmpy-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:06:38.669952 bmpy-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)    34522 2023-05-01 10:57:01.000000 bmpy-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-01 11:06:38.669952 bmpy-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-05-01 08:28:13.000000 bmpy-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:06:38.669952 bmpy-0.0.4/bmpy/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-01 11:06:31.000000 bmpy-0.0.4/bmpy/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9022 2023-05-01 11:06:06.000000 bmpy-0.0.4/bmpy/bmpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 11:06:38.669952 bmpy-0.0.4/bmpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-01 11:06:38.000000 bmpy-0.0.4/bmpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 11:06:38.669952 bmpy-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-05-01 10:44:00.000000 bmpy-0.0.4/setup.py
```

### Comparing `bmpy-0.0.3/LICENSE` & `bmpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bmpy-0.0.3/PKG-INFO` & `bmpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bmpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bounty Meter is a command-line utility tool designed for bug bounty hunters to define their bounty target for a year, maintain and keep record of their bounties on a monthly basis, and track their progress throughout the year. With Bounty Meter, you can add and subtract bounties, view your total bounties earned this year, and display an interactive stats card to visualize your progress.
 Home-page: https://github.com/720922/bountymeterPY
-Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.3.zip
+Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.4.zip
 Author: 720922
 License: GNU Affero General Public License v3.0
 Keywords: recon,bugbounty,pentesting,utility,hacking
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bmpy-0.0.3/README.md` & `bmpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bmpy-0.0.3/bmpy/bmpy.py` & `bmpy-0.0.4/bmpy/bmpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             bar.next()
 
 #########################################################
 #                   Main Function                        #
 #########################################################
 def main():
     if(len(sys.argv)>1):
-        match sys.argv[1]:
+        match str(sys.argv[1]):
             case "add":
                 if(len(sys.argv)> 3 and sys.argv[2]!="" and sys.argv[2].isalpha() and sys.argv[3].isnumeric()):
                     add(sys.argv[2],sys.argv[3])
                 else:
                     usage()
             case "sub":
                 if(len(sys.argv)> 3 and sys.argv[2]!="" and sys.argv[2].isalpha() and sys.argv[3].isnumeric()):
@@ -203,13 +203,13 @@
             case "stats":
                 stats() 
             case default:
                 usage()
     else:
         usage()
 
-# main()
+main()
 # #########################################################
 # #                   Script Start                        #
 # #########################################################
 # if __name__ == "__main__":
 #     main()
```

### Comparing `bmpy-0.0.3/bmpy.egg-info/PKG-INFO` & `bmpy-0.0.4/bmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bmpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bounty Meter is a command-line utility tool designed for bug bounty hunters to define their bounty target for a year, maintain and keep record of their bounties on a monthly basis, and track their progress throughout the year. With Bounty Meter, you can add and subtract bounties, view your total bounties earned this year, and display an interactive stats card to visualize your progress.
 Home-page: https://github.com/720922/bountymeterPY
-Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.3.zip
+Download-URL: https://github.com/720922/bountymeterPY/archive/v0.0.4.zip
 Author: 720922
 License: GNU Affero General Public License v3.0
 Keywords: recon,bugbounty,pentesting,utility,hacking
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `bmpy-0.0.3/setup.py` & `bmpy-0.0.4/setup.py`

 * *Files identical despite different names*

