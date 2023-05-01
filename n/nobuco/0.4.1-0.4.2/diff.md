# Comparing `tmp/nobuco-0.4.1.tar.gz` & `tmp/nobuco-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.1.tar", last modified: Tue Apr 25 18:16:07 2023, max compression
+gzip compressed data, was "nobuco-0.4.2.tar", last modified: Mon May  1 12:44:11 2023, max compression
```

## Comparing `nobuco-0.4.1.tar` & `nobuco-0.4.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-04-25 18:16:07.396770 nobuco-0.4.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20054 2023-04-25 18:07:04.000000 nobuco-0.4.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.1/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.396770 nobuco-0.4.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-25 18:16:07.392770 nobuco-0.4.1/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-25 18:16:07.000000 nobuco-0.4.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-25 18:15:04.000000 nobuco-0.4.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-25 18:16:07.396770 nobuco-0.4.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.525436 nobuco-0.4.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-05-01 12:44:11.525436 nobuco-0.4.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20054 2023-04-25 18:07:04.000000 nobuco-0.4.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.2/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14889 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.525436 nobuco-0.4.2/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.2/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10645 2023-05-01 12:37:49.000000 nobuco-0.4.2/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10637 2023-05-01 11:14:44.000000 nobuco-0.4.2/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.525436 nobuco-0.4.2/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.525436 nobuco-0.4.2/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.2/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-01 12:44:11.521436 nobuco-0.4.2/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21888 2023-05-01 12:44:11.000000 nobuco-0.4.2/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-01 12:44:11.000000 nobuco-0.4.2/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-01 12:44:11.000000 nobuco-0.4.2/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-01 12:44:11.000000 nobuco-0.4.2/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-01 12:44:11.000000 nobuco-0.4.2/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-01 12:37:49.000000 nobuco-0.4.2/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-01 12:44:11.525436 nobuco-0.4.2/setup.cfg
```

### Comparing `nobuco-0.4.1/LICENSE` & `nobuco-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/PKG-INFO` & `nobuco-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.1/README.md` & `nobuco-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/__init__.py` & `nobuco-0.4.2/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/commons.py` & `nobuco-0.4.2/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/convert.py` & `nobuco-0.4.2/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/converters/channel_ordering.py` & `nobuco-0.4.2/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/converters/node_converter.py` & `nobuco-0.4.2/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/converters/tensor.py` & `nobuco-0.4.2/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/converters/type_cast.py` & `nobuco-0.4.2/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/converters/validation.py` & `nobuco-0.4.2/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/entity/keras.py` & `nobuco-0.4.2/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/entity/pytorch.py` & `nobuco-0.4.2/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/funcs.py` & `nobuco-0.4.2/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/layers/channel_order.py` & `nobuco-0.4.2/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/layers/container.py` & `nobuco-0.4.2/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/layers/weight.py` & `nobuco-0.4.2/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/locate/link.py` & `nobuco-0.4.2/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/locate/locate.py` & `nobuco-0.4.2/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/activation.py` & `nobuco-0.4.2/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/boolean.py` & `nobuco-0.4.2/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.2/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/comparison.py` & `nobuco-0.4.2/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/convolution.py` & `nobuco-0.4.2/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/dropout.py` & `nobuco-0.4.2/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/interpolation.py` & `nobuco-0.4.2/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/linear.py` & `nobuco-0.4.2/nobuco/node_converters/linear.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from numbers import Number
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
 from nobuco.converters.tensor import dim_pytorch2keras
-
 from nobuco.converters.channel_ordering import get_channel_order
 from torch import Tensor
 
 import tensorflow as tf
 from tensorflow import keras
 import torch
 import torch.nn.functional as F
 from torch import nn
 
+import numpy as np
+
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.node_converter import converter
 
 
 @converter(nn.Linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_Linear(self, input: Tensor):
     out_filters, in_filters = self.weight.shape
@@ -26,30 +28,31 @@
         biases = self.bias.detach().numpy()
         params = [weights, biases]
     else:
         params = [weights]
     return keras.layers.Dense(out_filters, weights=params)
 
 
-# @converter(torch.nn.functional.linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
-# def converter_linear(input, weight, bias, out=None):
-#     out_filters, in_filters = weight.shape
-#     weights = weight.detach().numpy()
-#     weights = weights.transpose(1, 0)
-#
-#     if bias is not None:
-#         biases = bias.detach().numpy()
-#     else:
-#         biases = np.zeros(shape=(out_filters,))
-#
-#     layer = keras.layers.Dense(out_filters, weights=[weights, biases])
-#
-#     def func(input, weight, bias, out=None):
-#         return layer(input)
-#     return func
+@converter(torch.nn.functional.linear, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_linear(input, weight, bias, out=None):
+    out_filters, in_filters = weight.shape
+    weights = weight.detach().numpy()
+    weights = weights.transpose(1, 0)
+
+    if bias is not None:
+        biases = bias.detach().numpy()
+        params = [weights, biases]
+    else:
+        params = [weights]
+
+    layer = keras.layers.Dense(out_filters, weights=params)
+
+    def func(input, weight, bias, out=None):
+        return layer(input)
+    return func
 
 
 @converter(torch.matmul, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_matmul(input: Tensor, other: Tensor, *, out: Optional[Tensor]=None):
     def func(input, other, *, out=None):
         return tf.linalg.matmul(input, other)
     return func
@@ -79,14 +82,21 @@
 @converter(torch.bmm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_bmm(input: Tensor, mat2: Tensor, *, out: Optional[Tensor]=None):
     def func(input, mat2, *, out=None):
         return tf.linalg.matmul(input, mat2)
     return func
 
 
+@converter(torch.baddbmm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_baddbmm(input: Tensor, batch1: Tensor, batch2: Tensor, *, beta: Number=1, alpha: Number=1, out: Optional[Tensor]=None):
+    def func(input: Tensor, batch1, batch2, *, beta=1, alpha=1, out=None):
+        return beta*input + alpha*tf.linalg.matmul(batch1, batch2)
+    return func
+
+
 @converter(torch.einsum, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_einsum(*args: Any):
     def func(*args: Any):
         equation = args[0]
         operands = args[1:]
         return keras.layers.Lambda(lambda operands: tf.einsum(equation, *operands))(operands)
     return func
```

### Comparing `nobuco-0.4.1/nobuco/node_converters/math.py` & `nobuco-0.4.2/nobuco/node_converters/math.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,64 @@
-import numbers
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
 from torch import Tensor
 from torch.types import _int, _bool, Number, _dtype, _size
 
 import tensorflow as tf
 import torch
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
-from nobuco.converters.tensor import _dim_make_positive, dim_pytorch2keras
+from nobuco.converters.tensor import _dim_make_positive, dim_pytorch2keras, perm_keras2pytorch, _permute
 
 
-@converter(torch.sum, torch.Tensor.sum, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@converter(torch.sum, torch.Tensor.sum, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_sum(input: Tensor, dim: Sequence, keepdim: _bool=False, *, dtype: Optional[_dtype]=None, out: Optional[Tensor]=None):
     n_dims = input.dim()
 
     def func(input, dim, keepdim=False, *, dtype=None, out=None):
-        dim = _dim_make_positive(dim, n_dims)
-        if get_channel_order(input) == ChannelOrder.TENSORFLOW:
-            dim = dim_pytorch2keras(dim, n_dims)
-        return tf.reduce_sum(input, axis=dim, keepdims=keepdim)
+        order = get_channel_order(input)
+
+        if not keepdim and order == ChannelOrder.TENSORFLOW:
+            perm = perm_keras2pytorch(n_dims)
+            input = _permute(perm)(input)
+            out = tf.reduce_sum(input, axis=dim, keepdims=keepdim)
+            out = set_channel_order(out, ChannelOrder.PYTORCH)
+            return out
+        else:
+            dim = _dim_make_positive(dim, n_dims)
+            if order == ChannelOrder.TENSORFLOW:
+                dim = dim_pytorch2keras(dim, n_dims)
+            out = tf.reduce_sum(input, axis=dim, keepdims=keepdim)
+            out = set_channel_order(out, order)
+            return out
     return func
 
 
 @converter(torch.mean, torch.Tensor.mean, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_mean(input: Tensor, dim=None, keepdim: _bool = False, *, dtype: Optional[_dtype] = None, out: Optional[Tensor] = None):
     n_dims = input.dim()
 
-    def func(input, dim=None, keepdim=False, *, dtype=None, out=None):
-        if dim is not None:
+    def func(input, dim, keepdim=False, *, dtype=None, out=None):
+        order = get_channel_order(input)
+
+        if not keepdim and order == ChannelOrder.TENSORFLOW:
+            perm = perm_keras2pytorch(n_dims)
+            input = _permute(perm)(input)
+            out = tf.reduce_mean(input, axis=dim, keepdims=keepdim)
+            out = set_channel_order(out, ChannelOrder.PYTORCH)
+            return out
+        else:
             dim = _dim_make_positive(dim, n_dims)
-            if get_channel_order(input) == ChannelOrder.TENSORFLOW:
+            if order == ChannelOrder.TENSORFLOW:
                 dim = dim_pytorch2keras(dim, n_dims)
-        return tf.reduce_mean(input, axis=dim, keepdims=keepdim)
+            out = tf.reduce_mean(input, axis=dim, keepdims=keepdim)
+            out = set_channel_order(out, order)
+            return out
     return func
 
 
 @converter(torch.Tensor.add, torch.Tensor.__add__, torch.Tensor.__iadd__, torch.Tensor.__radd__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS_OR_PYTORCH, autocast=True)
 def converter_add(input, other, *args, **kwargs):
     def func(input, other, *args, **kwargs):
         return input + other
```

### Comparing `nobuco-0.4.1/nobuco/node_converters/misc.py` & `nobuco-0.4.2/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/normalization.py` & `nobuco-0.4.2/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/padding.py` & `nobuco-0.4.2/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/pooling.py` & `nobuco-0.4.2/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/recurrent.py` & `nobuco-0.4.2/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/slice.py` & `nobuco-0.4.2/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.2/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.2/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.2/nobuco/node_converters/tensor_manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,25 @@
     def func(self, split_size, dim=0):
         if get_channel_order(self) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, num_dims)
         return tf.split(self, num_or_size_splits=split_size, axis=dim)
     return func
 
 
+@converter(torch.Tensor.chunk, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_chunk(self, chunks, dim=0):
+    num_dims = self.dim()
+
+    def func(self, chunks, dim=0):
+        if get_channel_order(self) == ChannelOrder.TENSORFLOW:
+            dim = dim_pytorch2keras(dim, num_dims)
+        return tf.split(self, num_or_size_splits=chunks, axis=dim)
+    return func
+
+
 @converter(torch.Tensor.repeat, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_repeat(self, *sizes):
     def func(self, *sizes):
         if get_channel_order(self) == ChannelOrder.TENSORFLOW:
             sizes = permute_pytorch2keras(sizes)
         return tf.tile(self, sizes)
     return func
```

### Comparing `nobuco-0.4.1/nobuco/trace/tensor_storage.py` & `nobuco-0.4.2/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/trace/trace.py` & `nobuco-0.4.2/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/util.py` & `nobuco-0.4.2/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/vis/console_stylizer.py` & `nobuco-0.4.2/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco/vis/html_stylizer.py` & `nobuco-0.4.2/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.2/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.2/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.1/pyproject.toml` & `nobuco-0.4.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.1"
+version = "0.4.2"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

