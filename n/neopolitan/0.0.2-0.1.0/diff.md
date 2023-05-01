# Comparing `tmp/neopolitan-0.0.2.tar.gz` & `tmp/neopolitan-0.1.0.tar.gz`

## Comparing `neopolitan-0.0.2.tar` & `neopolitan-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.0.2/.pylintrc
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.0.2/Notes.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.0.2/pytest.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopolitan-0.0.2/setup.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/ReadMe.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/const.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/neop.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/os_detection.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/testboardrunner.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/board_functions/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/board_functions/board.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/board_functions/board_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/board_functions/colors.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/abstract_board_display.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/abstract_display.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/graphical_board_display.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/graphical_display.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/hardware_board_display.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/display/hardware_display.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/writing/ReadMe.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/writing/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/writing/data_transformation.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/writing/groups_8.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.0.2/neopolitan/writing/letters_8.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/ReadMe.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/board_test.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/data_transformation_test.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/flip_test.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/groups_test.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.0.2/tests/process_board_data_test.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.0.2/visual_tests/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.0.2/visual_tests/demo_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.0.2/visual_tests/main_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 neopolitan-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.0.2/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.0.2/README.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 neopolitan-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 neopolitan-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.0/.pylintrc
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.0/Notes.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.0/pytest.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopolitan-0.1.0/setup.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/ReadMe.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/const.py
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/neop.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/os_detection.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/testboardrunner.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/board_functions/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/board_functions/board.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/board_functions/board_data.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/board_functions/colors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/abstract_board_display.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/abstract_display.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/graphical_board_display.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/graphical_display.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/hardware_board_display.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/display/hardware_display.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/writing/ReadMe.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/writing/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/writing/data_transformation.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/writing/groups_8.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.0/neopolitan/writing/letters_8.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/ReadMe.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/board_test.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/data_transformation_test.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/flip_test.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/groups_test.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.0/tests/process_board_data_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.0/visual_tests/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.0/visual_tests/demo_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.0/visual_tests/main_test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 neopolitan-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.0/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 neopolitan-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 neopolitan-0.1.0/PKG-INFO
```

### Comparing `neopolitan-0.0.2/.github/workflows/python-package.yml` & `neopolitan-0.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/ReadMe.md` & `neopolitan-0.1.0/neopolitan/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/neop.py` & `neopolitan-0.1.0/neopolitan/neop.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/testboardrunner.py` & `neopolitan-0.1.0/neopolitan/testboardrunner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 from threading import Thread
 from queue import Queue
 
-import __init__
 from neopolitan.neop import main
 
 # doesn't this also need to listen tho??
 
 def add_to_queue(q, e, t):
     time.sleep(t)
     q.put(e)
```

### Comparing `neopolitan-0.0.2/neopolitan/board_functions/board.py` & `neopolitan-0.1.0/neopolitan/board_functions/board.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/board_functions/board_data.py` & `neopolitan-0.1.0/neopolitan/board_functions/board_data.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/display/abstract_display.py` & `neopolitan-0.1.0/neopolitan/display/abstract_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/display/graphical_board_display.py` & `neopolitan-0.1.0/neopolitan/display/graphical_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/display/graphical_display.py` & `neopolitan-0.1.0/neopolitan/display/graphical_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/display/hardware_board_display.py` & `neopolitan-0.1.0/neopolitan/display/hardware_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/display/hardware_display.py` & `neopolitan-0.1.0/neopolitan/display/hardware_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/writing/ReadMe.md` & `neopolitan-0.1.0/neopolitan/writing/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/writing/data_transformation.py` & `neopolitan-0.1.0/neopolitan/writing/data_transformation.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/writing/groups_8.py` & `neopolitan-0.1.0/neopolitan/writing/groups_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/neopolitan/writing/letters_8.py` & `neopolitan-0.1.0/neopolitan/writing/letters_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/tests/board_test.py` & `neopolitan-0.1.0/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/tests/data_transformation_test.py` & `neopolitan-0.1.0/tests/data_transformation_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/tests/flip_test.py` & `neopolitan-0.1.0/tests/flip_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/tests/groups_test.py` & `neopolitan-0.1.0/tests/groups_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/tests/process_board_data_test.py` & `neopolitan-0.1.0/tests/process_board_data_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/.gitignore` & `neopolitan-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/LICENSE` & `neopolitan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/README.md` & `neopolitan-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.0.2/PKG-INFO` & `neopolitan-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: neopolitan
-Version: 0.0.2
-Summary: Test Neopolitan package
+Version: 0.1.0
+Summary: Neopolitan: a library for displaying text on LED boards
+Project-URL: Homepage, https://github.com/alyoshenka/neopolitan
 Author: alyo
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

