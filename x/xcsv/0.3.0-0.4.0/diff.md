# Comparing `tmp/xcsv-0.3.0.tar.gz` & `tmp/xcsv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsv-0.3.0.tar", max compression
+gzip compressed data, was "xcsv-0.4.0.tar", max compression
```

## Comparing `xcsv-0.3.0.tar` & `xcsv-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv-0.3.0/LICENSE
--rw-r--r--   0        0        0     7694 2023-01-15 18:54:16.521734 xcsv-0.3.0/README.md
--rw-r--r--   0        0        0      595 2023-01-15 19:26:51.150949 xcsv-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    20732 2023-01-15 19:26:58.402981 xcsv-0.3.0/xcsv/__init__.py
--rw-r--r--   0        0        0     8553 1970-01-01 00:00:00.000000 xcsv-0.3.0/setup.py
--rw-r--r--   0        0        0     8482 1970-01-01 00:00:00.000000 xcsv-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7694 2023-01-15 18:54:16.521734 xcsv-0.4.0/README.md
+-rw-r--r--   0        0        0      595 2023-05-01 15:51:38.053435 xcsv-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    27985 2023-05-01 15:52:06.485727 xcsv-0.4.0/xcsv/__init__.py
+-rw-r--r--   0        0        0     8553 1970-01-01 00:00:00.000000 xcsv-0.4.0/setup.py
+-rw-r--r--   0        0        0     8482 1970-01-01 00:00:00.000000 xcsv-0.4.0/PKG-INFO
```

### Comparing `xcsv-0.3.0/LICENSE` & `xcsv-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsv-0.3.0/README.md` & `xcsv-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xcsv-0.3.0/pyproject.toml` & `xcsv-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcsv"
-version = "0.3.0"
+version = "0.4.0"
 description = "Package for working with extended CSV (XCSV) files"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/paul-breen/xcsv"
 homepage = "https://github.com/paul-breen/xcsv"
 documentation = "https://github.com/paul-breen/xcsv/blob/main/README.md"
```

### Comparing `xcsv-0.3.0/xcsv/__init__.py` & `xcsv-0.4.0/xcsv/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # Project: Extended CSV common file format
 # Purpose: Classes to encapsulate an extended CSV file
 # Author:  Paul M. Breen
 # Date:    2022-04-14
 ###############################################################################
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 import re
 import argparse
 
 import pandas as pd
 
 def _parse_tokens(s, pattern):
@@ -28,26 +28,48 @@
     matches = re.search(pattern, s)
 
     if matches:
         tokens = matches.groupdict()
 
     return tokens
 
+def _get_type_cast_value(str_value):
+    """
+    Cast a string representation of the given value to the most
+    appropriate primitive numeric type
+
+    :param str_value: The string representation of the numeric value
+    :type str_value: str
+    :returns: A suitably cast primitive type of the value or the string as-is
+    :rtype: One of [int, float, str]
+    """
+
+    for func in [int, float]:
+        try:
+            cast_value = func(str_value)
+            return cast_value
+        except (ValueError, TypeError):
+            continue
+
+    return str_value
+
 class XCSV(object):
     """
     Class for an extended CSV object
     """
 
     DEFAULTS = {
+        'file_header_keys': ['value', 'units'],
         'file_header_default_key': 'value',
         'file_header_pattern': r'(?P<value>.+)\s+\((?P<units>.+)\)$',
-        'file_header_template': '{value} ({units})',
+        'file_header_templates': ['{value}', '({units})'],
+        'column_header_keys': ['name', 'units', 'notes'],
         'column_header_default_key': 'name',
         'column_header_pattern': r'(?P<name>[^][)(]+)(\s+\((?P<units>.+)\))?(\s+\[(?P<notes>.+)\])?$',
-        'column_header_template': '{name} ({units}) [{notes}]',
+        'column_header_templates': ['{name}', '({units})', '[{notes}]'],
         'missing_value_key': 'missing_value'
     }
 
     def __init__(self, metadata=None, data=None):
         """
         Constructor
 
@@ -79,34 +101,58 @@
         """
 
         pattern = cls.DEFAULTS['column_header_pattern']
 
         return _parse_tokens(s, pattern)
 
     @classmethod
-    def reconstruct_file_header_string(cls, d):
+    def recombine_list_header_string(cls, l, sep='\n'):
+        """
+        Recombine the header value string from the given list
+        """
+
+        return sep.join(l)
+
+    @classmethod
+    def _reconstruct_header_string(cls, d, keys, templates, sep=' '):
         """
         Reconstruct the header value string from the given dict
-        See `cls.DEFAULTS['file_header_template']`
+
+        If a member of the header dict is None, then it is not included
+        in the output value string.  This allows reconstructing the header
+        as it would have appeared in the original file.
         """
 
-        template = cls.DEFAULTS['file_header_template']
+        template_components = []
+
+        for key, tmpl in zip(keys, templates):
+            if key in d and d[key] is not None:
+                template_components.append(tmpl)
+
+        template = sep.join(template_components)
 
         return template.format(**d)
 
     @classmethod
+    def reconstruct_file_header_string(cls, d):
+        """
+        Reconstruct the header value string from the given dict
+        See `cls.DEFAULTS['file_header_templates']`
+        """
+
+        return cls._reconstruct_header_string(d, cls.DEFAULTS['file_header_keys'], cls.DEFAULTS['file_header_templates'])
+
+    @classmethod
     def reconstruct_column_header_string(cls, d):
         """
         Reconstruct the column header string from the given dict
-        See `cls.DEFAULTS['column_header_template']`
+        See `cls.DEFAULTS['column_header_templates']`
         """
 
-        template = cls.DEFAULTS['column_header_template']
-
-        return template.format(**d)
+        return cls._reconstruct_header_string(d, cls.DEFAULTS['column_header_keys'], cls.DEFAULTS['column_header_templates'])
 
     def get_column_header_name_map(self):
         """
         Get a map of column header labels to column header names
 
         :returns: The column map
         :rtype: dict
@@ -148,14 +194,181 @@
         """
         Rename the data column headers to their labels
         """
 
         col_map = self.get_column_header_label_map()
         self.data.rename(columns=col_map, inplace=True)
 
+    def get_metadata_item(self, key, section='header', default=None):
+        """
+        Get the value of the given key from the metadata dict,
+        or default if not found
+
+        The value can be a simple string, a list of strings, or a dict
+
+        By default, the key is looked for in the 'header' section.  Set
+        section='column_headers' to look in the 'column_headers' section
+        instead.
+
+        :param key: The header item key
+        :type key: str
+        :param section: The metadata section.
+        One of ['header','column_headers']
+        :type section: str
+        :param default: The value to return if no matching key exists
+        :type default: any
+        :returns: The value of the given key or default if not found
+        :rtype: any
+        """
+
+        if section not in ['header', 'column_headers']:
+            raise KeyError(f"Unknown metadata section: {section}")
+
+        try:
+            value = self.metadata[section][key]
+        except KeyError:
+            value = default
+
+        return value
+
+    def get_metadata_item_string(self, key, section='header', default=None):
+        """
+        Get the original string value of the given key from the metadata dict,
+        or default if not found
+
+        If the value is a dict, then it is reconstructed as a string,
+        as it would appear in the original file.
+
+        If the value is a list, then its elements are joined into a
+        newline-separated string, as it would appear in the original file.
+
+        Otherwise the key's value is returned as-is, a simple string.
+
+        By default, the key is looked for in the 'header' section.  Set
+        section='column_headers' to look in the 'column_headers' section
+        instead.
+
+        :param key: The header item key
+        :type key: str
+        :param section: The metadata section.
+        One of ['header','column_headers']
+        :type section: str
+        :param default: The value to return if no matching key exists
+        :type default: any
+        :returns: The simple value of the given key or default if not found
+        :rtype: any
+        """
+
+        if section == 'header':
+            reconstruct_func = XCSV.reconstruct_file_header_string
+        elif section == 'column_headers':
+            reconstruct_func = XCSV.reconstruct_column_header_string
+        else:
+            raise KeyError(f"Unknown metadata section: {section}")
+
+        try:
+            value = self.metadata[section][key]
+
+            if isinstance(value, dict):
+                value = reconstruct_func(value)
+
+            if isinstance(value, list):
+                value = XCSV.recombine_list_header_string(value)
+        except KeyError:
+            value = default
+
+        return value
+
+    def get_metadata_item_value(self, key, section='header', default=None, cast=False):
+        """
+        Get the simple value of the given key from the metadata dict,
+        or default if not found
+
+        If the value is a dict, then the 'value' member for header items,
+        or 'name' member for column_headers items, is returned.
+
+        If the value is a list, then its elements are joined into a
+        newline-separated string, as it would appear in the original file.
+
+        If cast is true, then an attempt is made to cast the value to the
+        most appropriate numeric primitive type.  One of [int, float].
+
+        Otherwise the key's value is returned as-is, a simple string.
+
+        By default, the key is looked for in the 'header' section.  Set
+        section='column_headers' to look in the 'column_headers' section
+        instead.
+
+        :param key: The header item key
+        :type key: str
+        :param section: The metadata section.
+        One of ['header','column_headers']
+        :type section: str
+        :param default: The value to return if no matching key exists
+        :type default: any
+        :param cast: Cast scalar numeric string value to most appropriate
+        primitive type.  One of [int, float]
+        :type cast: bool
+        :returns: The simple value of the given key or default if not found
+        :rtype: any
+        """
+
+        if section == 'header':
+            subdict_key = self.DEFAULTS['file_header_default_key']
+        elif section == 'column_headers':
+            subdict_key = self.DEFAULTS['column_header_default_key']
+        else:
+            raise KeyError(f"Unknown metadata section: {section}")
+
+        try:
+            value = self.metadata[section][key]
+
+            if subdict_key in value:
+                value = value[subdict_key]
+
+            if isinstance(value, list):
+                value = XCSV.recombine_list_header_string(value)
+
+            if cast:
+                value = _get_type_cast_value(value)
+        except KeyError:
+            value = default
+
+        return value
+
+    def get_notes_for_column_header(self, key, default=None):
+        """
+        Get the string value of the extended header section item that
+        corresponds to the 'notes' element of the given column header key,
+        or default if not found
+
+        :param key: The column_headers item key
+        :type key: str
+        :param default: The value to return if no matching key exists
+        :type default: any
+        :returns: The header value corresponding to the notes element of the
+        given column header key or default if not found
+        :rtype: any
+        """
+
+        value = default
+        column_header = self.get_metadata_item(key, section='column_headers')
+
+        if column_header is not None:
+            try:
+                notes_id = column_header['notes']
+            except KeyError:
+                notes_id = None
+
+            if notes_id is not None:
+                header_key = f"[{notes_id}]"
+                value = self.get_metadata_item_string(header_key)
+
+        return value
+
 class Reader(object):
     """
     Class for reading extended CSV data from a file
     """
 
     def __init__(self, fp=None):
         """
@@ -344,28 +557,21 @@
         Cast a string representation of the missing_value to the most
         appropriate type, if it is present in the extended header section
 
         :returns: A suitably cast primitive type of the missing_value or None
         :rtype: One of [int, float, str, None]
         """
 
-        str_value = None
+        value = None
         key = XCSV.DEFAULTS['missing_value_key']
 
         if key in self.header:
-            str_value = self.header[key]
-
-            for func in [int, float]:
-                try:
-                    cast_value = func(str_value)
-                    return cast_value
-                except ValueError:
-                    continue
+            value = _get_type_cast_value(self.header[key])
 
-        return str_value
+        return value
 
     def mask_missing_values(self):
         """
         Mask any missing values in the data
 
         Missing values are defined by the missing_value header item
```

### Comparing `xcsv-0.3.0/setup.py` & `xcsv-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'xcsv',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Package for working with extended CSV (XCSV) files',
     'long_description': "# xcsv\n\nxcsv is a package for reading and writing extended CSV files.\n\n## Extended CSV format\n\n* Extended header section of parseable atttributes, introduced by '#'.\n* Header row of variable and units for each column.\n* Data rows.\n\n### Example\n\n#### Extended header section\n\n* No leading/trailing whitespace.\n* Each line introduced by a comment ('#') character.\n* Each line contains a single header item.\n* Key/value separator ': '.\n* Multi-line values naturally continued over to the next lines following the line introducing the key.\n* Continuation lines that contain the delimiter character in the value must be escaped by a leading delimiter.\n* Preferably use a common vocabulary for attribute name, such as [CF conventions](http://cfconventions.org/index.html).\n* Preferably include recommended attributes from [Attribute Convention for Data Discovery (ACDD)](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3).\n* Preferably use units from [Unified Code for Units of Measure](https://ucum.org/ucum.html) and/or [Udunits](https://www.unidata.ucar.edu/software/udunits/).\n* Units in parentheses.\n* Certain special keys are used to [further process the data](#automated-post-processing-of-the-data), for example the `missing_value` key.\n\n```\n# id: 1\n# title: The title\n# summary: This dataset...\n# The second summary paragraph.\n# : The third summary paragraph.  Escaped because it contains the delimiter in a URL https://dummy.domain\n# authors: A B, C D\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\n# elevation: 1897 (m a.s.l.)\n# [a]: 2012 not a complete year\n```\n\n#### Header row\n\n* No leading/trailing whitespace.\n* Preferably use a common vocabulary for variable name, such as [CF conventions](http://cfconventions.org/index.html).\n* Units in parentheses.\n* Optional notes in square brackets, that reference an item in the extended header section.\n\n```\ntime (year) [a],depth (m)\n```\n\n#### Data row\n\n* No leading/trailing whitespace.\n\n```\n2012,0.575\n```\n\n#### Automated post-processing of the data\n\nDepending on the presence of special keys in the extended header section, these will be used to automatically post-process the data.  To turn off this automatic behaviour, either remove or rename these keys, or set `parse_metadata=False` when reading in the data.\n\n* `missing_value`:  This is used to define those values in the data that are to be considered as missing values.  This is typically a value that is outside the domain of the data such as `-999.99`, or can be a symbolic value such as `NA`.  All such values appearing in the data will be masked, appearing as an `NA` value to pandas (i.e. `pd.isna(value)` returns `True`).  Note that pandas itself will automatically do this for certain values regardless of this key, such as for the strings `NaN` or `NA`, or the constant `None`.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv\n```\n\n## Using the package\n\nThe package has a general `XCSV` class, that has a `metadata` attribute that holds the parsed contents of the extended file header section and the parsed column headers from the data table, and a `data` attribute that holds the data table (including the column headers as-is).\n\nThe `metadata` attribute is a `dict`, with the following general structure:\n\n```python\n{'header': {}, 'column_headers': {}}\n```\n\nand the `data` attribute is a `pandas.DataFrame`, and so has all the features of the [pandas](https://pandas.pydata.org/docs/index.html) package.\n\nThe package also has a `Reader` class for reading an extended CSV file into an `XCSV` object, and similarly a `Writer` class for writing an `XCSV` object to a file in the extended CSV format.  In addition there is a `File` class that provides a convenient context manager for reading and writing these files.\n\n### Examples\n\n#### Simple read and print\n\nRead in a file and print the contents to `stdout`.  This shows how the contents of the extended CSV file are stored in the `XCSV` object.  Note how multi-line values, such as `summary` here, are stored in a list.  Given the following script called, say, `simple_read.py`:\n\n```python\nimport argparse\n\nimport xcsv\n\nparser = argparse.ArgumentParser()\nparser.add_argument('filename', help='filename.csv')\nargs = parser.parse_args()\n\nwith xcsv.File(args.filename) as f:\n    content = f.read()\n    print(content.metadata)\n    print(content.data)\n```\n\nRunning it would produce:\n\n```bash\n$ python3 simple_read.py example.csv\n{'header': {'id': '1', 'title': 'The title', 'summary': ['This dataset...', 'The second summary paragraph.', 'The third summary paragraph.  Escaped because it contains the delimiter in a URL https://dummy.domain'], 'authors': 'A B, C D', 'latitude': {'value': '-73.86', 'units': 'degree_north'}, 'longitude': {'value': '-65.46', 'units': 'degree_east'}, 'elevation': {'value': '1897', 'units': 'm a.s.l.'}, '[a]': '2012 not a complete year'}, 'column_headers': {'time (year) [a]': {'name': 'time', 'units': 'year', 'notes': 'a'}, 'depth (m)': {'name': 'depth', 'units': 'm', 'notes': None}}}\n   time (year) [a]  depth (m)\n0             2012      0.575\n1             2011      1.125\n2             2010      2.225\n```\n\n#### Simple read and print with missing values\n\nIf the above example header section included the following:\n\n```\n# missing_value: -999.99\n```\n\nand the data section looked like:\n\n```\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n2009,-999\n2008,999\n2007,-999.99\n2006,999.99\n2005,NA\n2004,NaN\n```\n\nRunning it would produce:\n\n```bash\n$ python3 simple_read.py missing_example.csv\n{'header': {'id': '1', 'title': 'The title', 'summary': ['This dataset...', 'The second summary paragraph.', 'The third summary paragraph.  Escaped because it contains the delimiter in a URL https://dummy.domain'], 'authors': 'A B, C D', 'latitude': {'value': '-73.86', 'units': 'degree_north'}, 'longitude': {'value': '-65.46', 'units': 'degree_east'}, 'elevation': {'value': '1897', 'units': 'm a.s.l.'}, 'missing_value': '-999.99', '[a]': '2012 not a complete year'}, 'column_headers': {'time (year) [a]': {'name': 'time', 'units': 'year', 'notes': 'a'}, 'depth (m)': {'name': 'depth', 'units': 'm', 'notes': None}}}\n   time (year) [a]  depth (m)\n0             2012      0.575\n1             2011      1.125\n2             2010      2.225\n3             2009   -999.000\n4             2008    999.000\n5             2007        NaN\n6             2006    999.990\n7             2005        NaN\n8             2004        NaN\n```\n\nNote that the `-999.99` value has been automatically masked as a missing value (shown as `NaN` in the printed pandas `DataFrame`), as well as the `NA` and `NaN` strings in the original data, which pandas automatically masks itself, irrespective of the `missing_value` header item.\n\n#### Simple read and plot\n\nRead a file and plot the data:\n\n```python\nimport argparse\n\nimport matplotlib.pyplot as plt\n\nimport xcsv\n\nparser = argparse.ArgumentParser()\nparser.add_argument('filename', help='filename.csv')\nargs = parser.parse_args()\n\nwith xcsv.File(args.filename) as f:\n    content = f.read()\n    content.data.plot(x='depth (m)', y='time (year) [a]')\n    plt.show()\n```\n\n#### Simple read and write\n\nRead a file in, manipulate the data in some way, and write this modified `XCSV` object out to a new file:\n\n```python\nimport argparse\n\nimport xcsv\n\nparser = argparse.ArgumentParser()\nparser.add_argument('in_filename', help='in_filename.csv')\nparser.add_argument('out_filename', help='out_filename.csv')\nargs = parser.parse_args()\n\nwith xcsv.File(args.in_filename) as f:\n    content = f.read()\n\n# Manipulate the data...\n\nwith xcsv.File(args.out_filename, mode='w') as f:\n    f.write(xcsv=content)\n```\n\n",
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/xcsv',
```

### Comparing `xcsv-0.3.0/PKG-INFO` & `xcsv-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsv
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for working with extended CSV (XCSV) files
 Home-page: https://github.com/paul-breen/xcsv
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

