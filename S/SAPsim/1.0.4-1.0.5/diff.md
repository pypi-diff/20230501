# Comparing `tmp/SAPsim-1.0.4.tar.gz` & `tmp/SAPsim-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.4.tar", last modified: Sat Apr 29 17:18:47 2023, max compression
+gzip compressed data, was "SAPsim-1.0.5.tar", last modified: Mon May  1 02:38:25 2023, max compression
```

## Comparing `SAPsim-1.0.4.tar` & `SAPsim-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:47.276142 SAPsim-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-29 17:18:37.000000 SAPsim-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-29 17:18:47.276142 SAPsim-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-29 17:18:37.000000 SAPsim-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:47.272142 SAPsim-1.0.4/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:47.272142 SAPsim-1.0.4/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-29 17:18:37.000000 SAPsim-1.0.4/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:47.272142 SAPsim-1.0.4/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-29 17:18:47.000000 SAPsim-1.0.4/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-29 17:18:47.000000 SAPsim-1.0.4/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:18:47.000000 SAPsim-1.0.4/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 17:18:47.000000 SAPsim-1.0.4/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 17:18:47.000000 SAPsim-1.0.4/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-29 17:18:37.000000 SAPsim-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:18:47.276142 SAPsim-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-29 17:18:37.000000 SAPsim-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:47.276142 SAPsim-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/test_instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-29 17:18:37.000000 SAPsim-1.0.4/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-01 02:38:17.000000 SAPsim-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-01 02:38:25.953122 SAPsim-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 02:38:17.000000 SAPsim-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.949122 SAPsim-1.0.5/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-01 02:38:17.000000 SAPsim-1.0.5/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 02:38:25.000000 SAPsim-1.0.5/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-01 02:38:17.000000 SAPsim-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:38:25.953122 SAPsim-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 02:38:17.000000 SAPsim-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:25.953122 SAPsim-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-01 02:38:17.000000 SAPsim-1.0.5/tests/test_run.py
```

### Comparing `SAPsim-1.0.4/LICENSE` & `SAPsim-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/PKG-INFO` & `SAPsim-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.4 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.5 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `SAPsim-1.0.4/README.md` & `SAPsim-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim/utils/exceptions.py` & `SAPsim-1.0.5/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim/utils/execute.py` & `SAPsim-1.0.5/SAPsim/utils/execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,18 +72,22 @@
             * Table format
             * Options: https://github.com/astanin/python-tabulate#table-format
             * Default value in ``global_vars`` is ``"simple_outline"``
         * *bits* (``int``) --
             * Number of bits in unsigned registers
             * Default value in ``global_vars`` is 8
         * *non_blocking* (``bool``) --
+            * This is used to unit test debug mode of ``run()``, you likely don't have a need for this
             * If ``True``, then ``run()`` won't block on input
             * ``input()`` won't be called in debug mode (i.e., don't have to press enter to continue execution)
             * If this is ``True``, then debug mode will be on even if ``debug`` isn't in kwargs
-            * This is used to unit test debug mode of ``run()``
+        * *no_print* (``bool``) --
+            * This is used to save computation time during unit testing
+            * If ``True``, then ``print()`` won't be called, except for error messages
+
     :return: ``None``
     """
     if not isinstance(prog_path, str):
         raise TypeError("Required parameter prog_path must be a str.")
     if "debug" in kwargs and not isinstance(kwargs["debug"], bool):
         raise TypeError("Keyword argument debug must be a bool.")
     if "change" in kwargs and not isinstance(kwargs["change"], str):
@@ -99,14 +103,16 @@
     if not path.suffix == ".csv":
         raise exceptions.FileNotCSV(path)
     helpers.setup_8bit()
     parser.parse_csv(path)
     if "bits" in kwargs:
         assert kwargs["bits"] > 1
         global_vars.NUM_BITS_IN_REGISTERS = kwargs["bits"]
+        # Don't need to call setup_n_bit.
+        # All it does is change NUM_BITS_IN_REGISTERS and reset globals.
     if "change" in kwargs:
         changes = kwargs["change"].split(",")
         for change in changes:
             if change.count(":") != 1:
                 print(
                     "Invalid syntax for change parameter, correct format is <addr>:<base-10 value>, <addr>:<base-10 value>, ..."
                 )
@@ -125,39 +131,42 @@
                     f"Invalid base-10 value for change: {value}. Negative or overflows registers."
                 )
                 exit(1)
             global_vars.RAM[addr] = value
     if "table_format" in kwargs:
         global_vars.table_format = kwargs["table_format"]
     if kwargs.get("debug") or kwargs.get("non_blocking"):
-        print(f"Initial state of simulation of {prog_path}")
-        helpers.print_RAM()
-        helpers.print_info()
-        print("Debug mode: press Enter to execute next instruction ( > ).")
+        if not kwargs.get("no_print"):
+            print(f"Initial state of simulation of {prog_path}")
+            helpers.print_RAM()
+            helpers.print_info()
+            print("Debug mode: press Enter to execute next instruction ( > ).")
         if not kwargs.get("non_blocking"):
             input()
         while global_vars.EXECUTING:
             # Special case so that you don't have to press Enter twice to halt on a HLT instruction
             if (
                 global_vars.PC in global_vars.RAM
                 and helpers.parse_opcode(global_vars.RAM[global_vars.PC]) == 0xF
             ):
                 execute_next()
                 break
             execute_next()
-            helpers.print_RAM()
-            helpers.print_info()
+            if not kwargs.get("no_print"):
+                helpers.print_RAM()
+                helpers.print_info()
             if not kwargs.get("non_blocking"):
                 input()
         print("Program halted.")
     else:
         execute_full_speed()
-        helpers.print_RAM()
-        helpers.print_info()
-        print("Program halted.")
+        if not kwargs.get("no_print"):
+            helpers.print_RAM()
+            helpers.print_info()
+            print("Program halted.")
 
 
 @is_documented_by(
     run,
     2,
     "",
     r"""
```

### Comparing `SAPsim-1.0.4/SAPsim/utils/global_vars.py` & `SAPsim-1.0.5/SAPsim/utils/global_vars.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim/utils/helpers.py` & `SAPsim-1.0.5/SAPsim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim/utils/instructions.py` & `SAPsim-1.0.5/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim/utils/parser.py` & `SAPsim-1.0.5/SAPsim/utils/parser.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.5/SAPsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.4 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.5 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `SAPsim-1.0.4/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.5/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/pyproject.toml` & `SAPsim-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/setup.py` & `SAPsim-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Check https://pypi.org/project/SAPsim/ for latest version number
-    version="1.0.4",
+    version="1.0.5",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.4/tests/test_example_progs.py` & `SAPsim-1.0.5/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/tests/test_exceptions.py` & `SAPsim-1.0.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/tests/test_helpers.py` & `SAPsim-1.0.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/tests/test_instructions.py` & `SAPsim-1.0.5/tests/test_instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.4/tests/test_run.py` & `SAPsim-1.0.5/tests/test_run.py`

 * *Files identical despite different names*

