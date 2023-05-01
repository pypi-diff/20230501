# Comparing `tmp/sklearn2pmml-0.92.0.tar.gz` & `tmp/sklearn2pmml-0.92.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.92.0.tar", last modified: Sun Apr  2 05:09:24 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.92.1.tar", last modified: Mon May  1 06:30:20 2023, max compression
```

## Comparing `sklearn2pmml-0.92.0.tar` & `sklearn2pmml-0.92.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-03-03 19:54:54.000000 sklearn2pmml-0.92.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2022-11-15 10:41:18.000000 sklearn2pmml-0.92.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2022-12-20 20:55:09.000000 sklearn2pmml-0.92.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      743 2022-12-07 19:44:40.000000 sklearn2pmml-0.92.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    10200 2022-12-07 19:44:40.000000 sklearn2pmml-0.92.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16904 2023-01-03 17:06:18.000000 sklearn2pmml-0.92.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2022-12-11 13:16:56.000000 sklearn2pmml-0.92.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2022-12-07 19:44:36.000000 sklearn2pmml-0.92.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7438 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-01-30 14:56:55.000000 sklearn2pmml-0.92.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2021-01-09 09:21:36.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9179 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     3237 2023-03-15 18:26:47.000000 sklearn2pmml-0.92.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2022-04-01 09:50:44.000000 sklearn2pmml-0.92.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1628 2022-12-11 13:56:03.000000 sklearn2pmml-0.92.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5098 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2020-07-25 07:02:00.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   432828 2023-03-12 10:28:00.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    84321 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pickle-1.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    27449 2023-03-28 18:11:11.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   466289 2023-04-01 19:15:11.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-python-1.1.14.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46362 2022-08-31 13:41:52.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-h2o-1.2.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-04-02 05:06:15.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5702 2023-04-02 05:06:16.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68186 2022-08-31 09:48:33.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-03-12 10:28:00.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-logger-3.40.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.92.0/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-04-02 05:05:45.000000 sklearn2pmml-0.92.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2022-04-15 15:03:20.000000 sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16198 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1720 2021-03-06 17:44:51.000000 sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1856 2021-03-06 17:44:51.000000 sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2022-12-19 19:21:40.000000 sklearn2pmml-0.92.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2022-06-06 08:17:18.000000 sklearn2pmml-0.92.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-04-02 05:09:24.000000 sklearn2pmml-0.92.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-03-03 19:54:54.000000 sklearn2pmml-0.92.1/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2022-11-15 10:41:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2022-12-20 20:55:09.000000 sklearn2pmml-0.92.1/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-04-30 07:17:22.000000 sklearn2pmml-0.92.1/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16904 2023-01-03 17:06:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2022-12-11 13:16:56.000000 sklearn2pmml-0.92.1/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2022-12-07 19:44:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-04-29 08:24:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-01-30 14:56:55.000000 sklearn2pmml-0.92.1/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2021-01-09 09:21:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9179 2023-02-25 19:29:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     3237 2023-03-15 18:26:47.000000 sklearn2pmml-0.92.1/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2022-04-01 09:50:44.000000 sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1628 2022-12-11 13:56:03.000000 sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5098 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2020-07-25 07:02:00.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    84321 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54279 2022-06-05 15:53:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pickle-1.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7312 2023-04-01 19:15:12.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    27449 2023-03-28 18:11:11.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   466289 2023-04-01 19:15:11.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198275 2023-03-11 19:58:17.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-python-1.1.14.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    46362 2022-08-31 13:41:52.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-h2o-1.2.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-05-01 06:28:14.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-05-01 06:28:15.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68186 2022-08-31 09:48:33.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.92.1/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-05-01 06:28:05.000000 sklearn2pmml-0.92.1/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2022-04-15 15:03:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16202 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-04-30 08:35:42.000000 sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2022-12-19 19:21:40.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2022-06-06 08:17:18.000000 sklearn2pmml-0.92.1/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-05-01 06:30:20.000000 sklearn2pmml-0.92.1/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-03-03 19:54:59.000000 sklearn2pmml-0.92.1/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.92.0/LICENSE.txt` & `sklearn2pmml-0.92.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/setup.py` & `sklearn2pmml-0.92.1/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/PKG-INFO` & `sklearn2pmml-0.92.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.92.0
+Version: 0.92.1
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.92.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.92.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.92.1/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.92.1/sklearn2pmml/tpot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sklearn2pmml import _supported_classes, _strip_module
+from sklearn2pmml import _strip_module, load_class_mapping
 
 def make_pmml_config(config, user_classpath = []):
 	"""Translates a regular TPOT configuration to a PMML-compatible TPOT configuration.
 
 	Parameters:
 	----------
 	obj: config
@@ -10,10 +10,11 @@
 
 	user_classpath: list of strings, optional
 		The paths to JAR files that provide custom Transformer, Selector and/or Estimator converter classes.
 		The SkLearn2PMML classpath is constructed by appending user JAR files to package JAR files.
 
 	"""
 	keys = set(config.keys())
-	classes = _supported_classes(user_classpath)
+	mapping = load_class_mapping(user_classpath)
+	classes = mapping.keys()
 	pmml_keys = (set(classes)).union(set([_strip_module(class_) for class_ in classes]))
 	return { key : config[key] for key in (keys).intersection(pmml_keys)}
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -298,19 +298,77 @@
 		line = line.decode("UTF-8").rstrip()
 		if line.startswith("#"):
 			continue
 		key, value = splitter.split(line)
 		properties[key] = value
 	return properties
 
-def _supported_classes(user_classpath):
-	classes = []
-	parser = lambda x: classes.extend(_parse_properties(x.readlines()).keys())
-	_process_classpath("META-INF/sklearn2pmml.properties", parser, user_classpath)
-	return classes
+def _format_properties(properties):
+	return ["{0} = {1}\n".format(k, v) for k, v in properties.items()]
+
+def _expand_complex_key(key):
+	begin = key.find("(")
+	end = key.find(")", begin + 1)
+	if begin < 0 or end < 0:
+		return [key]
+
+	prefix = key[:begin]
+	body = key[begin + 1:end]
+	suffix = key[end + 1:]
+
+	result = []
+	parts = body.split("|")
+	for part in parts:
+		result += _expand_complex_key(prefix + part + suffix)
+	return result
+
+def _expand_mapping(mapping):
+	result = dict()
+	for k, v in mapping.items():
+		pythonClazzes = _expand_complex_key(k)
+		javaClazz = v
+		for pythonClazz in pythonClazzes:
+			result[pythonClazz] = (javaClazz if javaClazz else pythonClazz)
+	return result
+
+def load_class_mapping(user_classpath = []):
+	"""Loads the class mapping.
+
+	Parameters:
+	----------
+	user_classpath: list of strings, optional
+		The paths to JAR files that provide custom Transformer, Selector and/or Estimator converter classes.
+
+	Returns:
+	-------
+	mapping: dict
+		Mapping from Python class names to Java converter class names.
+
+	"""
+	mapping = dict()
+	processor = lambda x: mapping.update(_expand_mapping(_parse_properties(x.readlines())))
+	_process_classpath("META-INF/sklearn2pmml.properties", processor, user_classpath)
+	return mapping
+
+def make_class_mapping_jar(path, mapping):
+	"""Generates a class mapping JAR file.
+
+	Parameters:
+	----------
+	path: string
+		The path to output JAR file.
+
+	mapping: dict of strings
+		Mapping from Python class names to Java converter class names.
+
+	"""
+	lines = _format_properties(mapping)
+
+	with ZipFile(path, mode = "w") as zipfile:
+		zipfile.writestr("META-INF/sklearn2pmml.properties", "".join(lines))
 
 def _strip_module(name):
 	parts = name.split(".")
 	if len(parts) > 1:
 		parts.pop(-2)
 		return ".".join(parts)
 	return name
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.92.1/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 	return Xt
 
 def eval_expr_rows(X, expr, dtype = object):
 	func = to_expr_func(expr)
 	return eval_rows(X, func, dtype = dtype)
 
 def fqn(obj):
-	clazz = obj.__class__
+	clazz = obj if inspect.isclass(obj) else obj.__class__
 	return ".".join([clazz.__module__, clazz.__name__])
 
 def is_instance_attr(obj, name):
 	if not hasattr(obj, name):
 		return False
 	if name.startswith("__") and name.endswith("__"):
 		return False
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.92.1/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.92.1/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.2.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,361 +1,361 @@
-Zip file size: 432828 bytes, number of entries: 359
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-09 15:17 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/
--rw-r--r--  2.0 unx     1699 b- defN 23-Mar-09 15:17 hex/ModelCategory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/
--rw-r--r--  2.0 unx      731 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/ModelDescriptor.class
--rw-r--r--  2.0 unx     3832 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
--rw-r--r--  2.0 unx      262 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
--rw-r--r--  2.0 unx     1415 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/ModelDescriptorBuilder.class
--rw-r--r--  2.0 unx     4531 b- defN 23-Mar-09 15:17 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
--rw-r--r--  2.0 unx     1088 b- defN 23-Mar-09 15:17 hex/genmodel/ModelMojoReader$RawValue.class
--rw-r--r--  2.0 unx     5067 b- defN 23-Mar-09 15:17 hex/genmodel/MojoReaderBackendFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/easy/
--rw-r--r--  2.0 unx     2069 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1698 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumEncoder.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EigenEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/
--rw-r--r--  2.0 unx      549 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
--rw-r--r--  2.0 unx      365 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/AbstractPrediction.class
--rw-r--r--  2.0 unx     1159 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
--rw-r--r--  2.0 unx      476 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
--rw-r--r--  2.0 unx      394 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
--rw-r--r--  2.0 unx      455 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
--rw-r--r--  2.0 unx      683 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/SortedClassProbability.class
--rw-r--r--  2.0 unx      606 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
--rw-r--r--  2.0 unx      479 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/Word2VecPrediction.class
--rw-r--r--  2.0 unx      665 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/BinomialModelPrediction.class
--rw-r--r--  2.0 unx      445 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
--rw-r--r--  2.0 unx      561 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/RegressionModelPrediction.class
--rw-r--r--  2.0 unx      414 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
--rw-r--r--  2.0 unx      430 b- defN 23-Mar-09 15:17 hex/genmodel/easy/prediction/KLimeModelPrediction.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/
--rw-r--r--  2.0 unx      454 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/PredictUnknownTypeException.class
--rw-r--r--  2.0 unx      683 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/PredictException.class
--rw-r--r--  2.0 unx      457 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/PredictNumberFormatException.class
--rw-r--r--  2.0 unx      475 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
--rw-r--r--  2.0 unx      831 b- defN 23-Mar-09 15:17 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
--rw-r--r--  2.0 unx     1302 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1309 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EigenEncoderColumnMapper.class
--rw-r--r--  2.0 unx    23998 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EasyPredictModelWrapper.class
--rw-r--r--  2.0 unx     5805 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
--rw-r--r--  2.0 unx      621 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
--rw-r--r--  2.0 unx      241 b- defN 23-Mar-09 15:17 hex/genmodel/easy/CategoricalEncoder.class
--rw-r--r--  2.0 unx     5444 b- defN 23-Mar-09 15:17 hex/genmodel/easy/RowToRawDataConverter.class
--rw-r--r--  2.0 unx      363 b- defN 23-Mar-09 15:17 hex/genmodel/easy/RowData.class
--rw-r--r--  2.0 unx      597 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
--rw-r--r--  2.0 unx     1939 b- defN 23-Mar-09 15:17 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1591 b- defN 23-Mar-09 15:17 hex/genmodel/easy/BinaryColumnMapper.class
--rw-r--r--  2.0 unx      872 b- defN 23-Mar-09 15:17 hex/genmodel/easy/DomainMapConstructor.class
--rw-r--r--  2.0 unx     1941 b- defN 23-Mar-09 15:17 hex/genmodel/easy/BinaryDomainMapConstructor.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Mar-09 15:17 hex/genmodel/easy/OneHotEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1962 b- defN 23-Mar-09 15:17 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2357 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumLimitedEncoder.class
--rw-r--r--  2.0 unx     2209 b- defN 23-Mar-09 15:17 hex/genmodel/easy/OneHotEncoder.class
--rw-r--r--  2.0 unx     2290 b- defN 23-Mar-09 15:17 hex/genmodel/easy/BinaryEncoder.class
--rw-r--r--  2.0 unx     1633 b- defN 23-Mar-09 15:17 hex/genmodel/easy/LabelEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/easy/error/
--rw-r--r--  2.0 unx      805 b- defN 23-Mar-09 15:17 hex/genmodel/easy/error/VoidErrorConsumer.class
--rw-r--r--  2.0 unx      702 b- defN 23-Mar-09 15:17 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
--rw-r--r--  2.0 unx     5332 b- defN 23-Mar-09 15:17 hex/genmodel/easy/error/CountingErrorConsumer.class
--rw-r--r--  2.0 unx     1269 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EasyPredictModelWrapper$1.class
--rw-r--r--  2.0 unx     1876 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2146 b- defN 23-Mar-09 15:17 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/tools/
--rw-r--r--  2.0 unx     1287 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
--rw-r--r--  2.0 unx     1026 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PredictCsv$1.class
--rw-r--r--  2.0 unx     5410 b- defN 23-Mar-09 15:17 hex/genmodel/tools/MungeCsv.class
--rw-r--r--  2.0 unx     1010 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
--rw-r--r--  2.0 unx    20777 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PredictCsv.class
--rw-r--r--  2.0 unx    14133 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PrintMojo.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
--rw-r--r--  2.0 unx     4591 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
--rw-r--r--  2.0 unx      826 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PrintMojo$2.class
--rw-r--r--  2.0 unx      722 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PrintMojo$1.class
--rw-r--r--  2.0 unx     7956 b- defN 23-Mar-09 15:17 hex/genmodel/tools/BuildPipeline.class
--rw-r--r--  2.0 unx     1294 b- defN 23-Mar-09 15:17 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
--rw-r--r--  2.0 unx     1202 b- defN 23-Mar-09 15:17 hex/genmodel/tools/MojoPrinter$Format.class
--rw-r--r--  2.0 unx      388 b- defN 23-Mar-09 15:17 hex/genmodel/tools/MojoPrinter.class
--rw-r--r--  2.0 unx      895 b- defN 23-Mar-09 15:17 hex/genmodel/ConverterFactoryProvidingModel.class
--rw-r--r--  2.0 unx     1538 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$6.class
--rw-r--r--  2.0 unx     2779 b- defN 23-Mar-09 15:17 hex/genmodel/MultiModelMojoReader.class
--rw-r--r--  2.0 unx     1583 b- defN 23-Mar-09 15:17 hex/genmodel/GenMunger$Step.class
--rw-r--r--  2.0 unx     1277 b- defN 23-Mar-09 15:17 hex/genmodel/GenModel$1.class
--rw-r--r--  2.0 unx     1403 b- defN 23-Mar-09 15:17 hex/genmodel/TmpMojoReaderBackend.class
--rw-r--r--  2.0 unx      215 b- defN 23-Mar-09 15:17 hex/genmodel/IClusteringModel.class
--rw-r--r--  2.0 unx     2445 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding.class
--rw-r--r--  2.0 unx     6310 b- defN 23-Mar-09 15:17 hex/genmodel/MojoPipelineBuilder.class
--rw-r--r--  2.0 unx     2276 b- defN 23-Mar-09 15:17 hex/genmodel/InMemoryMojoReaderBackend.class
--rw-r--r--  2.0 unx     5604 b- defN 23-Mar-09 15:17 hex/genmodel/MojoPipelineWriter.class
--rw-r--r--  2.0 unx     1729 b- defN 23-Mar-09 15:17 hex/genmodel/FolderMojoReaderBackend.class
--rw-r--r--  2.0 unx     1489 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$1.class
--rw-r--r--  2.0 unx      225 b- defN 23-Mar-09 15:17 hex/genmodel/PredictContributionsFactory.class
--rw-r--r--  2.0 unx      334 b- defN 23-Mar-09 15:17 hex/genmodel/PredictContributions.class
--rw-r--r--  2.0 unx     4315 b- defN 23-Mar-09 15:17 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
--rw-r--r--  2.0 unx      234 b- defN 23-Mar-09 15:17 hex/genmodel/MultiModelMojoReader$1.class
--rw-r--r--  2.0 unx     9766 b- defN 23-Mar-09 15:17 hex/genmodel/AbstractMojoWriter.class
--rw-r--r--  2.0 unx     2771 b- defN 23-Mar-09 15:17 hex/genmodel/MojoModel.class
--rw-r--r--  2.0 unx      228 b- defN 23-Mar-09 15:17 hex/genmodel/MojoPipelineWriter$1.class
--rw-r--r--  2.0 unx      345 b- defN 23-Mar-09 15:17 hex/genmodel/MojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/utils/
--rw-r--r--  2.0 unx     1366 b- defN 23-Mar-09 15:17 hex/genmodel/utils/StringEscapeUtils.class
--rw-r--r--  2.0 unx      770 b- defN 23-Mar-09 15:17 hex/genmodel/utils/IOUtils.class
--rw-r--r--  2.0 unx     7386 b- defN 23-Mar-09 15:17 hex/genmodel/utils/ArrayUtils.class
--rw-r--r--  2.0 unx     3399 b- defN 23-Mar-09 15:17 hex/genmodel/utils/ParseUtils.class
--rw-r--r--  2.0 unx     1869 b- defN 23-Mar-09 15:17 hex/genmodel/utils/ByteBufferWrapper.class
--rw-r--r--  2.0 unx     1329 b- defN 23-Mar-09 15:17 hex/genmodel/utils/MathUtils.class
--rw-r--r--  2.0 unx      988 b- defN 23-Mar-09 15:17 hex/genmodel/utils/ArrayUtils$1.class
--rw-r--r--  2.0 unx     1361 b- defN 23-Mar-09 15:17 hex/genmodel/utils/LinkFunctionType.class
--rw-r--r--  2.0 unx     1862 b- defN 23-Mar-09 15:17 hex/genmodel/utils/DistributionFamily.class
--rw-r--r--  2.0 unx     3320 b- defN 23-Mar-09 15:17 hex/genmodel/utils/GenmodelBitSet.class
--rw-r--r--  2.0 unx     1206 b- defN 23-Mar-09 15:17 hex/genmodel/utils/ArrayUtils$2.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Mar-09 15:17 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
--rw-r--r--  2.0 unx     7590 b- defN 23-Mar-09 15:17 hex/genmodel/GenMunger.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/annotations/
--rw-r--r--  2.0 unx      521 b- defN 23-Mar-09 15:17 hex/genmodel/annotations/ModelPojo.class
--rw-r--r--  2.0 unx     1527 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$3.class
--rw-r--r--  2.0 unx      398 b- defN 23-Mar-09 15:17 hex/genmodel/IGenModel.class
--rw-r--r--  2.0 unx     1539 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$5.class
--rw-r--r--  2.0 unx     1268 b- defN 23-Mar-09 15:17 hex/genmodel/NestedMojoReaderBackend.class
--rw-r--r--  2.0 unx    14911 b- defN 23-Mar-09 15:17 hex/genmodel/ModelMojoReader.class
--rw-r--r--  2.0 unx     2041 b- defN 23-Mar-09 15:17 hex/genmodel/ZipfileMojoReaderBackend.class
--rw-r--r--  2.0 unx    18923 b- defN 23-Mar-09 15:17 hex/genmodel/GenModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/svm/
--rw-r--r--  2.0 unx     1887 b- defN 23-Mar-09 15:17 hex/genmodel/algos/svm/SvmMojoReader.class
--rw-r--r--  2.0 unx     1340 b- defN 23-Mar-09 15:17 hex/genmodel/algos/svm/SvmMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/klime/
--rw-r--r--  2.0 unx     2319 b- defN 23-Mar-09 15:17 hex/genmodel/algos/klime/KLimeMojoModel.class
--rw-r--r--  2.0 unx     2687 b- defN 23-Mar-09 15:17 hex/genmodel/algos/klime/KLimeMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/word2vec/
--rw-r--r--  2.0 unx     1490 b- defN 23-Mar-09 15:17 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
--rw-r--r--  2.0 unx     3174 b- defN 23-Mar-09 15:17 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
--rw-r--r--  2.0 unx      220 b- defN 23-Mar-09 15:17 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/
--rw-r--r--  2.0 unx      863 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/MojoRule.class
--rw-r--r--  2.0 unx     1620 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/MojoCondition.class
--rw-r--r--  2.0 unx     2502 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
--rw-r--r--  2.0 unx     7385 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
--rw-r--r--  2.0 unx     3386 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
--rw-r--r--  2.0 unx     1177 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/MojoCondition$Type.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
--rw-r--r--  2.0 unx     1256 b- defN 23-Mar-09 15:17 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/
--rw-r--r--  2.0 unx      263 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
--rw-r--r--  2.0 unx     3299 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
--rw-r--r--  2.0 unx      880 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
--rw-r--r--  2.0 unx     4714 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoReader.class
--rw-r--r--  2.0 unx      353 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
--rw-r--r--  2.0 unx      657 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreTree0.class
--rw-r--r--  2.0 unx      202 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreTree.class
--rw-r--r--  2.0 unx      220 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAP$1.class
--rw-r--r--  2.0 unx      635 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreTree2.class
--rw-r--r--  2.0 unx     1101 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ConvertTreeOptions.class
--rw-r--r--  2.0 unx     8018 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeSubgraph.class
--rw-r--r--  2.0 unx     2998 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
--rw-r--r--  2.0 unx     8370 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAP.class
--rw-r--r--  2.0 unx      253 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
--rw-r--r--  2.0 unx      535 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
--rw-r--r--  2.0 unx      438 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
--rw-r--r--  2.0 unx     2835 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
--rw-r--r--  2.0 unx      657 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreTree1.class
--rw-r--r--  2.0 unx      712 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAPPredictor.class
--rw-r--r--  2.0 unx    16477 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeNode.class
--rw-r--r--  2.0 unx     1175 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/CalibrationMojoHelper.class
--rw-r--r--  2.0 unx     2634 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ContributionComposer.class
--rw-r--r--  2.0 unx      602 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreIsolationTree0.class
--rw-r--r--  2.0 unx     1395 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/NaSplitDir.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
--rw-r--r--  2.0 unx      611 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeBackedMojoModel.class
--rw-r--r--  2.0 unx     3699 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeGraph.class
--rw-r--r--  2.0 unx    24842 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
--rw-r--r--  2.0 unx     1707 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
--rw-r--r--  2.0 unx      199 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ScoreIsolationTree.class
--rw-r--r--  2.0 unx     1445 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
--rw-r--r--  2.0 unx      399 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
--rw-r--r--  2.0 unx     3805 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/ContributionsPredictor.class
--rw-r--r--  2.0 unx     2632 b- defN 23-Mar-09 15:17 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/coxph/
--rw-r--r--  2.0 unx     3758 b- defN 23-Mar-09 15:17 hex/genmodel/algos/coxph/CoxPHMojoModel.class
--rw-r--r--  2.0 unx     1144 b- defN 23-Mar-09 15:17 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
--rw-r--r--  2.0 unx     3613 b- defN 23-Mar-09 15:17 hex/genmodel/algos/coxph/CoxPHMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/drf/
--rw-r--r--  2.0 unx     1633 b- defN 23-Mar-09 15:17 hex/genmodel/algos/drf/DrfMojoReader.class
--rw-r--r--  2.0 unx      230 b- defN 23-Mar-09 15:17 hex/genmodel/algos/drf/DrfMojoModel$1.class
--rw-r--r--  2.0 unx     3129 b- defN 23-Mar-09 15:17 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
--rw-r--r--  2.0 unx     2700 b- defN 23-Mar-09 15:17 hex/genmodel/algos/drf/DrfMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isoforextended/
--rw-r--r--  2.0 unx     4170 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2306 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pca/
--rw-r--r--  2.0 unx     2645 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pca/PCAMojoModel.class
--rw-r--r--  2.0 unx     2819 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pca/PCAMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/
--rw-r--r--  2.0 unx     4318 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel.class
--rw-r--r--  2.0 unx     2466 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
--rw-r--r--  2.0 unx     1747 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModelBase.class
--rw-r--r--  2.0 unx      848 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
--rw-r--r--  2.0 unx      851 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
--rw-r--r--  2.0 unx      230 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$1.class
--rw-r--r--  2.0 unx     2647 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
--rw-r--r--  2.0 unx      836 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
--rw-r--r--  2.0 unx      626 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
--rw-r--r--  2.0 unx      272 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
--rw-r--r--  2.0 unx      724 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
--rw-r--r--  2.0 unx      842 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
--rw-r--r--  2.0 unx     3584 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glm/GlmMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/
--rw-r--r--  2.0 unx      677 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/ColumnsMapping.class
--rw-r--r--  2.0 unx     3493 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/EncodingMap.class
--rw-r--r--  2.0 unx     9375 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
--rw-r--r--  2.0 unx     2436 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/EncodingMaps.class
--rw-r--r--  2.0 unx     1417 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
--rw-r--r--  2.0 unx     8265 b- defN 23-Mar-09 15:17 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isotonic/
--rw-r--r--  2.0 unx      888 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
--rw-r--r--  2.0 unx      874 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
--rw-r--r--  2.0 unx     1680 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/
--rw-r--r--  2.0 unx      783 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
--rw-r--r--  2.0 unx     5224 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
--rw-r--r--  2.0 unx     1081 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
--rw-r--r--  2.0 unx      769 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
--rw-r--r--  2.0 unx      709 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
--rw-r--r--  2.0 unx     1096 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
--rw-r--r--  2.0 unx     6719 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/NeuralNetwork.class
--rw-r--r--  2.0 unx      934 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
--rw-r--r--  2.0 unx      323 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
--rw-r--r--  2.0 unx     2132 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils.class
--rw-r--r--  2.0 unx      798 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
--rw-r--r--  2.0 unx      663 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
--rw-r--r--  2.0 unx     6843 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
--rw-r--r--  2.0 unx      787 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
--rw-r--r--  2.0 unx      995 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
--rw-r--r--  2.0 unx      922 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
--rw-r--r--  2.0 unx     1007 b- defN 23-Mar-09 15:17 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/
--rw-r--r--  2.0 unx      196 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/SupportVectorScorer.class
--rw-r--r--  2.0 unx      422 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/KernelParameters.class
--rw-r--r--  2.0 unx     1388 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/ScorerFactory.class
--rw-r--r--  2.0 unx     1550 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/GaussianScorer.class
--rw-r--r--  2.0 unx      973 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/KernelType.class
--rw-r--r--  2.0 unx      699 b- defN 23-Mar-09 15:17 hex/genmodel/algos/psvm/ScorerFactory$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/ensemble/
--rw-r--r--  2.0 unx     3993 b- defN 23-Mar-09 15:17 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
--rw-r--r--  2.0 unx      974 b- defN 23-Mar-09 15:17 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
--rw-r--r--  2.0 unx     2165 b- defN 23-Mar-09 15:17 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isofor/
--rw-r--r--  2.0 unx     1835 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2021 b- defN 23-Mar-09 15:17 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/
--rw-r--r--  2.0 unx     1572 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamMojoModel.class
--rw-r--r--  2.0 unx     2046 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/ISplines.class
--rw-r--r--  2.0 unx     2045 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/NBSplinesTypeII.class
--rw-r--r--  2.0 unx    10957 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamMojoReader.class
--rw-r--r--  2.0 unx     1717 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
--rw-r--r--  2.0 unx      855 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
--rw-r--r--  2.0 unx     1902 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
--rw-r--r--  2.0 unx     3495 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/NBSplinesTypeI.class
--rw-r--r--  2.0 unx     2061 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
--rw-r--r--  2.0 unx    11583 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamMojoModelBase.class
--rw-r--r--  2.0 unx     1347 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/MSplines.class
--rw-r--r--  2.0 unx     4489 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamUtilsISplines.class
--rw-r--r--  2.0 unx      896 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamMojoModelBase$1.class
--rw-r--r--  2.0 unx     2234 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
--rw-r--r--  2.0 unx     1977 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
--rw-r--r--  2.0 unx     2518 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pipeline/
--rw-r--r--  2.0 unx     1732 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pipeline/MojoPipeline.class
--rw-r--r--  2.0 unx     6799 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pipeline/MojoPipelineReader.class
--rw-r--r--  2.0 unx      635 b- defN 23-Mar-09 15:17 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/kmeans/
--rw-r--r--  2.0 unx     1339 b- defN 23-Mar-09 15:17 hex/genmodel/algos/kmeans/KMeansMojoModel.class
--rw-r--r--  2.0 unx     2248 b- defN 23-Mar-09 15:17 hex/genmodel/algos/kmeans/KMeansMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gbm/
--rw-r--r--  2.0 unx     4006 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gbm/GbmMojoModel.class
--rw-r--r--  2.0 unx     2104 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gbm/GbmMojoReader.class
--rw-r--r--  2.0 unx      981 b- defN 23-Mar-09 15:17 hex/genmodel/algos/gbm/GbmMojoModel$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/
--rw-r--r--  2.0 unx     1345 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
--rw-r--r--  2.0 unx     4904 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmMojoReader.class
--rw-r--r--  2.0 unx     1567 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$5.class
--rw-r--r--  2.0 unx     2161 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$8.class
--rw-r--r--  2.0 unx     1232 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
--rw-r--r--  2.0 unx     1980 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
--rw-r--r--  2.0 unx      875 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
--rw-r--r--  2.0 unx     2578 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer.class
--rw-r--r--  2.0 unx     1219 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmInitialization.class
--rw-r--r--  2.0 unx     1075 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$2.class
--rw-r--r--  2.0 unx     2236 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$9.class
--rw-r--r--  2.0 unx     1512 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$6.class
--rw-r--r--  2.0 unx     1186 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$3.class
--rw-r--r--  2.0 unx     1290 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
--rw-r--r--  2.0 unx     1406 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
--rw-r--r--  2.0 unx     9537 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmMojoModel.class
--rw-r--r--  2.0 unx     1280 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
--rw-r--r--  2.0 unx      983 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$1.class
--rw-r--r--  2.0 unx     1510 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$7.class
--rw-r--r--  2.0 unx     1460 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
--rw-r--r--  2.0 unx     3178 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss.class
--rw-r--r--  2.0 unx     1499 b- defN 23-Mar-09 15:17 hex/genmodel/algos/glrm/GlrmLoss$4.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Mar-09 15:17 hex/genmodel/ModelMojoReader$1.class
--rw-r--r--  2.0 unx      855 b- defN 23-Mar-09 15:17 hex/genmodel/MojoReaderBackendFactory$1.class
--rw-r--r--  2.0 unx     1934 b- defN 23-Mar-09 15:17 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/
--rw-r--r--  2.0 unx     1045 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/SharedTreeModelAttributes.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/
--rw-r--r--  2.0 unx      773 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
--rw-r--r--  2.0 unx      420 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
--rw-r--r--  2.0 unx      590 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
--rw-r--r--  2.0 unx      777 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
--rw-r--r--  2.0 unx      449 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
--rw-r--r--  2.0 unx      630 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetrics.class
--rw-r--r--  2.0 unx      748 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
--rw-r--r--  2.0 unx      860 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
--rw-r--r--  2.0 unx      860 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
--rw-r--r--  2.0 unx      785 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
--rw-r--r--  2.0 unx      789 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
--rw-r--r--  2.0 unx      517 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
--rw-r--r--  2.0 unx      993 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/DeepLearningModelAttributes.class
--rw-r--r--  2.0 unx     5653 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelAttributes.class
--rw-r--r--  2.0 unx     1267 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/VariableImportances$1.class
--rw-r--r--  2.0 unx      495 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/SerializedName.class
--rw-r--r--  2.0 unx     2602 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/VariableImportances.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/Table$ColumnType.class
--rw-r--r--  2.0 unx     1155 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelAttributes$1.class
--rw-r--r--  2.0 unx     3376 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/Table.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/
--rw-r--r--  2.0 unx      874 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/ColumnSpecifier.class
--rw-r--r--  2.0 unx      249 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
--rw-r--r--  2.0 unx      953 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/KeyValue.class
--rw-r--r--  2.0 unx     1892 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/ModelParameter.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/ParameterKey$Type.class
--rw-r--r--  2.0 unx      880 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/FeatureContribution.class
--rw-r--r--  2.0 unx     1176 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/ParameterKey.class
--rw-r--r--  2.0 unx     1263 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/parameters/StringPair.class
--rw-r--r--  2.0 unx     1768 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelJsonReader$1.class
--rw-r--r--  2.0 unx     2522 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelAttributesGLM.class
--rw-r--r--  2.0 unx    15710 b- defN 23-Mar-09 15:17 hex/genmodel/attributes/ModelJsonReader.class
--rw-r--r--  2.0 unx     1541 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$2.class
--rw-r--r--  2.0 unx     1551 b- defN 23-Mar-09 15:17 hex/genmodel/CategoricalEncoding$4.class
--rw-r--r--  2.0 unx     1127 b- defN 23-Mar-09 15:17 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
--rw-r--r--  2.0 unx     5010 b- defN 23-Mar-09 15:17 hex/genmodel/ModelMojoFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 water/util/
--rw-r--r--  2.0 unx    10148 b- defN 23-Mar-09 15:17 water/util/H2OPredictor.class
--rw-r--r--  2.0 unx      606 b- defN 23-Mar-09 15:17 water/util/H2OPredictor$1.class
--rw-r--r--  2.0 unx     2742 b- defN 23-Mar-09 15:17 water/util/JavaVersionUtils.class
--rw-r--r--  2.0 unx      971 b- defN 23-Mar-09 15:17 water/util/ModelUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 water/genmodel/
--rw-r--r--  2.0 unx      873 b- defN 23-Mar-09 15:17 water/genmodel/AbstractBuildVersion$1.class
--rw-r--r--  2.0 unx     2965 b- defN 23-Mar-09 15:17 water/genmodel/AbstractBuildVersion.class
--rw-r--r--  2.0 unx      924 b- defN 23-Mar-09 15:17 water/genmodel/BuildVersion.class
--rw-r--r--  2.0 unx      921 b- defN 23-Mar-09 15:17 water/genmodel/IGeneratedModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 META-INF/services/
--rw-r--r--  2.0 unx       29 b- defN 23-Mar-09 15:17 META-INF/services/hex.genmodel.tools.MojoPrinter
-359 files, 759162 bytes uncompressed, 372214 bytes compressed:  51.0%
+Zip file size: 432826 bytes, number of entries: 359
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-28 12:08 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/
+-rw-r--r--  2.0 unx     1699 b- defN 23-Apr-28 12:08 hex/ModelCategory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/
+-rw-r--r--  2.0 unx      731 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptor.class
+-rw-r--r--  2.0 unx     3832 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
+-rw-r--r--  2.0 unx      262 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
+-rw-r--r--  2.0 unx     1415 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder.class
+-rw-r--r--  2.0 unx     4531 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
+-rw-r--r--  2.0 unx     1088 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader$RawValue.class
+-rw-r--r--  2.0 unx     5067 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/
+-rw-r--r--  2.0 unx     2069 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1698 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoder.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/
+-rw-r--r--  2.0 unx      549 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AbstractPrediction.class
+-rw-r--r--  2.0 unx     1159 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
+-rw-r--r--  2.0 unx      476 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
+-rw-r--r--  2.0 unx      455 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/SortedClassProbability.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
+-rw-r--r--  2.0 unx      479 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/Word2VecPrediction.class
+-rw-r--r--  2.0 unx      665 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/BinomialModelPrediction.class
+-rw-r--r--  2.0 unx      445 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
+-rw-r--r--  2.0 unx      561 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/RegressionModelPrediction.class
+-rw-r--r--  2.0 unx      414 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
+-rw-r--r--  2.0 unx      430 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/KLimeModelPrediction.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/
+-rw-r--r--  2.0 unx      454 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictUnknownTypeException.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictException.class
+-rw-r--r--  2.0 unx      457 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictNumberFormatException.class
+-rw-r--r--  2.0 unx      475 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
+-rw-r--r--  2.0 unx      831 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
+-rw-r--r--  2.0 unx     1302 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1309 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoderColumnMapper.class
+-rw-r--r--  2.0 unx    23998 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper.class
+-rw-r--r--  2.0 unx     5805 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
+-rw-r--r--  2.0 unx      621 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
+-rw-r--r--  2.0 unx      241 b- defN 23-Apr-28 12:08 hex/genmodel/easy/CategoricalEncoder.class
+-rw-r--r--  2.0 unx     5444 b- defN 23-Apr-28 12:08 hex/genmodel/easy/RowToRawDataConverter.class
+-rw-r--r--  2.0 unx      363 b- defN 23-Apr-28 12:08 hex/genmodel/easy/RowData.class
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
+-rw-r--r--  2.0 unx     1939 b- defN 23-Apr-28 12:08 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1591 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryColumnMapper.class
+-rw-r--r--  2.0 unx      872 b- defN 23-Apr-28 12:08 hex/genmodel/easy/DomainMapConstructor.class
+-rw-r--r--  2.0 unx     1941 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1962 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2357 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoder.class
+-rw-r--r--  2.0 unx     2209 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoder.class
+-rw-r--r--  2.0 unx     2290 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryEncoder.class
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-28 12:08 hex/genmodel/easy/LabelEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/
+-rw-r--r--  2.0 unx      805 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/VoidErrorConsumer.class
+-rw-r--r--  2.0 unx      702 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
+-rw-r--r--  2.0 unx     5332 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/CountingErrorConsumer.class
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$1.class
+-rw-r--r--  2.0 unx     1876 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2146 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/tools/
+-rw-r--r--  2.0 unx     1287 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
+-rw-r--r--  2.0 unx     1026 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$1.class
+-rw-r--r--  2.0 unx     5410 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MungeCsv.class
+-rw-r--r--  2.0 unx     1010 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
+-rw-r--r--  2.0 unx    20777 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv.class
+-rw-r--r--  2.0 unx    14133 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
+-rw-r--r--  2.0 unx     4591 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
+-rw-r--r--  2.0 unx      826 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$2.class
+-rw-r--r--  2.0 unx      722 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$1.class
+-rw-r--r--  2.0 unx     7956 b- defN 23-Apr-28 12:08 hex/genmodel/tools/BuildPipeline.class
+-rw-r--r--  2.0 unx     1294 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
+-rw-r--r--  2.0 unx     1202 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MojoPrinter$Format.class
+-rw-r--r--  2.0 unx      388 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MojoPrinter.class
+-rw-r--r--  2.0 unx      895 b- defN 23-Apr-28 12:08 hex/genmodel/ConverterFactoryProvidingModel.class
+-rw-r--r--  2.0 unx     1538 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$6.class
+-rw-r--r--  2.0 unx     2779 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader.class
+-rw-r--r--  2.0 unx     1583 b- defN 23-Apr-28 12:08 hex/genmodel/GenMunger$Step.class
+-rw-r--r--  2.0 unx     1277 b- defN 23-Apr-28 12:08 hex/genmodel/GenModel$1.class
+-rw-r--r--  2.0 unx     1403 b- defN 23-Apr-28 12:08 hex/genmodel/TmpMojoReaderBackend.class
+-rw-r--r--  2.0 unx      215 b- defN 23-Apr-28 12:08 hex/genmodel/IClusteringModel.class
+-rw-r--r--  2.0 unx     2445 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding.class
+-rw-r--r--  2.0 unx     6310 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineBuilder.class
+-rw-r--r--  2.0 unx     2276 b- defN 23-Apr-28 12:08 hex/genmodel/InMemoryMojoReaderBackend.class
+-rw-r--r--  2.0 unx     5604 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter.class
+-rw-r--r--  2.0 unx     1729 b- defN 23-Apr-28 12:08 hex/genmodel/FolderMojoReaderBackend.class
+-rw-r--r--  2.0 unx     1489 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$1.class
+-rw-r--r--  2.0 unx      225 b- defN 23-Apr-28 12:08 hex/genmodel/PredictContributionsFactory.class
+-rw-r--r--  2.0 unx      334 b- defN 23-Apr-28 12:08 hex/genmodel/PredictContributions.class
+-rw-r--r--  2.0 unx     4315 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
+-rw-r--r--  2.0 unx      234 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader$1.class
+-rw-r--r--  2.0 unx     9766 b- defN 23-Apr-28 12:08 hex/genmodel/AbstractMojoWriter.class
+-rw-r--r--  2.0 unx     2771 b- defN 23-Apr-28 12:08 hex/genmodel/MojoModel.class
+-rw-r--r--  2.0 unx      228 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter$1.class
+-rw-r--r--  2.0 unx      345 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/utils/
+-rw-r--r--  2.0 unx     1366 b- defN 23-Apr-28 12:08 hex/genmodel/utils/StringEscapeUtils.class
+-rw-r--r--  2.0 unx      770 b- defN 23-Apr-28 12:08 hex/genmodel/utils/IOUtils.class
+-rw-r--r--  2.0 unx     7386 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils.class
+-rw-r--r--  2.0 unx     3399 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ParseUtils.class
+-rw-r--r--  2.0 unx     1869 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ByteBufferWrapper.class
+-rw-r--r--  2.0 unx     1329 b- defN 23-Apr-28 12:08 hex/genmodel/utils/MathUtils.class
+-rw-r--r--  2.0 unx      988 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils$1.class
+-rw-r--r--  2.0 unx     1361 b- defN 23-Apr-28 12:08 hex/genmodel/utils/LinkFunctionType.class
+-rw-r--r--  2.0 unx     1862 b- defN 23-Apr-28 12:08 hex/genmodel/utils/DistributionFamily.class
+-rw-r--r--  2.0 unx     3320 b- defN 23-Apr-28 12:08 hex/genmodel/utils/GenmodelBitSet.class
+-rw-r--r--  2.0 unx     1206 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils$2.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
+-rw-r--r--  2.0 unx     7590 b- defN 23-Apr-28 12:08 hex/genmodel/GenMunger.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/annotations/
+-rw-r--r--  2.0 unx      521 b- defN 23-Apr-28 12:08 hex/genmodel/annotations/ModelPojo.class
+-rw-r--r--  2.0 unx     1527 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$3.class
+-rw-r--r--  2.0 unx      398 b- defN 23-Apr-28 12:08 hex/genmodel/IGenModel.class
+-rw-r--r--  2.0 unx     1539 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$5.class
+-rw-r--r--  2.0 unx     1268 b- defN 23-Apr-28 12:08 hex/genmodel/NestedMojoReaderBackend.class
+-rw-r--r--  2.0 unx    14911 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader.class
+-rw-r--r--  2.0 unx     2041 b- defN 23-Apr-28 12:08 hex/genmodel/ZipfileMojoReaderBackend.class
+-rw-r--r--  2.0 unx    18923 b- defN 23-Apr-28 12:08 hex/genmodel/GenModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/
+-rw-r--r--  2.0 unx     1887 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/SvmMojoReader.class
+-rw-r--r--  2.0 unx     1340 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/SvmMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/
+-rw-r--r--  2.0 unx     2319 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/KLimeMojoModel.class
+-rw-r--r--  2.0 unx     2687 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/KLimeMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/
+-rw-r--r--  2.0 unx     1490 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
+-rw-r--r--  2.0 unx     3174 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/
+-rw-r--r--  2.0 unx      863 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoRule.class
+-rw-r--r--  2.0 unx     1620 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition.class
+-rw-r--r--  2.0 unx     2502 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
+-rw-r--r--  2.0 unx     7385 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
+-rw-r--r--  2.0 unx     3386 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
+-rw-r--r--  2.0 unx     1177 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition$Type.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
+-rw-r--r--  2.0 unx     1256 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/
+-rw-r--r--  2.0 unx      263 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
+-rw-r--r--  2.0 unx     3299 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
+-rw-r--r--  2.0 unx     4714 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoReader.class
+-rw-r--r--  2.0 unx      353 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree0.class
+-rw-r--r--  2.0 unx      202 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$1.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree2.class
+-rw-r--r--  2.0 unx     1101 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ConvertTreeOptions.class
+-rw-r--r--  2.0 unx     8018 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeSubgraph.class
+-rw-r--r--  2.0 unx     2998 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
+-rw-r--r--  2.0 unx     8370 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP.class
+-rw-r--r--  2.0 unx      253 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
+-rw-r--r--  2.0 unx      535 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
+-rw-r--r--  2.0 unx      438 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
+-rw-r--r--  2.0 unx     2835 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree1.class
+-rw-r--r--  2.0 unx      712 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPPredictor.class
+-rw-r--r--  2.0 unx    16477 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeNode.class
+-rw-r--r--  2.0 unx     1175 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/CalibrationMojoHelper.class
+-rw-r--r--  2.0 unx     2634 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ContributionComposer.class
+-rw-r--r--  2.0 unx      602 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreIsolationTree0.class
+-rw-r--r--  2.0 unx     1395 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/NaSplitDir.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
+-rw-r--r--  2.0 unx      611 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeBackedMojoModel.class
+-rw-r--r--  2.0 unx     3699 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeGraph.class
+-rw-r--r--  2.0 unx    24842 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
+-rw-r--r--  2.0 unx     1707 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
+-rw-r--r--  2.0 unx      199 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreIsolationTree.class
+-rw-r--r--  2.0 unx     1445 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
+-rw-r--r--  2.0 unx      399 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
+-rw-r--r--  2.0 unx     3805 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ContributionsPredictor.class
+-rw-r--r--  2.0 unx     2632 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/
+-rw-r--r--  2.0 unx     3758 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoModel.class
+-rw-r--r--  2.0 unx     1144 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
+-rw-r--r--  2.0 unx     3613 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoReader.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel$1.class
+-rw-r--r--  2.0 unx     3129 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
+-rw-r--r--  2.0 unx     2700 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/
+-rw-r--r--  2.0 unx     4170 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2306 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/
+-rw-r--r--  2.0 unx     2645 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/PCAMojoModel.class
+-rw-r--r--  2.0 unx     2819 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/PCAMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/
+-rw-r--r--  2.0 unx     4318 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel.class
+-rw-r--r--  2.0 unx     2466 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
+-rw-r--r--  2.0 unx     1747 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModelBase.class
+-rw-r--r--  2.0 unx      848 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
+-rw-r--r--  2.0 unx      851 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$1.class
+-rw-r--r--  2.0 unx     2647 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
+-rw-r--r--  2.0 unx      836 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
+-rw-r--r--  2.0 unx      626 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
+-rw-r--r--  2.0 unx      272 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
+-rw-r--r--  2.0 unx      724 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
+-rw-r--r--  2.0 unx      842 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
+-rw-r--r--  2.0 unx     3584 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/
+-rw-r--r--  2.0 unx      677 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/ColumnsMapping.class
+-rw-r--r--  2.0 unx     3493 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/EncodingMap.class
+-rw-r--r--  2.0 unx     9375 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
+-rw-r--r--  2.0 unx     2436 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/EncodingMaps.class
+-rw-r--r--  2.0 unx     1417 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
+-rw-r--r--  2.0 unx     8265 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/
+-rw-r--r--  2.0 unx      888 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
+-rw-r--r--  2.0 unx      874 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
+-rw-r--r--  2.0 unx     1680 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/
+-rw-r--r--  2.0 unx      783 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
+-rw-r--r--  2.0 unx     5224 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
+-rw-r--r--  2.0 unx     1081 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
+-rw-r--r--  2.0 unx      769 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
+-rw-r--r--  2.0 unx      709 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
+-rw-r--r--  2.0 unx     1096 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
+-rw-r--r--  2.0 unx     6719 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/NeuralNetwork.class
+-rw-r--r--  2.0 unx      934 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
+-rw-r--r--  2.0 unx      323 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
+-rw-r--r--  2.0 unx     2132 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils.class
+-rw-r--r--  2.0 unx      798 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
+-rw-r--r--  2.0 unx      663 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
+-rw-r--r--  2.0 unx     6843 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
+-rw-r--r--  2.0 unx      787 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
+-rw-r--r--  2.0 unx      995 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
+-rw-r--r--  2.0 unx      922 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
+-rw-r--r--  2.0 unx     1007 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/
+-rw-r--r--  2.0 unx      196 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/SupportVectorScorer.class
+-rw-r--r--  2.0 unx      422 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/KernelParameters.class
+-rw-r--r--  2.0 unx     1388 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/ScorerFactory.class
+-rw-r--r--  2.0 unx     1550 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/GaussianScorer.class
+-rw-r--r--  2.0 unx      973 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/KernelType.class
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/ScorerFactory$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/
+-rw-r--r--  2.0 unx     3993 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
+-rw-r--r--  2.0 unx      974 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
+-rw-r--r--  2.0 unx     2165 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/
+-rw-r--r--  2.0 unx     1835 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2021 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/
+-rw-r--r--  2.0 unx     1572 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModel.class
+-rw-r--r--  2.0 unx     2046 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/ISplines.class
+-rw-r--r--  2.0 unx     2045 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeII.class
+-rw-r--r--  2.0 unx    10957 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoReader.class
+-rw-r--r--  2.0 unx     1717 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
+-rw-r--r--  2.0 unx     1902 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
+-rw-r--r--  2.0 unx     3495 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeI.class
+-rw-r--r--  2.0 unx     2061 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
+-rw-r--r--  2.0 unx    11583 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModelBase.class
+-rw-r--r--  2.0 unx     1347 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/MSplines.class
+-rw-r--r--  2.0 unx     4489 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsISplines.class
+-rw-r--r--  2.0 unx      896 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModelBase$1.class
+-rw-r--r--  2.0 unx     2234 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
+-rw-r--r--  2.0 unx     1977 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
+-rw-r--r--  2.0 unx     2518 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/
+-rw-r--r--  2.0 unx     1732 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipeline.class
+-rw-r--r--  2.0 unx     6799 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipelineReader.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/
+-rw-r--r--  2.0 unx     1339 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/KMeansMojoModel.class
+-rw-r--r--  2.0 unx     2248 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/KMeansMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/
+-rw-r--r--  2.0 unx     4006 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoModel.class
+-rw-r--r--  2.0 unx     2104 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoReader.class
+-rw-r--r--  2.0 unx      981 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoModel$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/
+-rw-r--r--  2.0 unx     1345 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
+-rw-r--r--  2.0 unx     4904 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmMojoReader.class
+-rw-r--r--  2.0 unx     1567 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$5.class
+-rw-r--r--  2.0 unx     2161 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$8.class
+-rw-r--r--  2.0 unx     1232 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
+-rw-r--r--  2.0 unx     1980 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
+-rw-r--r--  2.0 unx      875 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
+-rw-r--r--  2.0 unx     2578 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer.class
+-rw-r--r--  2.0 unx     1219 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmInitialization.class
+-rw-r--r--  2.0 unx     1075 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$2.class
+-rw-r--r--  2.0 unx     2236 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$9.class
+-rw-r--r--  2.0 unx     1512 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$6.class
+-rw-r--r--  2.0 unx     1186 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$3.class
+-rw-r--r--  2.0 unx     1290 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
+-rw-r--r--  2.0 unx     1406 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
+-rw-r--r--  2.0 unx     9537 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmMojoModel.class
+-rw-r--r--  2.0 unx     1280 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
+-rw-r--r--  2.0 unx      983 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$1.class
+-rw-r--r--  2.0 unx     1510 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$7.class
+-rw-r--r--  2.0 unx     1460 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
+-rw-r--r--  2.0 unx     3178 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss.class
+-rw-r--r--  2.0 unx     1499 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$4.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader$1.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory$1.class
+-rw-r--r--  2.0 unx     1934 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/
+-rw-r--r--  2.0 unx     1045 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/SharedTreeModelAttributes.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/
+-rw-r--r--  2.0 unx      773 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
+-rw-r--r--  2.0 unx      420 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
+-rw-r--r--  2.0 unx      590 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
+-rw-r--r--  2.0 unx      777 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
+-rw-r--r--  2.0 unx      449 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
+-rw-r--r--  2.0 unx      630 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetrics.class
+-rw-r--r--  2.0 unx      748 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
+-rw-r--r--  2.0 unx      785 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
+-rw-r--r--  2.0 unx      789 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
+-rw-r--r--  2.0 unx      517 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
+-rw-r--r--  2.0 unx      993 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/DeepLearningModelAttributes.class
+-rw-r--r--  2.0 unx     5653 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributes.class
+-rw-r--r--  2.0 unx     1267 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/VariableImportances$1.class
+-rw-r--r--  2.0 unx      495 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/SerializedName.class
+-rw-r--r--  2.0 unx     2602 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/VariableImportances.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/Table$ColumnType.class
+-rw-r--r--  2.0 unx     1155 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributes$1.class
+-rw-r--r--  2.0 unx     3376 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/Table.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/
+-rw-r--r--  2.0 unx      874 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ColumnSpecifier.class
+-rw-r--r--  2.0 unx      249 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
+-rw-r--r--  2.0 unx      953 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/KeyValue.class
+-rw-r--r--  2.0 unx     1892 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ModelParameter.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ParameterKey$Type.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/FeatureContribution.class
+-rw-r--r--  2.0 unx     1176 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ParameterKey.class
+-rw-r--r--  2.0 unx     1263 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/StringPair.class
+-rw-r--r--  2.0 unx     1768 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader$1.class
+-rw-r--r--  2.0 unx     2522 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributesGLM.class
+-rw-r--r--  2.0 unx    15710 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader.class
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$2.class
+-rw-r--r--  2.0 unx     1551 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$4.class
+-rw-r--r--  2.0 unx     1127 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
+-rw-r--r--  2.0 unx     5010 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/util/
+-rw-r--r--  2.0 unx    10148 b- defN 23-Apr-28 12:08 water/util/H2OPredictor.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Apr-28 12:08 water/util/H2OPredictor$1.class
+-rw-r--r--  2.0 unx     2742 b- defN 23-Apr-28 12:08 water/util/JavaVersionUtils.class
+-rw-r--r--  2.0 unx      971 b- defN 23-Apr-28 12:08 water/util/ModelUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/genmodel/
+-rw-r--r--  2.0 unx      873 b- defN 23-Apr-28 12:08 water/genmodel/AbstractBuildVersion$1.class
+-rw-r--r--  2.0 unx     2965 b- defN 23-Apr-28 12:08 water/genmodel/AbstractBuildVersion.class
+-rw-r--r--  2.0 unx      922 b- defN 23-Apr-28 12:08 water/genmodel/BuildVersion.class
+-rw-r--r--  2.0 unx      921 b- defN 23-Apr-28 12:08 water/genmodel/IGeneratedModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/services/
+-rw-r--r--  2.0 unx       29 b- defN 23-Apr-28 12:08 META-INF/services/hex.genmodel.tools.MojoPrinter
+359 files, 759160 bytes uncompressed, 372212 bytes compressed:  51.0%
```

#### water/genmodel/BuildVersion.class

##### procyon -ec {}

```diff
@@ -4,26 +4,26 @@
 public class BuildVersion extends AbstractBuildVersion
 {
     public String branchName() {
         return "rel-zz_kurka";
     }
     
     public String lastCommitHash() {
-        return "8c77ce3c7e274a73ac5ab0ccf48e845f01362e42";
+        return "5ff8870f912c6110d7b6988f577c020de10496ec";
     }
     
     public String describe() {
-        return "jenkins-master-6107-52-g8c77ce3";
+        return "jenkins-3.40.0.3-122-g5ff8870";
     }
     
     public String projectVersion() {
-        return "3.40.0.2";
+        return "3.40.0.4";
     }
     
     public String compiledOn() {
-        return "2023-03-09 15:17:18";
+        return "2023-04-28 12:08:23";
     }
     
     public String compiledBy() {
         return "jenkins";
     }
 }
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pickle-1.3.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pickle-1.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-statsmodels-1.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-sklearn-1.7.27.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-python-1.1.14.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-python-1.1.14.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-h2o-1.2.5.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-h2o-1.2.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/classpath.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sklearn2pmml-1.0-SNAPSHOT.jar
 gson-2.10.jar
 guava-21.0.jar
-h2o-genmodel-3.40.0.2.jar
-h2o-logger-3.40.0.2.jar
+h2o-genmodel-3.40.0.4.jar
+h2o-logger-3.40.0.4.jar
 h2o-tree-api-0.3.17.jar
 istack-commons-runtime-4.0.1.jar
 jackson-annotations-2.13.3.jar
 jakarta.activation-2.0.1.jar
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5702 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Apr-02 08:06 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-02 08:06 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-Apr-02 08:06 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Apr-02 08:06 com/sklearn2pmml/Main$1.class
+Zip file size: 5703 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-May-01 09:28 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-01 09:28 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-01 09:28 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-May-01 09:28 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-May-01 09:28 com/sklearn2pmml/Main$1.class
 -rw-rw-r--  2.0 unx     7844 b- defN 23-Apr-02 08:05 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Apr-02 08:06 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4226 bytes compressed:  67.5%
+-rw-rw-r--  2.0 unx       70 b- defN 23-May-01 09:28 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4227 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.92.0
+Implementation-Version: 0.92.1
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.2.2
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/pmml-lightgbm-1.4.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/h2o-logger-3.40.0.2.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 4526 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-09 15:17 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Mar-09 15:17 water/logging/
--rw-r--r--  2.0 unx     1853 b- defN 23-Mar-09 15:17 water/logging/Slf4JLogger.class
--rw-r--r--  2.0 unx      379 b- defN 23-Mar-09 15:17 water/logging/Logger.class
--rw-r--r--  2.0 unx     2473 b- defN 23-Mar-09 15:17 water/logging/LoggerFactory.class
--rw-r--r--  2.0 unx     1686 b- defN 23-Mar-09 15:17 water/logging/ConsoleLogger.class
--rw-r--r--  2.0 unx     1114 b- defN 23-Mar-09 15:17 water/logging/LoggingLevel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-28 12:08 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/logging/
+-rw-r--r--  2.0 unx     1853 b- defN 23-Apr-28 12:08 water/logging/Slf4JLogger.class
+-rw-r--r--  2.0 unx      379 b- defN 23-Apr-28 12:08 water/logging/Logger.class
+-rw-r--r--  2.0 unx     2473 b- defN 23-Apr-28 12:08 water/logging/LoggerFactory.class
+-rw-r--r--  2.0 unx     1686 b- defN 23-Apr-28 12:08 water/logging/ConsoleLogger.class
+-rw-r--r--  2.0 unx     1114 b- defN 23-Apr-28 12:08 water/logging/LoggingLevel.class
 9 files, 7530 bytes uncompressed, 3412 bytes compressed:  54.7%
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.92.1/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,17 +296,18 @@
 		return _col2d(Xt)
 
 class LookupTransformer(BaseEstimator, TransformerMixin):
 	"""Re-map 1D categorical data.
 
 	If the mapping is not found, returns `default_value`.
 
-	See also
+	See also:
 	--------
 	FilterLookupTransformer
+
 	"""
 
 	def __init__(self, mapping, default_value):
 		if type(mapping) is not dict:
 			raise TypeError("Input value to output value mapping is not a dict")
 		k_type = None
 		v_type = None
@@ -349,17 +350,18 @@
 		return _col2d(Xt)
 
 class FilterLookupTransformer(LookupTransformer):
 	"""Selectively re-map 1D categorical data.
 
 	If the mapping is not found, returns the original value unchanged.
 
-	See also
+	See also:
 	--------
 	LookupTransformer
+
 	"""
 
 	def __init__(self, mapping):
 		super(FilterLookupTransformer, self).__init__(mapping, default_value = None)
 		for k, v in mapping.items():
 			if v is None:
 				raise ValueError("Value is None")
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/xgboost.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from sklearn.preprocessing import LabelBinarizer, OneHotEncoder, OrdinalEncoder
 from sklearn2pmml import _is_categorical
 from sklearn2pmml.preprocessing import PMMLLabelBinarizer
 
 def make_xgboost_dataframe_mapper(dtypes, missing_value_aware = True):
 	"""Construct a DataFrameMapper for feeding complex data into an XGBModel.
 
-	Parameters
+	Parameters:
 	----------
 
 	dtypes: iterable of tuples (column, dtype)
 
 	missing_value_aware: boolean
 		If true, use missing value aware transformers.
 
-	Returns
+	Returns:
 	-------
 	DataFrameMapper
 
 	"""
 	features = list()
 	for column, dtype in dtypes.items():
 		if _is_categorical(dtype):
@@ -28,23 +28,23 @@
 		else:
 			features.append(([column], None))
 	return DataFrameMapper(features)
 
 def make_xgboost_column_transformer(dtypes, missing_value_aware = True):
 	"""Construct a ColumnTransformer for feeding complex data into an XGBModel.
 
-	Parameters
+	Parameters:
 	----------
 
 	dtypes: iterable of tuples (column, dtype)
 
 	missing_value_aware: boolean
 		If true, use missing value aware transformers.
 
-	Returns
+	Returns:
 	-------
 	ColumnTransformer
 
 	"""
 	transformers = list()
 	for column, dtype in dtypes.items():
 		if _is_categorical(dtype):
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.92.1/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from sklearn.preprocessing import LabelEncoder, OrdinalEncoder
 from sklearn2pmml import _is_categorical
 from sklearn2pmml.preprocessing import PMMLLabelEncoder
 
 def make_lightgbm_dataframe_mapper(dtypes, missing_value_aware = True):
 	"""Construct a DataFrameMapper for feeding complex data into a LGBMModel.
 
-	Parameters
+	Parameters:
 	----------
 
 	dtypes: iterable of tuples (column, dtype)
 
 	missing_value_aware: boolean
 		If true, use missing value aware transformers.
 
-	Returns
+	Returns:
 	-------
 	Tuple (DataFrameMapper, list of categorical columns indices)
 
 	"""
 	features = list()
 	categorical_features = list()
 	i = 0
@@ -31,23 +31,24 @@
 			features.append(([column], None))
 		i += 1
 	return (DataFrameMapper(features), categorical_features)
 
 def make_lightgbm_column_transformer(dtypes, missing_value_aware = True):
 	"""Construct a ColumnTransformer for feeding complex data into a LGBMModel.
 
-	Parameters
+	Parameters:
 	----------
 
 	dtypes: iterable of tuples (column, dtype)
 
 	missing_value_aware: boolean
 		If true, use missing value aware transformers.
 
 	Returns:
+	-------
 	Tuple (ColumnTransformer, list of categorical column indices)
 
 	"""
 	transformers = list()
 	categorical_features = list()
 	i = 0
 	for column, dtype in dtypes.items():
```

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.92.1/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.92.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.92.1/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

