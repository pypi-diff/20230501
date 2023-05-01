# Comparing `tmp/spectrochempy-0.6.2.tar.gz` & `tmp/spectrochempy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.2.tar", last modified: Tue Apr 25 16:33:51 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.3.tar", last modified: Mon May  1 07:46:29 2023, max compression
```

## Comparing `spectrochempy-0.6.2.tar` & `spectrochempy-0.6.3.tar`

### file list

```diff
@@ -1,227 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/requirements/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71384 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/kinetic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    43542 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/nnmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/analysis/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9945 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20966 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   120597 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37871 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    54110 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    29909 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.668978 spectrochempy-0.6.2/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.668978 spectrochempy-0.6.2/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-01 07:46:29.536927 spectrochempy-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/environment_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/requirements/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.500925 spectrochempy-0.6.3/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.508925 spectrochempy-0.6.3/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.508925 spectrochempy-0.6.3/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-01 07:46:29.536927 spectrochempy-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71352 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/kinetic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49002 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/nmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/analysis/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9945 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/application/plot_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.516926 spectrochempy-0.6.3/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120664 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37871 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54110 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.520926 spectrochempy-0.6.3/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.524926 spectrochempy-0.6.3/spectrochempy/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/processors/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.524926 spectrochempy-0.6.3/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29909 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/extern/traittypes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.528926 spectrochempy-0.6.3/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.532926 spectrochempy-0.6.3/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-01 07:46:07.000000 spectrochempy-0.6.3/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:46:29.512925 spectrochempy-0.6.3/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 07:46:29.000000 spectrochempy-0.6.3/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.2/.codeclimate.yml` & `spectrochempy-0.6.3/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/.conda/meta.yaml` & `spectrochempy-0.6.3/.conda/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -42,34 +42,32 @@
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
-    - numpydoc
+    - numpydoc>=1.2
     - pint
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
     - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
     - jupyterlab_widgets=3.0.5
     - ipympl
-
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
-
     # Jupyter lab
     - jupyterlab
     - nodejs
 
 
 #EOF
```

### Comparing `spectrochempy-0.6.2/.gitignore` & `spectrochempy-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/.pre-commit-config.yaml` & `spectrochempy-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/.pylintrc` & `spectrochempy-0.6.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/.zenodo.json` & `spectrochempy-0.6.3/.zenodo.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-05-01'", "'version'": "'0.6.3'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-04-25",
+    "publication_date": "2023-05-01",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.2"
+    "version": "0.6.3"
 }
```

### Comparing `spectrochempy-0.6.2/CITATION.cff` & `spectrochempy-0.6.3/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-04-25'
+date-released: '2023-05-01'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.2
+version: 0.6.3
```

### Comparing `spectrochempy-0.6.2/Dockerfile` & `spectrochempy-0.6.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSE` & `spectrochempy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.3/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.3/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.3/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.3/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.3/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/PKG-INFO` & `spectrochempy-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.2/README.md` & `spectrochempy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/environment.yml` & `spectrochempy-0.6.3/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,33 +31,31 @@
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
-    - numpydoc
+    - numpydoc>=1.2
     - pint
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
     - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
     - jupyterlab_widgets=3.0.5
     - ipympl
-
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
-
     # Jupyter lab
     - jupyterlab
     - nodejs
 
 
 #EOF
```

### Comparing `spectrochempy-0.6.2/environment_dev.yml` & `spectrochempy-0.6.3/environment_dev.yml`

 * *Files 21% similar despite different names*

```diff
@@ -31,63 +31,64 @@
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
-    - numpydoc
+    - numpydoc>=1.2
     - pint
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
     - pyyaml
     - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
     - jupyterlab_widgets=3.0.5
     - ipympl
-
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
-
     # Jupyter lab
     - jupyterlab
     - nodejs
 
-# DEV dependencies
+    # TEST dependencies
     # ----------------
-    # From here, the dependencies are essentially for development.
-    # They should not be necessary for the user of  spectrochempy.
+    - coverage
     - pytest
     - pytest-doctestplus
     - pytest-flake8
     - pytest-mock
     - pyfakefs
     - pep8-naming
+    - xarray
+# DEV dependencies
+    # ----------------
+    # From here, the dependencies are essentially for development.
+    # They should not be necessary for the user of  spectrochempy.
     - scikit-image
-    - coverage
     - black
     - pre-commit
     - mamba
-    - docrep
     - jupytext
     - sphinx=5.3
     - sphinx_rtd_theme=1.2
     - autodocsumm
     - sphinx-gallery
     - nbsphinx
     - jupyter_sphinx
     - json5
     - sphinx-copybutton
     - sphinxcontrib-bibtex
     - pandoc=2.19
     - conda-build
     - conda-verify
     - anaconda-client
+    - numpydoc>=1.2
 
 #EOF
```

### Comparing `spectrochempy-0.6.2/requirements/requirements.txt` & `spectrochempy-0.6.3/requirements/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dill
 docrep
 ipython
 jinja2
 matplotlib
 numba
 numpy
-numpydoc
+numpydoc>=1.2
 pint
 pytz
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
```

### Comparing `spectrochempy-0.6.2/requirements/requirements_dev.txt` & `spectrochempy-0.6.3/requirements/requirements_dev.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dill
 docrep
 ipython
 jinja2
 matplotlib
 numba
 numpy
-numpydoc
+numpydoc>=1.2
 pint
 pytz
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
@@ -34,30 +34,31 @@
 jupyterlab_widgets==3.0.5
 ipympl
 setuptools
 setuptools_scm
 gitpython
 jupyterlab
 nodejs
+coverage
 pytest
 pytest-doctestplus
 pytest-flake8
 pytest-mock
 pyfakefs
 pep8-naming
+xarray
 scikit-image
-coverage
 black
 pre-commit
 mamba
-docrep
 jupytext
 sphinx==5.3
 sphinx_rtd_theme==1.2
 autodocsumm
 sphinx-gallery
 nbsphinx
 jupyter_sphinx
 json5
 sphinx-copybutton
 sphinxcontrib-bibtex
 pandoc==2.19
+numpydoc>=1.2
```

### Comparing `spectrochempy-0.6.2/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.3/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.3/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.3/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.3/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.3/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.3/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.3/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.3/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.3/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.3/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.3/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.3/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scripts/checkindex.py` & `spectrochempy-0.6.3/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/scripts/validate_docstrings.py` & `spectrochempy-0.6.3/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/setup.cfg` & `spectrochempy-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/setup.py` & `spectrochempy-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/__init__.py` & `spectrochempy-0.6.3/spectrochempy/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/_base.py` & `spectrochempy-0.6.3/spectrochempy/analysis/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
             if n_components > X_transform.shape[1]:
                 warnings.warn(
                     "The number of components required for reduction "
                     "cannot be greater than the X_transform size : "
                     f"{X_transform.shape[1]}. We then use this latter value."
                 )
         elif X_transform is None:
-            X_transform = self.transform(**kwargs)
+            X_transform = self.transform(**kwargs).data
 
         X = self._inverse_transform(X_transform)
 
         return X
 
     _docstring.get_sections(
         _docstring.dedent(inverse_transform.__doc__),
@@ -961,15 +961,15 @@
 
     # ----------------------------------------------------------------------------------
     # Plot methods
     # ----------------------------------------------------------------------------------
     @_docstring.dedent
     def plotmerit(self, X=None, X_hat=None, **kwargs):
         r"""
-        Plot the input (:math:`X`\ ), reconstructed (:math:`\hat{X}`\ ) and residuals (:math:`E`\ ) datasets.
+        Plot the input (`X`\ ), reconstructed (`X_hat`\ ) and residuals.
 
         :math:`X` and :math:`\hat{X}` can be passed as arguments. If not,
         the `X` attribute is used for :math:`X`\ and :math:`\hat{X}`\ is computed by
         the `inverse_transform` method
 
         Parameters
         ----------
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/api.py` & `spectrochempy-0.6.3/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/efa.py` & `spectrochempy-0.6.3/spectrochempy/analysis/efa.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,48 +95,54 @@
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
             **kwargs,
         )
         if "used_components" in kwargs:
-            deprecated("used_components", replace="n_components", removed="0.6.5")
+            deprecated("used_components", replace="n_components", removed="0.7")
             kwargs["n_components"] = kwargs.pop("used_components")
 
     def _fit(self, X, Y=None):
         # X has already been validated and eventually
         # preprocessed. X is now a nd-array with masked elements removed.
         # and this method should return _outfit
         # Y is not used but necessary to fit the superclass
 
         # max number of components
         M, N = X.shape
         K = min(M, N)
 
+        percent_done_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
         # ------------------------------------------------------------------------------
         # forward analysis
         # ------------------------------------------------------------------------------
         f = np.zeros((M, K))
         for i in range(M):
 
             s = np.linalg.svd(X[: i + 1], compute_uv=False)
             k = s.size
             f[i, :k] = s**2
-            info_(f"Evolving Factor Analysis: {int(i / (2 * M) * 100)}% \r")
-
+            percent_done = int(i / (2 * M) * 100)
+            if percent_done in percent_done_list:
+                info_(f"Evolving Factor Analysis: {percent_done}% \r")
+                del percent_done_list[0]
         # ------------------------------------------------------------------------------
         # backward analysis
         # ------------------------------------------------------------------------------
         b = np.zeros((M, K))
         for i in range(M - 1, -1, -1):
             # if some rows are masked, we must skip them
             s = np.linalg.svd(X[i:M], compute_uv=False)
             k = s.size
             b[i, :k] = s**2
-            info_(f"Evolving Factor Analysis: {int(100 - i / (2 * M) * 100)} % \r")
+            percent_done = int(100 - i / (2 * M) * 100)
+            if percent_done in percent_done_list:
+                info_(f"Evolving Factor Analysis: {percent_done} % \r")
+                del percent_done_list[0]
 
         # store the components number (real or desired)
         self._n_components = K
 
         # return results
         _outfit = f, b
         return _outfit
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.3/spectrochempy/analysis/iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/kinetic_utilities.py` & `spectrochempy-0.6.3/spectrochempy/analysis/kinetic_utilities.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/linearregression.py` & `spectrochempy-0.6.3/spectrochempy/analysis/linearregression.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.3/spectrochempy/analysis/mcrals.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import base64
 import logging
 import warnings
 
 import dill
 import numpy as np
+import scipy
 import traitlets as tr
 from sklearn import decomposition
 
 from spectrochempy.analysis._base import (
     DecompositionAnalysis,
     NotFittedError,
     _wrap_ndarray_output_to_nddataset,
@@ -45,20 +46,20 @@
 
     __doc__ = _docstring.dedent(
         """
     Multivariate Curve Resolution Alternating Least Squares (MCRALS).
 
     :term:`MCR-ALS` ( ``Multivariate Curve Resolution Alternating Least Squares`` )
     resolve's a set (or several sets) of spectra :math:`X` of an evolving mixture
-    (or a set of mixtures) into the spectra :math:`S^T` of "pure" species and their
-    concentration profiles :math:`C` .
+    (or a set of mixtures) into the spectra :math:`S^t` of "pure" species and their
+    concentration profiles :math:`C`\ .
 
     In terms of matrix equation:
 
-    .. math:: X = C.S^T + E
+    .. math:: X = C.S^t + E
 
     where :math:`E` is the matrix of residuals.
 
     Parameters
     ----------
     %(AnalysisConfigurable.parameters)s
 
@@ -76,14 +77,15 @@
     # more prone to errors.
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # They will be written in a file from which the default can be modified)
     # Obviously, the parameters can also be modified at runtime as usual by assignment.
     # ----------------------------------------------------------------------------------
+
     tol = tr.Float(
         0.1,
         help=(
             "Convergence criterion on the change of residuals (percent change of "
             "standard deviation of residuals)."
         ),
     ).tag(config=True)
@@ -92,316 +94,447 @@
         config=True
     )
 
     maxdiv = tr.Integer(
         5, help="Maximum number of successive non-converging iterations."
     ).tag(config=True)
 
+    solverConc = tr.Enum(
+        ["lstsq", "nnls", "pnnls"],
+        default_value="lstsq",
+        help=(
+            r"""Solver used to get `C` from `X` and `St`\ .
+
+- ``'lstsq'``\ : uses ordinary least squares with `~numpy.linalg.lstsq`
+- ``'nnls'``\ : non-negative least squares (`~scipy.optimize.nnls`\ ) are applied
+  sequentially on all profiles
+- ``'pnnls'``\ : non-negative least squares (`~scipy.optimize.nnls`\ ) are applied on
+  profiles indicated in `nonnegConc` and ordinary least squares on other profiles.
+"""
+        ),
+    ).tag(config=True)
+
     nonnegConc = tr.Union(
         (tr.Enum(["all"]), tr.List()),
         default_value="all",
         help=(
-            "Non-negativity constraint on concentrations. If set to ``'all'`` (default) "
-            "all concentrations profiles are considered non-negative."
-            " If an array of indexes is passed, the corresponding profiles are "
-            "considered non-negative, not the others. "
-            "For instance ``[0, 2]`` indicates that profile \#0 and \#2 are "
-            "non-negative while profile \#1 *can* be negative. If set to ``[]`` , "
-            "all profiles can be negative."
+            r"""Non-negativity constraint on concentrations.
+
+- ``'all'``\ : all concentrations profiles are considered
+  non-negative.
+- `list` of indexes: the corresponding profiles are considered non-negative,
+  not the others. For instance ``[0, 2]`` indicates that profile \#0 and \#2
+  are non-negative while profile \#1 *can* be negative.
+- ``[]``\ : all profiles can be negative."""
         ),
     ).tag(config=True)
 
     unimodConc = tr.Union(
         (tr.Enum(["all"]), tr.List()),
         default_value="all",
         help=(
-            "Unimodality constraint on concentrations. If set to ``'all'`` "
-            "(default) all concentrations profiles are considered unimodal. "
-            "If an array of indexes is passed, the corresponding profiles are "
-            "considered unimodal, not the others."
-            "For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are "
-            "unimodal while profile ``#1`` *can* be multimodal. If set to ``[]``\ , "
-            "all profiles can be multimodal."
+            r"""Unimodality constraint on concentrations.
+
+- ``'all'``\ : all concentrations profiles are considered unimodal.
+- `list` of indexes: the corresponding profiles are considered unimodal, not the others.
+  For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are unimodal while
+  profile ``#1`` *can* be multimodal.
+- ``[]``\ : all profiles can be multimodal."""
         ),
     ).tag(config=True)
 
     unimodConcMod = tr.Enum(
         ["strict", "smooth"],
         default_value="strict",
-        help="""When set to ``'strict'``\ , values deviating from :term:`unimodality` are
-reset to the value of the previous point. When set to ``'smooth'``\ , both values
-(deviating point and previous point) are modified to avoid steps in the concentration
-profile.""",
+        help=(
+            r"""Method to apply unimodality.
+
+- ``'strict'``\ : values deviating from :term:`unimodality` are reset to the value of the
+  previous point.
+- ``'smooth'``\ : both values (deviating point and previous point) are modified to avoid
+  steps in the concentration profile."""
+        ),
     ).tag(config=True)
 
     unimodConcTol = tr.Float(
         default_value=1.1,
-        help="""Tolerance parameter for :term:`unimodality`\ . Correction is applied only
-if:
+        help=(
+            r"""Tolerance parameter for :term:`unimodality`\ .
+
+Correction is applied only if:
 
-* ``C[i,j] > C[i-1,j] * unimodTol`` on the decreasing branch of profile ``#j``\ ,
-* ``C[i,j] < C[i-1,j] * unimodTol`` on the increasing branch of profile ``#j``\ .""",
+- ``C[i,j] > C[i-1,j] * unimodTol`` on the decreasing branch of profile ``#j``\ ,
+- ``C[i,j] < C[i-1,j] * unimodTol`` on the increasing branch of profile ``#j``\ ."""
+        ),
     ).tag(config=True)
 
     monoDecConc = tr.List(
         default_value=[],
-        help="""Monotonic decrease constraint on concentrations.  If set to ``[]``
-(default) no constraint is applied. If an array of indexes is passed,
-the corresponding profiles are considered do decrease monotonically, not the
-others. For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are decreasing
-while profile ``#1`` *can* increase.""",
+        help=(
+            r"""Monotonic decrease constraint on concentrations.
+
+- ``[]``\ : no constraint is applied.
+- `list` of indexes: the corresponding profiles are considered to decrease
+  monotonically, not the others. For instance ``[0, 2]`` indicates that profile ``#0``
+  and ``#2`` are decreasing while profile ``#1`` *can* increase."""
+        ),
     ).tag(config=True)
 
     monoDecTol = tr.Float(
         default_value=1.1,
-        help="""Tolerance parameter for monotonic decrease. Correction is applied only
-if: ``C[i,j] > C[i-1,j] * unimodTol``  along profile ``#j``\ .""",
+        help=r"""Tolerance parameter for monotonic decrease.
+
+Correction is applied only if: ``C[i,j] > C[i-1,j] * unimodTol`` .""",
     ).tag(config=True)
 
     monoIncConc = tr.List(
         default_value=[],
-        help="""Monotonic increase constraint on concentrations.  If set to ``[]``
-(default) no constraint is applied. If an array of indexes is passed,
-the corresponding profiles are considered to increase monotonically, not the
-others. For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are increasing
-while profile ``#1`` *can* decrease.""",
+        help=(
+            r"""Monotonic increase constraint on concentrations.
+
+- ``[]``\ : no constraint is applied.
+- `list` of indexes: the corresponding profiles are considered to increase
+  monotonically, not the others. For instance ``[0, 2]`` indicates that profile
+  ``#0`` and ``#2`` are increasing while profile ``#1`` *can* decrease."""
+        ),
     ).tag(config=True)
 
     monoIncTol = tr.Float(
         default_value=1.1,
-        help="""Tolerance parameter for monotonic decrease. Correction is applied only
-if: ``C[i,j] < C[i-1,j] * unimodTol`` along profile ``#j``\ .""",
+        help="""Tolerance parameter for monotonic decrease.
+
+Correction is applied only if ``C[i,j] < C[i-1,j] * unimodTol`` along profile ``#j``\ .""",
+    ).tag(config=True)
+
+    unimodConc = tr.Union(
+        (tr.Enum(["all"]), tr.List()),
+        default_value="all",
+        help=(
+            r"""Unimodality constraint on concentrations.
+
+- ``'all'``\ : all concentrations profiles are considered unimodal.
+- `list` of indexes: the corresponding profiles are considered unimodal, not the others.
+  For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are unimodal while
+  profile ``#1`` *can* be multimodal.
+- ``[]``\ : all profiles can be multimodal."""
+        ),
     ).tag(config=True)
 
-    closureConc = tr.List(
+    closureConc = tr.Union(
+        (tr.Enum(["all"]), tr.List()),
         default_value=[],
-        help="""Defines the concentration profiles subjected to closure constraint.
-If set to ``[]``\ , no constraint is applied. If an array of indexes is
-passed, the corresponding profile will be constrained so that their
-weighted sum equals the `closureTarget`\ .""",
+        help=(
+            r"""Defines the concentration profiles subjected to closure constraint.
+
+- ``[]``\ : no constraint is applied.
+- ``'all'``\ : all profile are constrained so that their weighted sum equals the
+  `closureTarget`
+- `list` of indexes: the corresponding profiles are constrained so that their weighted sum
+  equals `closureTarget`\ ."""
+        ),
     ).tag(config=True)
 
     closureTarget = tr.Union(
         (tr.Enum(["default"]), Array()),
         default_value="default",
-        help="""The value of the sum of concentrations profiles subjected to closure.
-If set to ``'default'``\ , the total concentration is set to ``1.0`` for all observations.
-If an array is passed: the values of concentration for each observation. Hence,
-``np.ones(X.shape[0])`` would be equivalent to ``'default'``\ .""",
+        help=(
+            r"""The value of the sum of concentrations profiles subjected to closure.
+
+- ``'default'``\ : the total concentration is set to ``1.0`` for all observations.
+- :term:`array-like` of size :term:`n_observations`: the values of concentration for
+  each observation. Hence, ``np.ones(X.shape[0])`` would be equivalent to
+  ``'default'``\ ."""
+        ),
     ).tag(config=True)
 
     closureMethod = tr.Enum(
         ["scaling", "constantSum"],
         default_value="scaling",
-        help="""The method used to enforce :term:`closure` .
+        help=(
+            r"""The method used to enforce :term:`closure` (:cite:t:`omidikia:2018`).
 
-* ``'scaling'`` recompute the concentration profiles using linear algebra:
+- ``'scaling'`` recompute the concentration profiles using least squares:
 
-   .. code-block:: python
+  .. math::
 
-      C[:, closureConc] = np.dot(
-                            C.[:, closureConc],
-                            np.diag(
-                              np.linalg.lstsq(
-                                C[:, closureConc], closureTarget.T
-                                )[0]
-                            )
-                          )
+     C \leftarrow C \cdot \textrm{diag} \left( C_L^{-1} c_t \right)
 
-* ``'constantSum'`` normalize the sum of concentration profiles to `closureTarget`\ .""",
+  where :math:`c_t` is the vector given by `closureTarget` and :math:`C_L^{-1}`
+  is the left inverse of :math:`C`\ .
+- ``'constantSum'`` normalize the sum of concentration profiles to `closureTarget`\ .
+"""
+        ),
     ).tag(config=True)
 
     hardConc = tr.List(
         default_value=[],
-        help="""Defines hard constraints on the concentration profiles. If set to
-``[]``\ , no constraint is applied. If an array of indexes is passed, the
-corresponding profiles will set by `getC`\ .""",
+        help=(
+            r"""Defines hard constraints on the concentration profiles.
+
+- ``[]``\ : no constraint is applied.
+- `list` of indexes: the corresponding profiles will set by `getConc`\ ."""
+        ),
     ).tag(config=True)
 
     getConc = tr.Union(
         (tr.Callable(), tr.Unicode()),
         default_value=None,
         allow_none=True,
-        help="""An external function that will provide ``len(hardConc)`` concentration
+        help=(
+            r"""An external function that provide ``len(hardConc)`` concentration
 profiles.
 
 It should be using one of the following syntax:
 
-* ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC``
-* ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc``
-* ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc, extraOutputGetConc``
-
-where ``Ccurr`` is the current `C` dataset, ``\*argsGetConc`` are the parameters needed
-to completely specify the function. `hardC` is a `~numpy.ndarray` or `NDDataset` of shape
-``(C.y, len(hardConc)``\ , ``newArgsGetConc`` are the updated parameters for the next
-iteration (can be None), and ``extraOutputGetConc`` can be any other relevant output to
-be kept in `extraOutputGetConc` attribute, a list of ``extraOutputGetConc`` at each
-MCR ALS iterations.
+- ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC``
+- ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc``
+- ``getConc(Ccurr, *argsGetConc, **kwargsGetConc) -> hardC, newArgsGetConc,
+  extraOutputGetConc``
+
+with:
+
+- ``Ccurr`` is the current `C` dataset,
+- ``\*argsGetConc`` are the parameters needed to completely specify the function.
+- ``hardC`` is a `~numpy.ndarray` or `NDDataset` of shape
+  (:term:`n_observations` , len(``hardConc``\ ),
+- ``newArgsGetConc`` are the updated parameters for the next iteration (can be `None`),
+- ``extraOutputGetConc`` can be any other relevant output to be kept in
+  ``extraOutputGetConc`` attribute, a list of ``extraOutputGetConc`` at each MCR ALS
+  iteration.
 
 .. note::
-    it can be also a serialized function created using dill and base64 python libraries.
-    Normally not used directly, it is here for internal process.""",
+    ``getConc`` can be also a serialized function created using dill and base64
+    python libraries. Normally not used directly, it is here for internal
+    process."""
+        ),
     ).tag(config=True)
 
     argsGetConc = tr.Tuple(
         default_value=(),
         help="Supplementary positional arguments passed to the external function.",
     ).tag(config=True)
 
     kwargsGetConc = tr.Dict(
         default_value={},
         help="Supplementary keyword arguments passed to the external function.",
     ).tag(config=True)
 
-    hardC_to_C_idx = tr.Union(
+    getC_to_C_idx = tr.Union(
         (tr.Enum(["default"]), tr.List()),
         default_value="default",
-        help="""Indicates the correspondence between the indexes of the columns of
-`hardC` and of the `C` matrix. ``[1, None, 0]`` indicates that the first profile in
-`hardC` (index ``O``\ ) corresponds to the second profile of `C` (index ``1``\ ).""",
+        help=(
+            r"""Correspondence of the profiles returned by `getConc` and `C`.
+
+- ``'default'``: the profiles correspond to those of `C`. This is equivalent to
+  ``range(len(hardConc))``
+- `list` of indexes or of `None`. For instance ``[2, None, 0]`` indicates that the
+  first returned profile corresponds to the 3rd profile of `C`  (index ``2``\ ), the 2nd
+  returned profile does not correspond to any profile in `C`, the 3rd returned profile
+  corresponds to the first `C` profile (index ``0`` )."""
+        ),
+    ).tag(config=True)
+
+    solverSpec = tr.Enum(
+        ["lstsq", "nnls", "pnnls"],
+        default_value="lstsq",
+        help=(
+            r"""Solver used to get `St` from `X` and `C`\ .
+
+- ``'lstsq'``\ : uses ordinary least squares with `~numpy.linalg.lstsq`
+- ``'nnls'``\ : non-negative least squares (`~scipy.optimize.nnls`\ ) are applied
+  sequentially on all profiles
+- ``'pnnls'``\ : non-negative least squares (`~scipy.optimize.nnls`\ ) are applied on
+  profiles indicated in `nonnegConc` and ordinary least squares on other profiles."""
+        ),
     ).tag(config=True)
 
     nonnegSpec = tr.Union(
         (tr.Enum(["all"]), tr.List()),
         default_value="all",
-        help="""Indicates non-negative spectral profile. If set to ``'all'`` (default)
-all spectral profiles are considered non-negative. If an array of indexes is
-passed, the corresponding profiles are considered non-negative, not the others.
-For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are non-negative while
-profile ``#1`` *can* be negative. If set to ``None`` or ``[]``\ , all profiles can be
-negative.""",
+        help=(
+            r"""Non-negativity constraint on spectra.
+
+- ``'all'``\ : all profiles are considered non-negative.
+- `list` of indexes : the corresponding profiles are considered non-negative, not the
+  others. For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are
+  non-negative while profile ``#1`` *can* be negative.
+- ``[]``\ : all profiles can be negative."""
+        ),
     ).tag(config=True)
 
     normSpec = tr.Enum(
         [None, "euclid", "max"],
         default_value=None,
-        help="""Defines whether the spectral profiles should be normalized. If set to
-``None`` no normalization is applied.
-when set to ``"euclid"``\ , spectra are normalized with respect to their total area,
-when set to ``"max"``\ , spectra are normalized with respect to the maximum af their
-value.""",
+        help=(
+            r"""Defines whether the spectral profiles should be normalized.
+
+- `None`\ : no normalization is applied.
+- ``'euclid'``\ : spectra are normalized with respect to their total area,
+- ``'max'``\ : spectra are normalized with respect to their maximum value."""
+        ),
     ).tag(config=True)
 
     unimodSpec = tr.Union(
         (tr.Enum(["all"]), tr.List()),
         default_value=[],
-        help="""Unimodality constraint on Spectra. If the list of spectral profiles is
-void, all profiles can be multimodal. If set to ``'all'``\ , all profiles are unimodal.
-If an array of indexes is passed, the corresponding profiles are considered unimodal,
-not the others. For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are
-unimodal while profile ``#1`` *can* be multimodal.""",
+        help=(
+            r"""Unimodality constraint on Spectra.
+
+- ``[]``\ : all profiles can be multimodal.
+- ``'all'``\ : all profiles are unimodal (equivalent to ``range(n_components)``\ ).
+- array of indexes : the corresponding profiles are considered unimodal, not the others.
+  For instance ``[0, 2]`` indicates that profile ``#0`` and ``#2`` are unimodal while
+  profile ``#1`` *can* be multimodal."""
+        ),
     ).tag(config=True)
 
     unimodSpecMod = tr.Enum(
         ["strict", "smooth"],
         default_value="strict",
-        help=""" When set to ``"strict"``\ , values deviating from unimodality are reset
-to the value of the previous point. When set to ``"smooth"``\ , both values (deviating
-point and previous point) are modified to avoid steps
-in the concentration profile.""",
+        help=(
+            r"""Method used to apply unimodality.
+
+- ``'strict'``\ : values deviating from unimodality are reset to the value of the previous
+  point.
+- ``'smooth'``\ : both values (deviating point and previous point) are modified to avoid
+  steps in the concentration profile."""
+        ),
     ).tag(config=True)
 
     unimodSpecTol = tr.Float(
         default_value=1.1,
-        help="""Tolerance parameter for unimodality. Correction is applied only if the
-deviating point is larger/lower than ``St[j,i] > St[j, i-1] * unimodSpecTol``
-on the decreasing branch of profile ``#j``\ , ``St[j,i] < St[j, i-1] * unimodTol`` on
-the increasing branch of profile  ``#j``\ .""",
+        help=(
+            r"""Tolerance parameter for unimodality.
+
+Correction is applied only if the deviating point ``St[j, i]`` is larger than
+``St[j, i-1] * unimodSpecTol`` on the decreasing branch of profile
+``#j``\ , or lower than ``St[j, i-1] * unimodTol`` on the increasing branch of
+profile  ``#j``\ ."""
+        ),
     ).tag(config=True)
 
     hardSpec = tr.List(
         default_value=[],
-        help="""Defines hard constraints on the spectral profiles. If set to ``[]`` ,
-no constraint is applied. If an array of indexes is passed, the corresponding profiles
-will set by `getSt`\ .""",
+        help=(
+            r"""Defines hard constraints on the spectral profiles.
+
+- ``[]``\ : no constraint is applied.
+- `list` of indexes : the corresponding profiles will set by `getSpec`\ ."""
+        ),
     ).tag(config=True)
 
     getSpec = tr.Union(
         (tr.Callable(), tr.Unicode()),
         default_value=None,
         allow_none=True,
-        help="""An external function that will provide ``len(hardSpec)`` concentration
+        help=(
+            r"""An external function that will provide ``len(hardSpec)`` concentration
 profiles.
 
 It should be using one of the following syntax:
 
-* ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt``
-* ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt, newArgsGetSpec``
-* ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt, newArgsGetSpec, extraOutputGetSpec``
-
-where ``Stcurr`` is the current `St` dataset, ``\*argsGetSpec`` are the parameters
-needed to completely specify the function. `hardSt` is a `~numpy.ndarray` or `NDDataset` of
-shape ``(C.y, len(hardSpec)``\ , ``newArgsGetSpec`` are the updated parameters for the
-next iteration (can be None), and ``extraOutputGetSpec`` can be any other relevant
-output to be kept in `extraOutputGetSpec` attribute, a list of ``extraOutputGetSpec``
-at each iterations.
+- ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt``
+- ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt, newArgsGetSpec``
+- ``getSpec(Stcurr, *argsGetSpec, **kwargsGetSpec) -> hardSt, newArgsGetSpec,
+  extraOutputGetSpec``
+
+with:
+
+- ``Stcurr``\ : the current value of `St` in the :term:`ALS` loop,
+- ``*argsGetSpec`` and ``**kwargsGetSpec``\ : the parameters needed to completely
+  specify the function.
+- ``hardSt``\ : `~numpy.ndarray` or `NDDataset` of shape
+  ``(n_observations, len(hardSpec)``\ ,
+- ``newArgsGetSpec``\ : updated parameters for the next ALS iteration (can be None),
+- ``extraOutputGetSpec``\ : any other relevant output to be kept in
+  `extraOutputGetSpec` attribute, a list of ``extraOutputGetSpec`` at each iterations.
 
 .. note::
-    it can be also a serialized function created using dill and base64 python libraries.
-    Normally not used directly, it is here for internal process.""",
+    ``getSpec`` can be also a serialized function created using dill and base64
+    python libraries. Normally not used directly, it is here for internal process.
+"""
+        ),
     ).tag(config=True)
 
     argsGetSpec = tr.Tuple(
         default_value=(),
         help="Supplementary positional arguments passed to the external function.",
     ).tag(config=True)
 
     kwargsGetSpec = tr.Dict(
         default_value={},
         help="Supplementary keyword arguments passed to the external function.",
     ).tag(config=True)
 
-    hardSt_to_St_idx = tr.Union(
+    getSt_to_St_idx = tr.Union(
         (tr.Enum(["default"]), tr.List()),
         default_value="default",
-        help="""Indicates the correspondence between the indexes of the lines of
-`hardSt` and of the `St` matrix. ``[1, None, 0]`` indicates that the first profile in
-`hardSt` (index ``O`` ) corresponds to the second profile of `St` (index ``1``\ ).""",
+        help=(
+            r"""Correspondence between the indexes of the spectra returned by `getSpec`
+and `St`.
+
+- ``'default'``\ : the indexes correspond to those of `St`. This is equivalent
+  to ``range(len(hardSpec))``\ .
+- `list` of indexes : corresponding indexes in `St`, i.e. ``[2, None, 0]`` indicates that the
+  first returned profile corresponds to the third `St` profile (index ``2``\ ), the 2nd
+  returned profile does not correspond to any profile in `St`, the 3rd returned profile
+  corresponds to the first `St` profile (index ``0`` )."""
+        ),
     ).tag(config=True)
 
     # ----------------------------------------------------------------------------------
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *args,
         log_level=logging.WARNING,
         warm_start=False,
         **kwargs,
     ):
         if len(args) > 0:
             raise ValueError(
-                "Passing arguments such as MCRALS(X , profile) "
+                "Passing arguments such as MCRALS(X, profile) "
                 "is now deprecated. "
-                "Instead, use MCRAL() followed by MCRALS.fit(X , profile). "
-                "See the documentation and exemples"
+                "Instead, use MCRAL() followed by MCRALS.fit(X, profile). "
+                "See the documentation and examples"
             )
 
         # warn about deprecation
         # ----------------------
         # We use pop to remove the deprecated argument before processing the rest
-        # TODO: These arguments should be removed in version 0.6 probably
+        # TODO: These arguments should be removed in version 0.7 probably
 
         # verbose
         if "verbose" in kwargs:
-            deprecated("verbose", replace="log_level='INFO'", removed="0.6.5")
+            deprecated("verbose", replace="log_level='INFO'", removed="0.7")
             verbose = kwargs.pop("verbose")
             if verbose:
                 log_level = "INFO"
 
         # unimodTol deprecation
         if "unimodTol" in kwargs:
-            deprecated("unimodTol", replace="unimodConcTol", removed="0.6.5")
+            deprecated("unimodTol", replace="unimodConcTol", removed="0.7")
             kwargs["unimodConcTol"] = kwargs.pop("unimodTol")
 
         # unimodMod deprecation
         if "unimodMod" in kwargs:
-            deprecated("unimodMod", replace="unimodConcMod", removed="0.6.5")
+            deprecated("unimodMod", replace="unimodConcMod", removed="0.7")
             kwargs["unimodConcMod"] = kwargs.pop("unimodMod")
 
+        # hardC_to_C_idx deprecation
+        if "hardC_to_C_idx" in kwargs:
+            deprecated("hardC_to_C_idx", replace="getC_to_C_idx", removed="0.7")
+            kwargs["getC_to_C_idx"] = kwargs.pop("hardC_to_C_idx")
+
+        # hardSt_to_St_idx deprecation
+        if "hardSt_to_St_idx" in kwargs:
+            deprecated("hardSt_to_St_idx", replace="getSt_to_St_idx", removed="0.7")
+            kwargs["getSt_to_St_idx"] = kwargs.pop("hardSt_to_St_idx")
+
         # call the super class for initialisation
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
             **kwargs,
         )
 
@@ -410,89 +543,87 @@
             self.getConc = dill.loads(base64.b64decode(self.getConc))
         if self.getSpec is not None and isinstance(self.getSpec, str):
             self.getSpec = dill.loads(base64.b64decode(self.getSpec))
 
     # ----------------------------------------------------------------------------------
     # Private methods
     # ----------------------------------------------------------------------------------
+
+    def _solve_C(self, St):
+        if self.solverConc == "lstsq":
+            return _lstsq(St.T, self._X.data.T).T
+        elif self.solverConc == "nnls":
+            return _nnls(St.T, self._X.data.T).T
+        elif self.solverConc == "pnnls":
+            return _pnnls(St.T, self._X.data.T, nonneg=self.nonnegConc).T
+
+    def _solve_St(self, C):
+        if self.solverSpec == "lstsq":
+            return _lstsq(C, self._X.data)
+        elif self.solverSpec == "nnls":
+            return _nnls(C, self._X.data)
+        elif self.solverSpec == "pnnls":
+            return _pnnls(C, self._X.data, nonneg=self.nonnegSpec)
+
     def _guess_profile(self, profile):
-        """
-        Set or guess an initial profile.
+        # Set or guess an initial profile.
 
-        Parameters
-        ----------
-        profile : np.ndarray
-            Initial guess for the concentration or spectra profile.
-        """
         if self._X_is_missing:
             return
 
         # check the dimensions compatibility
-        # however as the dimension of profile should match the initial shape
+        # As the dimension of profile should match the initial shape
         # of X we use self._X_shape not self._X.shape (because for this masked columns
         # or rows have already been removed.
         if (self._X_shape[1] != profile.shape[1]) and (
             self._X_shape[0] != profile.shape[0]
         ):
             raise ValueError(
                 f"None of the dimensions of the given profile "
                 f"[{profile.shape}] correspond to any of those "
                 f"of X [{self._X_shape}]."
             )
 
-        # data array
-        Xdata = self._X.data
-
         # mask info
         if np.any(self._X_mask):
             masked_rows, masked_columns = self._get_masked_rc(self._X_mask)
 
         # make the profile
-        try:  # first try on concentration
-            # The data are validated in _C_validate()
-            # if it fails here due to shape mismatch, it goes to the except
-
-            Cdata = profile.copy()
-            n_components = Cdata.shape[1]
-            info_(f"Concentration profile initialized with {n_components} components")
-            # compute initial spectra (using the Xdata eventually masked
-            Stdata = np.linalg.lstsq(Cdata, Xdata, rcond=None)[0]
-            info_("Spectra profile computed")
+        if profile.shape[0] == self._X_shape[0]:
+            # this should be a concentration profile.
+            C = profile.copy()
+            self._n_components = C.shape[1]
+            info_(
+                f"Concentration profile initialized with {self._n_components} components"
+            )
+
+            # compute initial spectra (using X eventually masked)
+            St = self._solve_St(C)
+            info_("Initial spectra profile computed")
             # if everything went well here, C and St are set, we return
             # after having removed the eventual C mask!
             if np.any(self._X_mask):
-                Cdata = Cdata[~masked_rows]
-            # update the number of components
-            self._n_components = n_components
+                C = C[~masked_rows]
+            return C, St
 
-            return Cdata, Stdata
-
-        except np.linalg.LinAlgError as exc:
-            if "Incompatible dimensions" not in exc.args[0]:
-                raise exc
-            pass
-
-        # Again if something is wrong we let it raise the error
-        # as there is no other possibility (but this should not occur as we did
-        # already the test on the dimension's compatibility.
-        Stdata = profile.copy()
-        n_components = Stdata.shape[0]
-        info_(f"Spectra profile initialized with {n_components} components")
-        # compute initial concentration
-        Ctdata = np.linalg.lstsq(Stdata.T, Xdata.T, rcond=None)[0]
-        Cdata = Ctdata.T
-        info_("Concentration profile computed")
-        # if everything went well here, C and St are set, we return
-        # after having removed the eventual St mask!
-        if np.any(self._X_mask):
-            Stdata = Stdata[:, ~masked_columns]
-        # update the number of components
-        self._n_components = n_components
+        else:  # necessarily: profile.shape[1] == profile.shape[0]
+            St = profile.copy()
+            self._n_components = St.shape[0]
+            info_(f"Spectra profile initialized with {self._n_components} components")
+
+            # compute initial spectra
+            C = self._solve_C(St)
+            info_("Initial concentration profile computed")
+            # if everything went well here, C and St are set, we return
+            # after having removed the eventual St mask!
+            if np.any(self._X_mask):
+                St = St[:, ~masked_columns]
+            # update the number of components
 
-        return Cdata, Stdata
+            return C, St
 
     @_wrap_ndarray_output_to_nddataset(units=None, title=None, typex="components")
     def _C_2_NDDataset(self, C):
         # getconc takes the C NDDataset as first argument (to take advantage
         # of useful metadata). But the current C in fit method is a ndarray (without
         # the masked rows and colums, nor the coord information: this
         # function will create the corresponding dataset
@@ -547,14 +678,28 @@
         ):
             raise ValueError(
                 f"The profile has only {self._n_components} species, please check the "
                 f"`unimodConc` configuration (value:{unimodConc})"
             )
         return unimodConc
 
+    @tr.validate("closureConc")
+    def _validate_closureConc(self, proposal):
+        if self._X_is_missing:
+            return proposal.value
+        closureConc = proposal.value
+        if closureConc == "all":
+            closureConc = np.arange(self._n_components)
+        elif len(closureConc) > self._n_components:
+            raise ValueError(
+                f"The model contains only {self._n_components} components, please check "
+                f"the 'closureConc' configuration (value:{closureConc})"
+            )
+        return closureConc
+
     @tr.validate("closureTarget")
     def _validate_closureTarget(self, proposal):
         if self._X_is_missing:
             return proposal.value
         closureTarget = proposal.value
         ny = self.X.shape[0]
         if closureTarget == "default":
@@ -562,32 +707,32 @@
         elif len(closureTarget) != ny:
             raise ValueError(
                 f"The data contain only {ny} observations, please check "
                 f"the 'closureTarget' configuration (value:{closureTarget})"
             )
         return closureTarget
 
-    @tr.validate("hardC_to_C_idx")
-    def _validate_hardC_to_C_idx(self, proposal):
+    @tr.validate("getC_to_C_idx")
+    def _validate_getC_to_C_idx(self, proposal):
         if self._X_is_missing:
             return proposal.value
-        hardC_to_C_idx = proposal.value
+        getC_to_C_idx = proposal.value
         if not self._n_components:  # not initialized or 0
-            return hardC_to_C_idx
-        if hardC_to_C_idx == "default":
-            hardC_to_C_idx = np.arange(self._n_components).tolist()
+            return getC_to_C_idx
+        if getC_to_C_idx == "default":
+            getC_to_C_idx = np.arange(self._n_components).tolist()
         elif (
-            len(hardC_to_C_idx) > self._n_components
-            or max(hardC_to_C_idx) + 1 > self._n_components
+            len(getC_to_C_idx) > self._n_components
+            or max(getC_to_C_idx) + 1 > self._n_components
         ):
             raise ValueError(
                 f"The profile has only {self._n_components} species, please check "
-                f"the `hardC_to_C_idx`  configuration (value:{hardC_to_C_idx})"
+                f"the `getC_to_C_idx`  configuration (value:{getC_to_C_idx})"
             )
-        return hardC_to_C_idx
+        return getC_to_C_idx
 
     @tr.validate("nonnegSpec")
     def _validate_nonnegSpec(self, proposal):
         if self._X_is_missing:
             return proposal.value
         nonnegSpec = proposal.value
         if not self._n_components:  # not initialized or 0
@@ -619,54 +764,56 @@
         ):
             raise ValueError(
                 f"The profile has only {self._n_components} species, please check the "
                 f"`unimodSpec`configuration"
             )
         return unimodSpec
 
-    @tr.validate("hardSt_to_St_idx")
-    def _validate_hardSt_to_St_idx(self, proposal):
+    @tr.validate("getSt_to_St_idx")
+    def _validate_getSt_to_St_idx(self, proposal):
         if self._X_is_missing:
             return proposal.value
-        hardSt_to_St_idx = proposal.value
+        getSt_to_St_idx = proposal.value
         if not self._n_components:  # not initialized or 0
-            return hardSt_to_St_idx
-        if hardSt_to_St_idx == "default":
-            hardSt_to_St_idx = np.arange(self._n_components).tolist()
+            return getSt_to_St_idx
+        if getSt_to_St_idx == "default":
+            getSt_to_St_idx = np.arange(self._n_components).tolist()
         elif (
-            len(hardSt_to_St_idx) > self._n_components
-            or max(hardSt_to_St_idx) + 1 > self._n_components
+            len(getSt_to_St_idx) > self._n_components
+            or max(getSt_to_St_idx) + 1 > self._n_components
         ):
             raise ValueError(
                 f"The profile has only {self._n_components} species, please check "
-                f"the `hardSt_to_St_idx`  configuration (value:{hardSt_to_St_idx})"
+                f"the `getSt_to_St_idx`  configuration (value:{getSt_to_St_idx})"
             )
-        return hardSt_to_St_idx
+        return getSt_to_St_idx
 
-    @tr.observe("_Y_preprocessed")
-    def _Y_preprocessed_change(self, change):
+    @tr.observe("_n_components")
+    def _n_components_change(self, change):
+        # tiggered in _guess_profile
         if self._n_components > 0:
             # perform a validation of default configuration parameters
             # Indeed, if not forced here these parameters are validated only when they
             # are set explicitely.
             # Here is an ugly trick to force this validation. # TODO: better way?
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 self.closureTarget = self.closureTarget
-                self.hardC_to_C_idx = self.hardC_to_C_idx
-                self.hardSt_to_St_idx = self.hardSt_to_St_idx
+                self.getC_to_C_idx = self.getC_to_C_idx
+                self.getSt_to_St_idx = self.getSt_to_St_idx
                 self.nonnegConc = self.nonnegConc
                 self.nonnegSpec = self.nonnegSpec
                 self.unimodConc = self.unimodConc
                 self.unimodSpec = self.unimodSpec
+                self.closureConc = self.closureConc
 
     @tr.default("_components")
     def _components_default(self):
         if self._fitted:
-            # note: _outfit = (C, St, C_hard, St_soft, extraOutputGetConc, extraOutputGetSpec)
+            # note: _outfit = (C, St, C_constrained, St_unconstrained, extraOutputGetConc, extraOutputGetSpec)
             return self._outfit[1]
         else:
             raise NotFittedError("The model was not yet fitted. Execute `fit` first!")
 
     # ----------------------------------------------------------------------------------
     # Private methods (overloading abstract classes)
     # ----------------------------------------------------------------------------------
@@ -675,36 +822,36 @@
     @tr.observe("_Y")
     def _preprocess_as_Y_changed(self, change):
         # should be a tuple of profiles or only concentrations/spectra profiles
         profiles = change.new
         if isinstance(profiles, (list, tuple)):
             # we assume that the starting C and St are already computed
             # (for ex. from a previous run of fit)
-            Cdata, Stdata = [item.data for item in profiles]
-            self._n_components = Cdata.shape[1]
+            C, St = [item.data for item in profiles]
+            self._n_components = C.shape[1]
             # eventually remove mask
             if np.any(self._X_mask):
                 masked_rows, masked_columns = self._get_masked_rc(self._X_mask)
-                Stdata = Stdata[:, ~masked_columns]
-                Cdata = Cdata[~masked_rows]
+                St = St[:, ~masked_columns]
+                C = C[~masked_rows]
         else:
-            # not passed explicitly, try to guess
-            Cdata, Stdata = self._guess_profile(profiles.data)
+            # not passed explicitly, try to guess.
+            C, St = self._guess_profile(profiles.data)
 
         # we do a last validation
         shape = self._X.shape
-        if shape[0] != Cdata.shape[0]:
+        if shape[0] != C.shape[0]:
             # An error will be raised before if X is None.
             raise ValueError("The dimensions of C do not match those of X.")
-        if shape[1] != Stdata.shape[1]:
+        if shape[1] != St.shape[1]:
             # An error will be raised before if X is None.
             raise ValueError("The dimensions of St do not match those of X.")
         # return the list of C and St data
         # (with mask removed to fit the size of the _X data)
-        self._Y_preprocessed = (Cdata, Stdata)
+        self._Y_preprocessed = (C, St)
 
     def _fit(self, X, Y):
         # this method is called by the abstract class fit.
         # Input X is a np.ndarray
         # Y is a tuple of guessed profiles (each of them being np.ndarray)
         # So every computation below implies only numpy arrays, not NDDataset
         # as in previous versions
@@ -723,59 +870,58 @@
 
         # get sklearn PCA with same number of components for further comparison
         pca = decomposition.PCA(n_components=n_components)
         Xtransf = pca.fit_transform(X)
         Xpca = pca.inverse_transform(Xtransf)
 
         while change >= self.tol and niter < self.max_iter and ndiv < self.maxdiv:
-            C = np.linalg.lstsq(St.T, X.T, rcond=None)[0].T
+
             niter += 1
 
+            # Compute C
+            # ------------------------------------------
+            C = self._solve_C(St)
+
             # Force non-negative concentration
-            # --------------------------------
+            # ------------------------------------------
             if np.any(self.nonnegConc):
-                for s in self.nonnegConc:
-                    C[:, s] = C[:, s].clip(min=0)
+                C[:, self.nonnegConc] = C[:, self.nonnegConc].clip(min=0)
 
             # Force unimodal concentration
-            # ----------------------------
+            # ------------------------------------------
             if np.any(self.unimodConc):
                 C = _unimodal_2D(
                     C,
                     idxes=self.unimodConc,
                     axis=0,
                     tol=self.unimodConcTol,
                     mod=self.unimodConcMod,
                 )
 
             # Force monotonic increase
-            # ------------------------
+            # ------------------------------------------
             if np.any(self.monoIncConc):
                 for s in self.monoIncConc:
                     for curid in np.arange(ny - 1):
                         if C[curid + 1, s] < C[curid, s] / self.monoIncTol:
                             C[curid + 1, s] = C[curid, s]
 
             # Force monotonic decrease
-            # ----------------------------------------------
+            # ------------------------------------------
             if np.any(self.monoDecConc):
                 for s in self.monoDecConc:
                     for curid in np.arange(ny - 1):
                         if C[curid + 1, s] > C[curid, s] * self.monoDecTol:
                             C[curid + 1, s] = C[curid, s]
 
             # Closure
             # ------------------------------------------
             if self.closureConc:
                 if self.closureMethod == "scaling":
-                    Q = np.linalg.lstsq(
-                        C[:, self.closureConc],
-                        self.closureTarget.T,
-                        rcond=None,
-                    )[0]
+                    Q = _lstsq(C[:, self.closureConc], self.closureTarget.T)
                     C[:, self.closureConc] = np.dot(C[:, self.closureConc], np.diag(Q))
                 elif self.closureMethod == "constantSum":
                     totalConc = np.sum(C[:, self.closureConc], axis=1)
                     C[:, self.closureConc] = (
                         C[:, self.closureConc]
                         * self.closureTarget[:, None]
                         / totalConc[:, None]
@@ -801,43 +947,41 @@
                     if len(output) == 3:
                         extraOutputGetConc.append(output[2])
                     else:
                         fixedC = output
                 else:
                     fixedC = output
 
-                C[:, self.hardConc] = fixedC[:, self.hardC_to_C_idx]
+                C[:, self.hardConc] = fixedC[:, self.getC_to_C_idx]
 
-            # stores C in C_hard
-            C_hard = C.copy()
-
-            # compute St
-            St = np.linalg.lstsq(C, X, rcond=None)[0]
+            # stores C in C_constrained
+            # ------------------------------------------
+            C_constrained = C.copy()
 
-            # stores St in St_soft
-            St_soft = St.copy()
+            # Compute St taking into account non-negativity
+            # --------------------------------------------
+            St = self._solve_St(C)
 
-            # Force non-negative spectra
-            # --------------------------
-            if np.any(self.nonnegSpec):
-                St[self.nonnegSpec, :] = St[self.nonnegSpec, :].clip(min=0)
+            # stores St in St_unconstrained
+            # ------------------------------------------
+            St_unconstrained = St.copy()
 
             # Force unimodal spectra
-            # ----------------------------
+            # ------------------------------------------
             if np.any(self.unimodSpec):
                 St = _unimodal_2D(
                     St,
                     idxes=self.unimodSpec,
                     axis=1,
                     tol=self.unimodSpecTol,
                     mod=self.unimodSpecMod,
                 )
 
             # External spectral profile
-            # -----------------------------
+            # ------------------------------------------
             extraOutputGetSpec = []
             if np.any(self.hardSpec):
                 _St = self._St_2_NDDataset(St)
                 if self.kwargsGetSpec != {} and self.argsGetSpec != ():
                     output = self.getSpec(_St, *self.argsGetSpec, **self.kwargsGetSpec)
                 elif self.kwargsGetSpec == {} and self.argsGetSpec != ():
                     output = self.getSpec(_St, *self.argsGetSpecc)
@@ -852,44 +996,47 @@
                     if len(output) == 3:
                         extraOutputGetSpec.append(output[2])
                     else:
                         fixedSt = output.data
                 else:
                     fixedSt = output.data
 
-                print(self.hardSt_to_St_idx)
-                St[self.hardSpec, :] = fixedSt[self.hardSt_to_St_idx, :]
+                St[self.hardSpec, :] = fixedSt[self.getSt_to_St_idx, :]
 
-            # recompute C for consistency(soft modeling)
-            C = np.linalg.lstsq(St.T, X.T, rcond=-1)[0].T
+            # recompute C for consistency
+            # ------------------------------------------
+            C = self._solve_C(St)
 
-            # rescale spectra & concentrations
+            # rescale spectra and concentrations
+            # ------------------------------------------
             if self.normSpec == "max":
                 alpha = np.max(St, axis=1).reshape(self._n_components, 1)
                 St = St / alpha
                 C = C * alpha.T
             elif self.normSpec == "euclid":
                 alpha = np.linalg.norm(St, axis=1).reshape(self._n_components, 1)
                 St = St / alpha
                 C = C * alpha.T
 
             # compute residuals
-            # -----------------
-            Xhat = np.dot(C, St)
+            # ------------------------------------------
+            Xhat = C @ St
             stdev2 = np.std(Xhat - X)
             change = 100 * (stdev2 - stdev) / stdev
             stdev = stdev2
 
-            stdev_PCA = np.std(Xhat - Xpca)  #
-
+            stdev_PCA = np.std(Xhat - Xpca)
             info_(
                 f"{niter:3d}{' '*6}{stdev_PCA:10f}{' '*6}"
                 f"{stdev2:10f}{' '*6}{change:10f}"
             )
 
+            # check convergence
+            # ------------------------------------------
+
             if change > 0:
                 ndiv += 1
             else:
                 ndiv = 0
                 change = -change
 
             if change < self.tol:
@@ -907,15 +1054,22 @@
                     f"Convergence criterion ('tol') not reached after "
                     f"{ self.max_iter:d} iterations."
                 )
                 info_("Stop ALS optimization.")
 
         # return _fit results
         self._components = St
-        _outfit = (C, St, C_hard, St_soft, extraOutputGetConc, extraOutputGetSpec)
+        _outfit = (
+            C,
+            St,
+            C_constrained,
+            St_unconstrained,
+            extraOutputGetConc,
+            extraOutputGetSpec,
+        )
         return _outfit
 
     def _transform(self, X=None):
         # X is ignored for MCRALS
         return self._outfit[0]
 
     def _inverse_transform(self, X_transform=None):
@@ -1009,29 +1163,48 @@
         """
         St = self.components
         St.name = "Pure spectra profile, mcs-als of " + self.X.name
         return St
 
     @property
     @_wrap_ndarray_output_to_nddataset(units=None, title=None, typex="components")
-    def C_hard(self):
+    def C_constrained(self):
         """
-        The hard concentration profiles.
+        The constrained concentration profiles, i.e. after applying the hard and soft constraints.
         """
         return self._outfit[2]
 
     @property
-    @_wrap_ndarray_output_to_nddataset(units=None, title=None, typey="components")
-    def St_soft(self):
+    @deprecated(replace="C_constrained")
+    def C_hard(self):
+        """
+        Deprecated. Equivalent to `C_constrained`.
         """
+        return self.C_constrained
+
+    @property
+    @_wrap_ndarray_output_to_nddataset(units=None, title=None, typey="components")
+    def St_unconstrained(self):
+        r"""
         The soft spectra profiles.
+
+        Spectra obtained after solving :math:`C_{\textrm{constrained}} \cdot St = X`
+        for :math:`St`\ .
         """
         return self._outfit[3]
 
     @property
+    @deprecated(replace="St_unconstrained")
+    def S_soft(self):
+        """
+        Deprecated. Equivalent to `C_constrained`.
+        """
+        return self.St_unconstrained
+
+    @property
     def extraOutputGetConc(self):
         """
         The extra outputs of the external function used to get concentrations.
         """
         return self._outfit[4]
 
     @property
@@ -1041,16 +1214,58 @@
         """
         return self._outfit[5]
 
 
 # --------------------------------------------------------------------------------------
 # Utilities
 # --------------------------------------------------------------------------------------
+
+# LS solvers for W in the linear matrix equation X @ W = Y
+def _lstsq(X, Y, rcond=None):
+    # Least-squares solution to a linear matrix equation X @ W = Y
+    # Return W
+    W = np.linalg.lstsq(X, Y, rcond)[0]
+    return W
+
+
+def _nnls(X, Y, withres=False):
+    # Non negative least-squares solution to a linear matrix equation X @ W = Y
+    # Return W >= 0
+    # TODO: look at may be faster algorithm: see: https://gist.github.com/vene/7224672
+    nsamp, nfeat = X.shape
+    nsamp, ntarg = Y.shape
+    W = np.empty((nfeat, ntarg))
+    residuals = 0
+    for i in range(ntarg):
+        Y_ = Y[:, i]
+        W[:, i], res = scipy.optimize.nnls(X, Y_)
+        residuals += res**2
+    return (W, np.sqrt(residuals)) if withres else W
+
+
+def _pnnls(X, Y, nonneg=[], withres=False):
+    # Least-squares  solution to a linear matrix equation X @ W = Y
+    # with partial nonnegativity (indicated by the nonneg list of targets)
+    # Return W with eventually some column non negative.
+    nsamp, nfeat = X.shape
+    nsamp, ntarg = Y.shape
+    W = np.empty((nfeat, ntarg))
+    residuals = 0
+    for i in range(ntarg):
+        Y_ = Y[:, i]
+        if i in nonneg:
+            W[:, i], res = scipy.optimize.nnls(X, Y_)
+        else:
+            W[:, i], res = np.linalg.lstsq(X, Y_)[:2]
+        residuals += res**2
+    return (W, np.sqrt(residuals)) if withres else W
+
+
 def _unimodal_2D(a, axis, idxes, tol, mod):
-    # """Force unimodality on given lines or columnns od a 2D ndarray
+    # Force unimodality on given lines or columnns od a 2D ndarray
     #
     # a: ndarray
     #
     # axis: int
     #     axis along which the correction is applied
     #
     # idxes: list of int
@@ -1061,29 +1276,28 @@
     #     value of the previous point. When set to `"smooth"`\ , both values (deviating
     #     point and previous point) are modified to avoid "steps" in the profile.
     #
     # tol: float
     #     Tolerance parameter for unimodality. Correction is applied only if:
     #     `a[i] > a[i-1] * unimodTol`  on a decreasing branch of profile,
     #     `a[i] < a[i-1] * unimodTol`  on an increasing branch of profile.
-    # """
 
     if axis == 0:
         a_ = a
     elif axis == 1:
         a_ = a.T
 
     for col, idx in zip(a_[:, idxes].T, idxes):
         a_[:, idx] = _unimodal_1D(col, tol, mod)
 
     return a
 
 
 def _unimodal_1D(a: np.ndarray, tol: str, mod: str) -> np.ndarray:
-    # """force unimodal concentration
+    # force unimodal concentration
     #
     # makes a vector unimodal
     #
     # Parameters
     # ----------
     # a : 1D ndarray
     #
@@ -1093,15 +1307,14 @@
     #     previous point) are modified to avoid "steps"
     #     in the profile.
     #
     # tol: float
     #     Tolerance parameter for unimodality. Correction is applied only if:
     #     `a[i] > a[i-1] * unimodTol`  on a decreasing branch of profile,
     #     `a[i] < a[i-1] * unimodTol`  on an increasing branch of profile.
-    # """
 
     maxid = np.argmax(a)
     curmax = max(a)
     curid = maxid
 
     while curid > 0:
         # run backward
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/nnmf.py` & `spectrochempy-0.6.3/spectrochempy/analysis/nmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self,
         *,
         log_level="WARNING",
         warm_start=False,
         **kwargs,
     ):
         if "used_components" in kwargs:
-            deprecated("used_components", replace="n_components", removed="0.6.5")
+            deprecated("used_components", replace="n_components", removed="0.7")
             kwargs["n_components"] = kwargs.pop("used_components")
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/optimize/__init__.py` & `spectrochempy-0.6.3/spectrochempy/analysis/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/optimize/_models.py` & `spectrochempy-0.6.3/spectrochempy/analysis/optimize/_models.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/optimize/_parameters.py` & `spectrochempy-0.6.3/spectrochempy/analysis/optimize/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/optimize/optimize.py` & `spectrochempy-0.6.3/spectrochempy/analysis/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.3/spectrochempy/analysis/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         self,
         *,
         log_level="WARNING",
         warm_start=False,
         **kwargs,
     ):
         if "used_components" in kwargs:
-            deprecated("used_components", replace="n_components", removed="0.6.5")
+            deprecated("used_components", replace="n_components", removed="0.7")
             kwargs["n_components"] = kwargs.pop("used_components")
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.3/spectrochempy/analysis/peakfinding.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/pls.py` & `spectrochempy-0.6.3/spectrochempy/analysis/pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.3/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.3/spectrochempy/analysis/simplisma.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,23 @@
     interactive = tr.Bool(
         default_value=False,
         help=(
             "If True, the determination of purest variables is carried out "
             "interactively."
         ),
     ).tag(config=True)
-    max_components = tr.Integer(
+
+    n_components = tr.Integer(
         default_value=2,
         help=(
             "The maximum number of pure compounds. Used only for non interactive"
             "analysis."
         ),
     ).tag(config=True)
+
     tol = tr.Float(
         default_value=0.1,
         help="The convergence criterion on the percent of unexplained variance.",
     ).tag(config=True)
     noise = tr.Float(
         default_value=3,
         help=(
@@ -102,36 +104,39 @@
                 "Instead, use SIMPLISMA() followed by SIMPLISMA.fit(X). "
                 "See the documentation and exemples"
             )
 
         # warn about deprecations
         # -----------------------
         if "verbose" in kwargs:
-            deprecated("verbose", replace="log_level='INFO'", removed="0.6.5")
+            deprecated("verbose", replace="log_level='INFO'", removed="0.7")
             verbose = kwargs.pop("verbose")
             if verbose:
                 log_level = "INFO"
 
-        # unimodMod deprecation
         if "n_pc" in kwargs:
-            deprecated("n_pc", replace="max_components", removed="0.6.5")
-            kwargs["max_components"] = kwargs.pop("n_pc")
+            deprecated("n_pc", replace="n_components", removed="0.7")
+            kwargs["n_components"] = kwargs.pop("n_pc")
+
+        if "max_components" in kwargs:
+            deprecated("max_components", replace="n_components", removed="0.7")
+            kwargs["n_components"] = kwargs.pop("max_components")
 
         # call the super class for initialisation
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
             **kwargs,
         )
 
     # ----------------------------------------------------------------------------------
     # Private validation methods and default getter
     # ----------------------------------------------------------------------------------
-    @tr.validate("max_components")
-    def _max_components_validate(self, proposal):
+    @tr.validate("n_components")
+    def _n_components_validate(self, proposal):
         n = proposal.value
         if n < 2:
             raise ValueError(
                 "Oh you did not just... 'MA' in simplisMA stands for Mixture Analysis. "
                 "The number of pure compounds should be an integer larger than 2"
             )
         return n  # <-- do not forget this, or the returned value
@@ -193,15 +198,15 @@
         # remember most of the treatments is done in the abstract method
         # X is _X_preprocessed, so just a np.ndarray
         # Y is ignored
 
         interactive = self.interactive
         tol = self.tol
         noise = self.noise
-        n_components = self.max_components
+        n_components = self.n_components
         M, N = X.shape
         xdata = np.arange(N)
 
         if interactive:
             n_components = 100
 
         # ------------------------------------------------------------------------------
```

### Comparing `spectrochempy-0.6.2/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.3/spectrochempy/analysis/svd.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/api.py` & `spectrochempy-0.6.3/spectrochempy/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/application/application.py` & `spectrochempy-0.6.3/spectrochempy/application/application.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.3/spectrochempy/application/general_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/application/metaconfigurable.py` & `spectrochempy-0.6.3/spectrochempy/application/metaconfigurable.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.3/spectrochempy/application/plot_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/__init__.py` & `spectrochempy-0.6.3/spectrochempy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.3/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,20 +244,20 @@
         if filename:
             self.filename = filename
             return self.dump(filename, **kwargs)
 
     @classmethod
     def load(cls, filename, **kwargs):
         """
-        Open data from a '*.scp' (NDDataset) or '.pscp' (Project) file.
+        Open data from a '\*.scp' (NDDataset) or '\*.pscp' (Project) file.
 
         Parameters
         ----------
         filename :  `str` , `pathlib` or `file` objects
-            The name of the file to read (or a file objects.
+            The name of the file to read (or a file objects).
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Other Parameters
         ----------------
         content : str, optional
              The optional content of the file(s) to be loaded as a binary string.
```

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files 1% similar despite different names*

```diff
@@ -2298,31 +2298,32 @@
 
     @_from_numpy_method
     def random(cls, size=None, dtype=None, **kwargs):
         """
         Return random floats in the half-open interval [0.0, 1.0).
 
         Results are from the “continuous uniform” distribution over the stated interval.
-        To sample :math:`\\mathrm{Uniform}[a, b), b > a` multiply the output of random
-        by (b-a) and add a:
 
-            (b - a) * random() + a
+        .. note::
+            To sample :math:`\\mathrm{Uniform}[a, b)` with :math:`b > a`, multiply the
+            output of random by (b-a) and
+            add a, i.e.: :math:`(b - a) * \\mathrm{random}() + a`\ .
 
         Parameters
         ----------
         size : int or tuple of ints, optional
             Output shape. If the given shape is, e.g., (m, n, k), then m * n * k samples
-             are drawn.
+            are drawn.
             Default is None, in which case a single value is returned.
         dtype : dtype, optional
             Desired dtype of the result, only float64 and float32 are supported.
             The default value is np.float64.
         **kwargs
             Keywords argument used when creating the returned object, such as units,
-            name, title, ...
+            name, title, etc...
 
         Returns
         -------
         random
             Array of random floats of shape size (unless size=None, in which case a
             single float is returned).
         """
@@ -2344,15 +2345,15 @@
 
         Parameters
         ----------
         dataset : array_like
             Calculate the standard deviation of these values.
         dim : None or int or dimension name , optional
             Dimension or dimensions along which to operate.  By default, flattened input
-             is used.
+            is used.
         dtype : dtype, optional
             Type to use in computing the standard deviation. For arrays of
             integer type the default is float64, for arrays of float types it is
             the same as the array type.
         ddof : int, optional
             Means Delta Degrees of Freedom.  The divisor used in calculations
             is `N - ddof` , where `N` represents the number of elements.
```

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/arraymixins/npy.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/coord.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/coordset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.3/spectrochempy/core/dataset/nddataset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.3/spectrochempy/core/plotters/multiplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.3/spectrochempy/core/plotters/plot1d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.3/spectrochempy/core/plotters/plot2d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.3/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.3/spectrochempy/core/plotters/plotly.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/align.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/apodization.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/autosub.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/baseline.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/concatenate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/fft.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/filter.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/filter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/phasing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/shift.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/smooth.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/smooth.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/utils.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.3/spectrochempy/core/processors/zero_filling.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.3/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/project/project.py` & `spectrochempy-0.6.3/spectrochempy/core/project/project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/download.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/importer.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_carroucell.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_labspec.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_omnic.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_opus.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_quadera.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_soc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_spc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_topspin.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.3/spectrochempy/core/readers/read_zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.3/spectrochempy/core/script/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.3/spectrochempy/core/units/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.3/spectrochempy/core/writers/exporter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.3/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.3/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.3/spectrochempy/core/writers/write_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.3/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.3/spectrochempy/extern/nmrglue.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.3/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.3/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.3/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.3/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/citation.py` & `spectrochempy-0.6.3/spectrochempy/utils/citation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/constants.py` & `spectrochempy-0.6.3/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.3/spectrochempy/utils/coordrange.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/decorators.py` & `spectrochempy-0.6.3/spectrochempy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.3/spectrochempy/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.3/spectrochempy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/fake.py` & `spectrochempy-0.6.3/spectrochempy/utils/fake.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/file.py` & `spectrochempy-0.6.3/spectrochempy/utils/file.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.3/spectrochempy/utils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/misc.py` & `spectrochempy-0.6.3/spectrochempy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/objects.py` & `spectrochempy-0.6.3/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/optional.py` & `spectrochempy-0.6.3/spectrochempy/utils/optional.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.3/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/packages.py` & `spectrochempy-0.6.3/spectrochempy/utils/packages.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/plots.py` & `spectrochempy-0.6.3/spectrochempy/utils/plots.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/print.py` & `spectrochempy-0.6.3/spectrochempy/utils/print.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.3/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/system.py` & `spectrochempy-0.6.3/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/testing.py` & `spectrochempy-0.6.3/spectrochempy/utils/testing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/traits.py` & `spectrochempy-0.6.3/spectrochempy/utils/traits.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/version.py` & `spectrochempy-0.6.3/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.3/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/utils/zip.py` & `spectrochempy-0.6.3/spectrochempy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.3/spectrochempy/widgets/baselinecorrector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.3/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.2/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.3/spectrochempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.2/spectrochempy.egg-info/SOURCES.txt` & `spectrochempy-0.6.3/spectrochempy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 CITATION.cff
 Dockerfile
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 environment_dev.yml
+environment_test.yml
 pyproject.toml
 setup.cfg
 setup.py
 .conda/meta.yaml
 LICENSES/NMRGLUE_LICENSE.rst
 LICENSES/NNMF_LICENSE.rst
 LICENSES/PACKAGING_LICENSE.rst
 LICENSES/PANDAS_LICENSE.rst
 LICENSES/TRAITTYPES_LICENSE.rst
 requirements/requirements.txt
 requirements/requirements_dev.txt
+requirements/requirements_test.txt
 scp_data/__init__.py
 scp_data/databases/isotopes.csv
 scp_data/fonts/Felipa-Regular.ttf
 scp_data/fonts/Humor-Sans.ttf
 scp_data/fonts/LICENSE_felipa.txt
 scp_data/fonts/LICENSE_victormono.txt
 scp_data/fonts/VictorMono-Bold.ttf
@@ -72,15 +74,15 @@
 spectrochempy/analysis/_base.py
 spectrochempy/analysis/api.py
 spectrochempy/analysis/efa.py
 spectrochempy/analysis/iris.py
 spectrochempy/analysis/kinetic_utilities.py
 spectrochempy/analysis/linearregression.py
 spectrochempy/analysis/mcrals.py
-spectrochempy/analysis/nnmf.py
+spectrochempy/analysis/nmf.py
 spectrochempy/analysis/pca.py
 spectrochempy/analysis/peakfinding.py
 spectrochempy/analysis/pls.py
 spectrochempy/analysis/readme.rst
 spectrochempy/analysis/simplisma.py
 spectrochempy/analysis/svd.py
 spectrochempy/analysis/optimize/__init__.py
```

