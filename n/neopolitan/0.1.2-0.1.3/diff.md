# Comparing `tmp/neopolitan-0.1.2.tar.gz` & `tmp/neopolitan-0.1.3.tar.gz`

## Comparing `neopolitan-0.1.2.tar` & `neopolitan-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.2/.pylintrc
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.2/Notes.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.2/pytest.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.2/requirements.txt
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 neopolitan-0.1.2/setup.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/ReadMe.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/const.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/neop.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/os_detection.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/testboardrunner.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/board_functions/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/board_functions/board.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/board_functions/board_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/board_functions/colors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/abstract_board_display.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/abstract_display.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/graphical_board_display.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/graphical_display.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/hardware_board_display.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/display/hardware_display.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/writing/ReadMe.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/writing/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/writing/data_transformation.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/writing/groups_8.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.2/neopolitan/writing/letters_8.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/ReadMe.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/board_test.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/data_transformation_test.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/flip_test.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/groups_test.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.2/tests/process_board_data_test.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.2/visual_tests/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.2/visual_tests/demo_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.2/visual_tests/main_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 neopolitan-0.1.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.2/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.2/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.pylintrc
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.3/Notes.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.3/pytest.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/ReadMe.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/const.py
+-rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/neop.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/os_detection.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/testboardrunner.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/board.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/board_data.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/board_functions/colors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/abstract_board_display.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/abstract_display.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/graphical_board_display.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/graphical_display.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/hardware_board_display.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/display/hardware_display.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/ReadMe.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/data_transformation.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/groups_8.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.3/neopolitan/writing/letters_8.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/ReadMe.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/board_test.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/data_transformation_test.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/flip_test.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/groups_test.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.3/tests/process_board_data_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/demo_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.3/visual_tests/main_test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 neopolitan-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.3/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.3/PKG-INFO
```

### Comparing `neopolitan-0.1.2/.github/workflows/python-package.yml` & `neopolitan-0.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/ReadMe.md` & `neopolitan-0.1.3/neopolitan/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/neop.py` & `neopolitan-0.1.3/neopolitan/neop.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             # todo: error handling
         display.loop()
         if board_data.scroll_speed:
             board.scroll(wrap=board_data.should_wrap)
 
         time.sleep(board_data.scroll_wait)
 
+    del display
+
 def process_arguments():
     """Process the command line arguments and return them as a BoardData object"""
     board_data = default_board_data
 
     argument_list = sys.argv[1:]
     options = 'm:g:s:w:'
     long_options = ['message=', 'graphical=', 'scroll=', 'wrap=']
```

### Comparing `neopolitan-0.1.2/neopolitan/testboardrunner.py` & `neopolitan-0.1.3/neopolitan/testboardrunner.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/board_functions/board.py` & `neopolitan-0.1.3/neopolitan/board_functions/board.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/board_functions/board_data.py` & `neopolitan-0.1.3/neopolitan/board_functions/board_data.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/display/graphical_board_display.py` & `neopolitan-0.1.3/neopolitan/display/graphical_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/display/graphical_display.py` & `neopolitan-0.1.3/neopolitan/display/graphical_display.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         self.board = board
         self.size = size
         self.space = space
 
         self.board_display = GraphicalBoardDisplay(board, cols, rows)
         self.init_pygame()
 
+    def __del__(self):
+        """Clean up pygame"""
+        # pylint: disable=no-member
+        pygame.quit()
+
     def init_pygame(self):
         """Initialize pygame"""
         # ToDo
         # pylint: disable=no-member
         pygame.init()
         self.screen = pygame.display.set_mode((self.width, self.height))
         # pygame.display.set_caption('stock board simulator')
```

### Comparing `neopolitan-0.1.2/neopolitan/display/hardware_board_display.py` & `neopolitan-0.1.3/neopolitan/display/hardware_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/display/hardware_display.py` & `neopolitan-0.1.3/neopolitan/display/hardware_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/writing/ReadMe.md` & `neopolitan-0.1.3/neopolitan/writing/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/writing/data_transformation.py` & `neopolitan-0.1.3/neopolitan/writing/data_transformation.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/writing/groups_8.py` & `neopolitan-0.1.3/neopolitan/writing/groups_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/neopolitan/writing/letters_8.py` & `neopolitan-0.1.3/neopolitan/writing/letters_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/tests/board_test.py` & `neopolitan-0.1.3/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/tests/data_transformation_test.py` & `neopolitan-0.1.3/tests/data_transformation_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/tests/flip_test.py` & `neopolitan-0.1.3/tests/flip_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/tests/groups_test.py` & `neopolitan-0.1.3/tests/groups_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/tests/process_board_data_test.py` & `neopolitan-0.1.3/tests/process_board_data_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/.gitignore` & `neopolitan-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/LICENSE` & `neopolitan-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/README.md` & `neopolitan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.2/pyproject.toml` & `neopolitan-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "neopolitan"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "alyo" },
 ]
 description = "Neopolitan: a library for displaying text on LED boards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neopolitan-0.1.2/PKG-INFO` & `neopolitan-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopolitan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Neopolitan: a library for displaying text on LED boards
 Project-URL: Homepage, https://github.com/alyoshenka/neopolitan
 Author: alyo
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

