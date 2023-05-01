# Comparing `tmp/lskyup-0.1.1.tar.gz` & `tmp/lskyup-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lskyup-0.1.1.tar", last modified: Mon May  1 11:27:21 2023, max compression
+gzip compressed data, was "lskyup-0.1.2.tar", last modified: Mon May  1 11:39:58 2023, max compression
```

## Comparing `lskyup-0.1.1.tar` & `lskyup-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:27:21.474146 lskyup-0.1.1/
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)    35149 2023-05-01 09:17:04.000000 lskyup-0.1.1/LICENSE
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)      778 2023-05-01 11:27:21.471302 lskyup-0.1.1/PKG-INFO
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)      408 2023-05-01 10:56:35.000000 lskyup-0.1.1/README.md
-drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:27:21.455541 lskyup-0.1.1/lskyup/
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)       15 2023-05-01 10:20:22.000000 lskyup-0.1.1/lskyup/__init__.py
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)    10848 2023-05-01 11:26:41.000000 lskyup-0.1.1/lskyup/main.py
-drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:27:21.470031 lskyup-0.1.1/lskyup.egg-info/
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)      778 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/PKG-INFO
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)      242 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/SOURCES.txt
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)        1 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/dependency_links.txt
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)       43 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/entry_points.txt
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)       63 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/requires.txt
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)        7 2023-05-01 11:27:21.000000 lskyup-0.1.1/lskyup.egg-info/top_level.txt
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)       38 2023-05-01 11:27:21.474880 lskyup-0.1.1/setup.cfg
--rw-r--r--   0 zhuzhouyue   (501) staff       (20)      738 2023-05-01 11:26:22.000000 lskyup-0.1.1/setup.py
+drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:39:58.224522 lskyup-0.1.2/
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)    35149 2023-05-01 09:17:04.000000 lskyup-0.1.2/LICENSE
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)      778 2023-05-01 11:39:58.223600 lskyup-0.1.2/PKG-INFO
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)      408 2023-05-01 10:56:35.000000 lskyup-0.1.2/README.md
+drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:39:58.214592 lskyup-0.1.2/lskyup/
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)       15 2023-05-01 10:20:22.000000 lskyup-0.1.2/lskyup/__init__.py
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)    10941 2023-05-01 11:39:28.000000 lskyup-0.1.2/lskyup/main.py
+drwxr-xr-x   0 zhuzhouyue   (501) staff       (20)        0 2023-05-01 11:39:58.221884 lskyup-0.1.2/lskyup.egg-info/
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)      778 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/PKG-INFO
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)      242 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)        1 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)       43 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/entry_points.txt
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)       63 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/requires.txt
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)        7 2023-05-01 11:39:58.000000 lskyup-0.1.2/lskyup.egg-info/top_level.txt
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)       38 2023-05-01 11:39:58.224973 lskyup-0.1.2/setup.cfg
+-rw-r--r--   0 zhuzhouyue   (501) staff       (20)      738 2023-05-01 11:39:37.000000 lskyup-0.1.2/setup.py
```

### Comparing `lskyup-0.1.1/LICENSE` & `lskyup-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lskyup-0.1.1/PKG-INFO` & `lskyup-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lskyup
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool enables you to upload your img to your Lsky Server
 Author: JoeZhu
 Author-email: zhuzhouyue2005@outlook.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lskyup-0.1.1/lskyup/main.py` & `lskyup-0.1.2/lskyup/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 ███▌    ▄    ▄█    ███   ███ ▀███▄ ███   ███ ███    ███   ███        
 █████▄▄██  ▄████████▀    ███   ▀█▀  ▀█████▀  ████████▀   ▄████▀      
 ▀                        ▀                                           
     """,
                 fg="green"
                 )
     click.secho("""
-           Version 0.1.1 © JoeZhu ALL RIGHTS RESERVED
+           Version 0.1.2 © JoeZhu ALL RIGHTS RESERVED
                        LICENSE  GPL-V3
              CONTACT : zhuzhouyue2005@outlook.com
     """,
                 fg="yellow", bold=True)
     ctx.exit()
 
 
@@ -237,19 +237,22 @@
     setting(user_token, server_url)
 
 
 @cli.command()
 def clean():
     """Clean Img Cache"""
     dir_path = get_path("cache")
-    try:
-        shutil.rmtree(dir_path)
-        click.secho(f"{dir_path} Clean Img_cache successfully！", fg="green")
-    except OSError as e:
-        click.secho(f"Error: {dir_path} Fail to clean Img_cache！：{e}", fg="red")
+    if not os.path.exists(dir_path):
+        click.secho("The cache file has already been cleaned", fg="green")
+    else:
+        try:
+            shutil.rmtree(dir_path)
+            click.secho("Clean Img_cache successfully", fg="green")
+        except OSError as e:
+            click.secho(f"{dir_path} ERROR", fg="red")
 
 
 @cli.command()
 @click.option("-c", "--compress",
               is_flag=True,
               help="Compress your Images before uploading")
 @click.argument("img", nargs=-1, type=click.Path(exists=True))
```

### Comparing `lskyup-0.1.1/lskyup.egg-info/PKG-INFO` & `lskyup-0.1.2/lskyup.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lskyup
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool enables you to upload your img to your Lsky Server
 Author: JoeZhu
 Author-email: zhuzhouyue2005@outlook.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lskyup-0.1.1/setup.py` & `lskyup-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="lskyup",
     author="JoeZhu",
-    version="0.1.1",
+    version="0.1.2",
     author_email="zhuzhouyue2005@outlook.com",
     description="A tool enables you to upload your img to your Lsky Server",
     packages=find_packages(),
     install_requires=requirements,
     license="GPLv3+",
     entry_points={
         "console_scripts": ["lskyup = lskyup.main:cli"]
```

