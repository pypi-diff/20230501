# Comparing `tmp/unitranscode-0.3.0.tar.gz` & `tmp/unitranscode-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.3.0.tar", last modified: Fri Apr 28 03:38:10 2023, max compression
+gzip compressed data, was "unitranscode-0.3.1.tar", last modified: Mon May  1 05:08:32 2023, max compression
```

## Comparing `unitranscode-0.3.0.tar` & `unitranscode-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.667604 unitranscode-0.3.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-04-28 03:38:10.667604 unitranscode-0.3.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.0/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-04-28 03:38:10.667604 unitranscode-0.3.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-04-28 03:37:51.000000 unitranscode-0.3.0/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.0/tests/test_transcoder.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.0/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.0/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    24953 2023-04-28 03:34:41.000000 unitranscode-0.3.0/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.3.0/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-28 03:38:10.663604 unitranscode-0.3.0/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-04-28 03:38:10.000000 unitranscode-0.3.0/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.766454 unitranscode-0.3.1/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.1/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-01 05:08:32.766454 unitranscode-0.3.1/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.1/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-01 05:08:32.766454 unitranscode-0.3.1/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-01 05:08:08.000000 unitranscode-0.3.1/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.1/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.1/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.1/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    25244 2023-05-01 05:05:38.000000 unitranscode-0.3.1/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.3.1/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:08:32.742454 unitranscode-0.3.1/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-01 05:08:32.000000 unitranscode-0.3.1/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.3.0/LICENSE` & `unitranscode-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.0/PKG-INFO` & `unitranscode-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.0
+Version: 0.3.1
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 License: UNKNOWN
 Keywords: unitranscode
 Platform: UNKNOWN
```

### Comparing `unitranscode-0.3.0/README.md` & `unitranscode-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.0/setup.py` & `unitranscode-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='unitranscode',
-    version='0.3.0',
+    version='0.3.1',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `unitranscode-0.3.0/tests/test_transcoder.py` & `unitranscode-0.3.1/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.0/unitranscode/custom_types.py` & `unitranscode-0.3.1/unitranscode/custom_types.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.0/unitranscode/transcoder.py` & `unitranscode-0.3.1/unitranscode/transcoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,28 +92,31 @@
                 self._proc.kill()
 
     @cached_property
     def input_files_info(self) -> List[EncodingInfo]:
         return [self.transcoder.info(i) for i in self.input_files]
 
     @property
-    def stdout_str(self):
-        return b''.join(self.stdout_chunks).decode()
+    def stdout_bytes(self):
+        return b''.join(self.stdout_chunks)
 
     @property
-    def stderr_str(self):
-        return b''.join(self.stderr_chunks).decode()
+    def stderr_bytes(self):
+        return b''.join(self.stderr_chunks)
 
     def exec_error(self, return_code: int, info=''):
         assert self.cmd
         full_cmd = ' '.join("'{}'".format(i) for i in self.cmd)
+        debug_cmd_output = self.stdout_bytes.decode(
+            errors='ignore'
+        ) + self.stderr_bytes.decode(errors='ignore')
         return UnitranscodeExecError(
             (
                 f'Failed to run ffmpeg ({return_code}): {info}'
-                f'{self.stdout_str}{self.stderr_str}\n'
+                f'{debug_cmd_output}\n'
                 f'Full command: {full_cmd}',
                 self.cmd,
             )
         )
 
 
 class Transcoder:
@@ -241,20 +244,20 @@
                 ),
             ],
             *['-vn', '-sn', '-f', 'null', '/dev/null'],
             duration_s=self.info(in_file).duration_s if on_progress else None,
             op=op,
             on_progress=on_progress,
         )
-        bracket_blobs = re.findall(r'{[^{}]*}', op.stderr_str)
+        bracket_blobs: List[bytes] = re.findall(rb'{[^{}]*}', op.stderr_bytes)
         if not bracket_blobs:
-            bracket_blobs = re.findall(r'{[^{}]*}', op.stdout_str)
+            bracket_blobs = re.findall(rb'{[^{}]*}', op.stdout_bytes)
             if not bracket_blobs:
                 raise op.exec_error(0, 'Unexpected ouput')
-        return json.loads(bracket_blobs[-1])
+        return json.loads(bracket_blobs[-1].decode(errors='ignore'))
 
     def normalize(
         self,
         in_file: str,
         out_file: str,
         norm_info: dict,
         level=-20.0,
@@ -692,26 +695,28 @@
         self.ffmpeg(
             *args,
             duration_s=self.info(in_file).duration_s,
             on_progress=on_progress,
             op=op,
         )
         pre, suff = out_file_fmt.split('%d')
-        op.output_files = sorted(
+        out_filenames_raw = sorted(
             re.findall(
-                r"^\s*\[[^]]*]\s*Opening '(.*)' for writing\s*$",
+                rb"^\s*\[[^]]*]\s*Opening '(.*)' for writing\s*$",
                 (
-                    op.stderr_str.replace('\r', '\n')
-                    + '\n'
-                    + op.stdout_str.replace('\r', '\n')
+                    op.stderr_bytes.replace(b'\r', b'\n')
+                    + b'\n'
+                    + op.stdout_bytes.replace(b'\r', b'\n')
                 ),
                 re.MULTILINE,
             ),
             key=lambda x: int(remove_prefix_suffix(x, pre, suff)),
         )
+        # We assume filenames don't have any non-utf8 characters
+        op.output_files = [i.decode() for i in out_filenames_raw]
         return op.output_files
 
     def chunk(
         self,
         in_file: str,
         split_size_seconds: Optional[int] = None,
         out_file_format='{in_base}-%d.{in_ext}',
```

### Comparing `unitranscode-0.3.0/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.3.1/unitranscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.0
+Version: 0.3.1
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 License: UNKNOWN
 Keywords: unitranscode
 Platform: UNKNOWN
```

