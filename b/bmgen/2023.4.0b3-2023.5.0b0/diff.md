# Comparing `tmp/bmgen-2023.4.0b3.tar.gz` & `tmp/bmgen-2023.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmgen-2023.4.0b3.tar", last modified: Tue Apr 18 17:39:56 2023, max compression
+gzip compressed data, was "bmgen-2023.5.0b0.tar", last modified: Mon May  1 10:57:05 2023, max compression
```

## Comparing `bmgen-2023.4.0b3.tar` & `bmgen-2023.5.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/
--rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.4.0b3/LICENSE
--rw-rw-r--   0 ever      (1000) ever      (1000)     2427 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)     2089 2023-04-18 17:26:41.000000 bmgen-2023.4.0b3/README.md
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.826132 bmgen-2023.4.0b3/bmgen/
--rw-rw-r--   0 ever      (1000) ever      (1000)     5387 2023-04-18 17:32:45.000000 bmgen-2023.4.0b3/bmgen/__main__.py
--rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-04-18 17:38:08.000000 bmgen-2023.4.0b3/bmgen/info.py
-drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/bmgen.egg-info/
--rw-r--r--   0 ever      (1000) ever      (1000)     2427 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/PKG-INFO
--rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/SOURCES.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/dependency_links.txt
--rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/entry_points.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/requires.txt
--rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-04-18 17:39:56.000000 bmgen-2023.4.0b3/bmgen.egg-info/top_level.txt
--rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-04-18 17:39:56.830132 bmgen-2023.4.0b3/setup.cfg
--rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.4.0b3/setup.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-05-01 10:57:05.751045 bmgen-2023.5.0b0/
+-rw-rw-r--   0 ever      (1000) ever      (1000)    15830 2023-04-17 17:28:00.000000 bmgen-2023.5.0b0/LICENSE
+-rw-rw-r--   0 ever      (1000) ever      (1000)     2450 2023-05-01 10:57:05.751045 bmgen-2023.5.0b0/PKG-INFO
+-rw-rw-r--   0 ever      (1000) ever      (1000)     2112 2023-04-21 18:00:53.000000 bmgen-2023.5.0b0/README.md
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-05-01 10:57:05.751045 bmgen-2023.5.0b0/bmgen/
+-rw-rw-r--   0 ever      (1000) ever      (1000)     7989 2023-04-22 19:05:57.000000 bmgen-2023.5.0b0/bmgen/__main__.py
+-rw-rw-r--   0 ever      (1000) ever      (1000)       28 2023-05-01 10:55:17.000000 bmgen-2023.5.0b0/bmgen/info.py
+drwxrwxr-x   0 ever      (1000) ever      (1000)        0 2023-05-01 10:57:05.751045 bmgen-2023.5.0b0/bmgen.egg-info/
+-rw-r--r--   0 ever      (1000) ever      (1000)     2450 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/PKG-INFO
+-rw-r--r--   0 ever      (1000) ever      (1000)      234 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/SOURCES.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/dependency_links.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)       46 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/entry_points.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        9 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/requires.txt
+-rw-r--r--   0 ever      (1000) ever      (1000)        1 2023-05-01 10:57:05.000000 bmgen-2023.5.0b0/bmgen.egg-info/top_level.txt
+-rw-rw-r--   0 ever      (1000) ever      (1000)       38 2023-05-01 10:57:05.751045 bmgen-2023.5.0b0/setup.cfg
+-rw-r--r--   0 ever      (1000) ever      (1000)      748 2023-04-17 17:23:18.000000 bmgen-2023.5.0b0/setup.py
```

### Comparing `bmgen-2023.4.0b3/LICENSE` & `bmgen-2023.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmgen-2023.4.0b3/PKG-INFO` & `bmgen-2023.5.0b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1
-Name: bmgen
-Version: 2023.4.0b3
-Summary: Broken Mouse Studios' build solution
-Home-page: https://git.brokenmouse.studio/bms/bmgen
-Author: bms
-Author-email: bmgen@brokenmouse.studio
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bmgen - Broken Mouse Studios' build solution
 
 ## DISCLAIMER
+
 This project is currently in it's beta phase!
 
 It needs to be cleaned up and does not yet have it's full set of features. You may quickly hit it's limits.
 
-You should expect API changes and are welcome to give feedback via https://git.brokenmouse.studio/bms/bmgen/issues
+You should expect API changes and are welcome to give feedback via <https://git.brokenmouse.studio/bms/bmgen/issues>
 
 ## Features
+
 - build scripts written in Python
 - incremental builds
 - temporary build directories
 - colorful and easy to read output
 - simple build commands
 
 ## Installation
+
 - Install bmgen via `pip install bmgen` or `python3 -m pip install bmgen`
 
 ## Building a simple C project
+
 This example shows a script which builds two files named `main.c` and `game.c` into a binary named `mygame` with `SDL2`.
 
 The directory structure created by bmgen will look like this:
-```
+
+```plain
 - bin/
   - dbg/
     - obj/
       - main.o
       - game.o
     - mygame
 ```
 
 The following is a breakdown of the script.
 
 1. First import the `clang` command:
+
 ```python
 from bmgen.commands.clang import clang
 ```
+
 2. Then set the base output directory and tell bmgen to create the base, variant and the `clang` command's object directory:
+
 ```python
 inst.base_output_dir = 'bin'
 inst.update_output_dir()
 clang.update_object_dir()
 ```
+
 3. Build the program via `clang`:
+
 ```python
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 The final `bmgen.py` looks like this:
+
 ```python
 from bmgen.commands.clang import clang
 
 inst.base_output_dir = 'bin'
 inst.update_output_dir()
 clang.update_object_dir()
 
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 Building the program is now as easy as running `bmgen` in your terminal!
 
 ## License
+
 © Broken Mouse Studios 2023<br>
-https://brokenmouse.studio
+<https://brokenmouse.studio>
 
 This software and it's accompanying files are licensed under the *Mozilla Public License Version 2.0*.
 
-For the license's contents, see [LICENSE](LICENSE) or go to https://mozilla.org/MPL/2.0/.
+For the license's contents, see [LICENSE](LICENSE) or go to <https://mozilla.org/MPL/2.0/>.
 
 By submitting patches or merge/pull requests, you grant Broken Mouse Studios the permission to use, copy, modify, distribute, publish and/or relicense the contributions you have made to the project.
```

### Comparing `bmgen-2023.4.0b3/bmgen/__main__.py` & `bmgen-2023.5.0b0/bmgen/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 from typing import List
 import argparse
+import json
 import os
 import subprocess
 import sys
 import tempfile
 import time
 
 import colorama
@@ -34,14 +35,15 @@
         return (f'{colorama.Fore.YELLOW}{colorama.Style.BRIGHT}[{prefix}]{colorama.Style.NORMAL} ' if prefix else '') + colorama.Fore.BLUE + ' '.join(printable_args) + colorama.Fore.RESET
     
     def __init__(self, args: any):
         self.base_output_dir = '.'
         self.command_id = 0
         self.failed_command_num = 0
         self.output_dir = ''
+        self.json_mode = args.json
         self.rebuild = args.rebuild
         self.release_mode = args.release
         self.variant_dir = None
     
     def print_error(self, msg: str, prefix: str='ERROR') -> None:
         print(f'{colorama.Fore.RED}{colorama.Style.BRIGHT}[{prefix}]{colorama.Style.NORMAL} {msg}{colorama.Fore.RESET}', file=sys.stderr)
     
@@ -51,58 +53,109 @@
         sys.exit(1)
     
     def skip_file(self, source_path: str, output_path: str) -> bool:
         return os.path.exists(output_path) and os.path.getmtime(source_path) < os.path.getmtime(output_path)
     
     def update_output_dir(self) -> None:
         base = self.base_output_dir
-        variant_dir = self.variant_dir if self.variant_dir else 'release' if self.release_mode else 'dbg'
+        if base == '':
+            print('The base output directory is an empty string!', file=sys.stderr)
+            sys.exit(1)
+        
+        base_link = None
+        split_base = os.path.normpath(base).split(os.path.sep)
+        for i, comp in enumerate(split_base):
+            if comp != '..':
+                base_link = os.path.sep.join(split_base[:i + 1])
+                break
+        if base_link == None:
+            base_link = base
+        
+        variant_dir = self.variant_dir if self.variant_dir is not None else 'release' if self.release_mode else 'dbg'
         new = os.path.join(base, variant_dir)
         self.output_dir = new
         
-        if os.path.islink(base):
-            if not os.path.exists(base):
-                os.makedirs(os.path.join(Path(base).resolve(), variant_dir), exist_ok=True)
-        else:
-            os.symlink(tempfile.mkdtemp(prefix='bmgen-'), base)
+        base_link_exists = os.path.exists(base_link)
+        base_link_islink = os.path.islink(base_link)
+        if base_link_exists and not base_link_islink:
+            base_link = os.path.join(base_link, variant_dir.split(os.path.sep)[0])
+            base_link_exists = os.path.exists(base_link)
+            base_link_islink = os.path.islink(base_link)
+        
+        if base_link_islink:
+            os.makedirs(Path(base_link).resolve(), exist_ok=True)
+        elif not base_link_exists:
+            os.symlink(tempfile.mkdtemp(prefix='bmgen-'), base_link)
+        
         os.makedirs(new, exist_ok=True)
     
-    def start_command(self, title: str) -> None:
-        print(f'{colorama.Fore.MAGENTA}{colorama.Style.BRIGHT}[{self.command_id}]{colorama.Style.NORMAL} {title}{colorama.Fore.RESET}')
+    def start_command(self, title: str, suffix: str | None=None) -> None:
+        if self.json_mode:
+            json_info = {
+                'type': 'command_start',
+                'id': self.command_id,
+                'title': title,
+            }
+            if suffix: json_info['suffix'] = suffix
+            print(json.dumps(json_info))
+        else:
+            print(f'{colorama.Fore.MAGENTA}{colorama.Style.BRIGHT}[{self.command_id}]{colorama.Style.NORMAL} {title}{f" [{suffix}]" if suffix else ""}{colorama.Fore.RESET}')
     
     def command_error(self, msg: str, mandatory: bool) -> None:
         self.failed_command_num += 1
         self.print_error(msg)
+        
         if mandatory:
+            self.end_command()
             self.abort(f'Mandatory command #{self.command_id} wasn\'t successfully executed!')
-        else:
-            self.print_error(f'Command #{self.command_id} failed!', prefix='FAIL')
+        
+        self.print_error(f'Command #{self.command_id} failed!', prefix='FAIL')
     
-    def exec_command(self, args: List[str], mandatory: bool, print_command: bool=True, output_file: str | None=None, skip: bool=False) -> None:
+    def exec_command(self, args: List[str], mandatory: bool, cwd: str | None=None, print_command: bool=True, output_file: str | None=None, skip: bool=False) -> None:
+        if self.json_mode:
+            json_info = {
+                'type': 'command_exec',
+                'args': args,
+                'mandatory': mandatory,
+                'cwd': cwd,
+                'print_command': print_command,
+                'skip': skip,
+            }
+            if output_file: json_info['output_file'] = output_file
+        
         if skip:
-            if print_command:
+            if self.json_mode:
+                print(json.dumps(json_info))
+            elif print_command:
                 print(bmgen.get_printable_command(args, prefix='SKIP; ' + output_file))
             return
         
-        printable_command = bmgen.get_printable_command(args, prefix=output_file)
-        if print_command:
-            print(printable_command + '\n' + bmgen.SEP_STR)
-        
-        proc = subprocess.run(args, text=True)
-        
-        print(bmgen.SEP_STR)
-        if proc.returncode != 0:
-            self.command_error(f'Command exited with a non-zero exit code ({proc.returncode}): {printable_command}', mandatory)
+        if not self.json_mode:
+            printable_command = bmgen.get_printable_command(args, prefix=output_file)
+            if print_command:
+                print(printable_command + '\n' + bmgen.SEP_STR)
+        
+        proc = subprocess.run(args, cwd=cwd, text=True)
+        
+        if self.json_mode:
+            print(json.dumps(json_info))
+        else:
+            print(bmgen.SEP_STR)
+            if proc.returncode != 0:
+                self.command_error(f'Command exited with a non-zero exit code ({proc.returncode}): {printable_command}', mandatory)
     
     def end_command(self):
+        if self.json_mode:
+            print(json.dumps({'type': 'command_end'}))
         self.command_id += 1
 
 def main() -> None:
     ap = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     ap.add_argument('--version', action='store_true', help='print version and exit')
+    ap.add_argument('--json', action='store_true', help='enable JSON output mode')
     ap.add_argument('-d', '--directory', default='.', help='specify the working directory')
     ap.add_argument('-s', '--script', default='bmgen.py', help="path of the build script to execute")
     ap.add_argument('-r', '--rebuild', action='store_true', help="force the execution of all commands")
     ap.add_argument('-R', '--release', action='store_true', help='build in release-mode')
     args = ap.parse_args()
     
     if args.version:
@@ -114,22 +167,39 @@
     if not os.path.exists(args.script):
         print(f'Script "{args.script}" does not exist!', file=sys.stderr)
         sys.exit(1)
     
     with open(args.script, 'r') as f:
         script_code = f.read()
     
-    # TODO separate the code for modifying builtins
-    start_time = time.time()
     inst = bmgen(args)
+    if inst.json_mode:
+        print(json.dumps({
+            'type': 'build_start',
+            'args': args.__dict__,
+        }))
+    start_time = time.time()
+    # TODO separate the code for modifying builtins
     exec('import builtins\nbuiltins.bmgen = _bmgen\nbuiltins.inst = _inst\ndel _bmgen\ndel _inst\n' + script_code, {}, {'_bmgen': bmgen, '_inst': inst})
+    run_duration = time.time() - start_time
     
-    if inst.command_id > 0:
-        print()
-    
-    print(f'{colorama.Fore.GREEN}{colorama.Style.BRIGHT}Build finished after {"%.3f"%(time.time() - start_time)} seconds')
-    if inst.failed_command_num > 0:
-        print(colorama.Fore.YELLOW, end='')
-    print(f'{inst.failed_command_num} command{"" if inst.failed_command_num == 1 else "s"} failed{colorama.Style.RESET_ALL}')
+    if inst.json_mode:
+        print(json.dumps({
+            'type': 'build_end',
+            'command_num': inst.command_id,
+            'failed_command_num': inst.failed_command_num,
+            'run_duration': run_duration,
+        }))
+    else:
+        if inst.command_id > 0:
+            print()
+        
+        print(f'{colorama.Fore.GREEN}{colorama.Style.BRIGHT}Finished after {"%.3f"%(run_duration)} seconds')
+        if inst.failed_command_num == inst.command_id:
+            print(f'{colorama.Fore.RED}All commands failed!{colorama.Style.RESET_ALL}')
+        else:
+            if inst.failed_command_num > 0:
+                print(colorama.Fore.YELLOW, end='')
+            print(f'{inst.failed_command_num} command{"" if inst.failed_command_num == 1 else "s"} failed{colorama.Style.RESET_ALL}')
 
 if __name__ == '__main__':
   main()
```

### Comparing `bmgen-2023.4.0b3/bmgen.egg-info/PKG-INFO` & `bmgen-2023.5.0b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,95 @@
 Metadata-Version: 2.1
 Name: bmgen
-Version: 2023.4.0b3
+Version: 2023.5.0b0
 Summary: Broken Mouse Studios' build solution
 Home-page: https://git.brokenmouse.studio/bms/bmgen
 Author: bms
 Author-email: bmgen@brokenmouse.studio
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bmgen - Broken Mouse Studios' build solution
 
 ## DISCLAIMER
+
 This project is currently in it's beta phase!
 
 It needs to be cleaned up and does not yet have it's full set of features. You may quickly hit it's limits.
 
-You should expect API changes and are welcome to give feedback via https://git.brokenmouse.studio/bms/bmgen/issues
+You should expect API changes and are welcome to give feedback via <https://git.brokenmouse.studio/bms/bmgen/issues>
 
 ## Features
+
 - build scripts written in Python
 - incremental builds
 - temporary build directories
 - colorful and easy to read output
 - simple build commands
 
 ## Installation
+
 - Install bmgen via `pip install bmgen` or `python3 -m pip install bmgen`
 
 ## Building a simple C project
+
 This example shows a script which builds two files named `main.c` and `game.c` into a binary named `mygame` with `SDL2`.
 
 The directory structure created by bmgen will look like this:
-```
+
+```plain
 - bin/
   - dbg/
     - obj/
       - main.o
       - game.o
     - mygame
 ```
 
 The following is a breakdown of the script.
 
 1. First import the `clang` command:
+
 ```python
 from bmgen.commands.clang import clang
 ```
+
 2. Then set the base output directory and tell bmgen to create the base, variant and the `clang` command's object directory:
+
 ```python
 inst.base_output_dir = 'bin'
 inst.update_output_dir()
 clang.update_object_dir()
 ```
+
 3. Build the program via `clang`:
+
 ```python
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 The final `bmgen.py` looks like this:
+
 ```python
 from bmgen.commands.clang import clang
 
 inst.base_output_dir = 'bin'
 inst.update_output_dir()
 clang.update_object_dir()
 
 clang('mygame', ['main.c', 'game.c'], ['sdl2'])
 ```
 
 Building the program is now as easy as running `bmgen` in your terminal!
 
 ## License
+
 © Broken Mouse Studios 2023<br>
-https://brokenmouse.studio
+<https://brokenmouse.studio>
 
 This software and it's accompanying files are licensed under the *Mozilla Public License Version 2.0*.
 
-For the license's contents, see [LICENSE](LICENSE) or go to https://mozilla.org/MPL/2.0/.
+For the license's contents, see [LICENSE](LICENSE) or go to <https://mozilla.org/MPL/2.0/>.
 
 By submitting patches or merge/pull requests, you grant Broken Mouse Studios the permission to use, copy, modify, distribute, publish and/or relicense the contributions you have made to the project.
```

### Comparing `bmgen-2023.4.0b3/setup.py` & `bmgen-2023.5.0b0/setup.py`

 * *Files identical despite different names*

