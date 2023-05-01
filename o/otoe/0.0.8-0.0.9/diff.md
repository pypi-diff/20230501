# Comparing `tmp/otoe-0.0.8.tar.gz` & `tmp/otoe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.8.tar", last modified: Mon Apr 17 15:00:23 2023, max compression
+gzip compressed data, was "otoe-0.0.9.tar", last modified: Mon May  1 11:59:24 2023, max compression
```

## Comparing `otoe-0.0.8.tar` & `otoe-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.760335 otoe-0.0.8/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-17 15:00:23.760175 otoe-0.0.8/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.8/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.758354 otoe-0.0.8/otoe/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      559 2023-04-17 14:58:04.000000 otoe-0.0.8/otoe/__init__.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-17 05:25:00.000000 otoe-0.0.8/otoe/config.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1153 2023-04-17 05:25:00.000000 otoe-0.0.8/otoe/exceptions.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     5034 2023-04-17 05:40:12.000000 otoe-0.0.8/otoe/obsidian.py
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.759281 otoe-0.0.8/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      310 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        7 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/requires.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       11 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 15:00:23.760377 otoe-0.0.8/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1297 2023-04-17 15:00:20.000000 otoe-0.0.8/setup.py
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.759785 otoe-0.0.8/tests/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        0 2023-04-09 15:50:13.000000 otoe-0.0.8/tests/__init__.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2260 2023-04-17 05:26:48.000000 otoe-0.0.8/tests/test_md.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2949 2023-04-17 05:27:00.000000 otoe-0.0.8/tests/test_otoe.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-05-01 11:59:24.368848 otoe-0.0.9/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2118 2023-05-01 11:59:24.368700 otoe-0.0.9/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1794 2023-04-19 12:24:16.000000 otoe-0.0.9/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-05-01 11:59:24.366299 otoe-0.0.9/otoe/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      657 2023-05-01 11:58:31.000000 otoe-0.0.9/otoe/__init__.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-17 05:25:00.000000 otoe-0.0.9/otoe/config.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      587 2023-04-22 06:35:59.000000 otoe-0.0.9/otoe/dialogs.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        0 2023-04-19 12:51:10.000000 otoe-0.0.9/otoe/espanso.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1162 2023-04-17 15:18:15.000000 otoe-0.0.9/otoe/exceptions.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     3328 2023-05-01 11:56:23.000000 otoe-0.0.9/otoe/obsidian.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1852 2023-04-22 06:35:59.000000 otoe-0.0.9/otoe/parsers.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-05-01 11:59:24.368366 otoe-0.0.9/otoe/tests/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        0 2023-04-09 15:50:13.000000 otoe-0.0.9/otoe/tests/__init__.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2336 2023-04-17 15:18:16.000000 otoe-0.0.9/otoe/tests/test_md.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2909 2023-04-17 15:18:16.000000 otoe-0.0.9/otoe/tests/test_otoe.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-05-01 11:59:24.367771 otoe-0.0.9/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2118 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      373 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        7 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/requires.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-05-01 11:59:24.000000 otoe-0.0.9/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-05-01 11:59:24.368891 otoe-0.0.9/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1129 2023-05-01 11:57:54.000000 otoe-0.0.9/setup.py
```

### Comparing `otoe-0.0.8/otoe/exceptions.py` & `otoe-0.0.9/otoe/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 class OtoeException(Exception):
     """Base class for all Otoe exceptions."""
+
     pass
 
 
 class OtoeFileNotFoundError(OtoeException, FileNotFoundError):
     """Raised when a file is not found."""
+
     pass
 
 
 class OtoeDirectoryNotFoundError(OtoeException, FileNotFoundError):
     """Raised when a directory is not found."""
+
     pass
 
 
 class OtoeMarkdownFileNotFoundError(OtoeException, FileNotFoundError):
     """Raised when a yaml file is not found."""
+
     pass
 
 
 class OtoeEmptyDirectoryError(OtoeException, FileNotFoundError):
     """Raised when a directory is empty."""
+
     pass
 
 
 class OtoeInvalidYamlError(OtoeException, ValueError):
     """Raised when a yaml file is invalid."""
+
     pass
 
 
 class OtoeEmptyYamlError(OtoeException, ValueError):
     """Raised when a yaml file is empty."""
+
     pass
 
 
 class OtoeEmptyMarkdownError(OtoeException, ValueError):
     """Raised when a markdown file is empty."""
+
     pass
 
 
 class OtoeValueError(OtoeException, ValueError):
     """Raised when a value is invalid."""
+
     pass
 
 
 class OtoeInvalidMarkdownError(OtoeException, ValueError):
     pass
```

### Comparing `otoe-0.0.8/setup.py` & `otoe-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import setuptools
 
-with open("README.md", "r") as fh:
+with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
-    name="otoe",                     # This is the name of the package
-    version="0.0.8",                        # The initial release version
-    author="Yakov Varnaev",                     # Full name of the author
-    description="Sort of a UI for espanso configs.",
-    long_description=long_description,      # Long description read from the the readme file
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # List of all python modules to be installed
+    name='otoe',  # This is the name of the package
+    version='0.0.9',  # The initial release version
+    author='Yakov Varnaev',  # Full name of the author
+    description='Sort of a UI for espanso configs.',
+    long_description=long_description,  # Long description read from the the readme file
+    long_description_content_type='text/markdown',
+    packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.7',                # Minimum version requirement of the package
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],  # Information to filter the project on PyPi website
+    python_requires='>=3.11',  # Minimum version requirement of the package
     # py_modules=['obsidian'],             # Name of the python package
     # package_dir={'': 'otoe'},     # Directory of the source code of the package
-    install_requires=['pyyaml'],                     # Install other dependencies if any
-    entry_points={
-        'console_scripts': [
-            'otoe=otoe:main',
-       ],
-    }
+    install_requires=['pyyaml'],  # Install other dependencies if any
+    entry_points={'console_scripts': ['otoe=otoe:main',],},
 )
```

### Comparing `otoe-0.0.8/tests/test_md.py` & `otoe-0.0.9/otoe/tests/test_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import pytest
 from pathlib import Path
-from otoe.exceptions import OtoeEmptyMarkdownError, OtoeEmptyYamlError, OtoeFileNotFoundError
+from otoe.exceptions import (
+    OtoeEmptyMarkdownError,
+    OtoeEmptyYamlError,
+    OtoeFileNotFoundError,
+)
 
 from otoe.obsidian import MarkDownParser
 
 
 class TestMD:
-
     def test_load(self, data_path: Path):
         file_path = data_path / 'test_load.md'
         md = MarkDownParser(file_path)
         assert md.data.strip() == 'test'
 
     def test_load_not_existing(self, data_path: Path):
         file_path = data_path / 'not_existing.md'
         with pytest.raises(OtoeFileNotFoundError):
             MarkDownParser(file_path)
 
-
     def test_parse_md_part(self, data_path: Path):
         file_path = data_path / 'test_parse_md.md'
         md = MarkDownParser(file_path)
         assert md.parse_md_part(md.data) == 'tests\nline2'
 
     def test_parse_yaml_trigger(self, data_path: Path):
         file_path = data_path / 'test_trigger.md'
         md = MarkDownParser(file_path)
         assert md.parse_yaml_part(md.data) == {'trigger': ':keyword'}
-        
+
     def test_parse_yaml_part(self, data_path: Path):
         file_path = data_path / 'test_parse_yaml.md'
         md = MarkDownParser(file_path)
-        assert md.parse_yaml_part(md.data) == {'trigger': ':year', 'vars': [{'format': '%Y', 'name': 'year', 'type': 'date'}]}
-
+        assert md.parse_yaml_part(md.data) == {
+            'trigger': ':year',
+            'vars': [{'format': '%Y', 'name': 'year', 'type': 'date'}],
+        }
 
     def test_parse_md(self, data_path: Path):
         file_path = data_path / 'test.md'
         md = MarkDownParser(file_path)
         assert md.parse() == {'trigger': ':test', 'replace': 'here is some text'}
 
     def test_parse_empty_md_part(self, data_path: Path):
@@ -50,8 +54,11 @@
         with pytest.raises(OtoeEmptyYamlError):
             md = MarkDownParser(file_path)
             md.parse_yaml_part(md.data)
 
     def test_md_with_separator_in_text(self, data_path: Path):
         file_path = data_path / 'contains_separator.md'
         md = MarkDownParser(file_path)
-        assert md.parse() == {'trigger': 'keyword', 'replace': 'it ==== contains ==== sep====arator\n\n```\nif bla:\n    raise ...  # <=================== here\n```'}
+        assert md.parse() == {
+            'trigger': 'keyword',
+            'replace': 'it ==== contains ==== sep====arator\n\n```\nif bla:\n    raise ...  # <=================== here\n```',
+        }
```

### Comparing `otoe-0.0.8/tests/test_otoe.py` & `otoe-0.0.9/otoe/tests/test_otoe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import pytest
 
 from pathlib import Path
-from otoe.exceptions import , OtoeEmptyDirectoryError, OtoeFileNotFoundError, OtoeMarkdownFileNotFoundError, OtoeNoMatchesError
+from otoe.exceptions import (
+    OtoeFileNotFoundError,
+    OtoeMarkdownFileNotFoundError,
+    OtoeNoMatchesError,
+)
 from otoe.obsidian import ObsidianParser
 
 
 class TestObsidianParser:
-
     def test_md_dir_not_found(self):
         with pytest.raises(OtoeFileNotFoundError):
             ObsidianParser('not_found')
 
     def test_md_dir_empty(self, data_path: Path):
         dir_path = data_path / 'empty_dir'
         with pytest.raises(OtoeMarkdownFileNotFoundError):
@@ -30,38 +33,37 @@
     # test if dir contains files and empty directories
     def test_md_dir_files_and_empty_dirs(self, data_path: Path):
         dir_path = data_path / 'files_and_empty_dirs'
         data = ObsidianParser(dir_path).get_md_files()
         assert 'base' in data
         assert len(data) == 1, 'empty directories should not be included in the result'
         assert sorted(data['base']) == [dir_path / f for f in ['test.md', 'test2.md']]
-        
+
     # test only md files are processed
     def test_only_md_files_are_processed(self, data_path: Path):
         dir_path = data_path / 'non_md_files_with_dirs'
         data = ObsidianParser(dir_path).get_md_files()
         assert 'base' in data
         assert 'dir' in data
         assert sorted(data['base']) == [dir_path / f for f in ['test.md']]
         assert sorted(data['dir']) == [dir_path / 'dir' / f for f in ['test.md']]
 
     # test if dir contains files and directories and files are markdown and yaml is empty
     def test_md_with_no_yaml_are_omitted(self, data_path: Path):
         dir_path = data_path / 'empty_yamls'
         with pytest.raises(OtoeNoMatchesError):
             ObsidianParser(dir_path).generate_matches()
-        
+
     # test if dir contains files and directories and files are markdown and yaml is valid and markdown is empty
     def test_md_with_no_text_are_omitted(self, data_path: Path):
         dir_path = data_path / 'empty_md'
         with pytest.raises(OtoeNoMatchesError):
             ObsidianParser(dir_path).generate_matches()
-            
+
     def test_md_with_yaml_are_processed(self, data_path: Path):
         dir_path = data_path / 'valid'
         data = ObsidianParser(dir_path).generate_matches()
         for dir in ['base', 'dir']:
             assert dir in data
             assert len(data[dir]) == 1
             match = data[dir][0]
             assert match == {'trigger': 'keyword', 'replace': 'test'}
-
```

