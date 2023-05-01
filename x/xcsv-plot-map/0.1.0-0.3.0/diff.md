# Comparing `tmp/xcsv-plot-map-0.1.0.tar.gz` & `tmp/xcsv_plot_map-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsv-plot-map-0.1.0.tar", last modified: Wed May 18 21:29:23 2022, max compression
+gzip compressed data, was "xcsv_plot_map-0.3.0.tar", max compression
```

## Comparing `xcsv-plot-map-0.1.0.tar` & `xcsv_plot_map-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv-plot-map-0.1.0/LICENSE
--rw-r--r--   0        0        0     5871 2022-05-18 19:45:36.841703 xcsv-plot-map-0.1.0/README.md
--rw-r--r--   0        0        0      817 2022-05-18 20:48:30.325446 xcsv-plot-map-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12701 2022-05-17 07:27:29.675387 xcsv-plot-map-0.1.0/xcsv/plot_map/__init__.py
--rw-r--r--   0        0        0     5173 2022-05-18 19:27:29.676890 xcsv-plot-map-0.1.0/xcsv/plot_map/__main__.py
--rw-r--r--   0        0        0     6924 2022-05-18 21:29:23.614770 xcsv-plot-map-0.1.0/setup.py
--rw-r--r--   0        0        0     6745 2022-05-18 21:29:23.615145 xcsv-plot-map-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot_map-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6213 2023-03-27 08:49:05.970225 xcsv_plot_map-0.3.0/README.md
+-rw-r--r--   0        0        0      836 2023-05-01 19:20:53.512312 xcsv_plot_map-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22015 2023-05-01 19:17:05.273533 xcsv_plot_map-0.3.0/xcsv/plot_map/__init__.py
+-rw-r--r--   0        0        0     5747 2023-03-27 08:49:05.974225 xcsv_plot_map-0.3.0/xcsv/plot_map/__main__.py
+-rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 xcsv_plot_map-0.3.0/setup.py
+-rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 xcsv_plot_map-0.3.0/PKG-INFO
```

### Comparing `xcsv-plot-map-0.1.0/LICENSE` & `xcsv_plot_map-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsv-plot-map-0.1.0/README.md` & `xcsv_plot_map-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,20 +66,21 @@
 
 ## Command line usage
 
 Calling the script with the `--help` option will show the following usage:
 
 ```bash
 $ python -m xcsv.plot_map --help
-usage: __main__.py [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
-                   [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
-                   [--invert-y-axis] [--title TITLE] [--caption CAPTION]
-                   [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
-                   [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
-                   in_file [in_file ...]
+usage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
+                     [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
+                     [--invert-y-axis] [--title TITLE] [--caption CAPTION]
+                     [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
+                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
+                     [-P PLOT_OPTS] [-S] [-V]
+                     in_file [in_file ...]
 
 plot the given XCSV files and locate the data on a map
 
 positional arguments:
   in_file               input XCSV file(s)
 
 optional arguments:
@@ -109,14 +110,19 @@
                         projection to use for displaying the site coordinates
                         on the map (one of the CRS classes provided by
                         Cartopy)
   -b BG_IMG_PATH, --background-image BG_IMG_PATH
                         path to an image to show in the background of the plot
   -o OUT_FILE, --out-file OUT_FILE
                         output plot file
+  -P PLOT_OPTS, --plot-options PLOT_OPTS
+                        options for the plot, specified as a simple JSON
+                        object
+  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot
+  -V, --version         show program's version number and exit
 
 Examples
 
 Given an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:
 
 # id: 1
 # title: The title
```

### Comparing `xcsv-plot-map-0.1.0/pyproject.toml` & `xcsv_plot_map-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcsv-plot-map"
-version = "0.1.0"
+version = "0.3.0"
 description = "Subpackage to plot and locate on a map, data from extended CSV (XCSV) files"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/paul-breen/xcsv-plot-map"
 homepage = "https://github.com/paul-breen/xcsv-plot-map"
 documentation = "https://github.com/paul-breen/xcsv-plot-map/blob/main/README.md"
@@ -13,17 +13,18 @@
 ]
 
 [tool.poetry.scripts]
 xcsv_plot_map = "xcsv.plot_map.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-xcsv-plot = "^0.1.0"
+xcsv-plot = "^0.3.0"
 matplotlib = "^3.5.2"
-Cartopy = "^0.20.2"
+Cartopy = "^0.21.1"
+shapely = "^2.0.1"
 scipy = "^1.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `xcsv-plot-map-0.1.0/xcsv/plot_map/__main__.py` & `xcsv_plot_map-0.3.0/xcsv/plot_map/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Project: Extended CSV common file format
 # Purpose: Classes to plot data from an extended CSV file
 # Author:  Paul M. Breen
 # Date:    2022-05-13
 ###############################################################################
 
 import argparse
+import json
 
 import cartopy.crs as ccrs
 
 import xcsv
 import xcsv.plot_map as xpm
 
 def get_datasets(filenames):
@@ -67,15 +68,15 @@
 2010,2.225
 
 then the columns to be used for the x- and y-axes can be specified thus:
 
 python3 -m xcsv.plot_map -x 0 -y 1 input.csv
 """
 
-    parser = argparse.ArgumentParser(description='plot the given XCSV files and locate the data on a map', epilog=epilog, formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser = argparse.ArgumentParser(description='plot the given XCSV files and locate the data on a map', epilog=epilog, formatter_class=argparse.RawDescriptionHelpFormatter, prog='xcsv_plot_map')
 
     parser.add_argument('in_file', help='input XCSV file(s)', nargs='+')
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument('-x', '--x-idx', help='column index (zero-based) containing values for the x-axis', dest='xidx', default=None, type=int)
     group.add_argument('-X', '--x-column', help='column label containing values for the x-axis', dest='xcol', default=None, type=str)
 
@@ -96,32 +97,41 @@
     parser.add_argument('-s', '--figsize', help='size of the figure (width height)', dest='figsize', nargs=2, default=None, type=int)
     parser.add_argument('-p', '--map-projection', help='projection to use for displaying the site coordinates on the map (one of the CRS classes provided by Cartopy)', dest='projection', default=None, type=str)
 
     parser.add_argument('-b', '--background-image', help='path to an image to show in the background of the plot', dest='bg_img_path', default=None, type=str)
 
     parser.add_argument('-o', '--out-file', help='output plot file')
 
+    parser.add_argument('-P', '--plot-options', help="options for the plot, specified as a simple JSON object", dest='plot_opts', default={}, type=json.loads)
+    parser.add_argument('-S', '--scatter-plot', help="set plot options (see -P) to produce a scatter plot", dest='plot_opts', action='store_const', const={'marker': '.', 'ls': ''})
+
+    parser.add_argument('-V', '--version', action='version', version=f"%(prog)s {xpm.__version__}")
+
     args = parser.parse_args()
 
     return args
 
 def main():
     """
     Main function
     """
 
     args = parse_cmdln()
     datasets = get_datasets(args.in_file)
     plotter = xpm.Plot()
 
     if args.figsize or args.projection:
-        projection = xpm.Plot().get_crs_class_from_string(args.projection)
+        if args.projection:
+            projection = xpm.Plot().get_crs_class_from_string(args.projection)
+        else:
+            projection = None
+
         plotter.setup_figure_and_axes(figsize=args.figsize, projection=projection)
 
-    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, title_wrap=True, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, show=False)
+    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, title_wrap=True, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, show=False, opts=args.plot_opts)
 
     if args.bg_img_path:
         plotter.add_plot_bg(img_path=args.bg_img_path)
 
     if args.out_file:
         plotter.savefig(args.out_file)
     else:
```

### Comparing `xcsv-plot-map-0.1.0/setup.py` & `xcsv_plot_map-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 packages = \
 ['plot_map']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Cartopy>=0.20.2,<0.21.0',
+['Cartopy>=0.21.1,<0.22.0',
  'matplotlib>=3.5.2,<4.0.0',
  'scipy>=1.8.1,<2.0.0',
- 'xcsv-plot>=0.1.0,<0.2.0']
+ 'shapely>=2.0.1,<3.0.0',
+ 'xcsv-plot>=0.3.0,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['xcsv_plot_map = xcsv.plot_map.__main__:main']}
 
 setup_kwargs = {
     'name': 'xcsv-plot-map',
-    'version': '0.1.0',
+    'version': '0.3.0',
     'description': 'Subpackage to plot and locate on a map, data from extended CSV (XCSV) files',
-    'long_description': "# xcsv-plot-map\n\nxcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot-map\n```\n\n## Notes on installing Cartopy\n\nxcsv-plot-map has a dependency on Cartopy.  In turn, Cartopy requires the Proj library.  If you find that you can't install Cartopy because the version of the Proj library on your system is too old, then you can build a local version of the Proj library.  This should be a fairly straightforward build.  You may then find that the Cartopy package installs OK, but that you get the following segfault at runtime when trying to use xcsv-plot-map:\n\n```bash\nfree(): invalid size\nAborted (core dumped)\n```\n\nThis is a known issue.  A suggested fix for this is to reinstall the Python `shapely` package.  First remove it:\n\n```bash\n$ pip uninstall shapely\n```\n\nand then reinstall it with specific `pip` options:\n\n```bash\n$ pip install --no-binary :all: shapely\n```\n\nThis may take a while, but should resolve the segfault issue and everything should work.\n\n## Using the package\n\nAn XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, including geographical coordinates in `longitude` and `latitude` header items, and well-annotated column-headers, already provides much of the text needed to make an informative plot and map, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot-map` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot_map -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot-map` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot_map -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot`.  This is inherited from the `xcsv-plot.Plot` class, with some overridden methods.  The class provides methods to plot a given list of datasets (XCSV objects), and locate them on a map:\n\n```python\nimport xcsv\nimport xcsv.plot_map as xpm\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xpm.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python -m xcsv.plot_map --help\nusage: __main__.py [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                   [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                   [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                   [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]\n                   [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]\n                   in_file [in_file ...]\n\nplot the given XCSV files and locate the data on a map\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -p PROJECTION, --map-projection PROJECTION\n                        projection to use for displaying the site coordinates\n                        on the map (one of the CRS classes provided by\n                        Cartopy)\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points, and will locate the coordinates on a map:\n\npython3 -m xcsv.plot_map input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot_map -x 0 -y 1 input.csv\n```\n\n",
+    'long_description': "# xcsv-plot-map\n\nxcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot-map\n```\n\n## Notes on installing Cartopy\n\nxcsv-plot-map has a dependency on Cartopy.  In turn, Cartopy requires the Proj library.  If you find that you can't install Cartopy because the version of the Proj library on your system is too old, then you can build a local version of the Proj library.  This should be a fairly straightforward build.  You may then find that the Cartopy package installs OK, but that you get the following segfault at runtime when trying to use xcsv-plot-map:\n\n```bash\nfree(): invalid size\nAborted (core dumped)\n```\n\nThis is a known issue.  A suggested fix for this is to reinstall the Python `shapely` package.  First remove it:\n\n```bash\n$ pip uninstall shapely\n```\n\nand then reinstall it with specific `pip` options:\n\n```bash\n$ pip install --no-binary :all: shapely\n```\n\nThis may take a while, but should resolve the segfault issue and everything should work.\n\n## Using the package\n\nAn XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, including geographical coordinates in `longitude` and `latitude` header items, and well-annotated column-headers, already provides much of the text needed to make an informative plot and map, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot-map` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot_map -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot-map` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot_map -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot`.  This is inherited from the `xcsv-plot.Plot` class, with some overridden methods.  The class provides methods to plot a given list of datasets (XCSV objects), and locate them on a map:\n\n```python\nimport xcsv\nimport xcsv.plot_map as xpm\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xpm.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python -m xcsv.plot_map --help\nusage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                     [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                     [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                     [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]\n                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]\n                     [-P PLOT_OPTS] [-S] [-V]\n                     in_file [in_file ...]\n\nplot the given XCSV files and locate the data on a map\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -p PROJECTION, --map-projection PROJECTION\n                        projection to use for displaying the site coordinates\n                        on the map (one of the CRS classes provided by\n                        Cartopy)\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n  -P PLOT_OPTS, --plot-options PLOT_OPTS\n                        options for the plot, specified as a simple JSON\n                        object\n  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot\n  -V, --version         show program's version number and exit\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points, and will locate the coordinates on a map:\n\npython3 -m xcsv.plot_map input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot_map -x 0 -y 1 input.csv\n```\n\n",
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/xcsv-plot-map',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11',
 }
```

### Comparing `xcsv-plot-map-0.1.0/PKG-INFO` & `xcsv_plot_map-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: xcsv-plot-map
-Version: 0.1.0
+Version: 0.3.0
 Summary: Subpackage to plot and locate on a map, data from extended CSV (XCSV) files
 Home-page: https://github.com/paul-breen/xcsv-plot-map
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Cartopy (>=0.20.2,<0.21.0)
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: Cartopy (>=0.21.1,<0.22.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
-Requires-Dist: xcsv-plot (>=0.1.0,<0.2.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
+Requires-Dist: xcsv-plot (>=0.3.0,<0.4.0)
 Project-URL: Documentation, https://github.com/paul-breen/xcsv-plot-map/blob/main/README.md
 Project-URL: Repository, https://github.com/paul-breen/xcsv-plot-map
 Description-Content-Type: text/markdown
 
 # xcsv-plot-map
 
 xcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.
@@ -87,20 +89,21 @@
 
 ## Command line usage
 
 Calling the script with the `--help` option will show the following usage:
 
 ```bash
 $ python -m xcsv.plot_map --help
-usage: __main__.py [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
-                   [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
-                   [--invert-y-axis] [--title TITLE] [--caption CAPTION]
-                   [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
-                   [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
-                   in_file [in_file ...]
+usage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
+                     [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
+                     [--invert-y-axis] [--title TITLE] [--caption CAPTION]
+                     [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
+                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
+                     [-P PLOT_OPTS] [-S] [-V]
+                     in_file [in_file ...]
 
 plot the given XCSV files and locate the data on a map
 
 positional arguments:
   in_file               input XCSV file(s)
 
 optional arguments:
@@ -130,14 +133,19 @@
                         projection to use for displaying the site coordinates
                         on the map (one of the CRS classes provided by
                         Cartopy)
   -b BG_IMG_PATH, --background-image BG_IMG_PATH
                         path to an image to show in the background of the plot
   -o OUT_FILE, --out-file OUT_FILE
                         output plot file
+  -P PLOT_OPTS, --plot-options PLOT_OPTS
+                        options for the plot, specified as a simple JSON
+                        object
+  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot
+  -V, --version         show program's version number and exit
 
 Examples
 
 Given an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:
 
 # id: 1
 # title: The title
```

