# Comparing `tmp/xcsv_plot-0.2.0.tar.gz` & `tmp/xcsv_plot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsv_plot-0.2.0.tar", max compression
+gzip compressed data, was "xcsv_plot-0.3.0.tar", max compression
```

## Comparing `xcsv_plot-0.2.0.tar` & `xcsv_plot-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot-0.2.0/LICENSE
--rw-r--r--   0        0        0     4529 2023-03-26 19:11:15.830946 xcsv_plot-0.2.0/README.md
--rw-r--r--   0        0        0      714 2023-03-26 19:11:15.830946 xcsv_plot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    13534 2023-03-26 19:11:15.830946 xcsv_plot-0.2.0/xcsv/plot/__init__.py
--rw-r--r--   0        0        0     5025 2023-03-26 19:11:15.830946 xcsv_plot-0.2.0/xcsv/plot/__main__.py
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 xcsv_plot-0.2.0/setup.py
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 xcsv_plot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4529 2023-03-26 19:11:15.830946 xcsv_plot-0.3.0/README.md
+-rw-r--r--   0        0        0      714 2023-05-01 16:16:56.047116 xcsv_plot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12414 2023-05-01 16:17:15.947364 xcsv_plot-0.3.0/xcsv/plot/__init__.py
+-rw-r--r--   0        0        0     5025 2023-03-26 19:11:15.830946 xcsv_plot-0.3.0/xcsv/plot/__main__.py
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 xcsv_plot-0.3.0/setup.py
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 xcsv_plot-0.3.0/PKG-INFO
```

### Comparing `xcsv_plot-0.2.0/LICENSE` & `xcsv_plot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsv_plot-0.2.0/README.md` & `xcsv_plot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xcsv_plot-0.2.0/pyproject.toml` & `xcsv_plot-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcsv-plot"
-version = "0.2.0"
+version = "0.3.0"
 description = "Subpackage for plotting extended CSV (XCSV) files"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/paul-breen/xcsv-plot"
 homepage = "https://github.com/paul-breen/xcsv-plot"
 documentation = "https://github.com/paul-breen/xcsv-plot/blob/main/README.md"
@@ -13,15 +13,15 @@
 ]
 
 [tool.poetry.scripts]
 xcsv_plot = "xcsv.plot.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-xcsv = "^0.3.0"
+xcsv = "^0.4.0"
 matplotlib = "^3.5.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `xcsv_plot-0.2.0/xcsv/plot/__init__.py` & `xcsv_plot-0.3.0/xcsv/plot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # Project: Extended CSV common file format
 # Purpose: Classes to plot data from an extended CSV file
 # Author:  Paul M. Breen
 # Date:    2022-05-13
 ###############################################################################
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 import re
 
 import matplotlib.pyplot as plt
 
 import xcsv
 
@@ -58,47 +58,14 @@
         if xcol is None:
             extent = [0, max([len(dataset.data) - 1 for dataset in datasets]), min([dataset.data[ycol].min() for dataset in datasets]), max([dataset.data[ycol].max() for dataset in datasets])]
         else:
             extent = [min([dataset.data[xcol].min() for dataset in datasets]), max([dataset.data[xcol].max() for dataset in datasets]), min([dataset.data[ycol].min() for dataset in datasets]), max([dataset.data[ycol].max() for dataset in datasets])]
 
         return extent
 
-    def get_metadata_item_value(self, dataset, key, section='header'):
-        """
-        Get the value of the given key from the metadata dict of the given
-        dataset, or the empty string if not found
-
-        If the value is a list, then its elements are joined into a
-        newline-separated string, as it would appear in the original file
-
-        By default, the key is looked for in the 'header' section.  Set
-        section='column_headers' to look in the 'column_headers' section
-        instead.
-
-        :param dataset: The dataset to query
-        :type dataset: XCSV object
-        :param key: The header item key
-        :type key: str
-        :param section: The metadata section.
-        One of ['header','column_headers']
-        :type section: str
-        :returns: The value of the given key or the empty string if not found
-        :rtype: str
-        """
-
-        try:
-            value = dataset.metadata[section][key]
-
-            if isinstance(value, list):
-                value = '\n'.join(value)
-        except KeyError:
-            value = ''
-
-        return value
-
     def setup_data_plot(self, fig, ax, xlabel=None, ylabel=None, caption=None, caption_x=0.1, caption_y=0.02, caption_wrap=True, subplots_adjust_bottom=0.15):
         """
         Setup the data plot
 
         This sets fixed annotations, such as the x- and y-axis labels.
 
         :param fig: The figure object
@@ -317,18 +284,18 @@
 
         self.datasets = datasets
         self.xcol = xcol
         self.ycol = ycol
         generate_colors = True
 
         if not title:
-            title = self.get_metadata_item_value(datasets[0], self.DEFAULTS['title_key'])
+            title = datasets[0].get_metadata_item_value(self.DEFAULTS['title_key'])
 
         if not caption:
-            caption = self.get_metadata_item_value(datasets[0], self.DEFAULTS['caption_key'])
+            caption = datasets[0].get_metadata_item_value(self.DEFAULTS['caption_key'])
 
         if not label_key:
             label_key = self.DEFAULTS['label_key']
 
         if not xcol:
             if xidx is not None:
                 self.xcol = datasets[0].data.iloc[:, xidx].name
@@ -345,15 +312,15 @@
         if 'color' in opts:
             generate_colors = False
 
         self.fig.suptitle(title, wrap=title_wrap)
         self.setup_data_plot(self.fig, self.axs[axs_idx], caption=caption, xlabel=xlabel, ylabel=ylabel)
 
         for i, dataset in enumerate(datasets):
-            label = self.get_metadata_item_value(dataset, label_key)
+            label = dataset.get_metadata_item_value(label_key)
 
             if generate_colors:
                 opts.update({'color': f'C{i}'})
 
             self.plot_data(self.fig, self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
 
         if show:
```

### Comparing `xcsv_plot-0.2.0/xcsv/plot/__main__.py` & `xcsv_plot-0.3.0/xcsv/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `xcsv_plot-0.2.0/setup.py` & `xcsv_plot-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['plot']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.5.2,<4.0.0', 'xcsv>=0.3.0,<0.4.0']
+['matplotlib>=3.5.2,<4.0.0', 'xcsv>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['xcsv_plot = xcsv.plot.__main__:main']}
 
 setup_kwargs = {
     'name': 'xcsv-plot',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Subpackage for plotting extended CSV (XCSV) files',
     'long_description': "# xcsv-plot\n\nxcsv-plot is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot\n```\n\n## Using the package\n\nXCSV data can be plotted directly, as the data table is a `pandas` table:\n\n```python\ncontent.data.plot(x='time (year) [a]', y='depth (m)')\n```\n\nand of course for more control over the plot, the data can be plotted using `matplotlib`, say.\n\nBut an XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, and well-annotated column-headers, already provides much of the text needed to make an informative plot, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot` which provides methods to plot a given list of datasets (XCSV objects):\n\n```python\nimport xcsv\nimport xcsv.plot as xp\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xp.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python3 -m xcsv.plot --help\nusage: xcsv_plot [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                 [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                 [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                 [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE] [-b BG_IMG_PATH]\n                 [-o OUT_FILE] [-P PLOT_OPTS] [-S] [-V]\n                 in_file [in_file ...]\n\nplot the given XCSV files\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n  -P PLOT_OPTS, --plot-options PLOT_OPTS\n                        options for the plot, specified as a simple JSON\n                        object\n  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot\n  -V, --version         show program's version number and exit\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points:\n\npython3 -m xcsv.plot input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot -x 0 -y 1 input.csv\n```\n\n",
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/xcsv-plot',
```

### Comparing `xcsv_plot-0.2.0/PKG-INFO` & `xcsv_plot-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: xcsv-plot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Subpackage for plotting extended CSV (XCSV) files
 Home-page: https://github.com/paul-breen/xcsv-plot
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
-Requires-Dist: xcsv (>=0.3.0,<0.4.0)
+Requires-Dist: xcsv (>=0.4.0,<0.5.0)
 Project-URL: Documentation, https://github.com/paul-breen/xcsv-plot/blob/main/README.md
 Project-URL: Repository, https://github.com/paul-breen/xcsv-plot
 Description-Content-Type: text/markdown
 
 # xcsv-plot
 
 xcsv-plot is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files.
```

