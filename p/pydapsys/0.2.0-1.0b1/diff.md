# Comparing `tmp/pydapsys-0.2.0.tar.gz` & `tmp/pydapsys-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydapsys-0.2.0.tar", max compression
+gzip compressed data, was "pydapsys-1.0b1.tar", max compression
```

## Comparing `pydapsys-0.2.0.tar` & `pydapsys-1.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1580 2023-03-10 18:58:03.069491 pydapsys-0.2.0/LICENSE
--rw-r--r--   0        0        0     5594 2023-05-01 10:00:25.233504 pydapsys-0.2.0/README.md
--rw-r--r--   0        0        0       93 2023-05-01 09:53:49.285933 pydapsys-0.2.0/pydapsys/__init__.py
--rw-r--r--   0        0        0    11074 2023-05-01 09:58:19.156021 pydapsys-0.2.0/pydapsys/binaryreader.py
--rw-r--r--   0        0        0     3570 2023-05-01 09:53:49.308933 pydapsys-0.2.0/pydapsys/file.py
--rw-r--r--   0        0        0     1027 2023-05-01 09:41:17.193387 pydapsys-0.2.0/pydapsys/neo_converters/__init__.py
--rw-r--r--   0        0        0     9323 2023-05-01 09:36:27.665418 pydapsys-0.2.0/pydapsys/neo_converters/helper.py
--rw-r--r--   0        0        0      334 2023-05-01 07:54:23.697527 pydapsys-0.2.0/pydapsys/neo_converters/interface.py
--rw-r--r--   0        0        0     5383 2023-05-01 09:53:49.303933 pydapsys-0.2.0/pydapsys/neo_converters/ni_pulse_stim.py
--rw-r--r--   0        0        0     1823 2023-03-08 10:13:49.890995 pydapsys-0.2.0/pydapsys/page.py
--rw-r--r--   0        0        0     4926 2023-04-04 14:49:11.762581 pydapsys-0.2.0/pydapsys/read.py
--rw-r--r--   0        0        0       70 2023-05-01 09:53:49.298933 pydapsys-0.2.0/pydapsys/toc/__init__.py
--rw-r--r--   0        0        0      970 2023-04-04 14:49:11.762581 pydapsys-0.2.0/pydapsys/toc/display.py
--rw-r--r--   0        0        0     4326 2023-04-04 14:49:11.762581 pydapsys-0.2.0/pydapsys/toc/entry.py
--rw-r--r--   0        0        0     1072 2023-04-04 14:48:28.559904 pydapsys-0.2.0/pydapsys/toc/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-31 15:29:24.391135 pydapsys-0.2.0/pydapsys/util/__init__.py
--rw-r--r--   0        0        0      342 2023-01-31 15:35:28.305695 pydapsys-0.2.0/pydapsys/util/floats.py
--rw-r--r--   0        0        0     3286 2023-04-04 13:35:15.855031 pydapsys-0.2.0/pydapsys/util/structs.py
--rw-r--r--   0        0        0      932 2023-05-01 09:25:16.013016 pydapsys-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6684 1970-01-01 00:00:00.000000 pydapsys-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1580 2023-03-10 18:58:03.069491 pydapsys-1.0b1/LICENSE
+-rw-r--r--   0        0        0     5604 2023-04-04 15:18:26.917594 pydapsys-1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-02-01 10:54:52.662661 pydapsys-1.0b1/pydapsys/__init__.py
+-rw-r--r--   0        0        0    11074 2023-04-02 10:57:22.614984 pydapsys-1.0b1/pydapsys/binaryreader.py
+-rw-r--r--   0        0        0     3106 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/file.py
+-rw-r--r--   0        0        0        0 2023-01-31 09:49:52.052722 pydapsys-1.0b1/pydapsys/neo_convert/__init__.py
+-rw-r--r--   0        0        0     9705 2023-04-04 14:25:22.974192 pydapsys-1.0b1/pydapsys/neo_convert/abstract_converter.py
+-rw-r--r--   0        0        0     5316 2023-03-19 09:37:53.746926 pydapsys-1.0b1/pydapsys/neo_convert/ni_pulse_stim.py
+-rw-r--r--   0        0        0     1823 2023-03-08 10:13:49.890995 pydapsys-1.0b1/pydapsys/page.py
+-rw-r--r--   0        0        0     4926 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/read.py
+-rw-r--r--   0        0        0        0 2023-01-13 15:03:45.620258 pydapsys-1.0b1/pydapsys/toc/__init__.py
+-rw-r--r--   0        0        0      970 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/toc/display.py
+-rw-r--r--   0        0        0     4326 2023-04-04 14:49:11.762581 pydapsys-1.0b1/pydapsys/toc/entry.py
+-rw-r--r--   0        0        0     1072 2023-04-04 14:48:28.559904 pydapsys-1.0b1/pydapsys/toc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-01-31 15:29:24.391135 pydapsys-1.0b1/pydapsys/util/__init__.py
+-rw-r--r--   0        0        0      342 2023-01-31 15:35:28.305695 pydapsys-1.0b1/pydapsys/util/floats.py
+-rw-r--r--   0        0        0     3286 2023-04-04 13:35:15.855031 pydapsys-1.0b1/pydapsys/util/structs.py
+-rw-r--r--   0        0        0      803 2023-04-04 14:53:29.208657 pydapsys-1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 pydapsys-1.0b1/setup.py
+-rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 pydapsys-1.0b1/PKG-INFO
```

### Comparing `pydapsys-0.2.0/LICENSE` & `pydapsys-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/README.md` & `pydapsys-1.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PyDapsys - Read DAPSYS recordings with Python
 
 [![PyPI](https://img.shields.io/pypi/v/pydapsys?style=for-the-badge)](https://pypi.org/project/pydapsys/)
 
 PyDapsys is a package to read neurography recordings made with [DAPSYS](http://dapsys.net/) (Data Acquisition Processor System). It is based on a reverse-engineered specification of the binary data format used by the latest DAPSYS version.
 
-Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastructures, from where they can be exported into various other formats.
+Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastrucutres, from where they can be exported into various other formats.
 
 ## Installation
 
 Either download the wheel file for offline installation or use pypi.
 
 ### Basic functionalities
 
@@ -31,33 +31,33 @@
 ### Quickstart
 
 A DAPSYS file is made up of two parts: A sequential list of blocks or **pages**, which store either a text with a timestamp or a waveform with associated timestamps, and a table of contents (toc). The toc consists of **folders** and **streams**. Each page has an id unique in the context of the file. Streams in the toc have an array of ids of the pages belonging to the stream. A stream is either a text stream (referring only to text pages) or a data stream (referring only to recording pages).
 
 #### Load a file
 Use `File.from_binary` to read from a BinaryIO object.
 ```python
-from pydapsys import read_file
+from pydapsys.file import File
 from pathlib import Path
 MY_DAPSYS_FILE = Path(".")/"to"/"my"/"dapsys_file.dps"
 with open(MY_DAPSYS_FILE, 'rb') as file:
-    file = read_file(file)
+    file = File.from_binary(file)
 ```
 The `File` object has two fields, the root of the table of contents and a dictionary mapping the page ids to their respective pages.
 ##### Inspect file structure
 To inspect the ToC structure of a loaded file, use the `structure` property of the toc `Root`, preferable together with `pprint`:
 ```python
 import pprint
 pprint.PrettyPrinter(indent=4).pprint(file.toc.structure)
 ```
 This will print the structure, names and types of all elements in the table of contents. For Streams, the number of associated pages it also printed after their type.
 #### Access data from a file
 To access data, use the `File.get_data` method. The method takes a path from the toc structure (WITHOUT THE NAME OF THE ROOT!) and will return all associated pages.
 Please note, that the path is  case insensitive
 ```python
-from pydapsys.toc import StreamType
+from pydapsys.toc.entry import StreamType
 my_texts = list(file.get_data("myrecording/my text stream", stype=StreamType.Text))
 my_waveforms = list(file.get_data("myrecording/somewhere else/ my waveform stream", stype=StreamType.Waveform))
 ```
 ##### Text pages
 
 A text page consists of three fields:
 
@@ -91,18 +91,18 @@
 
 ### NI Pulse stimulator
 
 Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence. 
 Waveform pages of the continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold (`grouping_tolerance`).
 
 ```python
-from pydapsys.neo_converters import NIPulseStimRecordingConverter
+from pydapsys.neo_convert.ni_pulse_stim import NIPulseStimulatorToNeo
 
 # convert a recording to a neo block
-neo_block = NIPulseStimRecordingConverter(file, grouping_tolerance=1e-9).to_neo()
+neo_block = NIPulseStimulatorToNeo(file, grouping_tolerance=1e-9).to_neo()
 ```
 
 #### Expected file structure
 
 {stim_folder} must be one of "NI Puls Stimulator", "pulse stimulator", "NI Pulse stimulator", but can be changed by adding entries to `NIPulseStimulatorToNeo.stim_foler_names`
 
 * Root
```

### Comparing `pydapsys-0.2.0/pydapsys/binaryreader.py` & `pydapsys-1.0b1/pydapsys/binaryreader.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/file.py` & `pydapsys-1.0b1/pydapsys/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,16 +63,7 @@
         """Reads a DAPSYS file from the given binary io object and directly constructs a new File class from it.
         :param binio: BinaryIO object to read from
         :param byte_order: byte order to use when reading from the binary io object. Defaults to little endian.
         :return: The File object constructed from the contents of the io stream
         """
         toc_root, pages = read_from(binio, byte_order=byte_order)
         return File(toc_root, pages)
-
-
-def read_file(binio: BinaryIO, byte_order='<') -> File:
-    """Reads a DAPSYS file from the given binary io object and directly constructs a new File class from it.
-    :param binio: BinaryIO object to read from
-    :param byte_order: byte order to use when reading from the binary io object. Defaults to little endian.
-    :return: The File object constructed from the contents of the io stream
-    """
-    return File.from_binary(binio, byte_order=byte_order)
```

### Comparing `pydapsys-0.2.0/pydapsys/neo_converters/helper.py` & `pydapsys-1.0b1/pydapsys/neo_convert/abstract_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+from abc import ABC, abstractmethod
 from typing import Sequence, Union, Optional, Iterable, List, Dict
 
 import neo
 import numpy as np
 import numpy.typing as npt
 import quantities as pq
 
 from pydapsys.file import File
 from pydapsys.page import DataPage, WaveformPage, TextPage, PageType
 from pydapsys.toc.entry import Stream, StreamType
 from pydapsys.util.floats import float_comp
 
 
-class DapsysToNeoHelper:
-    """ Converter to put various Dapsys streams neo structures
-
+class DapsysToNeoConverter(ABC):
+    """ Converter to put Dapsys recordings into the neo structure
 
+    This abstract base class provides common functionalities to transform Dapsys streams into common neo structures
     :param file: PyDapsys dapsys file
     """
 
     def __init__(self, file: File):
         self.file = file
 
+    @abstractmethod
+    def to_neo(self) -> neo.Block:
+        """
+        Create a neo structure based on the given recording
+        :return: A neo block containing the data from the recording
+        """
+        ...
+
     def _get_datapage_typechecked(self, pid: int, ptype: PageType) -> DataPage:
         """
         gets the page with the given id and checks if it is of the requested type.
         Throws an exception if the type doesn't match
         """
         page = self.file.pages[pid]
         if page.type != ptype:
```

### Comparing `pydapsys-0.2.0/pydapsys/neo_converters/ni_pulse_stim.py` & `pydapsys-1.0b1/pydapsys/neo_convert/ni_pulse_stim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import datetime
 from typing import Optional, Iterable
 
 import neo
 
 from pydapsys.file import File
-from pydapsys.neo_converters.helper import DapsysToNeoHelper
-from pydapsys.neo_converters.interface import INeoConverter
+from pydapsys.neo_convert.abstract_converter import DapsysToNeoConverter
 from pydapsys.toc.entry import Folder, Stream, StreamType
 
 
-class NIPulseStimRecordingConverter(DapsysToNeoHelper, INeoConverter):
+class NIPulseStimulatorToNeo(DapsysToNeoConverter):
     """Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence.
     Waveform pages of continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold.
 
 
     Expected structure is:
 
     - Root
```

### Comparing `pydapsys-0.2.0/pydapsys/page.py` & `pydapsys-1.0b1/pydapsys/page.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/read.py` & `pydapsys-1.0b1/pydapsys/read.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/toc/display.py` & `pydapsys-1.0b1/pydapsys/toc/display.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/toc/entry.py` & `pydapsys-1.0b1/pydapsys/toc/entry.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/toc/exceptions.py` & `pydapsys-1.0b1/pydapsys/toc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pydapsys/util/structs.py` & `pydapsys-1.0b1/pydapsys/util/structs.py`

 * *Files identical despite different names*

### Comparing `pydapsys-0.2.0/pyproject.toml` & `pydapsys-1.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 [tool.poetry]
 name = "pydapsys"
-version = "0.2.0"
+version = "1.0b1"
 description = "Read recordings made with DAPSYS"
 authors = ["Peter Konradi <codingchipmunk@posteo.net>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/Digital-C-Fiber/PyDapsys"
 keywords = ["microneurography", "dapsys", "neurophysiology", "electrophysiology"]
 classifiers = ["Development Status :: 4 - Beta",
-    "Intended Audience :: Developers", "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers","Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3 :: Only",
-]
+    ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21"
-neo = { version = ">=0.12, <1", optional = true }
+neo = { version = "^0.11.1", optional = true }
 
 [tool.poetry.extras]
 neo = ["neo"]
 
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-Sphinx = "^6.1.3"
-sphinx-book-theme = "^1.0.0"
-
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydapsys-0.2.0/PKG-INFO` & `pydapsys-1.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydapsys
-Version: 0.2.0
+Version: 1.0b1
 Summary: Read recordings made with DAPSYS
 Home-page: https://github.com/Digital-C-Fiber/PyDapsys
 License: BSD-3-Clause
 Keywords: microneurography,dapsys,neurophysiology,electrophysiology
 Author: Peter Konradi
 Author-email: codingchipmunk@posteo.net
 Requires-Python: >=3.8,<4.0
@@ -13,29 +13,28 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: neo
-Requires-Dist: neo (>=0.12,<1) ; extra == "neo"
+Requires-Dist: neo (>=0.11.1,<0.12.0); extra == "neo"
 Requires-Dist: numpy (>=1.21,<2.0)
 Project-URL: Repository, https://github.com/Digital-C-Fiber/PyDapsys
 Description-Content-Type: text/markdown
 
 # PyDapsys - Read DAPSYS recordings with Python
 
 [![PyPI](https://img.shields.io/pypi/v/pydapsys?style=for-the-badge)](https://pypi.org/project/pydapsys/)
 
 PyDapsys is a package to read neurography recordings made with [DAPSYS](http://dapsys.net/) (Data Acquisition Processor System). It is based on a reverse-engineered specification of the binary data format used by the latest DAPSYS version.
 
-Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastructures, from where they can be exported into various other formats.
+Optionally, the library provides functionality to store loaded data into [Neo](https://github.com/NeuralEnsemble/python-neo) datastrucutres, from where they can be exported into various other formats.
 
 ## Installation
 
 Either download the wheel file for offline installation or use pypi.
 
 ### Basic functionalities
 
@@ -58,33 +57,33 @@
 ### Quickstart
 
 A DAPSYS file is made up of two parts: A sequential list of blocks or **pages**, which store either a text with a timestamp or a waveform with associated timestamps, and a table of contents (toc). The toc consists of **folders** and **streams**. Each page has an id unique in the context of the file. Streams in the toc have an array of ids of the pages belonging to the stream. A stream is either a text stream (referring only to text pages) or a data stream (referring only to recording pages).
 
 #### Load a file
 Use `File.from_binary` to read from a BinaryIO object.
 ```python
-from pydapsys import read_file
+from pydapsys.file import File
 from pathlib import Path
 MY_DAPSYS_FILE = Path(".")/"to"/"my"/"dapsys_file.dps"
 with open(MY_DAPSYS_FILE, 'rb') as file:
-    file = read_file(file)
+    file = File.from_binary(file)
 ```
 The `File` object has two fields, the root of the table of contents and a dictionary mapping the page ids to their respective pages.
 ##### Inspect file structure
 To inspect the ToC structure of a loaded file, use the `structure` property of the toc `Root`, preferable together with `pprint`:
 ```python
 import pprint
 pprint.PrettyPrinter(indent=4).pprint(file.toc.structure)
 ```
 This will print the structure, names and types of all elements in the table of contents. For Streams, the number of associated pages it also printed after their type.
 #### Access data from a file
 To access data, use the `File.get_data` method. The method takes a path from the toc structure (WITHOUT THE NAME OF THE ROOT!) and will return all associated pages.
 Please note, that the path is  case insensitive
 ```python
-from pydapsys.toc import StreamType
+from pydapsys.toc.entry import StreamType
 my_texts = list(file.get_data("myrecording/my text stream", stype=StreamType.Text))
 my_waveforms = list(file.get_data("myrecording/somewhere else/ my waveform stream", stype=StreamType.Waveform))
 ```
 ##### Text pages
 
 A text page consists of three fields:
 
@@ -118,18 +117,18 @@
 
 ### NI Pulse stimulator
 
 Converter class for Dapsys recording created using an NI Pulse stimulator. Puts everything into one neo sequence. 
 Waveform pages of the continuous recording are merged if the difference between a pair of consecutive pages is less than a specified threshold (`grouping_tolerance`).
 
 ```python
-from pydapsys.neo_converters import NIPulseStimRecordingConverter
+from pydapsys.neo_convert.ni_pulse_stim import NIPulseStimulatorToNeo
 
 # convert a recording to a neo block
-neo_block = NIPulseStimRecordingConverter(file, grouping_tolerance=1e-9).to_neo()
+neo_block = NIPulseStimulatorToNeo(file, grouping_tolerance=1e-9).to_neo()
 ```
 
 #### Expected file structure
 
 {stim_folder} must be one of "NI Puls Stimulator", "pulse stimulator", "NI Pulse stimulator", but can be changed by adding entries to `NIPulseStimulatorToNeo.stim_foler_names`
 
 * Root
```

