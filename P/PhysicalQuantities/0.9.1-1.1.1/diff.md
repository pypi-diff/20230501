# Comparing `tmp/PhysicalQuantities-0.9.1.tar.gz` & `tmp/PhysicalQuantities-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PhysicalQuantities-0.9.1.tar", last modified: Wed Aug 29 16:58:55 2018, max compression
+gzip compressed data, was "PhysicalQuantities-1.1.1.tar", last modified: Mon May  1 13:15:04 2023, max compression
```

## Comparing `PhysicalQuantities-0.9.1.tar` & `PhysicalQuantities-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,113 @@
-drwxr-xr-x   0 juhasch   (1000) juhasch   (1000)        0 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1369 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PKG-INFO
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     2626 2018-08-29 16:51:02.000000 PhysicalQuantities-0.9.1/README.rst
-drwxr-xr-x   0 juhasch   (1000) juhasch   (1000)        0 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)        1 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/dependency_links.txt
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)       20 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/requires.txt
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1369 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/PKG-INFO
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)       19 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/top_level.txt
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)      816 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/SOURCES.txt
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)      366 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/setup.cfg
-drwxr-xr-x   0 juhasch   (1000) juhasch   (1000)        0 2018-08-29 16:58:55.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1445 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/prefixes.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)    22261 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/dBQuantity.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     3743 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/default_units.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)      289 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/currency.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1018 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/extend_prefixed.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1890 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/trait.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     3149 2018-08-29 16:20:28.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/quantityarray.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)    25112 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/quantity.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)      932 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/constants.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     3314 2018-08-28 19:14:22.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/more_units.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     2062 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/NDict.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     2862 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/decorator.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     4027 2018-08-29 16:53:50.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/__init__.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     2090 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/ipython.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1013 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/binary_units.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     7362 2018-08-26 15:45:59.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/numpywrapper.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     3371 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/imperial.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)    25845 2018-08-29 13:15:19.000000 PhysicalQuantities-0.9.1/PhysicalQuantities/unit.py
--rw-r--r--   0 juhasch   (1000) juhasch   (1000)     1405 2018-08-29 16:53:50.000000 PhysicalQuantities-0.9.1/setup.py
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.962994 PhysicalQuantities-1.1.1/
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.948386 PhysicalQuantities-1.1.1/.circleci/
+-rw-r--r--   0 juhasch    (501) staff       (20)      431 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/.circleci/config.yml
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.945643 PhysicalQuantities-1.1.1/.github/
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.948661 PhysicalQuantities-1.1.1/.github/workflows/
+-rw-r--r--   0 juhasch    (501) staff       (20)     1305 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/.github/workflows/api.yml
+-rw-r--r--   0 juhasch    (501) staff       (20)      571 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/.gitignore
+-rw-r--r--   0 juhasch    (501) staff       (20)     1007 2023-05-01 13:01:42.000000 PhysicalQuantities-1.1.1/CHANGELOG.md
+-rw-r--r--   0 juhasch    (501) staff       (20)     1750 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/COPYING.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     1204 2023-05-01 13:15:04.962862 PhysicalQuantities-1.1.1/PKG-INFO
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.952498 PhysicalQuantities-1.1.1/PhysicalQuantities/
+-rw-r--r--   0 juhasch    (501) staff       (20)     2504 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/NDict.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     4103 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/__init__.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      893 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/binary_units.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1023 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/constants.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1374 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/currency.py
+-rw-r--r--   0 juhasch    (501) staff       (20)    22827 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/dBQuantity.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     2858 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/decorator.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     3743 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/default_units.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1019 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/extend_prefixed.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     3371 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/imperial.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     6147 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/ipython.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     4107 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/more_units.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     7441 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/numpywrapper.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1431 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/prefixes.py
+-rw-r--r--   0 juhasch    (501) staff       (20)    25533 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/quantity.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     4770 2023-05-01 11:21:46.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/quantityarray.py
+-rw-r--r--   0 juhasch    (501) staff       (20)    26753 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/PhysicalQuantities/unit.py
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.953082 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/
+-rw-r--r--   0 juhasch    (501) staff       (20)     1204 2023-05-01 13:15:04.000000 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/PKG-INFO
+-rw-r--r--   0 juhasch    (501) staff       (20)     2541 2023-05-01 13:15:04.000000 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/SOURCES.txt
+-rw-r--r--   0 juhasch    (501) staff       (20)        1 2023-05-01 13:15:04.000000 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/dependency_links.txt
+-rw-r--r--   0 juhasch    (501) staff       (20)       20 2023-05-01 13:15:04.000000 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/requires.txt
+-rw-r--r--   0 juhasch    (501) staff       (20)       19 2023-05-01 13:15:04.000000 PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/top_level.txt
+-rw-r--r--   0 juhasch    (501) staff       (20)     2628 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/README.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.953498 PhysicalQuantities-1.1.1/conda.recipe/
+-rw-r--r--   0 juhasch    (501) staff       (20)       51 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/conda.recipe/bld.bat
+-rw-r--r--   0 juhasch    (501) staff       (20)       38 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/conda.recipe/build.sh
+-rw-r--r--   0 juhasch    (501) staff       (20)      405 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/conda.recipe/meta.yaml
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.954041 PhysicalQuantities-1.1.1/docs/
+-rw-r--r--   0 juhasch    (501) staff       (20)     7462 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/Makefile
+-rw-r--r--   0 juhasch    (501) staff       (20)        0 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/README.md
+-rw-r--r--   0 juhasch    (501) staff       (20)     2148 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/make.cmd
+-rw-r--r--   0 juhasch    (501) staff       (20)       86 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.956784 PhysicalQuantities-1.1.1/docs/source/
+-rw-r--r--   0 juhasch    (501) staff       (20)      631 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/Quantity.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     2085 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/QuantityArray.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)       67 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/Unit.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     9805 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/docs/source/conf.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1036 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/constants.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.956905 PhysicalQuantities-1.1.1/docs/source/images/
+-rw-r--r--   0 juhasch    (501) staff       (20)     4385 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/images/rc.png
+-rw-r--r--   0 juhasch    (501) staff       (20)     1646 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/index.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     2684 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-array.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)      465 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-autoscale.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     5096 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-basics.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     4052 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-dbquantity.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     6643 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-decorators.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     2151 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-example.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.957196 PhysicalQuantities-1.1.1/docs/source/pq-example_files/
+-rw-r--r--   0 juhasch    (501) staff       (20)    15102 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-example_files/pq-example_15_0.png
+-rw-r--r--   0 juhasch    (501) staff       (20)    15092 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-example_files/pq-example_16_0.png
+-rw-r--r--   0 juhasch    (501) staff       (20)     2080 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-formatting.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     1834 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-imperial.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     6258 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-ipython.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)     1949 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-numpy.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.957337 PhysicalQuantities-1.1.1/docs/source/pq-numpy_files/
+-rw-r--r--   0 juhasch    (501) staff       (20)    10977 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-numpy_files/pq-numpy_13_0.png
+-rw-r--r--   0 juhasch    (501) staff       (20)      135 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-numpywrapper.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)    10052 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-q-units.rst
+-rw-r--r--   0 juhasch    (501) staff       (20)      748 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-sympy.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.957469 PhysicalQuantities-1.1.1/docs/source/pq-sympy_files/
+-rw-r--r--   0 juhasch    (501) staff       (20)     1336 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-sympy_files/pq-sympy_9_0.png
+-rw-r--r--   0 juhasch    (501) staff       (20)     1313 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/docs/source/pq-uncertainties.rst
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.959834 PhysicalQuantities-1.1.1/examples/
+-rw-r--r--   0 juhasch    (501) staff       (20)     2569 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/Index.ipynb
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.959959 PhysicalQuantities-1.1.1/examples/images/
+-rw-r--r--   0 juhasch    (501) staff       (20)     4385 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/images/rc.png
+-rw-r--r--   0 juhasch    (501) staff       (20)     7956 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-array.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)     2625 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-autoscale.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    11423 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-basics.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    10366 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-dbquantity.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    21341 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-decorators.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    94806 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-example.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)     6397 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-formatting.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)     2014 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-imperial.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    11108 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-ipython.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    57912 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-numpy.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)    14957 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-q-units.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)     6251 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-sympy.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)     4254 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/examples/pq-uncertainties.ipynb
+-rw-r--r--   0 juhasch    (501) staff       (20)      175 2023-05-01 13:01:05.000000 PhysicalQuantities-1.1.1/readthedocs.yml
+-rw-r--r--   0 juhasch    (501) staff       (20)       60 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/requirements.txt
+-rw-r--r--   0 juhasch    (501) staff       (20)      222 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/runtests.py
+-rw-r--r--   0 juhasch    (501) staff       (20)       38 2023-05-01 13:15:04.963032 PhysicalQuantities-1.1.1/setup.cfg
+-rw-r--r--   0 juhasch    (501) staff       (20)     1405 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/setup.py
+drwxr-xr-x   0 juhasch    (501) staff       (20)        0 2023-05-01 13:15:04.962551 PhysicalQuantities-1.1.1/tests/
+-rw-r--r--   0 juhasch    (501) staff       (20)     2574 2023-05-01 11:21:46.000000 PhysicalQuantities-1.1.1/tests/test_array.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      392 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_binary_units.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      695 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_complex.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1073 2023-05-01 11:57:53.000000 PhysicalQuantities-1.1.1/tests/test_currency.py
+-rw-r--r--   0 juhasch    (501) staff       (20)    13705 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/tests/test_dbquantity.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1758 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_decorator.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     3167 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_imperial.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      613 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_init.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1499 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_ipython.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1087 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_lists_arrays.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     1149 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_ndict.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      529 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_numpy.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     4071 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/test_numpywrapper.py
+-rw-r--r--   0 juhasch    (501) staff       (20)    12328 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/tests/test_quantity.py
+-rw-r--r--   0 juhasch    (501) staff       (20)     6718 2023-05-01 11:22:51.000000 PhysicalQuantities-1.1.1/tests/test_units.py
+-rw-r--r--   0 juhasch    (501) staff       (20)      699 2023-04-15 21:37:39.000000 PhysicalQuantities-1.1.1/tests/text_exp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PhysicalQuantities-0.9.1/PKG-INFO` & `PhysicalQuantities-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: PhysicalQuantities
-Version: 0.9.1
+Version: 1.1.1
 Summary: Allow calculations using physical quantities
 Home-page: https://github.com/juhasch/PhysicalQuantities
 Author: Juergen Hasch
 Author-email: juergen.hasch@elbonia.de
 License: BSD
-Description: 
-        *PhysicalQuantities* is a Python module that allows calculations to be aware of physical units. Built-in unit
-        conversion ensures that calculations will result in the correct unit.
-        
-        The main goals are:
-         * easy use, especially conversion, scaling and interoperating with different units
-         * focus on using units for engineering tasks
-         * provide logarithmic dB calculations
-         * allow seamless Numpy array operation
-        
-        The module also contains an extension for IPython. This allows much simplified usage by typing in physical quantities
-        as number and unit:
-        
-            >>> a = 1m ; b = 1s
-            >>> print("a=", a, ", b=",b,", a/b=", a/b)
-            a= 1 m , b= 1 s , a/b= 1.0 m/s
-            >>> u = 10V
-            >>> u.dB
-            >>> 20.0 dBV
-        
-        
 Keywords: Physical Quantities IPython
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: COPYING.rst
+
+
+*PhysicalQuantities* is a Python module that allows calculations to be aware of physical units. Built-in unit
+conversion ensures that calculations will result in the correct unit.
+
+The main goals are:
+ * easy use, especially conversion, scaling and interoperating with different units
+ * focus on using units for engineering tasks
+ * provide logarithmic dB calculations
+ * allow seamless Numpy array operation
+
+The module also contains an extension for IPython. This allows much simplified usage by typing in physical quantities
+as number and unit:
+
+    >>> a = 1m ; b = 1s
+    >>> print("a=", a, ", b=",b,", a/b=", a/b)
+    a= 1 m , b= 1 s , a/b= 1.0 m/s
+    >>> u = 10V
+    >>> u.dB
+    >>> 20.0 dBV
+
```

### Comparing `PhysicalQuantities-0.9.1/README.rst` & `PhysicalQuantities-1.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 .. image:: https://badge.fury.io/py/physicalquantities.svg
     :target: https://badge.fury.io/py/physicalquantities
 
 .. image:: https://travis-ci.org/juhasch/PhysicalQuantities.svg
     :target: https://travis-ci.org/juhasch/PhysicalQuantities
 
 
-=====================================================
- PhysicalQuantites - Calculation in Python with Units
-=====================================================
+======================================================
+ PhysicalQuantities - Calculation in Python with Units
+======================================================
 
 Overview
 ========
 
 PhysicalQuantities is a module for Python 3.6 that allows calculations to be aware 
 of physical units with a focus on engineering applications. 
 Built-in unit conversion ensures that calculations will result in the correct aggregate 
@@ -112,8 +112,7 @@
 
 to generate a conda package. I will upload a receipe to conda-forge at a later time.
 
 Note
 ----
 This module is originally based on the IPython extension by Georg Brandl at
 https://bitbucket.org/birkenfeld/ipython-physics.
-
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities.egg-info/PKG-INFO` & `PhysicalQuantities-1.1.1/PhysicalQuantities.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: PhysicalQuantities
-Version: 0.9.1
+Version: 1.1.1
 Summary: Allow calculations using physical quantities
 Home-page: https://github.com/juhasch/PhysicalQuantities
 Author: Juergen Hasch
 Author-email: juergen.hasch@elbonia.de
 License: BSD
-Description: 
-        *PhysicalQuantities* is a Python module that allows calculations to be aware of physical units. Built-in unit
-        conversion ensures that calculations will result in the correct unit.
-        
-        The main goals are:
-         * easy use, especially conversion, scaling and interoperating with different units
-         * focus on using units for engineering tasks
-         * provide logarithmic dB calculations
-         * allow seamless Numpy array operation
-        
-        The module also contains an extension for IPython. This allows much simplified usage by typing in physical quantities
-        as number and unit:
-        
-            >>> a = 1m ; b = 1s
-            >>> print("a=", a, ", b=",b,", a/b=", a/b)
-            a= 1 m , b= 1 s , a/b= 1.0 m/s
-            >>> u = 10V
-            >>> u.dB
-            >>> 20.0 dBV
-        
-        
 Keywords: Physical Quantities IPython
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: COPYING.rst
+
+
+*PhysicalQuantities* is a Python module that allows calculations to be aware of physical units. Built-in unit
+conversion ensures that calculations will result in the correct unit.
+
+The main goals are:
+ * easy use, especially conversion, scaling and interoperating with different units
+ * focus on using units for engineering tasks
+ * provide logarithmic dB calculations
+ * allow seamless Numpy array operation
+
+The module also contains an extension for IPython. This allows much simplified usage by typing in physical quantities
+as number and unit:
+
+    >>> a = 1m ; b = 1s
+    >>> print("a=", a, ", b=",b,", a/b=", a/b)
+    a= 1 m , b= 1 s , a/b= 1.0 m/s
+    >>> u = 10V
+    >>> u.dB
+    >>> 20.0 dBV
+
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/prefixes.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/prefixes.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ('Y', 1.e24), ('Z', 1.e21), ('E', 1.e18), ('P', 1.e15), ('T', 1.e12),
     ('G', 1.e9), ('M', 1.e6), ('k', 1.e3), ('h', 1.e2), ('da', 1.e1),
     ('d', 1.e-1), ('c', 1.e-2), ('m', 1.e-3), ('u', 1.e-6), ('n', 1.e-9),
     ('p', 1.e-12), ('f', 1.e-15), ('a', 1.e-18), ('z', 1.e-21),
     ('y', 1.e-24),
 ]
 
-# educed set of scaling prefixes for engineering purposes:
+# reduced set of scaling prefixes for engineering purposes:
 _engineering_prefixes = [
     ('T', 1.e12),
     ('G', 1.e9), ('M', 1.e6), ('k', 1.e3),
     ('c', 1.e-2), ('m', 1.e-3), ('u', 1.e-6), ('n', 1.e-9),
     ('p', 1.e-12), ('f', 1.e-15), ('a', 1.e-18),
 ]
 
@@ -35,9 +35,9 @@
         _prefixes = _engineering_prefixes
     else:
         _prefixes = _full_prefixes
     unit = unit_table[unitname]
     for prefix in _prefixes:
         prefixedname = prefix[0] + unitname
         if prefixedname not in unit_table:
-            add_composite_unit(prefixedname, prefix[1], unitname, prefixed=True, baseunit=unit, verbosename=unit.verbosename,
+            add_composite_unit(prefixedname, prefix[1], unitname, prefixed=True, verbosename=unit.verbosename,
                     url=unit.url)
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/dBQuantity.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/dBQuantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 """
 
 import copy
 
 import numpy as np
 from IPython import get_ipython
 
-from .quantity import PhysicalQuantity, PhysicalUnit, UnitError, unit_table
+from .quantity import PhysicalQuantity
+from .unit import PhysicalUnit, UnitError, unit_table
 
 __all__ = ['dB10', 'dB20', 'PhysicalQuantity_to_dBQuantity', 'dBQuantity', 'dB_unit_table']
 
 # Dynamically generated list of all dB units
 dB_unit_table = {}
 
 
@@ -35,25 +36,26 @@
         Name of dB unit
     unit: PhysicalUnit
         Physical representation of the dB value
     offset: float
         Offset, used e.g. for dBd vs. dBi
 
     """
-    def __init__(self, name, physicalunit, offset=0, factor=0, z0=PhysicalQuantity(50, 'Ohm')):
+    def __init__(self, name: str, physicalunit: PhysicalUnit, offset: float = 0, factor: float = 0,
+                 z0=PhysicalQuantity(50, 'Ohm')):
         """
 
         Parameters
         ----------
-        name: str
+        name
             Name of dB unit
         physicalunit: PhysicalUnit
             Physical representation of the dB value
-        offset: float
-            Offset, used e.g. for dBd vs. dBi
+        offset
+            Specify offset used e.g. for dBd vs. dBi
 
         """
         self.name = name
         self.physicalunit = physicalunit
         self.offset = offset
         self.factor = factor
         self.z0 = z0
@@ -66,15 +68,15 @@
         return self.physicalunit.is_power
 
     @property
     def __name__(self):
         return self.name
 
 
-def _add_dB_units(name, unit,  offset=0, factor=0):
+def _add_dB_units(name, unit,  offset: float = 0, factor: float = 0):
     dB_unit_table[name] = dBUnit(name, unit, offset, factor)
 
 
 # Predefined dB units
 _add_dB_units('dB', unit=None)
 _add_dB_units('dBm', unit=unit_table['mW'])
 _add_dB_units('dBW', unit=unit_table['W'])
@@ -82,15 +84,15 @@
 _add_dB_units('dBuV', unit=unit_table['uV'])
 _add_dB_units('dBmV', unit=unit_table['mV'])
 _add_dB_units('dBV', unit=unit_table['V'])
 _add_dB_units('dBnA', unit=unit_table['nA'])
 _add_dB_units('dBuA', unit=unit_table['uA'])
 _add_dB_units('dBmA', unit=unit_table['mA'])
 _add_dB_units('dBA', unit=unit_table['A'])
-_add_dB_units('dBsm', unit=PhysicalQuantity(1,'m**2').unit)
+_add_dB_units('dBsm', unit=PhysicalQuantity(1, 'm**2').unit)
 _add_dB_units('dBd', unit=None, factor=10, offset=2.15)
 _add_dB_units('dBi', unit=None, factor=10)
 _add_dB_units('dBc', unit=None, factor=10)
 
 
 def PhysicalQuantity_to_dBQuantity(x, dBunitname=None):
     """ Conversion from a PhysicalQuantity to correct dB<x> value
@@ -110,24 +112,25 @@
     """
     if isinstance(x, PhysicalQuantity):
         dbbase = None
         value = None
 
         if dBunitname is not None and dB_unit_table[dBunitname] is not None:
             if dB_unit_table[dBunitname].physicalunit.baseunit.name == x.unit.baseunit.name:
-                    dbbase = dBunitname
-                    value = x.to(dB_unit_table[dBunitname].physicalunit.name).value
-                    _unit = dB_unit_table[dBunitname].physicalunit  # FIXME
+                dbbase = dBunitname
+                value = x.to(dB_unit_table[dBunitname].physicalunit.name).value
+                _unit = dB_unit_table[dBunitname].physicalunit  # FIXME
         else:
             for key in dB_unit_table:
                 if dB_unit_table[key].physicalunit is not None and dB_unit_table[key].physicalunit.name == x.unit.name:
                     dbbase = key
                     value = x.value
                     break
-                elif dB_unit_table[key].physicalunit is not None and dB_unit_table[key].physicalunit.baseunit.name == x.unit.baseunit.name:
+                elif dB_unit_table[key].physicalunit is not None and dB_unit_table[key].physicalunit.baseunit.name == \
+                        x.unit.baseunit.name:
                     dbbase = key
                     value = x.base.value
         _unit = x.unit
         if dbbase is None:
             raise UnitError(f'Cannot handle unit {x.unit}')
         factor = 20 - 10 * _unit.is_power
         dbvalue = factor * np.log10(value)
@@ -209,26 +212,26 @@
             raise UnitError(f'Unknown unit {unitname}')
 
         ip = get_ipython()
         if ip is not None:
             self.ptformatter = ip.display_formatter.formatters['text/plain']
         else:
             self.ptformatter = None
-        self.format = '' # display format for number to string conversion
+        self.format = ''  # display format for number to string conversion
 
         if islog is True:
             self.value = value
         else:
             self.value = self.unit.factor * np.log10(value) - self.unit.offset
 
     def __dir__(self):
         """ return list for tab completion
             Include conversions to linear and their dB units
         """
-        x = super().__dir__()
+        x = list(super().__dir__())
         # This is required, as strange things happen with IPython...
         for cruft in ['__builtins__', '__args__']:
             try:
                 del unit_table[cruft]
             except KeyError:
                 pass
 
@@ -258,21 +261,20 @@
         Raises
         ------
         UnitError
             If no conversion between units is possible
 
         Examples
         --------
-        >>> a = 2 mm
+        >>> from PhysicalQuantities import q
+        >>> a = 2 * q.dBm
+        >>> a
+        2 dBm
         >>> a._
         2
-        >>> a.mm_
-        2
-        >>> a.m_
-        0.002
         """
         dropunit = (attr[-1] == '_')
         unitname = attr.strip('_')
         if unitname == '' and dropunit is True:
             return self.value
 
         isdbunit = unitname in dB_unit_table.keys()
@@ -284,15 +286,16 @@
         
         # convert to different scaling
         if self.unit.name is unitname:
             return self
         else:
             # convert to same base unit, only scaling
             if self.unit.physicalunit is not None:
-                scaling = self.unit.factor * np.log10( self.unit.physicalunit.factor / dB_unit_table[unitname].physicalunit.factor)
+                scaling = self.unit.factor * np.log10(self.unit.physicalunit.factor /
+                                                      dB_unit_table[unitname].physicalunit.factor)
             else:
                 scaling = self.unit.offset
             value = self.value + scaling
             if dropunit is False:
                 return self.__class__(value, unitname, islog=True)
             else:
                 return value
@@ -312,38 +315,43 @@
         ----------
         unitname: str
             Name of new dB unit
 
         """
         if unitname in dB_unit_table.keys():
             # convert to same base unit, only scaling
-            scaling = self.unit.factor * np.log10( self.unit.physicalunit.factor / dB_unit_table[unitname].physicalunit.factor)
+            scaling = self.unit.factor * np.log10(self.unit.physicalunit.factor /
+                                                  dB_unit_table[unitname].physicalunit.factor)
             value = self.value + scaling
             return self.__class__(value, unitname, islog=True)
 
-    def copy(self):
-        """Return a copy of the dBQuantity including the value.
-        Needs deepcopy to copy the value
-        """
-        return copy.deepcopy(self)
+    def __deepcopy__(self, memo: dict):
+        """ Return a copy of the PhysicalQuantity including the value.
+            Needs deepcopy to copy the value
+        """
+        new_value = copy.deepcopy(self.value)
+        new_instance = self.__class__(new_value, self.unit.name, islog=True)
+        memo[id(self)] = new_instance
+        return new_instance
 
     def __getitem__(self, key):
         """ Allow indexing if quantities if underlying object is array or list
             e.g. obj[0] or obj[0:4]
         """
         if isinstance(self.value, np.ndarray) or isinstance(self.value, list):
             return self.__class__(self.value[key], self.unit.name)
         raise AttributeError('Not a list or array: %s' % self)        
 
     def __setitem__(self, key, value):
         """ Set quantities if underlying object is array or list
 
             >>> from PhysicalQuantities import q
-            >>> obj = np.linspace(0,10,10) * 1 q.dBm
+            >>> obj = np.linspace(0,10,10) * q.dBm
             >>> obj[0] = 0 q.dBm
+
         """
         if not isinstance(value, dBQuantity):
             raise AttributeError('Not a dBQuantity')
         if isinstance(self.value, np.ndarray) or isinstance(self.value, list):
             self.value[key] = value.to(self.unit.name).value
             return self.__class__(self.value[key], self.unit.name)
         raise AttributeError('Not a dBQuantity array or list')
@@ -446,18 +454,18 @@
         3 dB
         >>> 1 dBm + 2 dB
         3 dBm
         >>> 1 dBm + 1 dBm
         4.01 dBm
         """
         
-        if (self.unit.name is 'dB') or (other.unit.name is 'dB'):
+        if (self.unit.name == 'dB') or (other.unit.name == 'dB'):
             # easy unitless adding
             value = self.value + other.value
-            unit = other.unit.name if self.unit.name is 'dB' else self.unit.name
+            unit = other.unit.name if self.unit.name == 'dB' else self.unit.name
             return self.__class__(value, unit, islog=True)
         elif dB_unit_table[self.unit.name] is dB_unit_table[other.unit.name]:
             # same unit adding
             val1 = float(self)
             val2 = float(other)
             return self.__class__(val1+val2, self.unit.name, islog=False)
         else:
@@ -476,30 +484,30 @@
         Examples
         --------
         >>> 0 dBm + 1 dB
         1 dBm
         >>> 0 dBm + 1 dBW
         xx dBm
         """
-        if self.unit.name is 'dB' or other.unit.name is 'dB':
+        if self.unit.name == 'dB' or other.unit.name == 'dB':
             # easy unitless adding
             value = self.value - other.value
             return self.__class__(value, self.unit.name, islog=True)
         elif self.unit.physicalunit is other.unit.physicalunit:
             # same unit subtraction
             val1 = float(self)
             val2 = float(other)
             return self.__class__(val1-val2, self.unit.name, islog=False)
         else:
             raise UnitError('Cannot add unequal units %s and %s' % (self.unit.name, other.unit.name))
 
     __rsub__ = __sub__
     
     def __mul__(self, other):
-        if  not hasattr(other,'unit'):
+        if not hasattr(other, 'unit'):
             # dB values will be multiplied with a factor to enable "a = 2 * q.dBm"
             value = self.value * other
             return self.__class__(value, self.unit.name, islog=True)
 
     __rmul__ = __mul__
 
     def __div__(self, other):
@@ -513,47 +521,60 @@
         Returns
         -------
         dBQuantity
             divided dBQuantity
         
         >>> 3 dB / 4
         """
-        if self.unit.name is 'dB' and not hasattr(other, 'unit'):
+        if self.unit.name == 'dB' and not hasattr(other, 'unit'):
             # dB without physical dimension can be divided by a factor
             value = self.value / other
             return self.__class__(value, self.unit.name, islog=True)
         raise UnitError('Cannot divide dB units')
 
     __truediv__ = __div__
 
     def __floordiv__(self, other):
         """ Divide a dB value by another factor
         Only valid if the dB value is not associated whith a physical quantity
-        
-        :param other: dBQuantity
-        :return: divided dBQuantity
+
+        Parameters
+        ----------
+        other: dBQuantity
+
+        Returns
+        -------
+        dBQuantity
+            divided dBQuantity
         
         >>> 3 dB / 4
         """
-        if self.unit.name is 'dB' and not hasattr(other, 'unit'):
+        if self.unit.name == 'dB' and not hasattr(other, 'unit'):
             # dB without physical dimension can be divided by a factor
             value = self.value // other
             return self.__class__(value, self.unit.name, islog=True)
         raise UnitError('Cannot divide dB units')
             
     def __rfloordiv__(self, other):
         """ Divide a dB value by another factor
         Only valid if the dB value is not associated whith a physical quantity
-        
-        :param other: dBQuantity
-        :return: divided dBQuantity
+
+        Parameters
+        ----------
+        other: dBQuantity
+            Divisor
+
+        Returns
+        -------
+        dBQuantity
+            divided dBQuantity
         
         >>> 3 dB / 4
         """
-        if self.unit.name is 'dB' and not hasattr(other, 'unit'):
+        if self.unit.name == 'dB' and not hasattr(other, 'unit'):
             # dB without physical dimension can be divided by a factor
             value = other // self.value
             return self.__class__(value, self.unit.name, islog=True)
         
     def __neg__(self):
         """ Return negative value """
         return self.__class__(-self.value, self.unit.name, islog=True)
@@ -563,18 +584,18 @@
         if self.unit.factor == 0:
             raise UnitError('Cannot convert dB unit with unknown factor to linear')
 
         val = self.value / self.unit.factor
         return pow(10, val)
     
     def __str__(self):
-        if self.ptformatter is not None and self.format is '' and isinstance(self.value,float):
+        if self.ptformatter is not None and self.format == '' and isinstance(self.value, float):
             # %precision magic only works for floats
-            format = self.ptformatter.float_format
-            return "%s %s" % (format % self.value, str(self.unit.name))
+            fmt = self.ptformatter.float_format
+            return "%s %s" % (fmt % self.value, str(self.unit.name))
         return '{0:{format}} {1}'.format(self.value, str(self.unit.name), format=self.format)
 
     def __repr__(self):
         return self.__str__()
 
     def __gt__(self, other):
         """ Test if quantity is greater than other
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/default_units.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/default_units.py`

 * *Files identical despite different names*

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/extend_prefixed.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/extend_prefixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Extend prefixrange of prefixed units from engineering (1e+-12) to full (1e+-24)
+# Extend prefix range of prefixed units from engineering (1e+-12) to full (1e+-24)
 from .prefixes import addprefixed
 
 addprefixed('m', prefixrange='full')
 addprefixed('g', prefixrange='full')
 addprefixed('s', prefixrange='full')
 addprefixed('A', prefixrange='full')
 addprefixed('K', prefixrange='full')
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/quantityarray.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/quantityarray.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,42 +17,87 @@
         # add the new attribute to the created instance
         obj.unit = findunit(unit)
         # Finally, we must return the newly created object:
         return obj
 
     def __array_finalize__(self, obj):
         # see InfoArray.__array_finalize__ for comments
-        if obj is None: return
+        if obj is None:
+            return
         self.unit = getattr(obj, 'unit', None)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+        # add, substract
+        # divide
+        # square, power
         args = []
-        in_no = []
-        for i, input_ in enumerate(inputs):
-            if isinstance(input_, PhysicalQuantityArray):
-                in_no.append(i)
-                args.append(input_.view(np.ndarray))
-                if input_.unit != self.unit:
+        op = ufunc.__name__
+        out_unit = self.unit
+        args.append(self.view(np.ndarray))
+
+        if op in ['add', 'subtract']:
+            par1, par2 = inputs
+            if isinstance(par2, PhysicalQuantityArray):
+                if par2.unit != self.unit:
                     raise ValueError('Incompatible units.')
+                args.append(par2.view(np.ndarray))
             else:
-                args.append(input_)
+                args.append(par2)
+        elif op in ['multiply']:
+            par1, par2 = inputs
+            if isinstance(par2, PhysicalQuantityArray):
+                args.append(par2.view(np.ndarray))
+                out_unit *= par2.unit
+            else:
+                args.append(par2)
+        elif op in ['true_divide']:
+            par1, par2 = inputs
+            if isinstance(par2, PhysicalQuantityArray):
+                args.append(par2.view(np.ndarray))
+                out_unit /= par2.unit
+            else:
+                args.append(par2)
+        elif op in ['square']:
+            out_unit = out_unit ** 2
+        elif op in ['square', 'power']:
+            par1, par2 = inputs
+            if isinstance(par2, PhysicalQuantityArray):
+                raise ValueError('Incompatible units.')
+            else:
+                args.append(par2)
+                out_unit = out_unit ** par2
+        elif op in ['bitwise_or', 'bitwise_and', 'bitwise_xir']:
+            args = []
+            for par in inputs:
+                args.append(par.view(np.ndarray))
+            kwargs=dict(out=self.view(np.ndarray))
+        else:
+            args = []
+            for par2 in inputs:
+                if isinstance(par2, PhysicalQuantityArray):
+                    if par2.unit != self.unit:
+                        raise ValueError('Incompatible units.')
+                    args.append(par2.view(np.ndarray))
+                else:
+                    args.append(par2)
+
         results = super().__array_ufunc__(ufunc, method, *args, **kwargs)
-        return results
+        return self.__class__(results, out_unit)
 
     def __dir__(self):
         ulist = super().__dir__()
         u = unit_table.values()
         for _u in u:
             if isphysicalunit(_u):
                 if str(_u.baseunit) is str(self.unit.baseunit):
                     ulist.append(_u.name)
         return ulist
 
     def __getattr__(self, attr):
-        dropunit = (attr[-1] is '_')
+        dropunit = (attr[-1] == '_')
         attr = attr.strip('_')
         if attr == '' and dropunit is True:
             return self.view(ndarray)
         try:
             attrunit = unit_table[attr]
         except KeyError:
             raise AttributeError(f'Unit {attr} not found')
@@ -63,15 +108,15 @@
 
     def __repr__(self):
         arrstr = super().__str__()
         return f'PhysicalQuantityArray({arrstr}, unit={self.unit})'
 
     def to(self, *units):
         units = list(map(findunit, units))
-        if len(units) is 1:
+        if len(units) == 1:
             unit = units[0]
             factor = convertvalue(1, self.unit, unit)
             return self.__class__(self * factor, unit)
         raise ValueError('More than one unit given to convert to')
 
     @property
     def base(self):
@@ -84,12 +129,12 @@
                 denom += '/' + unit
                 if power < -1:
                     denom += '**' + str(-power)
             elif power > 0:
                 num += '*' + unit
                 if power > 1:
                     num += '**' + str(power)
-        if len(num) is 0:
+        if len(num) == 0:
             num = '1'
         else:
             num = num[1:]
         return self.__class__((self + self.unit.offset) * self.unit.factor, num + denom)
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/quantity.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """ PhysicalQuantity class definition
 
 """
 
-# TODO:
-# - deepcopy does not work
-
 
 try:
     from sympy import printing
 except ImportError:  # pragma: no cover
-    pass
+    def printing():
+        pass
 
 import copy
 import json
 
 import numpy as np
 from IPython import get_ipython
 
 from .unit import (
     PhysicalUnit, UnitError, base_names, convertvalue, findunit,
     isphysicalunit, unit_table,
 )
 
-__all__ = ['PhysicalQuantity']
-
+__all__ = ['PhysicalQuantity', 'PhysicalUnit', 'UnitError', 'unit_table']
 
 class PhysicalQuantity:
     """ Physical quantity with units.
 
         PhysicalQuantity instances allow addition, subtraction, multiplication, and
         division with each other as well as multiplication, division, and
         exponentiation with numbers.  Addition and subtraction check that the units
         of the two operands are compatible and return the result in the units of the
         first operand. A limited set of mathematical functions (from numpy) is
         applicable as well.
     """
 
-    __array_priority__ = 1000  # make sure numpy arrays do not get iterated
+    __array_priority__: int = 1000  # make sure numpy arrays do not get iterated
+    format: str = ''                # display format for number to string conversion
+    annotation: str = None          # optional annotation of Quantity
 
-    def __init__(self, value, unit=None):
+    def __init__(self, value: float, unit=None, annotation: str = None):
         """There are two constructor calling patterns
 
         Parameters
         ----------
         value: any
             value of the quantity
         
@@ -56,26 +55,26 @@
         1 V
         """
         ip = get_ipython()
         if ip is not None:  # pragma: no cover
             self.ptformatter = ip.display_formatter.formatters['text/plain']
         else:
             self.ptformatter = None
-        self.format = ''  # display format for number to string conversion
         self.value = value
+        self.annotation = annotation
         self.unit = findunit(unit)
 
     def __dir__(self):
-        """ List available attributes including conversion to other scaling prefixes
+        """List available attributes including conversion to other scaling prefixes
+
         Returns
         -------
-        list
-            list of units for tab completion
+        list of units for tab completion
         """
-        ulist = super().__dir__()
+        ulist = list(super().__dir__())
         u = unit_table.values()
         for _u in u:
             if isphysicalunit(_u):
                 if str(_u.baseunit) is str(self.unit.baseunit):
                     ulist.append(_u.name)
         return ulist
     
@@ -100,15 +99,15 @@
         >>> a._
         2
         >>> a.mm_
         2
         >>> a.m_
         0.002
         """
-        dropunit = (attr[-1] is '_')
+        dropunit = (attr[-1] == '_')
         attr = attr.strip('_')
         if attr == '' and dropunit is True:
             return self.value
         try:
             attrunit = unit_table[attr]
         except KeyError:
             raise AttributeError(f'Unit {attr} not found')
@@ -142,16 +141,19 @@
         """ Return length of quantity if underlying object is array or list
             e.g. len(obj)
         """
         if isinstance(self.value, np.ndarray) or isinstance(self.value, list):
             return len(self.value)
         raise TypeError('Object of type %s has no len()' % type(self.value))
 
+    def _ipython_key_completions_(self):
+        return self.unit_table.keys()
+
     @property
-    def dB(self):
+    def dB(self):  # noqa
         """ Convert to dB scaled unit, if possible. Guess if it is a power unit to select 10*log10 or 20*log10
 
         Returns
         -------
         dBQuantity
             dB quantity converted from PhysicalQuantity
         
@@ -160,15 +162,15 @@
         --------
         >>> from PhysicalQuantities import q
         >>> (10 q.V).dB
         20.0 dBV
         >>> (10 q.W).dB
         10.0 dBW
         """
-        from .dBQuantity import dBQuantity, PhysicalQuantity_to_dBQuantity
+        from .dBQuantity import PhysicalQuantity_to_dBQuantity
         return PhysicalQuantity_to_dBQuantity(self)
 
     def rint(self):
         """ Round elements to the nearest integer
 
         Returns
         -------
@@ -183,15 +185,15 @@
             e.g. str(obj)
             
         Returns
         -------
         string
             string representation of PhysicalQuantity            
         """
-        if self.ptformatter is not None and self.format is '' and isinstance(self.value, float):  # pragma: no cover
+        if self.ptformatter is not None and self.format == '' and isinstance(self.value, float):  # pragma: no cover
             # %precision magic only works for floats
             fmt = self.ptformatter.float_format
             return u"%s %s" % (fmt % self.value, str(self.unit))
         return '{0:{format}} {1}'.format(self.value, str(self.unit), format=self.format)
 
     def __complex__(self):
         """ Return complex number without units converted to base units 
@@ -207,15 +209,15 @@
         """ Return string representation
         """
         return self.__str__()
 
     def _repr_markdown_(self):
         """ Return markdown representation for IPython notebook
         """
-        if self.ptformatter is not None and self.format is '' and isinstance(self.value, float):  # pragma: no cover
+        if self.ptformatter is not None and self.format == '' and isinstance(self.value, float):  # pragma: no cover
             # %precision magic only works for floats
             fmt = self.ptformatter.float_format
             return u"%s %s" % (fmt % self.value, self.unit._repr_markdown_())
         if str(type(self.value)).find('sympy') > 0:
             # sympy
             return '${0}$ {1}'.format(printing.latex(self.value), self.unit.markdown)
         return '{0:{format}} {1}'.format(self.value, self.unit.markdown, format=self.format)
@@ -242,15 +244,15 @@
 
         Returns
         -------
         PhysicalQuantity
             sum of the two quantities
         """
         if not isinstance(other, PhysicalQuantity):
-            raise UnitError('Incompatible types %s' % type(other))
+            raise UnitError(f'Incompatible types {type(self)} and {type(other)}')
         new_value = sign1 * self.value + \
             sign2 * other.value * other.unit.conversion_factor_to(self.unit)
         return self.__class__(new_value, self.unit)
 
     def __add__(self, other):
         return self._sum(other, 1, 1)
 
@@ -555,45 +557,48 @@
     @staticmethod
     def _round(x):
         if np.greater(x, 0.):
             return np.floor(x)
         else:
             return np.ceil(x)
 
-    def copy(self):
+    def __deepcopy__(self, memo: dict):
         """ Return a copy of the PhysicalQuantity including the value.
             Needs deepcopy to copy the value
         """
-        return copy.deepcopy(self)
+        new_value = copy.deepcopy(self.value)
+        new_instance = self.__class__(new_value, self.unit)
+        memo[id(self)] = new_instance
+        return new_instance
 
     @property
     def autoscale(self):
         """ Autoscale to a reasonable unit, if possible
 
-        Example
-        -------
+        Examples
+        --------
         >>> b = PhysicalQuantity(4e-9, 'F')
         >>> b.autoscale
         4 nF
         """
-        if len(self.unit.names) is 1:
+        if len(self.unit.names) == 1:
             b = self.base
-            n = np.log10(b.value)
+            n = np.log10(abs(b.value))
             # we want to be between 0..999 
             _scale = np.floor(n)
             # now search for unit
             for i in unit_table:
                 u = unit_table[i]
                 if isinstance(u, PhysicalUnit):
                     if u.baseunit is self.unit.baseunit:
                         f = np.log10(u.factor) - _scale
                         if (f > -3) and (f < 1):
                             return self.to(i)
         return self
-    
+
     def to(self, *units):
         """ Express the quantity in different units.
 
         Parameters
         ----------
         units: str
             Name of the unit
@@ -612,26 +617,26 @@
             If one unit is specified, a new PhysicalQuantity object is returned that expresses the quantity in
             that unit. If several units are specified, the return value is a tuple of PhysicalObject instances with
             one element per unit such that the sum of all quantities in the tuple equals the the original quantity and
             all the values except for the last one are integers. This is used to convert to irregular unit systems like
             hour/minute/second.
         """
         units = list(map(findunit, units))
-        if len(units) is 1:
+        if len(units) == 1:
             unit = units[0]
             value = convertvalue(self.value, self.unit, unit)
             return self.__class__(value, unit)
         else:
             units.sort()
             result = []
             value = self.value
             unit = self.unit
             for i in range(len(units)-1, -1, -1):
                 value *= unit.conversion_factor_to(units[i])
-                if i is 0:
+                if i == 0:
                     rounded = value
                 else:
                     rounded = self._round(value)
                 result.append(self.__class__(rounded, units[i]))
                 value = value - rounded
                 unit = units[i]
             return tuple(result)
@@ -662,15 +667,15 @@
                 denom += '/' + unit
                 if power < -1:
                     denom += '**' + str(-power)
             elif power > 0:
                 num += '*' + unit
                 if power > 1:
                     num += '**' + str(power)
-        if len(num) is 0:
+        if len(num) == 0:
             num = '1'
         else:
             num = num[1:]
         return self.__class__(new_value, num + denom)
 
     # make it easier using complex numbers
     @property
@@ -801,15 +806,15 @@
 
         Returns
         -------
         str
             JSON string describing PhysicalQuantity
 
         """
-        json_quantity = json.dumps({ 'PhysicalQuantity' : self.to_dict})
+        json_quantity = json.dumps({'PhysicalQuantity': self.to_dict})
         return json_quantity
 
     @staticmethod
     def from_dict(quantity_dict: dict):
         """Retrieve PhysicalUnit from dict description
 
         Parameters
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/constants.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from math import pi
 
 import numpy as np
 
 from .quantity import *
 
-c0 = PhysicalQuantity(299792458., 'm/s')
-mu0 = PhysicalQuantity(4*np.pi*1e-7, 'N/A**2')
-eps0 = PhysicalQuantity(8.854188e-12, 'F/m')
+c0 = PhysicalQuantity(299792458., 'm/s', 'Speed of light')
+mu0 = PhysicalQuantity(4*np.pi*1e-7, 'N/A**2', 'Permeability of vacuum')
+eps0 = PhysicalQuantity(8.854188e-12, 'F/m', 'Permittivity of vacuum')
 Grav = PhysicalQuantity(6.67384e-11, 'm**3/kg/s**2')
 hpl = PhysicalQuantity(6.62606957e-34, 'J*s')
 hbar = PhysicalQuantity(6.62606957e-34/(2*pi), 'J*s')
 e0 = PhysicalQuantity(1.602176565e-19, 'C')
 me = PhysicalQuantity(9.10938291e-31, 'kg')
 mp = PhysicalQuantity(1.672621777e-27, 'kg')
 mn = PhysicalQuantity(1.674927351e-27, 'kg')
 NA = PhysicalQuantity(6.02214129e23, '1/mol')
-kb = PhysicalQuantity(1.3806488e-23, 'J/K')
+kb = PhysicalQuantity(1.3806488e-23, 'J/K', 'Boltzman constant')
 g0 = PhysicalQuantity(9.80665, 'm/s**2')
 R = PhysicalQuantity(8.3144621, 'J/mol/K')
 Ry = PhysicalQuantity(10973731.568539, '1/m')
 mu_n = PhysicalQuantity(-0.96623647e-26, 'J/T')
 gamma = PhysicalQuantity(183.247179, 'MHz/T')
 sigmaT = PhysicalQuantity(6.652453e-29, 'm**2')
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/NDict.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/NDict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
  Adapted from ScientificPython:
  Written by Konrad Hinsen <hinsen@cnrs-orleans.fr>
  with contributions from Greg Ward
  last revision: 2007-5-25
 """
 
@@ -13,64 +12,72 @@
     An instance of this class acts like an array of number with generalized
     (non-integer) indices. A value of zero is assumed for undefined
     entries. NumberDict instances support addition, and subtraction with other
     NumberDict instances, and multiplication and division by scalars.
     """
 
     def __getitem__(self, item):
+        """Return the value of the item, or 0 if it is not defined."""
         try:
             return dict.__getitem__(self, item)
         except KeyError:
             return 0
 
     def __add__(self, other):
-        sum_dict = NumberDict()
+        """Return the sum of self and other."""
+        sum_dict: NumberDict = NumberDict()
         for key in self.keys():
             sum_dict[key] = self[key]
         for key in other.keys():
             sum_dict[key] = sum_dict[key] + other[key]
         return sum_dict
     __radd__ = __add__
 
     def __sub__(self, other):
+        """Return the difference of self and other."""
         sum_dict = NumberDict()
         for key in self.keys():
             sum_dict[key] = self[key]
         for key in other.keys():
             sum_dict[key] = sum_dict[key] - other[key]
         return sum_dict
     __rsub__ = __sub__
 
     def __mul__(self, other):
+        """Return the product of self and other."""
         new = NumberDict()
         for key in self.keys():
             new[key] = other*self[key]
         return new
 
     __rmul__ = __mul__
 
     def __div__(self, other):
+        """Return the quotient of self and other."""
         new = NumberDict()
         for key in self.keys():
             new[key] = self[key]/other
         return new
 
     def __rdiv__(self, other):
+        """Return the quotient of other and self."""
         new = NumberDict()
         for key in self.keys():
             new[key] = other/self[key]
         return new
 
     __truediv__ = __div__
     __rtruediv__ = __rdiv__
 
     def __floordiv__(self, other):
+        """Return the floored quotient of self and other."""
         new = NumberDict()
         for key in self.keys():
             new[key] = self[key] // other
         return new
 
     def __rfloordiv__(self, other):
+        """Return the floored quotient of other and self."""
         new = NumberDict()
         for key in self.keys():
             new[key] = other // self[key]
         return new
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/decorator.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     -------
         wrapper function
 
     >>> @require_units('V', 'A')
     >>> def power(u, i):
     >>>     return (u*i).W
 
-    >>> @require_units(u='V', u='A')
+    >>> @require_units(u='V', i='A')
     >>> def power(u, i):
     >>>     return (u*i).W
 
     """
     @wrapt.decorator
     def wrapper(wrapped, instance, args, kwargs):
         for i, arg in enumerate(args):
@@ -90,26 +90,26 @@
 
     :param units: list of units for arguments
 
     >>> @optional_units('V','A', return_unit='W')
     >>> def powero(u, i):
     >>>     return u*i
 
-    >>> @optional_units(u='V', u='A', return_unit='W')
+    >>> @optional_units(u='V', i='A', return_unit='W')
     >>> def power(u,i):
     >>>     return (u*i).W
 
     """
     @wrapt.decorator
     def wrapper(wrapped, instance, args, kwargs):
         newargs = []
         for i, arg in enumerate(args):
             newargs.append(dropunit(arg, units[i]))
         newkwargs = {}
         for i, key in enumerate(kwargs):
             newkwargs[key] = dropunit(kwargs.get(key), kunits.get(key))
         return_value = wrapped(*newargs, **newkwargs)
         return_unit = kunits.get('return_unit','')
-        if return_unit is not '':
+        if return_unit != '':
             return_value = PhysicalQuantity(return_value, return_unit)
         return return_value
     return wrapper
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/__init__.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,97 +26,100 @@
 import collections
 import sys
 
 from .quantity import PhysicalQuantity
 from .unit import unit_table, addunit, isphysicalunit, PhysicalUnit
 from .prefixes import *
 from .default_units import *
-from PhysicalQuantities.dBQuantity import dBQuantity, dB_unit_table
-from PhysicalQuantities.quantityarray import PhysicalQuantityArray
+from .dBQuantity import dBQuantity, dB_unit_table
+from .quantityarray import PhysicalQuantityArray
 
-if sys.version_info < (3, 6):
-    sys.exit('Sorry, Python < 3.6 is not supported')
+if sys.version_info < (3, 8):
+    sys.exit('Sorry, Python < 3.8 is not supported')
 
-__version__ = '0.9.1'
+__version__ = '1.1.1'
 
 Q = PhysicalQuantity
 U = PhysicalUnit
 QA = PhysicalQuantityArray
 
 
 class _Quantity:
     """Class to provide attributes for all known units include prefixes
 
     Examples
     --------
-    >>> from PhysicalQuantities import _Quantity
-    >>> q = _Quantity()
+    >>> from PhysicalQuantities import q
     >>> q['m']
     1 m
     >>> q.m
     1 m
     >>>  type(q['m'])
     PhysicalQuantities.quantity.PhysicalQuantity
 
     Notes
     -----
-    When adding more units, the class has to be reinitialized using `__init__()`for the new units to be listed.
+    When adding more units, the class has to be reinitialized using `update()`for the new units to be listed.
     """
     def __init__(self):
         self.table = {}
+        self.update()
+
+    def update(self):
+        """ Update the table of known units"""
         for key in dB_unit_table:
             self.table[key] = dBQuantity(1, key)
         for key in unit_table:
             self.table[key] = PhysicalQuantity(1, unit_table[key])
 
     def __dir__(self):
         return self.table.keys()
 
     def __getitem__(self, key):
         try:
-            if type(key) is str:
+            if isinstance(key, str):
                 _Q = self.table[key]
             else:
                 _Q = self.table[key.name]
-        except KeyError:
-            raise KeyError(f'Unit {key} not found')
+        except KeyError as exc:
+            raise KeyError(f'Unit {key} not found') from exc
         return _Q
 
     def __getattr__(self, attr):
         try:
             _Q = self.table[attr]
-        except KeyError:
-            raise KeyError(f'Unit {attr} not found')
+        except KeyError as exc:
+            raise KeyError(f'Unit {attr} not found') from exc
         return _Q
     
     def _ipython_key_completions_(self):
         return list(self.table.keys())
 
 
 q = _Quantity()
 
 
 def isphysicalquantity(x) -> bool:
     """ Test if parameter is a PhysicalQuantity or dBQuantity object
 
     Parameters
     ----------
-    x
+    x:  PhysicalQuantity or dBQuantity
         parameter to test
 
     Returns
     -------
         True if x is a PhysicalQuantity
 
     Examples
     --------
     >>> isphysicalquantity( PhysicalQuantity(1, 'V'))
     True
     """
-    return isinstance(x, PhysicalQuantity) or isinstance(x, dBQuantity)
+    return isinstance(x, (PhysicalQuantity, dBQuantity))
 
 
 def units_html_list():
     """ List all defined units in a HTML table
 
     Returns
     -------
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/binary_units.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/binary_units.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Binary units, i.e. Bits"""
 import PhysicalQuantities
 
 from .unit import add_composite_unit
 
-add_composite_unit('Byte', 8, 'Bit', verbosename='Byte', prefixed=True, baseunit=PhysicalQuantities.q.Bit,
-                   url='https://en.wikipedia.org/wiki/Byte')
+add_composite_unit('Byte', 8, 'Bit', verbosename='Byte', prefixed=True, url='https://en.wikipedia.org/wiki/Byte')
 PhysicalQuantities.q.__init__()
 
 
 _units = {'Ki': 2 ** 10,
           'Mi': 2 ** 20,
           'Gi': 2 ** 30,
           'Ti': 2 ** 40,
@@ -17,17 +16,16 @@
           'Zi': 2 ** 70,
           'Yi': 2 ** 80,
           }
 
 for key in _units.keys():
     name = key + 'Bit'
     scale = _units[key]
-    add_composite_unit(name, scale, 'Bit', verbosename=name, prefixed=True, baseunit=PhysicalQuantities.q.Bit,
-                    url='https://en.wikipedia.org/wiki/Bit')
+    add_composite_unit(name, scale, 'Bit', verbosename=name, prefixed=True,
+                       url='https://en.wikipedia.org/wiki/Bit')
 
     name = key + 'Byte'
     scale = _units[key]
-    add_composite_unit(name, scale, 'Byte', verbosename=name, prefixed=True, baseunit=PhysicalQuantities.q.Byte,
-                    url='https://en.wikipedia.org/wiki/Byte')
-
+    add_composite_unit(name, scale, 'Byte', verbosename=name, prefixed=True,
+                       url='https://en.wikipedia.org/wiki/Byte')
 
 PhysicalQuantities.q.__init__()
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/numpywrapper.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/numpywrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,107 +4,107 @@
 from . import isphysicalquantity, q
 from .quantity import *
 from .unit import UnitError
 
 __all__ = ['floor', 'ceil', 'sqrt', 'linspace', 'tophysicalquantity']
 
 
-def max(q):
+def max(qu: np.array):
     """Return the maximum of an array or maximum along an axis.
 
     Parameters
     ----------
-    q : array_like
+    qu :
         Input data
 
     Returns
     -------
     array_like
         Maximum of an array or maximum along an axis
     """
-    if isphysicalquantity(q):
-        return q.__class__(np.max(q.value), q.unit)
+    if isphysicalquantity(qu):
+        return qu.__class__(np.max(qu.value), qu.unit)
     else:
-        return np.max(q)
+        return np.max(qu)
 
     
-def floor(q):
+def floor(qu: np.array):
     """ Return the floor of the input, element-wise.
 
     Parameters
     ----------
-    q : array_like
+    qu:
         Input data
 
     Returns
     -------
     PhysicalQuantity
         The floor of each element
 
-    Example
-    -------
+    Examples
+    --------
     >>> import PhysicalQuantities.numpywrapper as nw
     >>> nw.floor(1.3 mm)
     1 mm
     """
-    if isphysicalquantity(q):
-        return q.__class__(np.floor(q.value), q.unit)
+    if isphysicalquantity(qu):
+        return qu.__class__(np.floor(qu.value), qu.unit)
     else:
-        return np.floor(q)
+        return np.floor(qu)
 
 
-def ceil(q):
+def ceil(qu: np.array):
     """ Return the ceiling of the input, element-wise.
 
     Parameters
     ----------
-    q : array_like
+    qu:
         Input data
 
     Returns
     -------
     PhysicalQuantity
         The ceiling of each element
 
-    Example
-    -------
+    Examples
+    --------
     >>> import PhysicalQuantities.numpywrapper as nw
     >>> nw.ceil(1.3 mm)
     2.0 mm
     """
-    if isphysicalquantity(q):
-        return q.__class__(np.ceil(q.value), q.unit)
+    if isphysicalquantity(qu):
+        return qu.__class__(np.ceil(qu.value), qu.unit)
     else:
-        return np.ceil(q)
+        return np.ceil(qu)
 
 
-def sqrt(q):
+def sqrt(qu: np.array):
     """ Return the square root of the input, element-wise.
 
     Parameters
     ----------
-    q : array_like
+    qu:
         Input data
 
     Returns
     -------
     PhysicalQuantity
         The floor of each element
 
-    Example
-    -------
+    Examples
+    --------
     >>> import PhysicalQuantities.numpywrapper as nw
     >>> nw.sqrt(4 m**2)
     2.0 m
     """
-    if isphysicalquantity(q):
-        value = np.sqrt(q.value)
-        return q.__class__(value, q.unit**0.5)
+    if isphysicalquantity(qu):
+        value = np.sqrt(qu.value)
+        return qu.__class__(value, qu.unit ** 0.5)
     else:
-        return np.sqrt(q)
+        return np.sqrt(qu)
 
 
 def linspace(start, stop, num=50,  endpoint=True, retstep=False):
     """ A units-enabled linspace
 
     Parameters
     ----------
@@ -119,16 +119,16 @@
     retstep: bool
         If true, return (samples, step)
 
     Returns
     -------
         Return equally spaced samples between start and stop
 
-    Example
-    -------
+    Examples
+    --------
     >>> import PhysicalQuantities.numpywrapper as nw
     >>> nw.linspace(0 GHz, 100 GHz, 200)
     """
     if not isinstance(start, PhysicalQuantity) and not isinstance(stop, PhysicalQuantity):
         return np.linspace(start, stop, num,  endpoint, retstep)
 
     if isinstance(start, PhysicalQuantity) and isinstance(stop, PhysicalQuantity):
@@ -156,23 +156,25 @@
 
 
 def tophysicalquantity(arr, unit=None):
     """ Convert numpy array or list containing PhysicalQuantity elements to PhysicalQuantity object containing array or list
 
     Parameters
     -----------
-    arr: array_like
+    arr: list or numpy array
+
+    unit: unit name or unit object
 
     Returns
     -------
     PhysicalQuantity
         Array wrapped as PhysicalQuantity
 
-    Example
-    -------
+    Examples
+    --------
     >>> a = [ 1mm, 2m, 3mm]
     >>> b = toPhysicalQuantity(a)
     >>> b
     [ 1 2000 3] mm
     """
     if isphysicalquantity(arr):
         if type(arr.value) is np.ndarray:
@@ -239,14 +241,15 @@
     """
     
     if isphysicalquantity(array):
         return np.argsort(array.value)
     else:
         return np.argsort(array)
 
+
 def insert(array, obj, values):
     """Insert values along the given axis before the given indices.
     Parameters:	
     -----------
     arr : array_like
         Input array.
```

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/imperial.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/imperial.py`

 * *Files identical despite different names*

### Comparing `PhysicalQuantities-0.9.1/PhysicalQuantities/unit.py` & `PhysicalQuantities-1.1.1/PhysicalQuantities/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,24 @@
 """ PhysicalUnit class definition
 
 Original author: Georg Brandl <georg@python.org>, https://bitbucket.org/birkenfeld/ipython-physics
 """
-
 import copy
 import json
-from functools import reduce
+from functools import reduce, lru_cache
 
 import numpy as np
 
 from .NDict import *
 
 
 class UnitError(ValueError):
     pass
 
 
-# Helper functions
-def findunit(unitname):
-    """ Return PhysicalUnit class if given parameter is a valid unit
-
-    Parameters
-    ----------
-    unitname: str or PhysicalUnit
-        Unit to check if valid
-
-    Returns
-    -------
-    PhysicalUnit
-        Unit
-
-    Examples
-    --------
-    >>> findunit('mm')
-     <PhysicalUnit mm>
-    """
-    if isinstance(unitname, str):
-        if unitname == '':
-            raise UnitError('Empty unit name is not valid')
-        name = str(unitname).strip().replace('^', '**')
-        if name[0:2] == '1/':
-            name = '(' + name[2:] + ')**-1'
-        try:
-            unit = eval(name, unit_table)
-        except NameError:
-            raise UnitError('Invalid or unknown unit %s' % name)
-        for cruft in ['__builtins__', '__args__']:
-            try:
-                del unit_table[cruft]
-            except KeyError:
-                pass
-    else:
-        unit = unitname
-    if not isphysicalunit(unit):
-        raise UnitError(f'{str(unit)} is not a unit')
-    return unit
-
-
-def convertvalue(value, src_unit, target_unit):
-    """ Convert between units, if possible
-
-    Parameters
-    ----------
-    value:
-        Value in source units
-    src_unit: PhysicalUnit
-        Source unit
-    target_unit: PhysicalUnit
-        Target unit
-
-    Returns
-    -------
-    any
-        Value scaled to target unit
-
-    Examples
-    --------
-    >>> from PhysicalQuantities import q
-    >>> convertvalue(1, q.mm.unit, q.km.unit)
-    1e-06
-    """
-    (factor, offset) = src_unit.conversion_tuple_to(target_unit)
-    if isinstance(value, list):
-        raise UnitError('Cannot convert units for a list')
-    return (value + offset) * factor
-
-
-def isphysicalunit(x):
-    """ Return true if valid PhysicalUnit class
-
-    Parameters
-    ----------
-    x: PhysicalUnit
-        Unit
-    """
-    return isinstance(x, PhysicalUnit)
-
-
 class PhysicalUnit:
     """Physical unit.
 
     A physical unit is defined by a name (possibly composite), a scaling factor, and the exponentials of each of
     the SI base units that enter into it. Units can be multiplied, divided, and raised to integer powers.
 
     Attributes
@@ -121,40 +39,41 @@
         An additive offset to the unit (used only for temperatures)
     url: str
         URL describing the unit
     verbosename: str
         The verbose name of the unit (e.g. Coulomb)
     unece_code: str
         Official unit code
-        (see http://www.unece.org/fileadmin/DAM/cefact/recommendations/rec20/rec20_Rev9e_2014.xls)
+        (see https://www.unece.org/fileadmin/DAM/cefact/recommendations/rec20/rec20_Rev9e_2014.xls)
 
     """
 
-    def __init__(self, names, factor, powers, offset=0, url=None, verbosename=None, unece_code=None):
+    def __init__(self, names, factor: float, powers: list, offset: float = 0, url: str = None, verbosename: str = None,
+                 unece_code: str = None):
         """ Initialize object
 
         Parameters
         ----------
         names: NumberDict|str
             A dictionary mapping each name component to its associated integer power (e.g. C{{'m': 1, 's': -1}})
             for M{m/s}). As a shorthand, a string may be passed which is assigned an implicit power 1.
-        factor: float
+        factor:
             A scaling factor from base units
-        powers: list
+        powers:
             The integer powers for each of the nine base units:
             ['m', 'kg', 's', 'A', 'K', 'mol', 'cd', 'rad', 'sr']
-        offset: float
+        offset:
             An additive offset to the unit (used only for temperatures)
-        url: str
+        url:
             URL describing the unit
-        verbosename: str
+        verbosename:
             The verbose name of the unit (e.g. Coulomb)
-        unece_code: str
+        unece_code:
             Official unit code
-            (see http://www.unece.org/fileadmin/DAM/cefact/recommendations/rec20/rec20_Rev9e_2014.xls)
+            (see https://www.unece.org/fileadmin/DAM/cefact/recommendations/rec20/rec20_Rev9e_2014.xls)
 
         """
         self.prefixed = False
         self.baseunit = self
         self.verbosename = verbosename
         self.url = url
         if isinstance(names, str):
@@ -221,34 +140,34 @@
 
         """
         num = ''
         denom = ''
         for unit in self.names.keys():
             power = self.names[unit]
             if power < 0:
-                if denom is '':
+                if denom == '':
                     denom = '\\text{' + unit + '}'
                 else:
                     denom = denom + '\\cdot \\text{' + unit + '}'
                 if power < -1:
                     denom = denom + '^' + str(-power)
             elif power > 0:
-                if num is '':
+                if num == '':
                     num = '\\text{' + unit + '}'
                 else:
                     num = num + '\\cdot \\text{' + unit + '}'
                 if power > 1:
                     num = num + '^{' + str(power) + '}'
-        if num is '':
+        if num == '':
             num = '1'
-        if denom is not '':
+        if denom != '':
             name = '\\frac{' + num + '}{' + denom + '}'
         else:
             name = num
-        name = name.replace('u', u'µ').replace('\\text{deg}', '\\,^{\\circ}').replace(' pi', ' \\pi ')
+        name = name.replace('\\text{deg}', '\\,^{\\circ}').replace(' pi', ' \\pi ')
         return name
 
     @property
     def is_power(self):
         """ Test if unit is a power unit. Used of dB conversion
         TODO: basically very dumb right now
 
@@ -454,17 +373,18 @@
         if self.offset != 0 or (isphysicalunit(other) and other.offset != 0):
             raise UnitError(f'Cannot multiply units {self} and {other} with non-zero offset')
         if isphysicalunit(other):
             return PhysicalUnit(self.names + other.names,
                                 self.factor * other.factor,
                                 list(map(lambda a, b: a + b, self.powers, other.powers)))
         elif isinstance(other, PhysicalQuantity):
-        # TODO: add test
+            other = other.unit
+            newpowers = [a + b for a, b in zip(other.powers, self.powers)]
             return PhysicalUnit(self.names + NumberDict({str(other): 1}),
-                                self.factor * other.factor, self.powers, self.offset)
+                                self.factor * other.factor, newpowers, self.offset)
         else:
             return PhysicalQuantity(other, self)
 
     __rmul__ = __mul__
 
     def __div__(self, other):
         """ Divide two units
@@ -481,22 +401,27 @@
 
         Examples
         --------
         >>> from PhysicalQuantities import q
         >>> q.m.unit / q.s.unit
         m/s
         """
+        from .quantity import PhysicalQuantity
         if self.offset != 0 or (isphysicalunit(other) and other.offset != 0):
             raise UnitError(f'Cannot divide units {self} and {other} with non-zero offset')
         if isphysicalunit(other):
             return PhysicalUnit(self.names - other.names,
                                 self.factor / other.factor,
                                 list(map(lambda a, b: a - b, self.powers, other.powers)))
+        elif isinstance(other, PhysicalQuantity):
+            other = other.unit
+            newpowers = [a - b for a, b in zip(other.powers, self.powers)]
+            return PhysicalUnit(self.names + NumberDict({str(other): 1}),
+                                self.factor / other.factor, newpowers)
         else:
-            # TODO: add test
             return PhysicalUnit(self.names + NumberDict({str(other): -1}),
                                 self.factor/other.factor, self.powers)
 
     def __rdiv__(self, other):
         if self.offset != 0 or (isphysicalunit(other) and other.offset != 0):
             raise UnitError('Cannot divide units %s and %s with non-zero offset' % (self, other))
         if isphysicalunit(other):
@@ -587,14 +512,18 @@
                         for i in range(len(p)):
                             names[base_names[i]] = p[i]
                     return PhysicalUnit(names, f, p)
                 else:
                     raise UnitError('Illegal exponent %f' % exponent)
         raise UnitError('Only integer and inverse integer exponents allowed')
 
+    def __hash__(self):
+        """Custom hash function"""
+        return hash((self.factor, self.offset, str(self.powers)))
+
     def conversion_factor_to(self, other):
         """Return conversion factor to another unit
 
         Parameters
         ----------
         other: PhysicalUnit
             Unit to compute conversion factor for
@@ -677,15 +606,15 @@
                      'verbosename': self.verbosename,
                      'offset': self.offset,
                      'factor': self.factor
                      }
         b = self.baseunit
         p = b.powers
         base_dict = {}
-        for i,exponent in enumerate(p):
+        for i, exponent in enumerate(p):
             base_dict[base_names[i]] = exponent
         unit_dict['base_exponents'] = base_dict
         return unit_dict
 
     @property
     def to_json(self):
         """Export unit as JSON
@@ -789,22 +718,21 @@
         url='https://en.wikipedia.org/wiki/Radian', verbosename='Radian',
         unece_code='C81'))
 addunit(PhysicalUnit('sr', 1., [0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0],
         url='https://en.wikipedia.org/wiki/Steradian', verbosename='Steradian',
         unece_code='D27'))
 addunit(PhysicalUnit('Bit', 1, [0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0],
         url='https://en.wikipedia.org/wiki/Bit', verbosename='Bit',
-        unece_code=None))
+        unece_code=''))
 addunit(PhysicalUnit('currency', 1., [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
         url='https://en.wikipedia.org/wiki/Currency', verbosename='Currency',
-        unece_code=None))
+        unece_code=''))
 
 
-
-def add_composite_unit(name, factor, units, offset=0, verbosename='', prefixed=False, baseunit=None, url=''):
+def add_composite_unit(name, factor, units, offset=0, verbosename='', prefixed=False, url=''):
     """ Add new unit to the unit_table
 
     Parameters
     -----------
     name: str
         Name of the unit
     factor: float
@@ -813,44 +741,137 @@
         Composed units of new unit
     offset: float
         Offset factor
     verbosename: str
         A more verbose name for the unit
     prefixed: bool
         This is a prefixed unit
-    baseunit : PhysicalUnit
-        Base unit
     url: str
         A URL linking to more information about the unit
 
     Returns
     -------
     str
         Name of new unit
 
     Raises
     ------
     KeyError
-        If unit already exists
-
+        If unit already exists or if units string is invalid
+    ValueError
+        If factor or offset is not numeric
     """
     if name in unit_table:
         raise KeyError(f'Unit {name} already defined')
-    baseunit = eval(units, unit_table)
-    for cruft in ['__builtins__', '__args__']:
-        try:
-            del unit_table[cruft]
-        except KeyError:
-            pass
+    # Parse composed units string
+    try:
+        baseunit = eval(units, unit_table)
+    except (SyntaxError, ValueError):
+        raise KeyError(f'Invalid units string: {units}')
+
+    # Validate factor and offset values
+    for value in (factor, offset):
+        if not isinstance(value, (int, float)):
+            raise ValueError('Factor and offset values should be numeric')
+
+    # Remove unwanted keys from unit_table
+    for key in ['__builtins__', '__args__']:
+        unit_table.pop(key, None)
+
     newunit = copy.deepcopy(baseunit)
     newunit.set_name(name)
     newunit.verbosename = verbosename
-    if prefixed is True:
-        newunit.baseunit = baseunit
-    else:
-        newunit.baseunit = newunit
+    newunit.baseunit = baseunit if prefixed else newunit
     newunit.prefixed = prefixed
     newunit.url = url
-    newunit.factor = newunit.factor * factor
-    newunit.offset = newunit.offset + offset
+    newunit.factor *= factor
+    newunit.offset += offset
     unit_table[name] = newunit
+
     return name
+
+
+# Helper functions
+@lru_cache(maxsize=None)
+def findunit(unitname):
+    """ Return PhysicalUnit class if given parameter is a valid unit
+
+    Parameters
+    ----------
+    unitname: str or PhysicalUnit
+        Unit to check if valid
+
+    Returns
+    -------
+    PhysicalUnit
+        Unit
+
+    Raises
+    ------
+    UnitError
+        If the input is invalid.
+
+    Examples
+    --------
+    >>> findunit('mm')
+     <PhysicalUnit mm>
+    """
+    if isinstance(unitname, str):
+        if unitname == '':
+            raise UnitError('Empty unit name is not valid')
+        name = unitname.strip().replace('^', '**')
+        if name.startswith('1/'):
+            name = '(' + name[2:] + ')**-1'
+        try:
+            unit = eval(name, unit_table)
+        except NameError:
+            raise UnitError('Invalid or unknown unit %s' % name)
+        for cruft in ['__builtins__', '__args__']:
+            try:
+                del unit_table[cruft]
+            except KeyError:
+                pass
+    else:
+        unit = unitname
+    if not isphysicalunit(unit):
+        raise UnitError(f'{str(unit)} is not a unit')
+    return unit
+
+
+def convertvalue(value, src_unit, target_unit):
+    """ Convert between units, if possible
+
+    Parameters
+    ----------
+    value:
+        Value in source units
+    src_unit: PhysicalUnit
+        Source unit
+    target_unit: PhysicalUnit
+        Target unit
+
+    Returns
+    -------
+    any
+        Value scaled to target unit
+
+    Examples
+    --------
+    >>> from PhysicalQuantities import q
+    >>> convertvalue(1, q.mm.unit, q.km.unit)
+    1e-06
+    """
+    (factor, offset) = src_unit.conversion_tuple_to(target_unit)
+    if isinstance(value, list):
+        raise UnitError('Cannot convert units for a list')
+    return (value + offset) * factor
+
+
+def isphysicalunit(x):
+    """ Return true if valid PhysicalUnit class
+
+    Parameters
+    ----------
+    x: PhysicalUnit
+        Unit
+    """
+    return isinstance(x, PhysicalUnit)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PhysicalQuantities-0.9.1/setup.py` & `PhysicalQuantities-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
     name="PhysicalQuantities",
-    version="0.9.1",
+    version="1.1.1",
     author="Juergen Hasch",
     author_email="juergen.hasch@elbonia.de",
     description="Allow calculations using physical quantities",
     license="BSD",
     keywords="Physical Quantities IPython",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     url="https://github.com/juhasch/PhysicalQuantities",
     packages=find_packages(),
     install_requires=['numpy', 'IPython', 'wrapt'],
     long_description_content_type='text/markdown',
     long_description="""
 *PhysicalQuantities* is a Python module that allows calculations to be aware of physical units. Built-in unit
 conversion ensures that calculations will result in the correct unit.
```

