# Comparing `tmp/pycm-3.8.tar.gz` & `tmp/pycm-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycm-3.8.tar", last modified: Wed Feb  1 14:11:26 2023, max compression
+gzip compressed data, was "pycm-3.9.tar", last modified: Mon May  1 17:09:00 2023, max compression
```

## Comparing `pycm-3.8.tar` & `pycm-3.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:11:26.716664 pycm-3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-01 14:11:15.000000 pycm-3.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-02-01 14:11:15.000000 pycm-3.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-01 14:11:15.000000 pycm-3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-01 14:11:15.000000 pycm-3.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:11:26.708664 pycm-3.8/Otherfiles/
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/PSF.png
--rw-r--r--   0 runner    (1001) docker     (123)    69490 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52087 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/compare_block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   116776 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/plot1.png
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/plot2.png
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/plot3.png
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/recommendation_block_diagram.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)    67581 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/test.html
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-02-01 14:11:15.000000 pycm-3.8/Otherfiles/test.pycm
--rw-r--r--   0 runner    (1001) docker     (123)    48221 2023-02-01 14:11:26.716664 pycm-3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-02-01 14:11:15.000000 pycm-3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-01 14:11:15.000000 pycm-3.8/TODO.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-01 14:11:15.000000 pycm-3.8/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-01 14:11:15.000000 pycm-3.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:11:26.708664 pycm-3.8/paper/
--rw-r--r--   0 runner    (1001) docker     (123)   125670 2023-02-01 14:11:15.000000 pycm-3.8/paper/10.21105.joss.00729.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-01 14:11:15.000000 pycm-3.8/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-02-01 14:11:15.000000 pycm-3.8/paper/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:11:26.716664 pycm-3.8/pycm/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-01 14:11:15.000000 pycm-3.8/pycm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-01 14:11:15.000000 pycm-3.8/pycm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_class_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)    38225 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    30403 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_overall_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-02-01 14:11:15.000000 pycm-3.8/pycm/pycm_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:11:26.716664 pycm-3.8/pycm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48221 2023-02-01 14:11:26.000000 pycm-3.8/pycm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-01 14:11:26.000000 pycm-3.8/pycm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 14:11:26.000000 pycm-3.8/pycm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-01 14:11:26.000000 pycm-3.8/pycm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-01 14:11:26.000000 pycm-3.8/pycm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-01 14:11:15.000000 pycm-3.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-01 14:11:15.000000 pycm-3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-01 14:11:26.716664 pycm-3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-02-01 14:11:15.000000 pycm-3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-01 17:08:48.000000 pycm-3.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-05-01 17:08:48.000000 pycm-3.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-01 17:08:48.000000 pycm-3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 17:08:48.000000 pycm-3.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.286590 pycm-3.9/Otherfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/PSF.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69490 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52087 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/compare_block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   116776 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/plot3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/recommendation_block_diagram.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    68164 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-05-01 17:08:48.000000 pycm-3.9/Otherfiles/test.pycm
+-rw-r--r--   0 runner    (1001) docker     (123)    49262 2023-05-01 17:09:00.290590 pycm-3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27716 2023-05-01 17:08:48.000000 pycm-3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-01 17:08:48.000000 pycm-3.9/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 17:08:48.000000 pycm-3.9/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 17:08:48.000000 pycm-3.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.286590 pycm-3.9/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)   125670 2023-05-01 17:08:48.000000 pycm-3.9/paper/10.21105.joss.00729.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-01 17:08:48.000000 pycm-3.9/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 17:08:48.000000 pycm-3.9/paper/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/pycm/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-01 17:08:48.000000 pycm-3.9/pycm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-01 17:08:48.000000 pycm-3.9/pycm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21695 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_class_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39335 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_overall_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32973 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-05-01 17:08:48.000000 pycm-3.9/pycm/pycm_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:09:00.290590 pycm-3.9/pycm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49262 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 17:09:00.000000 pycm-3.9/pycm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 17:08:48.000000 pycm-3.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 17:08:48.000000 pycm-3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 17:09:00.290590 pycm-3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-01 17:08:48.000000 pycm-3.9/setup.py
```

### Comparing `pycm-3.8/AUTHORS.md` & `pycm-3.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pycm-3.8/CHANGELOG.md` & `pycm-3.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,54 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [3.9] - 2023-05-01
+### Added
+- `OVERALL_PARAMS` dictionary
+- `__imbalancement_handler__` function
+- `vector_serializer` function
+- NPV micro/macro
+- `log_loss` method
+- 23 new distance/similarity
+	1. Dennis 
+	2. Digby
+	3. Dispersion
+	4. Doolittle
+	5. Eyraud
+	6. Fager & McGowan
+	7. Faith
+	8. Fleiss-Levin-Paik
+	9. Forbes I
+	10. Forbes II
+	11. Fossum
+	12. Gilbert & Wells
+	13. Goodall
+	14. Goodman & Kruskal's Lambda
+	15. Goodman & Kruskal Lambda-r
+	16. Guttman's Lambda A
+	17. Guttman's Lambda B
+	18. Hamann
+	19. Harris & Lahey
+	20. Hawkins & Dotson
+	21. Kendall's Tau
+	22. Kent & Foster I
+	23. Kent & Foster II
+### Changed
+- `metrics_off` parameter added to ConfusionMatrix `__init__` method
+- `CLASS_PARAMS` changed to a dictionary
+- Code style modified
+- `sort` parameter added to `relabel` method
+- Document modified
+- `CONTRIBUTING.md` updated
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
 ## [3.8] - 2023-02-01
 ### Added
 - `distance` method
 - `__contains__` method
 - `__getitem__` method
 - Goodman-Kruskal's Lambda A benchmark
 - Goodman-Kruskal's Lambda B benchmark
@@ -648,15 +688,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.8...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
 [3.2]: https://github.com/sepandhaghighi/pycm/compare/v3.1...v3.2
@@ -690,10 +731,7 @@
 [0.7]: https://github.com/sepandhaghighi/pycm/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/pycm/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/pycm/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/pycm/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/pycm/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/pycm/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/pycm/compare/1e238cd...v0.1
-
-
-
```

### Comparing `pycm-3.8/LICENSE` & `pycm-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/PSF.png` & `pycm-3.9/Otherfiles/PSF.png`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/block_diagram.jpg` & `pycm-3.9/Otherfiles/block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/compare_block_diagram.jpg` & `pycm-3.9/Otherfiles/compare_block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/logo.png` & `pycm-3.9/Otherfiles/logo.png`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/plot1.png` & `pycm-3.9/Otherfiles/plot1.png`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/plot2.png` & `pycm-3.9/Otherfiles/plot2.png`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/plot3.png` & `pycm-3.9/Otherfiles/plot3.png`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/recommendation_block_diagram.jpg` & `pycm-3.9/Otherfiles/recommendation_block_diagram.jpg`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/test.csv` & `pycm-3.9/Otherfiles/test.csv`

 * *Files identical despite different names*

### Comparing `pycm-3.8/Otherfiles/test.html` & `pycm-3.9/Otherfiles/test.html`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,22 @@
 <td style="border:1px solid black;padding:4px;">0.52421</td>
 </tr>
 <tr style="text-align:center;">
 <td style="border:1px solid black;padding:4px;text-align:left;background-color:transparent;"><a href="http://www.pycm.io/doc/index.html#NIR-(No-information-rate)" style="text-decoration:None;">NIR</a></td>
 <td style="border:1px solid black;padding:4px;">0.41667</td>
 </tr>
 <tr style="text-align:center;">
+<td style="border:1px solid black;padding:4px;text-align:left;background-color:aqua;"><a href="http://www.pycm.io/doc/index.html#NPV_Macro" style="text-decoration:None;">NPV Macro</a></td>
+<td style="border:1px solid black;padding:4px;">0.77778</td>
+</tr>
+<tr style="text-align:center;">
+<td style="border:1px solid black;padding:4px;text-align:left;background-color:transparent;"><a href="http://www.pycm.io/doc/index.html#NPV_Micro" style="text-decoration:None;">NPV Micro</a></td>
+<td style="border:1px solid black;padding:4px;">0.79167</td>
+</tr>
+<tr style="text-align:center;">
 <td style="border:1px solid black;padding:4px;text-align:left;background-color:aqua;"><a href="http://www.pycm.io/doc/index.html#Overall_ACC" style="text-decoration:None;">Overall ACC</a></td>
 <td style="border:1px solid black;padding:4px;">0.58333</td>
 </tr>
 <tr style="text-align:center;">
 <td style="border:1px solid black;padding:4px;text-align:left;background-color:transparent;"><a href="http://www.pycm.io/doc/index.html#Overall_CEN" style="text-decoration:None;">Overall CEN</a></td>
 <td style="border:1px solid black;padding:4px;">0.46381</td>
 </tr>
@@ -775,10 +783,10 @@
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;background-color:transparent;"><a href="http://www.pycm.io/doc/index.html#sInd-(Similarity-index)" style="text-decoration:None;">sInd</a></td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.71716</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.61921</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;">0.58547</td>
 <td style="border:1px solid black;padding:4px;border-collapse: collapse;text-align:left;">Similarity index</td>
 </tr>
 </table>
-<p style="text-align:center;border-top:1px solid black;">Generated By <a href="http://www.pycm.io" style="text-decoration:none;color:red;">PyCM</a> Version 3.8</p>
+<p style="text-align:center;border-top:1px solid black;">Generated By <a href="http://www.pycm.io" style="text-decoration:none;color:red;">PyCM</a> Version 3.9</p>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -54,14 +54,16 @@
 Kappa_Standard_Error     0.22036
 Kappa_Unbiased           0.34426
 Krippendorff_Alpha       0.37158
 Lambda_A                 0.42857
 Lambda_B                 0.16667
 Mutual_Information       0.52421
 NIR                      0.41667
+NPV_Macro                0.77778
+NPV_Micro                0.79167
 Overall_ACC              0.58333
 Overall_CEN              0.46381
 Overall_J                (1.225,0.40833)
 Overall_MCC              0.36667
 Overall_MCEN             0.51894
 Overall_RACC             0.35417
 Overall_RACCU            0.36458
@@ -158,8 +160,8 @@
 TOP   3         3          6          Test outcome positive
 TP    3         1          3          True positive/hit
 TPR   0.6       0.5        0.6        Sensitivity, recall, hit rate, or true
                                       positive rate
 Y     0.6       0.3        0.17143    Youden index
 dInd  0.4       0.53852    0.58624    Distance index
 sInd  0.71716   0.61921    0.58547    Similarity index
-Generated By PyCM Version 3.8
+Generated By PyCM Version 3.9
```

### Comparing `pycm-3.8/Otherfiles/test.pycm` & `pycm-3.9/Otherfiles/test.pycm`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 Kappa Standard Error                                              0.22036
 Kappa Unbiased                                                    0.34426
 Krippendorff Alpha                                                0.37158
 Lambda A                                                          0.42857
 Lambda B                                                          0.16667
 Mutual Information                                                0.52421
 NIR                                                               0.41667
+NPV Macro                                                         0.77778
+NPV Micro                                                         0.79167
 Overall ACC                                                       0.58333
 Overall CEN                                                       0.46381
 Overall J                                                         (1.225,0.40833)
 Overall MCC                                                       0.36667
 Overall MCEN                                                      0.51894
 Overall RACC                                                      0.35417
 Overall RACCU                                                     0.36458
```

### Comparing `pycm-3.8/PKG-INFO` & `pycm-3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pycm
-Version: 3.8
+Version: 3.9
 Summary: Multi-class confusion matrix library in Python
 Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.8
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9
 Author: PyCM Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Webpage, https://www.pycm.io
 Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f
 Keywords: confusion-matrix python3 python machine_learning ML
@@ -133,22 +133,22 @@
 ## Installation
 
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.8](https://github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need root access)
+- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
@@ -237,15 +237,15 @@
 
 ```
 
 ### Direct CM
 
 ```pycon
 >>> from pycm import *
->>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2": {"Class1": 0, "Class2": 5}})
+>>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2": {"Class1": 0, "Class2": 5}})
 >>> cm2
 pycm.ConfusionMatrix(classes: ['Class1', 'Class2'])
 >>> cm2.classes
 ['Class1', 'Class2']
 >>> cm2.print_matrix()
 Predict      Class1       Class2       
 Actual
@@ -319,15 +319,15 @@
 `transpose` is added in `version 1.2` in order to transpose input matrix (only in `Direct CM` mode)
 
 ### Relabel
 
 `relabel` method is added in `version 1.5` in order to change ConfusionMatrix classnames.
 
 ```pycon
->>> cm.relabel(mapping={0:"L1",1:"L2",2:"L3"})
+>>> cm.relabel(mapping={0: "L1", 1: "L2", 2: "L3"})
 >>> cm
 pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3'])
 ```
 
 ### Position
 
 `position` method is added in `version 2.8` in order to find the indexes of observations in `predict_vector` which made TP, TN, FP, FN.
@@ -439,34 +439,34 @@
 ['MCC', 'TPR Micro', 'ACC', 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one Loss', 'ERR', 'PPV Micro', 'Overall ACC']
 
 ```
 
 `is_imbalanced` parameter has been added in `version 3.3`, so the user can indicate whether the concerned dataset is imbalanced or not. As long as the user does not provide any information in this regard, the automatic detection algorithm will be used.
 
 ```pycon
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True)
 >>> cm.imbalance
 True
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = False)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
 >>> cm.imbalance
 False
 ```
 
 ### Compare
 
 In `version 2.0`, a method for comparing several confusion matrices is introduced. This option is a combination of several overall and class-based benchmarks. Each of the benchmarks evaluates the performance of the classification algorithm from good to poor and give them a numeric score. The score of good and poor performances are 1 and 0, respectively.
 
 After that, two scores are calculated for each confusion matrices, overall and class-based. The overall score is the average of the score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based score is the average of the score of six class-based benchmarks which are Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power Interpretation, AUC value Interpretation, Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It should be noticed that if one of the benchmarks returns none for one of the classes, that benchmarks will be eliminated in total averaging. If the user sets weights for the classes, the averaging over the value of class-based benchmark scores will transform to a weighted average.
 
 If the user sets the value of `by_class` boolean input `True`, the best confusion matrix is the one with the maximum class-based score. Otherwise, if a confusion matrix obtains the maximum of both overall and class-based scores, that will be reported as the best confusion matrix, but in any other case, the compared object doesn’t select the best confusion matrix.
 
 ```pycon
->>> cm2 = ConfusionMatrix(matrix={0:{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}})
->>> cm3 = ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55, 2:2}})
->>> cp = Compare({"cm2":cm2, "cm3":cm3})
+>>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1: 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}})
+>>> cm3 = ConfusionMatrix(matrix={0: {0: 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}})
+>>> cp = Compare({"cm2": cm2, "cm3": cm3})
 >>> print(cp)
 Best : cm2
 
 Rank  Name   Class-Score       Overall-Score
 1     cm2    0.50278           0.58095
 2     cm3    0.33611           0.52857
 
@@ -502,14 +502,15 @@
 4. `digit`: `int`
 5. `threshold` : `FunctionType (function or lambda)`
 6. `file` : `File object`
 7. `sample_weight` : python `list` or numpy `array` of numbers
 8. `transpose` : `bool`
 9. `classes` : python `list`
 10. `is_imbalanced` : `bool`
+11. `metrics_off` : `bool`
 
 * Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
 
 **Compare**
 
 1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
 2. `by_class` : `bool`
@@ -629,14 +630,54 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [3.9] - 2023-05-01
+### Added
+- `OVERALL_PARAMS` dictionary
+- `__imbalancement_handler__` function
+- `vector_serializer` function
+- NPV micro/macro
+- `log_loss` method
+- 23 new distance/similarity
+	1. Dennis 
+	2. Digby
+	3. Dispersion
+	4. Doolittle
+	5. Eyraud
+	6. Fager & McGowan
+	7. Faith
+	8. Fleiss-Levin-Paik
+	9. Forbes I
+	10. Forbes II
+	11. Fossum
+	12. Gilbert & Wells
+	13. Goodall
+	14. Goodman & Kruskal's Lambda
+	15. Goodman & Kruskal Lambda-r
+	16. Guttman's Lambda A
+	17. Guttman's Lambda B
+	18. Hamann
+	19. Harris & Lahey
+	20. Hawkins & Dotson
+	21. Kendall's Tau
+	22. Kent & Foster I
+	23. Kent & Foster II
+### Changed
+- `metrics_off` parameter added to ConfusionMatrix `__init__` method
+- `CLASS_PARAMS` changed to a dictionary
+- Code style modified
+- `sort` parameter added to `relabel` method
+- Document modified
+- `CONTRIBUTING.md` updated
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
 ## [3.8] - 2023-02-01
 ### Added
 - `distance` method
 - `__contains__` method
 - `__getitem__` method
 - Goodman-Kruskal's Lambda A benchmark
 - Goodman-Kruskal's Lambda B benchmark
@@ -1276,15 +1317,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.8...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
 [3.2]: https://github.com/sepandhaghighi/pycm/compare/v3.1...v3.2
@@ -1318,10 +1360,7 @@
 [0.7]: https://github.com/sepandhaghighi/pycm/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/pycm/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/pycm/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/pycm/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/pycm/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/pycm/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/pycm/compare/1e238cd...v0.1
-
-
-
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pycm Version: 3.8 Summary: Multi-class confusion
+Metadata-Version: 2.1 Name: pycm Version: 3.9 Summary: Multi-class confusion
 matrix library in Python Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.8 Author: PyCM
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9 Author: PyCM
 Development Team Author-email: info@pycm.io License: MIT Project-URL: Webpage,
 https://www.pycm.io Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f Keywords:
 confusion-matrix python3 python machine_learning ML Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -64,21 +64,21 @@
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
 ## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
 **Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.8](https://
-github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://
+**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
+github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
 r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
 Run `python3 setup.py install` or `python setup.py install` (Need root access)
 ### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need
+installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
 root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` (Need root access) - Run `conda install
 -c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
 --upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
 (https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
 and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
 [x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
@@ -101,15 +101,15 @@
 error) 0 2 3 FP(False positive/type 1 error/false alarm) 2 1 2 FPR(Fall-out or
 false positive rate) 0.22222 0.11111 0.33333 N(Condition negative) 9 9 6 P
 (Condition positive or support) 3 3 6 POP(Population) 12 12 12 PPV(Precision or
 positive predictive value) 0.6 0.5 0.6 TN(True negative/correct rejection) 7 8
 4 TON(Test outcome negative) 7 10 7 TOP(Test outcome positive) 5 2 5 TP(True
 positive/hit) 3 1 3 TPR(Sensitivity, recall, hit rate, or true positive rate)
 1.0 0.33333 0.5 ``` ### Direct CM ```pycon >>> from pycm import * >>> cm2 =
-ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2":
+ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2":
 {"Class1": 0, "Class2": 5}}) >>> cm2 pycm.ConfusionMatrix(classes: ['Class1',
 'Class2']) >>> cm2.classes ['Class1', 'Class2'] >>> cm2.print_matrix() Predict
 Class1 Class2 Actual Class1 1 2 Class2 0 5 >>> cm2.print_normalized_matrix()
 Predict Class1 Class2 Actual Class1 0.33333 0.66667 Class2 0.0 1.0 >>> cm2.stat
 (summary=True) Overall Statistics : ACC Macro 0.75 F1 Macro 0.66667 FPR Macro
 0.33333 Kappa 0.38462 Overall ACC 0.75 PPV Macro 0.85714 SOA1(Landis & Koch)
 Fair TPR Macro 0.66667 Zero-one Loss 2 Class Statistics : Classes Class1 Class2
@@ -129,16 +129,16 @@
 `version 0.9.5` in order to load saved confusion matrix with `.obj` format
 generated by `save_obj` method. For more information visit [Example4](http://
 www.pycm.io/doc/Example4.html "Example4") ### Sample weights `sample_weight` is
 added in `version 1.2` For more information visit [Example5](http://
 www.pycm.io/doc/Example5.html "Example5") ### Transpose `transpose` is added in
 `version 1.2` in order to transpose input matrix (only in `Direct CM` mode) ###
 Relabel `relabel` method is added in `version 1.5` in order to change
-ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0:"L1",1:"L2",2:
-"L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
+ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0: "L1", 1: "L2",
+2: "L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
 Position `position` method is added in `version 2.8` in order to find the
 indexes of observations in `predict_vector` which made TP, TN, FP, FN. ```pycon
 >>> cm.position() {0: {'FN': [], 'FP': [0, 7], 'TP': [1, 4, 9], 'TN': [2, 3, 5,
 6, 8, 10, 11]}, 1: {'FN': [5, 10], 'FP': [3], 'TP': [6], 'TN': [0, 1, 2, 4, 7,
 8, 9, 11]}, 2: {'FN': [0, 3, 7], 'FP': [5, 10], 'TP': [2, 8, 11], 'TN': [1, 4,
 6, 9]}} ``` ### To array `to_array` method is added in `version 2.9` in order
 to returns the confusion matrix in the form of a NumPy array. This can be
@@ -200,72 +200,72 @@
 capabilities which had been claimed by the paper. ```pycon >>> cm.imbalance
 False >>> cm.binary False >>> cm.recommended_list ['MCC', 'TPR Micro', 'ACC',
 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one
 Loss', 'ERR', 'PPV Micro', 'Overall ACC'] ``` `is_imbalanced` parameter has
 been added in `version 3.3`, so the user can indicate whether the concerned
 dataset is imbalanced or not. As long as the user does not provide any
 information in this regard, the automatic detection algorithm will be used.
-```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True) >>>
-cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced =
-False) >>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for
-comparing several confusion matrices is introduced. This option is a
-combination of several overall and class-based benchmarks. Each of the
-benchmarks evaluates the performance of the classification algorithm from good
-to poor and give them a numeric score. The score of good and poor performances
-are 1 and 0, respectively. After that, two scores are calculated for each
-confusion matrices, overall and class-based. The overall score is the average
-of the score of seven overall benchmarks which are Landis & Koch, Cramer,
-Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B,
-Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based
-score is the average of the score of six class-based benchmarks which are
-Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio
-Interpretation, Discriminant Power Interpretation, AUC value Interpretation,
-Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It
-should be noticed that if one of the benchmarks returns none for one of the
-classes, that benchmarks will be eliminated in total averaging. If the user
-sets weights for the classes, the averaging over the value of class-based
-benchmark scores will transform to a weighted average. If the user sets the
-value of `by_class` boolean input `True`, the best confusion matrix is the one
-with the maximum class-based score. Otherwise, if a confusion matrix obtains
-the maximum of both overall and class-based scores, that will be reported as
-the best confusion matrix, but in any other case, the compared object doesnât
-select the best confusion matrix. ```pycon >>> cm2 = ConfusionMatrix(matrix={0:
-{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}}) >>> cm3 =
-ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55,
-2:2}}) >>> cp = Compare({"cm2":cm2, "cm3":cm3}) >>> print(cp) Best : cm2 Rank
-Name Class-Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>>
-cp.best pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3']
->>> cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
+```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True) >>>
+cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
+>>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for comparing
+several confusion matrices is introduced. This option is a combination of
+several overall and class-based benchmarks. Each of the benchmarks evaluates
+the performance of the classification algorithm from good to poor and give them
+a numeric score. The score of good and poor performances are 1 and 0,
+respectively. After that, two scores are calculated for each confusion
+matrices, overall and class-based. The overall score is the average of the
+score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews,
+Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha,
+and Pearson's C. In the same manner, the class-based score is the average of
+the score of six class-based benchmarks which are Positive Likelihood Ratio
+Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power
+Interpretation, AUC value Interpretation, Matthews Correlation Coefficient
+Interpretation and Yule's Q Interpretation. It should be noticed that if one of
+the benchmarks returns none for one of the classes, that benchmarks will be
+eliminated in total averaging. If the user sets weights for the classes, the
+averaging over the value of class-based benchmark scores will transform to a
+weighted average. If the user sets the value of `by_class` boolean input
+`True`, the best confusion matrix is the one with the maximum class-based
+score. Otherwise, if a confusion matrix obtains the maximum of both overall and
+class-based scores, that will be reported as the best confusion matrix, but in
+any other case, the compared object doesnât select the best confusion matrix.
+```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
+50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
+50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
+Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
+Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
+pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
+cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
 `version 1.1` in order to open each statistics definition in web browser
 ```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
 ("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
 calling `online_help()` (without argument) * If PyCM website is not available,
 set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
 **ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
 stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
 stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
 `FunctionType (function or lambda)` 6. `file` : `File object` 7.
 `sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` * Run `help
-(ConfusionMatrix)` for `ConfusionMatrix` object details **Compare** 1.
-`cm_dict` : python `dict` of `ConfusionMatrix` object (`str` :
-`ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` : python `dict` of
-class weights (`class_name` : `float`) 4. `class_benchmark_weight`: python
-`dict` of class benchmark weights (`class_benchmark_name` : `float`) 5.
-`overall_benchmark_weight`: python `dict` of overall benchmark weights
-(`overall_benchmark_name` : `float`) 6. `digit`: `int` * Run `help(Compare)`
-for `Compare` object details **ROCCurve** 1. `actual_vector` : python `list` or
-numpy `array` of any stringable objects 2. `probs` : python `list` or numpy
-`array` 3. `classes` : python `list` 4. `thresholds`: python `list` or numpy
-`array` 5. `sample_weight`: python `list` or numpy `array` **PRCurve** 1.
+`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
+`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
+object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
+object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
+python `dict` of class weights (`class_name` : `float`) 4.
+`class_benchmark_weight`: python `dict` of class benchmark weights
+(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
+of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
+`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
 `actual_vector` : python `list` or numpy `array` of any stringable objects 2.
 `probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
 `thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` For more information visit [here](https://github.com/
-sepandhaghighi/pycm/tree/master/Document "Document")
+or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
+`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
+3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
+`sample_weight`: python `list` or numpy `array` For more information visit
+[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
@@ -313,17 +313,29 @@
 ## Show your support ### Star this repo Give a â­ï¸ if this project helped
 you! ### Donate to our project If you do like our project and we hope that you
 do, can you please support us? Our project is not and is never going to be
 working for profit. We need the money just so we can continue doing what we do
 ;-) . [PyCM_Donation] # Changelog All notable changes to this project will be
 documented in this file. The format is based on [Keep a Changelog](http://
 keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.8] - 2023-02-01 ###
-Added - `distance` method - `__contains__` method - `__getitem__` method -
-Goodman-Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.9] - 2023-05-01 ###
+Added - `OVERALL_PARAMS` dictionary - `__imbalancement_handler__` function -
+`vector_serializer` function - NPV micro/macro - `log_loss` method - 23 new
+distance/similarity 1. Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6.
+Fager & McGowan 7. Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11.
+Fossum 12. Gilbert & Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15.
+Goodman & Kruskal Lambda-r 16. Guttman's Lambda A 17. Guttman's Lambda B 18.
+Hamann 19. Harris & Lahey 20. Hawkins & Dotson 21. Kendall's Tau 22. Kent &
+Foster I 23. Kent & Foster II ### Changed - `metrics_off` parameter added to
+ConfusionMatrix `__init__` method - `CLASS_PARAMS` changed to a dictionary -
+Code style modified - `sort` parameter added to `relabel` method - Document
+modified - `CONTRIBUTING.md` updated - `codecov` removed from `dev-
+requirements.txt` - Test system modified ## [3.8] - 2023-02-01 ### Added -
+`distance` method - `__contains__` method - `__getitem__` method - Goodman-
+Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
 Krippendorff's Alpha benchmark - Pearson's C benchmark - 30 new distance/
 similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta 4. Baroni-Urbani
 & Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7. Baulieu I 8.
 Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu VI 13.
 Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI 18.
 Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I 23.
 Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni &
@@ -520,17 +532,18 @@
 benchmark - `overall_stat` ## [0.2] - 2018-01-24 ### Added - Population -
 Condition positive - Condition negative - Test outcome positive - Test outcome
 negative - Prevalence - G-measure - Matrix method - Normalized matrix method -
 Params method ### Changed - `statistic_result` to `class_stat` - `params` to
 `stat` ## [0.1] - 2018-01-22 ### Added - ACC - BM - DOR - F1-Score - FDR - FNR
 - FOR - FPR - LR+ - LR- - MCC - MK - NPV - PPV - TNR - TPR - documents and
 `README.md` [Unreleased]: https://github.com/sepandhaghighi/pycm/compare/
-v3.8...dev [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
-[3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https:
-//github.com/sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
+v3.9...dev [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
+[3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https:
+//github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
+sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
 sepandhaghighi/pycm/compare/v3.4...v3.5 [3.4]: https://github.com/
 sepandhaghighi/pycm/compare/v3.3...v3.4 [3.3]: https://github.com/
 sepandhaghighi/pycm/compare/v3.2...v3.3 [3.2]: https://github.com/
 sepandhaghighi/pycm/compare/v3.1...v3.2 [3.1]: https://github.com/
 sepandhaghighi/pycm/compare/v3.0...v3.1 [3.0]: https://github.com/
 sepandhaghighi/pycm/compare/v2.9...v3.0 [2.9]: https://github.com/
 sepandhaghighi/pycm/compare/v2.8...v2.9 [2.8]: https://github.com/
```

### Comparing `pycm-3.8/README.md` & `pycm-3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,22 @@
 ## Installation
 
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.8](https://github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need root access)
+- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
@@ -194,15 +194,15 @@
 
 ```
 
 ### Direct CM
 
 ```pycon
 >>> from pycm import *
->>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2": {"Class1": 0, "Class2": 5}})
+>>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2": {"Class1": 0, "Class2": 5}})
 >>> cm2
 pycm.ConfusionMatrix(classes: ['Class1', 'Class2'])
 >>> cm2.classes
 ['Class1', 'Class2']
 >>> cm2.print_matrix()
 Predict      Class1       Class2       
 Actual
@@ -276,15 +276,15 @@
 `transpose` is added in `version 1.2` in order to transpose input matrix (only in `Direct CM` mode)
 
 ### Relabel
 
 `relabel` method is added in `version 1.5` in order to change ConfusionMatrix classnames.
 
 ```pycon
->>> cm.relabel(mapping={0:"L1",1:"L2",2:"L3"})
+>>> cm.relabel(mapping={0: "L1", 1: "L2", 2: "L3"})
 >>> cm
 pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3'])
 ```
 
 ### Position
 
 `position` method is added in `version 2.8` in order to find the indexes of observations in `predict_vector` which made TP, TN, FP, FN.
@@ -396,34 +396,34 @@
 ['MCC', 'TPR Micro', 'ACC', 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one Loss', 'ERR', 'PPV Micro', 'Overall ACC']
 
 ```
 
 `is_imbalanced` parameter has been added in `version 3.3`, so the user can indicate whether the concerned dataset is imbalanced or not. As long as the user does not provide any information in this regard, the automatic detection algorithm will be used.
 
 ```pycon
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True)
 >>> cm.imbalance
 True
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = False)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
 >>> cm.imbalance
 False
 ```
 
 ### Compare
 
 In `version 2.0`, a method for comparing several confusion matrices is introduced. This option is a combination of several overall and class-based benchmarks. Each of the benchmarks evaluates the performance of the classification algorithm from good to poor and give them a numeric score. The score of good and poor performances are 1 and 0, respectively.
 
 After that, two scores are calculated for each confusion matrices, overall and class-based. The overall score is the average of the score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based score is the average of the score of six class-based benchmarks which are Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power Interpretation, AUC value Interpretation, Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It should be noticed that if one of the benchmarks returns none for one of the classes, that benchmarks will be eliminated in total averaging. If the user sets weights for the classes, the averaging over the value of class-based benchmark scores will transform to a weighted average.
 
 If the user sets the value of `by_class` boolean input `True`, the best confusion matrix is the one with the maximum class-based score. Otherwise, if a confusion matrix obtains the maximum of both overall and class-based scores, that will be reported as the best confusion matrix, but in any other case, the compared object doesn’t select the best confusion matrix.
 
 ```pycon
->>> cm2 = ConfusionMatrix(matrix={0:{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}})
->>> cm3 = ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55, 2:2}})
->>> cp = Compare({"cm2":cm2, "cm3":cm3})
+>>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1: 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}})
+>>> cm3 = ConfusionMatrix(matrix={0: {0: 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}})
+>>> cp = Compare({"cm2": cm2, "cm3": cm3})
 >>> print(cp)
 Best : cm2
 
 Rank  Name   Class-Score       Overall-Score
 1     cm2    0.50278           0.58095
 2     cm3    0.33611           0.52857
 
@@ -459,14 +459,15 @@
 4. `digit`: `int`
 5. `threshold` : `FunctionType (function or lambda)`
 6. `file` : `File object`
 7. `sample_weight` : python `list` or numpy `array` of numbers
 8. `transpose` : `bool`
 9. `classes` : python `list`
 10. `is_imbalanced` : `bool`
+11. `metrics_off` : `bool`
 
 * Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
 
 **Compare**
 
 1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
 2. `by_class` : `bool`
```

#### html2text {}

```diff
@@ -39,21 +39,21 @@
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
 ## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
 **Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.8](https://
-github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://
+**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
+github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
 r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
 Run `python3 setup.py install` or `python setup.py install` (Need root access)
 ### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need
+installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
 root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` (Need root access) - Run `conda install
 -c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
 --upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
 (https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
 and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
 [x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
@@ -76,15 +76,15 @@
 error) 0 2 3 FP(False positive/type 1 error/false alarm) 2 1 2 FPR(Fall-out or
 false positive rate) 0.22222 0.11111 0.33333 N(Condition negative) 9 9 6 P
 (Condition positive or support) 3 3 6 POP(Population) 12 12 12 PPV(Precision or
 positive predictive value) 0.6 0.5 0.6 TN(True negative/correct rejection) 7 8
 4 TON(Test outcome negative) 7 10 7 TOP(Test outcome positive) 5 2 5 TP(True
 positive/hit) 3 1 3 TPR(Sensitivity, recall, hit rate, or true positive rate)
 1.0 0.33333 0.5 ``` ### Direct CM ```pycon >>> from pycm import * >>> cm2 =
-ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2":
+ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2":
 {"Class1": 0, "Class2": 5}}) >>> cm2 pycm.ConfusionMatrix(classes: ['Class1',
 'Class2']) >>> cm2.classes ['Class1', 'Class2'] >>> cm2.print_matrix() Predict
 Class1 Class2 Actual Class1 1 2 Class2 0 5 >>> cm2.print_normalized_matrix()
 Predict Class1 Class2 Actual Class1 0.33333 0.66667 Class2 0.0 1.0 >>> cm2.stat
 (summary=True) Overall Statistics : ACC Macro 0.75 F1 Macro 0.66667 FPR Macro
 0.33333 Kappa 0.38462 Overall ACC 0.75 PPV Macro 0.85714 SOA1(Landis & Koch)
 Fair TPR Macro 0.66667 Zero-one Loss 2 Class Statistics : Classes Class1 Class2
@@ -104,16 +104,16 @@
 `version 0.9.5` in order to load saved confusion matrix with `.obj` format
 generated by `save_obj` method. For more information visit [Example4](http://
 www.pycm.io/doc/Example4.html "Example4") ### Sample weights `sample_weight` is
 added in `version 1.2` For more information visit [Example5](http://
 www.pycm.io/doc/Example5.html "Example5") ### Transpose `transpose` is added in
 `version 1.2` in order to transpose input matrix (only in `Direct CM` mode) ###
 Relabel `relabel` method is added in `version 1.5` in order to change
-ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0:"L1",1:"L2",2:
-"L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
+ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0: "L1", 1: "L2",
+2: "L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
 Position `position` method is added in `version 2.8` in order to find the
 indexes of observations in `predict_vector` which made TP, TN, FP, FN. ```pycon
 >>> cm.position() {0: {'FN': [], 'FP': [0, 7], 'TP': [1, 4, 9], 'TN': [2, 3, 5,
 6, 8, 10, 11]}, 1: {'FN': [5, 10], 'FP': [3], 'TP': [6], 'TN': [0, 1, 2, 4, 7,
 8, 9, 11]}, 2: {'FN': [0, 3, 7], 'FP': [5, 10], 'TP': [2, 8, 11], 'TN': [1, 4,
 6, 9]}} ``` ### To array `to_array` method is added in `version 2.9` in order
 to returns the confusion matrix in the form of a NumPy array. This can be
@@ -175,72 +175,72 @@
 capabilities which had been claimed by the paper. ```pycon >>> cm.imbalance
 False >>> cm.binary False >>> cm.recommended_list ['MCC', 'TPR Micro', 'ACC',
 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one
 Loss', 'ERR', 'PPV Micro', 'Overall ACC'] ``` `is_imbalanced` parameter has
 been added in `version 3.3`, so the user can indicate whether the concerned
 dataset is imbalanced or not. As long as the user does not provide any
 information in this regard, the automatic detection algorithm will be used.
-```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True) >>>
-cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced =
-False) >>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for
-comparing several confusion matrices is introduced. This option is a
-combination of several overall and class-based benchmarks. Each of the
-benchmarks evaluates the performance of the classification algorithm from good
-to poor and give them a numeric score. The score of good and poor performances
-are 1 and 0, respectively. After that, two scores are calculated for each
-confusion matrices, overall and class-based. The overall score is the average
-of the score of seven overall benchmarks which are Landis & Koch, Cramer,
-Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B,
-Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based
-score is the average of the score of six class-based benchmarks which are
-Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio
-Interpretation, Discriminant Power Interpretation, AUC value Interpretation,
-Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It
-should be noticed that if one of the benchmarks returns none for one of the
-classes, that benchmarks will be eliminated in total averaging. If the user
-sets weights for the classes, the averaging over the value of class-based
-benchmark scores will transform to a weighted average. If the user sets the
-value of `by_class` boolean input `True`, the best confusion matrix is the one
-with the maximum class-based score. Otherwise, if a confusion matrix obtains
-the maximum of both overall and class-based scores, that will be reported as
-the best confusion matrix, but in any other case, the compared object doesnât
-select the best confusion matrix. ```pycon >>> cm2 = ConfusionMatrix(matrix={0:
-{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}}) >>> cm3 =
-ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55,
-2:2}}) >>> cp = Compare({"cm2":cm2, "cm3":cm3}) >>> print(cp) Best : cm2 Rank
-Name Class-Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>>
-cp.best pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3']
->>> cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
+```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True) >>>
+cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
+>>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for comparing
+several confusion matrices is introduced. This option is a combination of
+several overall and class-based benchmarks. Each of the benchmarks evaluates
+the performance of the classification algorithm from good to poor and give them
+a numeric score. The score of good and poor performances are 1 and 0,
+respectively. After that, two scores are calculated for each confusion
+matrices, overall and class-based. The overall score is the average of the
+score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews,
+Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha,
+and Pearson's C. In the same manner, the class-based score is the average of
+the score of six class-based benchmarks which are Positive Likelihood Ratio
+Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power
+Interpretation, AUC value Interpretation, Matthews Correlation Coefficient
+Interpretation and Yule's Q Interpretation. It should be noticed that if one of
+the benchmarks returns none for one of the classes, that benchmarks will be
+eliminated in total averaging. If the user sets weights for the classes, the
+averaging over the value of class-based benchmark scores will transform to a
+weighted average. If the user sets the value of `by_class` boolean input
+`True`, the best confusion matrix is the one with the maximum class-based
+score. Otherwise, if a confusion matrix obtains the maximum of both overall and
+class-based scores, that will be reported as the best confusion matrix, but in
+any other case, the compared object doesnât select the best confusion matrix.
+```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
+50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
+50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
+Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
+Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
+pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
+cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
 `version 1.1` in order to open each statistics definition in web browser
 ```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
 ("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
 calling `online_help()` (without argument) * If PyCM website is not available,
 set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
 **ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
 stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
 stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
 `FunctionType (function or lambda)` 6. `file` : `File object` 7.
 `sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` * Run `help
-(ConfusionMatrix)` for `ConfusionMatrix` object details **Compare** 1.
-`cm_dict` : python `dict` of `ConfusionMatrix` object (`str` :
-`ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` : python `dict` of
-class weights (`class_name` : `float`) 4. `class_benchmark_weight`: python
-`dict` of class benchmark weights (`class_benchmark_name` : `float`) 5.
-`overall_benchmark_weight`: python `dict` of overall benchmark weights
-(`overall_benchmark_name` : `float`) 6. `digit`: `int` * Run `help(Compare)`
-for `Compare` object details **ROCCurve** 1. `actual_vector` : python `list` or
-numpy `array` of any stringable objects 2. `probs` : python `list` or numpy
-`array` 3. `classes` : python `list` 4. `thresholds`: python `list` or numpy
-`array` 5. `sample_weight`: python `list` or numpy `array` **PRCurve** 1.
+`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
+`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
+object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
+object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
+python `dict` of class weights (`class_name` : `float`) 4.
+`class_benchmark_weight`: python `dict` of class benchmark weights
+(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
+of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
+`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
 `actual_vector` : python `list` or numpy `array` of any stringable objects 2.
 `probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
 `thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` For more information visit [here](https://github.com/
-sepandhaghighi/pycm/tree/master/Document "Document")
+or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
+`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
+3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
+`sample_weight`: python `list` or numpy `array` For more information visit
+[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
```

### Comparing `pycm-3.8/TODO.md` & `pycm-3.9/TODO.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,8 @@
   - [x] Overall CEN
   - [x] Overall MCEN
   - [x] AUNU
   - [x] AUNP
   - [x] Overall MCC
   - [x] CBA
   - [x] RCI
-  - [x] Pearson's C
+  - [x] Pearson's C
```

### Comparing `pycm-3.8/paper/10.21105.joss.00729.pdf` & `pycm-3.9/paper/10.21105.joss.00729.pdf`

 * *Files identical despite different names*

### Comparing `pycm-3.8/paper/paper.bib` & `pycm-3.9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `pycm-3.8/paper/paper.md` & `pycm-3.9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `pycm-3.8/pycm/__main__.py` & `pycm-3.9/pycm/__main__.py`

 * *Files identical despite different names*

### Comparing `pycm-3.8/pycm/pycm_ci.py` & `pycm-3.9/pycm/pycm_ci.py`

 * *Files identical despite different names*

### Comparing `pycm-3.8/pycm/pycm_class_func.py` & `pycm-3.9/pycm/pycm_class_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
     :param FP: false positive
     :type FP: dict
     :param FN: false negative
     :type FN: dict
     :return: basic statistics as dict
     """
     result = {}
-    for i in CLASS_PARAMS:
+    for i in CLASS_PARAMS.keys():
         result[i] = {}
     result["TP"] = TP
     result["TN"] = TN
     result["FP"] = FP
     result["FN"] = FN
     return result
```

### Comparing `pycm-3.8/pycm/pycm_compare.py` & `pycm-3.9/pycm/pycm_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 from warnings import warn
 
 
 class Compare():
     """
     Compare class.
 
-    >>> cm1 = ConfusionMatrix(matrix={0:{0:2,1:50,2:6},1:{0:5,1:50,2:3},2:{0:1,1:7,2:50}})
-    >>> cm2 = ConfusionMatrix(matrix={0:{0:50,1:2,2:6},1:{0:50,1:5,2:3},2:{0:1,1:55,2:2}})
-    >>> cp = Compare({"cm1":cm1,"cm2":cm2})
+    >>> cm1 = ConfusionMatrix(matrix={0:{0:2,1:50,2:6}, 1:{0:5,1:50,2:3}, 2:{0:1,1:7,2:50}})
+    >>> cm2 = ConfusionMatrix(matrix={0:{0:50,1:2,2:6}, 1:{0:50,1:5,2:3}, 2:{0:1,1:55,2:2}})
+    >>> cp = Compare({"cm1": cm1, "cm2": cm2})
     >>> print(cp)
     Best : cm1
-
-    Rank  Name   Class-Score         Overall-Score
-    1     cm1    3.01667             2.55
-    2     cm2    2.01667             1.98333
-
+    <BLANKLINE>
+    Rank  Name   Class-Score       Overall-Score
+    1     cm1    0.50278           0.58095
+    2     cm2    0.33611           0.52857
+    <BLANKLINE>
     >>> cp.best
     pycm.ConfusionMatrix(classes: [0, 1, 2])
     >>> cp.sorted
     ['cm1', 'cm2']
     >>> cp.best_name
     'cm1'
     """
@@ -78,18 +78,16 @@
                 self.best_name = max_class_name
             else:
                 if max_overall_name == max_class_name:
                     self.best = cm_dict[max_class_name]
                     self.best_name = max_overall_name
                 else:
                     warn(COMPARE_RESULT_WARNING, RuntimeWarning)
-                    # print('Warning: ' + COMPARE_RESULT_WARNING)
         else:
             warn(COMPARE_RESULT_WARNING, RuntimeWarning)
-            # print('Warning: ' + COMPARE_RESULT_WARNING)
 
     def print_report(self):
         """
         Print Compare report.
 
         :return: None
         """
@@ -230,16 +228,14 @@
             compare.scores[x]['overall'],
             compare.scores[x]['class']))
     sorted_by_class.reverse()
     sorted_by_overall.reverse()
     compare.sorted = sorted_by_class
     max_overall_name = sorted_by_overall[0]
     max_class_name = sorted_by_class[0]
-    #max_class_score = compare.scores[max_class_name]["class"]
-    #max_overall_score = compare.scores[max_overall_name]["overall"]
     return (max_overall_name, max_class_name)
 
 
 def __compare_weight_handler__(compare, weight, weight_type):
     """
     Handle different weights validation.
 
@@ -302,23 +298,26 @@
     :return: None
     """
     if not isinstance(cm_dict, dict):
         raise pycmCompareError(COMPARE_FORMAT_ERROR)
     if not all(isinstance(item, ConfusionMatrix)
                for item in cm_dict.values()):
         raise pycmCompareError(COMPARE_TYPE_ERROR)
+    if any(item.metrics_off for item in cm_dict.values()):
+        raise pycmCompareError(COMPARE_METRICS_OFF_ERROR)
     if not list_check_equal([getattr(item, "POP")
                              for item in cm_dict.values()]):
         raise pycmCompareError(COMPARE_DOMAIN_ERROR)
     if len(cm_dict) < 2:
         raise pycmCompareError(COMPARE_NUMBER_ERROR)
     compare.classes = list(cm_dict.values())[0].classes
     compare.class_weight = {k: 1 for k in compare.classes}
     compare.class_benchmark_weight = {k: 1 for k in CLASS_BENCHMARK_LIST}
-    compare.overall_benchmark_weight = {k: 0 if k in KAPPA_BENCHMARK_LIST[1:] else 1 for k in OVERALL_BENCHMARK_LIST}
+    compare.overall_benchmark_weight = {
+        k: 0 if k in KAPPA_BENCHMARK_LIST[1:] else 1 for k in OVERALL_BENCHMARK_LIST}
     compare.digit = digit
     compare.best = None
     compare.best_name = None
     compare.sorted = None
     compare.scores = {k: {"overall": 0, "class": 0}.copy()
                       for k in cm_dict.keys()}
     __compare_weight_handler__(compare, class_weight, "class_weight")
```

### Comparing `pycm-3.8/pycm/pycm_curve.py` & `pycm-3.9/pycm/pycm_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import numpy
 
 
 class Curve:
     """
     Curve class.
 
-    >>> crv = Curve(actual_vector = np.array([1, 1, 2, 2]), probs = np.array([[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]]), classes=[2, 1])
+    >>> import numpy as np
+    >>> crv = Curve(actual_vector=np.array([1, 1, 2, 2]), probs=np.array([[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]]), classes=[2, 1])
     >>> crv.classes
     [2, 1]
     >>> crv.thresholds
     [0.1, 0.2, 0.35, 0.4, 0.6, 0.65, 0.8, 0.9]
     >>> crv.data[2]["TPR"]
     [1.0, 1.0, 1.0, 0.5, 0.5, 0.5, 0.5, 0.0]
     >>> crv.data[2]["FPR"]
@@ -164,14 +165,15 @@
         return "pycm.Curve(classes: " + str(self.classes) + ")"
 
 
 class ROCCurve(Curve):
     """
     ROCCurve class.
 
+    >>> import numpy as np
     >>> crv = ROCCurve(actual_vector = np.array([1, 1, 2, 2]), probs = np.array([[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]]), classes=[2, 1])
     >>> crv.thresholds
     [0.1, 0.2, 0.35, 0.4, 0.6, 0.65, 0.8, 0.9]
     >>> auc_trp = crv.area()
     >>> auc_trp[1]
     0.75
     >>> auc_trp[2]
@@ -205,14 +207,15 @@
         return "pycm.ROCCurve(classes: " + str(self.classes) + ")"
 
 
 class PRCurve(Curve):
     """
     PRCurve class.
 
+    >>> import numpy as np
     >>> crv = PRCurve(actual_vector = np.array([1, 1, 2, 2]), probs = np.array([[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]]), classes=[2, 1])
     >>> crv.thresholds
     [0.1, 0.2, 0.35, 0.4, 0.6, 0.65, 0.8, 0.9]
     >>> auc_trp = crv.area()
     >>> auc_trp[1]
     0.29166666666666663
     >>> auc_trp[2]
```

### Comparing `pycm-3.8/pycm/pycm_error.py` & `pycm-3.9/pycm/pycm_error.py`

 * *Files identical despite different names*

### Comparing `pycm-3.8/pycm/pycm_interpret.py` & `pycm-3.9/pycm/pycm_interpret.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,14 @@
     Analysis Q(Yule's Q) with interpretation table.
 
     :param Q: Yule's Q
     :type Q: float
     :return: interpretation result as str
     """
     try:
-        if Q == "None":
-            return "None"
         if Q < 0.25:
             return "Negligible"
         if Q >= 0.25 and Q < 0.5:
             return "Weak"
         if Q >= 0.5 and Q < 0.75:
             return "Moderate"
         return "Strong"
@@ -29,16 +27,14 @@
     Analysis MCC(Matthews correlation coefficient) with interpretation table.
 
     :param MCC: Matthews correlation coefficient
     :type MCC: float
     :return: interpretation result as str
     """
     try:
-        if MCC == "None":
-            return "None"
         if MCC < 0.3:
             return "Negligible"
         if MCC >= 0.3 and MCC < 0.5:
             return "Weak"
         if MCC >= 0.5 and MCC < 0.7:
             return "Moderate"
         if MCC >= 0.7 and MCC < 0.9:
@@ -53,16 +49,14 @@
     Analysis NLR(Negative likelihood ratio) with interpretation table.
 
     :param NLR: negative likelihood ratio
     :type NLR: float
     :return: interpretation result as str
     """
     try:
-        if NLR == "None":
-            return "None"
         if NLR < 0.1:
             return "Good"
         if NLR >= 0.1 and NLR < 0.2:
             return "Fair"
         if NLR >= 0.2 and NLR < 0.5:
             return "Poor"
         return "Negligible"
@@ -75,16 +69,14 @@
     Analysis Cramer's V with interpretation table.
 
     :param V: Cramer's V
     :type V: float
     :return: interpretation result as str
     """
     try:
-        if V == "None":
-            return "None"
         if V < 0.1:
             return "Negligible"
         if V >= 0.1 and V < 0.2:
             return "Weak"
         if V >= 0.2 and V < 0.4:
             return "Moderate"
         if V >= 0.4 and V < 0.6:
@@ -101,17 +93,14 @@
     Analysis PLR(Positive likelihood ratio) with interpretation table.
 
     :param PLR: positive likelihood ratio
     :type PLR : float
     :return: interpretation result as str
     """
     try:
-
-        if PLR == "None":
-            return "None"
         if PLR < 1:
             return "Negligible"
         if PLR >= 1 and PLR < 5:
             return "Poor"
         if PLR >= 5 and PLR < 10:
             return "Fair"
         return "Good"
@@ -124,16 +113,14 @@
     Analysis DP with interpretation table.
 
     :param DP: discriminant power
     :type DP : float
     :return: interpretation result as str
     """
     try:
-        if DP == "None":
-            return "None"
         if DP < 1:
             return "Poor"
         if DP >= 1 and DP < 2:
             return "Limited"
         if DP >= 2 and DP < 3:
             return "Fair"
         return "Good"
@@ -146,16 +133,14 @@
     Analysis AUC with interpretation table.
 
     :param AUC: area under the ROC curve
     :type AUC : float
     :return: interpretation result as str
     """
     try:
-        if AUC == "None":
-            return "None"
         if AUC < 0.6:
             return "Poor"
         if AUC >= 0.6 and AUC < 0.7:
             return "Fair"
         if AUC >= 0.7 and AUC < 0.8:
             return "Good"
         if AUC >= 0.8 and AUC < 0.9:
```

### Comparing `pycm-3.8/pycm/pycm_obj.py` & `pycm-3.9/pycm/pycm_obj.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 """ConfusionMatrix module."""
 from __future__ import division
 from .pycm_error import pycmVectorError, pycmMatrixError, pycmCIError, pycmAverageError, pycmPlotError
 from .pycm_handler import __class_stat_init__, __overall_stat_init__
 from .pycm_handler import __obj_assign_handler__, __obj_file_handler__, __obj_matrix_handler__, __obj_vector_handler__, __obj_array_handler__
+from .pycm_handler import __imbalancement_handler__
 from .pycm_class_func import F_calc, IBA_calc, TI_calc, NB_calc, sensitivity_index_calc
-from .pycm_overall_func import weighted_kappa_calc, weighted_alpha_calc, alpha2_calc, brier_score_calc
+from .pycm_overall_func import weighted_kappa_calc, weighted_alpha_calc, alpha2_calc, brier_score_calc, log_loss_calc
 from .pycm_distance import DistanceType, DISTANCE_MAPPER
 from .pycm_output import *
 from .pycm_util import *
 from .pycm_param import *
 from .pycm_ci import __CI_overall_handler__, __CI_class_handler__
 import os
 import json
@@ -24,27 +25,32 @@
     >>> y_actu = [2, 0, 2, 2, 0, 1, 1, 2, 2, 0, 1, 2]
     >>> y_pred = [0, 0, 2, 1, 0, 2, 1, 0, 2, 0, 2, 2]
     >>> cm = ConfusionMatrix(y_actu, y_pred)
     >>> cm.classes
     [0, 1, 2]
     >>> cm.table
     {0: {0: 3, 1: 0, 2: 0}, 1: {0: 0, 1: 1, 2: 2}, 2: {0: 2, 1: 1, 2: 3}}
-    >>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2},"Class2": {"Class1": 0, "Class2": 5}})
+    >>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2": {"Class1": 0, "Class2": 5}})
     >>> cm2
     pycm.ConfusionMatrix(classes: ['Class1', 'Class2'])
     """
 
     def __init__(
             self,
             actual_vector=None,
             predict_vector=None,
             matrix=None,
-            digit=5, threshold=None, file=None,
-            sample_weight=None, transpose=False,
-            classes=None, is_imbalanced=None):
+            digit=5,
+            threshold=None,
+            file=None,
+            sample_weight=None,
+            transpose=False,
+            classes=None,
+            is_imbalanced=None,
+            metrics_off=False):
         """
         Init method.
 
         :param actual_vector: actual vector
         :type actual_vector: python list or numpy array of any stringable objects
         :param predict_vector: vector of predictions
         :type predict_vector: python list or numpy array of any stringable objects
@@ -60,17 +66,20 @@
         :type sample_weight: list
         :param transpose: transpose flag
         :type transpose: bool
         :param classes: ordered labels of classes
         :type classes: list
         :param is_imbalanced: imbalance dataset flag
         :type is_imbalanced: bool
+        :param metrics_off: metrics off flag
+        :type metrics_off: bool
         """
         self.actual_vector = actual_vector
         self.predict_vector = predict_vector
+        self.metrics_off = metrics_off
         self.prob_vector = None
         self.digit = digit
         self.weights = None
         self.classes = None
         self.imbalance = None
         if isinstance(transpose, bool):
             self.transpose = transpose
@@ -84,20 +93,18 @@
         elif isinstance(matrix, (list, numpy.ndarray)):
             matrix_param = __obj_array_handler__(
                 matrix, classes, self.transpose)
         else:
             matrix_param = __obj_vector_handler__(
                 self, actual_vector, predict_vector, threshold, sample_weight, classes)
         __obj_assign_handler__(self, matrix_param)
-        __class_stat_init__(self)
-        __overall_stat_init__(self)
-        if self.imbalance is None:
-            if is_imbalanced is None:
-                is_imbalanced = imbalance_check(self.P)
-            self.imbalance = is_imbalanced
+        if not metrics_off:
+            __class_stat_init__(self)
+            __overall_stat_init__(self)
+            __imbalancement_handler__(self, is_imbalanced)
         self.binary = binary_check(self.classes)
         self.recommended_list = statistic_recommend(
             self.classes, self.imbalance)
         self.sparse_matrix = None
         self.sparse_normalized_matrix = None
         self.positions = None
         self.label_map = {x: x for x in self.classes}
@@ -157,14 +164,15 @@
                     classes, normalized_table)
             print(sparse_table_print(self.sparse_normalized_matrix))
         else:
             print(table_print(classes, normalized_table))
         if len(classes) >= CLASS_NUMBER_THRESHOLD:
             warn(CLASS_NUMBER_WARNING, RuntimeWarning)
 
+    @metrics_off_check
     def stat(
             self,
             overall_param=None,
             class_param=None,
             class_name=None,
             summary=False):
         """
@@ -325,18 +333,15 @@
     def save_html(
             self,
             name,
             address=True,
             overall_param=None,
             class_param=None,
             class_name=None,
-            color=(
-                0,
-                0,
-                0),
+            color=(0, 0, 0),
             normalize=False,
             summary=False,
             alt_link=False,
             shortener=True):
         """
         Save ConfusionMatrix in HTML file.
 
@@ -493,22 +498,17 @@
             predict_vector_temp = self.predict_vector
             prob_vector_temp = self.prob_vector
             weights_vector_temp = self.weights
             matrix_temp = {k: self.table[k].copy() for k in self.classes}
             matrix_items = []
             for i in self.classes:
                 matrix_items.append((i, list(matrix_temp[i].items())))
-            if isinstance(actual_vector_temp, numpy.ndarray):
-                actual_vector_temp = actual_vector_temp.tolist()
-            if isinstance(predict_vector_temp, numpy.ndarray):
-                predict_vector_temp = predict_vector_temp.tolist()
-            if isinstance(prob_vector_temp, numpy.ndarray):
-                prob_vector_temp = prob_vector_temp.tolist()
-            if isinstance(weights_vector_temp, numpy.ndarray):
-                weights_vector_temp = weights_vector_temp.tolist()
+            actual_vector_temp, predict_vector_temp, prob_vector_temp, weights_vector_temp = map(
+                vector_serializer, [
+                    actual_vector_temp, predict_vector_temp, prob_vector_temp, weights_vector_temp])
             dump_dict = {"Actual-Vector": actual_vector_temp,
                          "Predict-Vector": predict_vector_temp,
                          "Prob-Vector": prob_vector_temp,
                          "Matrix": matrix_items,
                          "Digit": self.digit,
                          "Sample-Weight": weights_vector_temp,
                          "Transpose": self.transpose,
@@ -545,26 +545,28 @@
                     FP=self.FP[i],
                     FN=self.FN[i],
                     beta=beta)
             return F_dict
         except Exception:
             return {}
 
+    @metrics_off_check
     def sensitivity_index(self):
         """
         Calculate sensitivity index for all classes.
 
         :return: sensitivity index for all classes as dict
         """
         sensitivity_index_dict = {}
         for i in self.classes:
             sensitivity_index_dict[i] = sensitivity_index_calc(
                 self.TPR[i], self.FPR[i])
         return sensitivity_index_dict
 
+    @metrics_off_check
     def IBA_alpha(self, alpha):
         """
         Calculate IBA_alpha score for all classes.
 
         :param alpha: alpha parameter
         :type alpha: float
         :return: IBA_alpha score for all classes as dict
@@ -592,14 +594,15 @@
             for i in self.classes:
                 TI_dict[i] = TI_calc(
                     self.TP[i], self.FP[i], self.FN[i], alpha, beta)
             return TI_dict
         except Exception:
             return {}
 
+    @metrics_off_check
     def NB(self, w=1):
         """
         Calculate Net benefit for all classes.
 
         :param w: weight
         :type w: float
         :return: NB for all classes as dict
@@ -624,14 +627,15 @@
         if not isinstance(metric, DistanceType):
             raise pycmMatrixError(DISTANCE_METRIC_TYPE_ERROR)
         for i in self.classes:
             distance_dict[i] = DISTANCE_MAPPER[metric](
                 TP=self.TP[i], FP=self.FP[i], FN=self.FN[i], TN=self.TN[i])
         return distance_dict
 
+    @metrics_off_check
     def CI(
             self,
             param,
             alpha=0.05,
             one_sided=False,
             binom_method="normal-approx"):
         """
@@ -724,20 +728,22 @@
         """
         Create a copy of the confusion matrix.
 
         :return: copy of the ConfusionMatrix object
         """
         return self.__copy__()
 
-    def relabel(self, mapping):
+    def relabel(self, mapping, sort=False):
         """
         Rename the confusion matrix classes.
 
         :param mapping: mapping dictionary
         :type mapping: dict
+        :param sort: flag for sorting new classes
+        :type sort: bool
         :return: None
         """
         if not isinstance(mapping, dict):
             raise pycmMatrixError(MAPPING_FORMAT_ERROR)
         if set(self.classes) != set(mapping.keys()):
             raise pycmMatrixError(MAPPING_CLASS_NAME_ERROR)
         if len(self.classes) != len(set(mapping.values())):
@@ -765,20 +771,23 @@
             self.class_stat[param] = temp_dict
         temp_label_map = {}
         for prime_label, new_label in self.label_map.items():
             temp_label_map[prime_label] = mapping[new_label]
         self.label_map = temp_label_map
         self.positions = None
         self.classes = [mapping[x] for x in self.classes]
+        if sort:
+            self.classes = sorted(self.classes)
         self.TP = self.class_stat["TP"]
         self.TN = self.class_stat["TN"]
         self.FP = self.class_stat["FP"]
         self.FN = self.class_stat["FN"]
         __class_stat_init__(self)
 
+    @metrics_off_check
     def average(self, param, none_omit=False):
         """
         Calculate the average of the input parameter.
 
         :param param: input parameter
         :type param: str
         :param none_omit: none items omitting flag
@@ -786,14 +795,15 @@
         :return: average of the input parameter
         """
         return self.weighted_average(
             param=param,
             weight=self.POP,
             none_omit=none_omit)
 
+    @metrics_off_check
     def weighted_average(self, param, weight=None, none_omit=False):
         """
         Calculate the weighted average of the input parameter.
 
         :param param: input parameter
         :type param: str
         :param weight: explicitly passes weights
@@ -823,14 +833,15 @@
                     continue
                 weight_list.append(selected_weight[class_name])
                 param_list.append(selected_param[class_name])
             return numpy.average(param_list, weights=weight_list)
         except Exception:
             return "None"
 
+    @metrics_off_check
     def weighted_kappa(self, weight=None):
         """
         Calculate weighted kappa.
 
         :param weight: weight matrix
         :type weight: dict
         :return: weighted kappa as float
@@ -845,14 +856,15 @@
             self.classes,
             self.table,
             self.P,
             self.TOP,
             self.POP,
             weight)
 
+    @metrics_off_check
     def weighted_alpha(self, weight=None):
         """
         Calculate weighted Krippendorff's alpha.
 
         :param weight: weight matrix
         :type weight: dict
         :return: weighted alpha as float
@@ -867,14 +879,15 @@
             self.classes,
             self.table,
             self.P,
             self.TOP,
             self.POP,
             weight)
 
+    @metrics_off_check
     def aickin_alpha(self, max_iter=200, epsilon=0.0001):
         """
         Calculate Aickin's alpha.
 
         :param max_iter: maximum number of iterations
         :type max_iter: int
         :param epsilon: difference threshold
@@ -895,24 +908,46 @@
         Calculate Brier score.
 
         :param pos_class: positive class name
         :type pos_class: int/str
         :return: Brier score as float
         """
         if self.prob_vector is None or not self.binary:
-            raise pycmVectorError(BRIER_SCORE_PROB_ERROR)
+            raise pycmVectorError(BRIER_LOG_LOSS_PROB_ERROR)
         if pos_class is None and isinstance(self.classes[0], str):
-            raise pycmVectorError(BRIER_SCORE_CLASS_ERROR)
+            raise pycmVectorError(BRIER_LOG_LOSS_CLASS_ERROR)
         return brier_score_calc(
             self.classes,
             self.prob_vector,
             self.actual_vector,
             self.weights,
             pos_class)
 
+    def log_loss(self, normalize=True, pos_class=None):
+        """
+        Calculate Log loss.
+
+        :param normalize: normalization flag
+        :type normalize: bool
+        :param pos_class: positive class name
+        :type pos_class: int/str
+        :return: Log loss as float
+        """
+        if self.prob_vector is None or not self.binary:
+            raise pycmVectorError(BRIER_LOG_LOSS_PROB_ERROR)
+        if pos_class is None and isinstance(self.classes[0], str):
+            raise pycmVectorError(BRIER_LOG_LOSS_CLASS_ERROR)
+        return log_loss_calc(
+            self.classes,
+            self.prob_vector,
+            self.actual_vector,
+            normalize,
+            self.weights,
+            pos_class)
+
     def position(self):
         """
         Return indices of TP, FP, TN and FN in the predict_vector.
 
         :return: TP, FP, TN, FN indices separated for each class as dictionary
         """
         if self.predict_vector is None or self.actual_vector is None:
@@ -968,27 +1003,29 @@
                 table = normalized_table_calc(classes, table)
         array = []
         for key in classes:
             row = [table[key][i] for i in classes]
             array.append(row)
         return numpy.array(array)
 
-    def combine(self, other):
+    def combine(self, other, metrics_off=False):
         """
         Return the combination of two confusion matrices.
 
         :param other: the other matrix that is going to be combined
         :type other: pycm.ConfusionMatrix
+        :param metrics_off: metrics off flag
+        :type metrics_off: bool
         :return: the combination of two matrices as a new confusion matrix
         """
         if isinstance(other, ConfusionMatrix) is False:
             raise pycmMatrixError(COMBINE_TYPE_ERROR)
         return ConfusionMatrix(
             matrix=matrix_combine(
-                self.matrix, other.matrix))
+                self.matrix, other.matrix), metrics_off=metrics_off)
 
     def plot(
             self,
             normalized=False,
             one_vs_all=False,
             class_name=None,
             title='Confusion Matrix',
```

### Comparing `pycm-3.8/pycm/pycm_output.py` & `pycm-3.9/pycm/pycm_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,9 +515,9 @@
             webbrowser.open_new_tab(
                 document_link + PARAMS_LINK[params_link_keys[param - 1]])
         else:
             print("Please choose one parameter : \n")
             print('Example : online_help("J") or online_help(2)\n')
             for index, item in enumerate(params_link_keys):
                 print(str(index + 1) + "-" + item)
-    except Exception: # pragma: no cover
+    except Exception:  # pragma: no cover
         print("Error in online help")
```

### Comparing `pycm-3.8/pycm/pycm_overall_func.py` & `pycm-3.9/pycm/pycm_overall_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,59 @@
 import operator as op
 from functools import reduce
 from .pycm_interpret import *
 from .pycm_ci import kappa_SE_calc, CI_calc, SE_calc
 from .pycm_util import complement
 
 
+def log_loss_calc(
+        classes,
+        prob_vector,
+        actual_vector,
+        normalize=True,
+        sample_weight=None,
+        pos_class=None):
+    """
+    Calculate Log loss.
+
+    :param classes: confusion matrix classes
+    :type classes: list
+    :param prob_vector: probability vector
+    :type prob_vector: python list or numpy array
+    :param actual_vector: actual vector
+    :type actual_vector: python list or numpy array
+    :param normalize: normalization flag
+    :type normalize: bool
+    :param sample_weight: sample weights list
+    :type sample_weight: list
+    :param pos_class: positive class name
+    :type pos_class: int/str
+    :return: Log loss as float
+    """
+    try:
+        vector_length = len(actual_vector)
+        if sample_weight is None:
+            sample_weight = [1] * vector_length
+        weight_sum = sum(sample_weight)
+        if pos_class is None:
+            pos_class = max(classes)
+        result = 0
+        for index, item in enumerate(actual_vector):
+            filtered_item = 0
+            if item == pos_class:
+                filtered_item = 1
+            result += -1 * (sample_weight[index] / weight_sum) * ((filtered_item * math.log(
+                prob_vector[index])) + (1 - filtered_item) * math.log(1 - prob_vector[index]))
+        if not normalize:
+            result = result * weight_sum
+        return result
+    except Exception:
+        return "None"
+
+
 def brier_score_calc(
         classes,
         prob_vector,
         actual_vector,
         sample_weight=None,
         pos_class=None):
     """
@@ -71,15 +116,15 @@
     """
     try:
         p_A = {i: TOP[i] / POP[i] for i in classes}
         p_B = {i: P[i] / POP[i] for i in classes}
         step = 1
         alpha = 0
         alpha_prev = 0
-        while(True):
+        while True:
             p_e = 0
             for i in classes:
                 p_e += (p_A[i] * p_B[i])
             alpha_prev = alpha
             alpha = reliability_calc(p_e, ACC)
             for i in classes:
                 p_A[i] = TOP[i] / \
@@ -823,37 +868,37 @@
         return result
     except Exception:
         return "None"
 
 
 def micro_calc(item1, item2):
     """
-    Calculate TPR, TNR, PPV, FNR, FPR, or F1 micro.
+    Calculate TPR, TNR, PPV, NPV, FNR, FPR, or F1 micro.
 
     :param item1: item1 in micro averaging
     :type item1:dict
     :param item2: item2 in micro averaging
     :type item2: dict
-    :return: PPV, TPR, TNR, FNR, FPR, or F1 micro as float
+    :return: PPV, NPV, TPR, TNR, FNR, FPR, or F1 micro as float
     """
     try:
         item1_sum = sum(item1.values())
         item2_sum = sum(item2.values())
         return item1_sum / (item1_sum + item2_sum)
     except Exception:
         return "None"
 
 
 def macro_calc(item):
     """
-    Calculate PPV_Macro and TPR_Macro.
+    Calculate PPV_Macro, NPV_Macro, and TPR_Macro.
 
     :param item: True positive rate (TPR) or Positive predictive value (PPV)
     :type item:dict
-    :return: PPV_Macro or TPR_Macro as float
+    :return: PPV_Macro, NPV_Macro, or TPR_Macro as float
     """
     try:
         item_sum = sum(item.values())
         item_len = len(item.values())
         return item_sum / item_len
     except Exception:
         return "None"
@@ -1032,19 +1077,22 @@
     result["SOA2(Fleiss)"] = kappa_analysis_fleiss(result["Kappa"])
     result["SOA3(Altman)"] = kappa_analysis_altman(result["Kappa"])
     result["SOA4(Cicchetti)"] = kappa_analysis_cicchetti(result["Kappa"])
     result["SOA5(Cramer)"] = V_analysis(result["Cramer V"])
     result["SOA6(Matthews)"] = MCC_analysis(result["Overall MCC"])
     result["SOA7(Lambda A)"] = lambda_analysis(result["Lambda A"])
     result["SOA8(Lambda B)"] = lambda_analysis(result["Lambda B"])
-    result["SOA9(Krippendorff Alpha)"] = alpha_analysis(result["Krippendorff Alpha"])
+    result["SOA9(Krippendorff Alpha)"] = alpha_analysis(
+        result["Krippendorff Alpha"])
     result["SOA10(Pearson C)"] = pearson_C_analysis(result["Pearson C"])
     result["FPR Macro"] = complement(result["TNR Macro"])
     result["FNR Macro"] = complement(result["TPR Macro"])
     result["PPV Macro"] = macro_calc(kwargs["PPV"])
+    result["NPV Macro"] = macro_calc(kwargs["NPV"])
     result["ACC Macro"] = macro_calc(kwargs["ACC"])
     result["F1 Macro"] = macro_calc(kwargs["F1"])
     result["FPR Micro"] = complement(result["TNR Micro"])
     result["FNR Micro"] = complement(result["TPR Micro"])
     result["PPV Micro"] = result["TPR Micro"]
     result["F1 Micro"] = result["TPR Micro"]
+    result["NPV Micro"] = micro_calc(item1=kwargs["TN"], item2=kwargs["FN"])
     return result
```

### Comparing `pycm-3.8/pycm/pycm_param.py` & `pycm-3.9/pycm/pycm_param.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """Parameters and constants."""
-PYCM_VERSION = "3.8"
+PYCM_VERSION = "3.9"
 
 
 OVERVIEW = '''
 PyCM is a multi-class confusion matrix library written in Python that
 supports both input data vectors and direct matrix, and a proper tool for
 post-classification model evaluation that supports most classes and overall
 statistics parameters.
@@ -64,14 +64,15 @@
 PLOT_MARKERS_CLASS_MISMATCH_ERROR = "Given markers and classes have not the same length."
 VECTOR_TYPE_ERROR = "The type of input vectors is assumed to be a list or a NumPy array"
 VECTOR_SIZE_ERROR = "Input vectors must have same length"
 VECTOR_EMPTY_ERROR = "Input vectors are empty"
 VECTOR_ONLY_ERROR = "This option only works in vector mode"
 VECTOR_UNIQUE_CLASS_ERROR = "The classes list isn't unique. It contains duplicated labels."
 CLASS_NUMBER_ERROR = "Number of the classes is lower than 2"
+METRICS_OFF_ERROR = "This method cannot be executed while 'metrics_off=True'."
 CLASSES_ERROR = "Used classes is not a subset of matrix's classes."
 COMPARE_FORMAT_ERROR = "The input type is supposed to be dictionary but it's not!"
 CLASSES_LENGHT_ERROR = "Classes length is not equal to the array length."
 AREA_METHOD_ERROR = "The numeric integral method can only be selected between 'trapezoidal' and 'midpoint'!"
 
 COMPARE_TYPE_ERROR = "The input is supposed to consist of pycm.ConfusionMatrix object but it's not!"
 COMPARE_DOMAIN_ERROR = "The domain of all ConfusionMatrix objects must be same! The sample size or the number " \
@@ -87,29 +88,31 @@
 
 COMPARE_CLASS_WEIGHT_WARNING = "The class_weight format is wrong, the result is for unweighted mode."
 
 COMPARE_CLASS_BENCHMARK_WEIGHT_WARNING = "The class_benchmark_weight format is wrong, the result is for unweighted mode."
 
 COMPARE_OVERALL_BENCHMARK_WEIGHT_WARNING = "The overall_benchmark_weight format is wrong, the result is for unweighted mode."
 
+COMPARE_METRICS_OFF_ERROR = "Compare cannot be executed while in either of matrices 'metrics_off=True'."
+
 COMBINE_TYPE_ERROR = "The input type is supposed to be pycm.ConfusionMatrix object but it's not!"
 
 COMPARE_RESULT_WARNING = "Confusion matrices are too close and the best one can not be recognized."
 
 WEIGHTED_KAPPA_WARNING = "The weight format is wrong, the result is for unweighted kappa."
 
 WEIGHTED_ALPHA_WARNING = "The weight format is wrong, the result is for unweighted alpha."
 
 AVERAGE_WEIGHT_ERROR = "The weight type must be dictionary and also must be specified for all of the classes."
 
 AVERAGE_INVALID_ERROR = "Invalid parameter!"
 
-BRIER_SCORE_CLASS_ERROR = "Actual vector contains string so pos_class should be explicitly specified"
+BRIER_LOG_LOSS_CLASS_ERROR = "Actual vector contains string so pos_class should be explicitly specified"
 
-BRIER_SCORE_PROB_ERROR = "This option only works in binary probability mode"
+BRIER_LOG_LOSS_PROB_ERROR = "This option only works in binary probability mode"
 
 CLASS_NUMBER_WARNING = "The confusion matrix is a high dimension matrix and won't be demonstrated properly.\n" \
                        "If confusion matrix has too many zeros (sparse matrix) you can set `sparse` flag to True in printing functions "\
                        "otherwise by using save_csv method to save the confusion matrix in csv format you'll have better demonstration."
 
 CLASSES_WARNING = "Used classes is not a subset of classes in actual and predict vectors."
 
@@ -119,88 +122,162 @@
 
 DISTANCE_METRIC_TYPE_ERROR = "The metric type must be DistanceType"
 
 CLASS_NUMBER_THRESHOLD = 10
 
 BALANCE_RATIO_THRESHOLD = 3
 
-CLASS_PARAMS = [
-    "TPR",
-    "TNR",
-    "PPV",
-    "NPV",
-    "FNR",
-    "FPR",
-    "FDR",
-    "FOR",
-    "ACC",
-    "F1",
-    "MCC",
-    "BM",
-    "MK",
-    "PLR",
-    "NLR",
-    "DOR",
-    "TP",
-    "TN",
-    "FP",
-    "FN",
-    "POP",
-    "P",
-    "N",
-    "TOP",
-    "TON",
-    "PRE",
-    "G",
-    "RACC",
-    "F0.5",
-    "F2",
-    "ERR",
-    "RACCU",
-    "J",
-    "IS",
-    "CEN",
-    "MCEN",
-    "AUC",
-    "sInd",
-    "dInd",
-    "DP",
-    "Y",
-    "PLRI",
-    "DPI",
-    "AUCI",
-    "GI",
-    "LS",
-    "AM",
-    "BCD",
-    "OP",
-    "IBA",
-    "GM",
-    "Q",
-    "AGM",
-    "NLRI",
-    "MCCI",
-    "AGF",
-    "OC",
-    "OOC",
-    "AUPR",
-    "ICSI",
-    "QI",
-    "HD",
-    "BB"]
+CLASS_PARAMS = {
+    "TPR": "TPR",
+    "TNR": "TNR",
+    "PPV": "PPV",
+    "NPV": "NPV",
+    "FNR": "FNR",
+    "FPR": "FPR",
+    "FDR": "FDR",
+    "FOR": "FOR",
+    "ACC": "ACC",
+    "F1": "F1",
+    "MCC": "MCC",
+    "BM": "BM",
+    "MK": "MK",
+    "PLR": "PLR",
+    "NLR": "NLR",
+    "DOR": "DOR",
+    "TP": "TP",
+    "TN": "TN",
+    "FP": "FP",
+    "FN": "FN",
+    "POP": "POP",
+    "P": "P",
+    "N": "N",
+    "TOP": "TOP",
+    "TON": "TON",
+    "PRE": "PRE",
+    "G": "G",
+    "RACC": "RACC",
+    "F0.5": "F05",
+    "F2": "F2",
+    "ERR": "ERR",
+    "RACCU": "RACCU",
+    "J": "J",
+    "IS": "IS",
+    "CEN": "CEN",
+    "MCEN": "MCEN",
+    "AUC": "AUC",
+    "sInd": "sInd",
+    "dInd": "dInd",
+    "DP": "DP",
+    "Y": "Y",
+    "PLRI": "PLRI",
+    "DPI": "DPI",
+    "AUCI": "AUCI",
+    "GI": "GI",
+    "LS": "LS",
+    "AM": "AM",
+    "BCD": "BCD",
+    "OP": "OP",
+    "IBA": "IBA",
+    "GM": "GM",
+    "Q": "Q",
+    "AGM": "AGM",
+    "NLRI": "NLRI",
+    "MCCI": "MCCI",
+    "AGF": "AGF",
+    "OC": "OC",
+    "OOC": "OOC",
+    "AUPR": "AUPR",
+    "ICSI": "ICSI",
+    "QI": "QI",
+    "HD": "HD",
+    "BB": "BB",
+}
+
+OVERALL_PARAMS = {
+    'Overall ACC': 'Overall_ACC',
+    'Overall RACCU': 'Overall_RACCU',
+    'Overall RACC': 'Overall_RACC',
+    'Kappa': 'Kappa',
+    'Gwet AC1': 'AC1',
+    'Bennett S': 'S',
+    'Kappa Standard Error': 'Kappa_SE',
+    'Kappa Unbiased': 'KappaUnbiased',
+    'Scott PI': 'PI',
+    'Kappa No Prevalence': 'KappaNoPrevalence',
+    'Kappa 95% CI': 'Kappa_CI',
+    'Standard Error': 'SE',
+    '95% CI': 'CI95',
+    'Chi-Squared': 'Chi_Squared',
+    'Phi-Squared': 'Phi_Squared',
+    'Cramer V': 'V',
+    'Response Entropy': 'ResponseEntropy',
+    'Reference Entropy': 'ReferenceEntropy',
+    'Cross Entropy': 'CrossEntropy',
+    'Joint Entropy': 'JointEntropy',
+    'Conditional Entropy': 'ConditionalEntropy',
+    'Mutual Information': 'MutualInformation',
+    'KL Divergence': 'KL',
+    'Lambda B': 'LambdaB',
+    'Lambda A': 'LambdaA',
+    'Chi-Squared DF': 'DF',
+    'Overall J': 'Overall_J',
+    'Hamming Loss': 'HammingLoss',
+    'Zero-one Loss': 'ZeroOneLoss',
+    'NIR': 'NIR',
+    'P-Value': 'PValue',
+    'Overall CEN': 'Overall_CEN',
+    'Overall MCEN': 'Overall_MCEN',
+    'Overall MCC': 'Overall_MCC',
+    'RR': 'RR',
+    'CBA': 'CBA',
+    'AUNU': 'AUNU',
+    'AUNP': 'AUNP',
+    'RCI': 'RCI',
+    'Pearson C': 'C',
+    'TPR Micro': 'TPR_Micro',
+    'TPR Macro': 'TPR_Macro',
+    'CSI': 'CSI',
+    'ARI': 'ARI',
+    'TNR Micro': 'TNR_Micro',
+    'TNR Macro': 'TNR_Macro',
+    'Bangdiwala B': 'B',
+    'Krippendorff Alpha': 'Alpha',
+    'SOA1(Landis & Koch)': 'SOA1',
+    'SOA2(Fleiss)': 'SOA2',
+    'SOA3(Altman)': 'SOA3',
+    'SOA4(Cicchetti)': 'SOA4',
+    'SOA5(Cramer)': 'SOA5',
+    'SOA6(Matthews)': 'SOA6',
+    'SOA7(Lambda A)': 'SOA7',
+    'SOA8(Lambda B)': 'SOA8',
+    'SOA9(Krippendorff Alpha)': 'SOA9',
+    'SOA10(Pearson C)': 'SOA10',
+    'FPR Macro': 'FPR_Macro',
+    'FNR Macro': 'FNR_Macro',
+    'PPV Macro': 'PPV_Macro',
+    'NPV Macro': 'NPV_Macro',
+    'ACC Macro': 'ACC_Macro',
+    'F1 Macro': 'F1_Macro',
+    'FPR Micro': 'FPR_Micro',
+    'FNR Micro': 'FNR_Micro',
+    'PPV Micro': 'PPV_Micro',
+    'NPV Micro': 'NPV_Micro',
+    'F1 Micro': 'F1_Micro',
+}
 
 SUMMARY_OVERALL = [
     "ACC Macro",
     "Kappa",
     "Overall ACC",
     "SOA1(Landis & Koch)",
     "Zero-one Loss",
     "F1 Macro",
     "TPR Macro",
     "PPV Macro",
+    "NPV Macro",
     "FPR Macro"]
 
 SUMMARY_CLASS = [
     "ACC",
     "AUC",
     "AUCI",
     "F1",
@@ -267,14 +344,15 @@
 
 MULTICLASS_RECOMMEND = [
     "ERR",
     "TPR Micro",
     "TPR Macro",
     "F1 Macro",
     "PPV Macro",
+    "NPV Macro",
     "ACC",
     "Overall ACC",
     "MCC",
     "MCCI",
     "Overall MCC",
     "SOA6(Matthews)",
     "BCD",
@@ -562,22 +640,24 @@
     "SOA3(Altman)": "SOA3-(Altman's-benchmark)",
     "SOA4(Cicchetti)": "SOA4-(Cicchetti's-benchmark)",
     "TPR Macro": "TPR_Macro",
     "FNR Macro": "FNR_Macro",
     "TNR Macro": "TNR_Macro",
     "FPR Macro": "FPR_Macro",
     "PPV Macro": "PPV_Macro",
+    "NPV Macro": "NPV_Macro",
     "F1 Macro": "F1_Macro",
     "F1 Micro": "F1_Micro",
     "ACC Macro": "ACC_Macro",
     "TPR Micro": "TPR_Micro",
     "FNR Micro": "FNR_Micro",
     "TNR Micro": "TNR_Micro",
     "FPR Micro": "FPR_Micro",
     "PPV Micro": "PPV_Micro",
+    "NPV Micro": "NPV_Micro",
     "Scott PI": "Scott's-Pi",
     "Gwet AC1": "Gwet's-AC1",
     "Bennett S": "Bennett's-S",
     "Kappa 95% CI": "Kappa-95%25-CI",
     "Kappa Standard Error": "Kappa-standard-error",
     "Chi-Squared": "Chi-squared",
     "Phi-Squared": "Phi-squared",
@@ -768,15 +848,15 @@
         "None": "White"},
     "SOA10(Pearson C)": {
         "Not Appreciable": "Red",
         "Weak": "Orange",
         "Medium": "LawnGreen",
         "Strong": "Green",
         "None": "White"}
-    }
+}
 
 BENCHMARK_LIST = list(BENCHMARK_COLOR.keys())
 
 
 TABLE_COLOR = {
     # Pink Colors
     "pink": [255, 192, 203],
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*- """Parameters and constants.""" PYCM_VERSION = "3.8"
+# -*- coding: utf-8 -*- """Parameters and constants.""" PYCM_VERSION = "3.9"
 OVERVIEW = ''' PyCM is a multi-class confusion matrix library written in Python
 that supports both input data vectors and direct matrix, and a proper tool for
 post-classification model evaluation that supports most classes and overall
 statistics parameters. PyCM is the swiss-army knife of confusion matrices,
 targeted mainly at data scientists that need a broad array of metrics for
 predictive models and an accurate evaluation of large variety of classifiers.
 If you use PyCM in your research, we would appreciate citations to the
@@ -40,15 +40,16 @@
 PLOT_COLORS_CLASS_MISMATCH_ERROR = "Given colors and classes have not the same
 length." PLOT_MARKERS_CLASS_MISMATCH_ERROR = "Given markers and classes have
 not the same length." VECTOR_TYPE_ERROR = "The type of input vectors is assumed
 to be a list or a NumPy array" VECTOR_SIZE_ERROR = "Input vectors must have
 same length" VECTOR_EMPTY_ERROR = "Input vectors are empty" VECTOR_ONLY_ERROR =
 "This option only works in vector mode" VECTOR_UNIQUE_CLASS_ERROR = "The
 classes list isn't unique. It contains duplicated labels." CLASS_NUMBER_ERROR =
-"Number of the classes is lower than 2" CLASSES_ERROR = "Used classes is not a
+"Number of the classes is lower than 2" METRICS_OFF_ERROR = "This method cannot
+be executed while 'metrics_off=True'." CLASSES_ERROR = "Used classes is not a
 subset of matrix's classes." COMPARE_FORMAT_ERROR = "The input type is supposed
 to be dictionary but it's not!" CLASSES_LENGHT_ERROR = "Classes length is not
 equal to the array length." AREA_METHOD_ERROR = "The numeric integral method
 can only be selected between 'trapezoidal' and 'midpoint'!" COMPARE_TYPE_ERROR
 = "The input is supposed to consist of pycm.ConfusionMatrix object but it's
 not!" COMPARE_DOMAIN_ERROR = "The domain of all ConfusionMatrix objects must be
 same! The sample size or the number " \ "of classes are different."
@@ -60,59 +61,91 @@
 specified for all of the class benchmarks."
 COMPARE_OVERALL_BENCHMARK_WEIGHT_ERROR = "The overall_benchmark_weight type
 must be dictionary and also must be specified for all of the overall
 benchmarks." COMPARE_CLASS_WEIGHT_WARNING = "The class_weight format is wrong,
 the result is for unweighted mode." COMPARE_CLASS_BENCHMARK_WEIGHT_WARNING =
 "The class_benchmark_weight format is wrong, the result is for unweighted
 mode." COMPARE_OVERALL_BENCHMARK_WEIGHT_WARNING = "The overall_benchmark_weight
-format is wrong, the result is for unweighted mode." COMBINE_TYPE_ERROR = "The
-input type is supposed to be pycm.ConfusionMatrix object but it's not!"
-COMPARE_RESULT_WARNING = "Confusion matrices are too close and the best one can
-not be recognized." WEIGHTED_KAPPA_WARNING = "The weight format is wrong, the
-result is for unweighted kappa." WEIGHTED_ALPHA_WARNING = "The weight format is
-wrong, the result is for unweighted alpha." AVERAGE_WEIGHT_ERROR = "The weight
-type must be dictionary and also must be specified for all of the classes."
-AVERAGE_INVALID_ERROR = "Invalid parameter!" BRIER_SCORE_CLASS_ERROR = "Actual
-vector contains string so pos_class should be explicitly specified"
-BRIER_SCORE_PROB_ERROR = "This option only works in binary probability mode"
-CLASS_NUMBER_WARNING = "The confusion matrix is a high dimension matrix and
-won't be demonstrated properly.\n" \ "If confusion matrix has too many zeros
-(sparse matrix) you can set `sparse` flag to True in printing functions "\
-"otherwise by using save_csv method to save the confusion matrix in csv format
-you'll have better demonstration." CLASSES_WARNING = "Used classes is not a
-subset of classes in actual and predict vectors." CLASSES_TYPE_WARNING = "The
-classes is neither a list nor None so it'll be ignored." CURVE_NONE_WARNING =
-"The curve axes contain non-numerical value(s)." DISTANCE_METRIC_TYPE_ERROR =
-"The metric type must be DistanceType" CLASS_NUMBER_THRESHOLD = 10
-BALANCE_RATIO_THRESHOLD = 3 CLASS_PARAMS = [ "TPR", "TNR", "PPV", "NPV", "FNR",
-"FPR", "FDR", "FOR", "ACC", "F1", "MCC", "BM", "MK", "PLR", "NLR", "DOR", "TP",
-"TN", "FP", "FN", "POP", "P", "N", "TOP", "TON", "PRE", "G", "RACC", "F0.5",
-"F2", "ERR", "RACCU", "J", "IS", "CEN", "MCEN", "AUC", "sInd", "dInd", "DP",
-"Y", "PLRI", "DPI", "AUCI", "GI", "LS", "AM", "BCD", "OP", "IBA", "GM", "Q",
-"AGM", "NLRI", "MCCI", "AGF", "OC", "OOC", "AUPR", "ICSI", "QI", "HD", "BB"]
-SUMMARY_OVERALL = [ "ACC Macro", "Kappa", "Overall ACC", "SOA1(Landis & Koch)",
-"Zero-one Loss", "F1 Macro", "TPR Macro", "PPV Macro", "FPR Macro"]
-SUMMARY_CLASS = [ "ACC", "AUC", "AUCI", "F1", "TPR", "FPR", "PPV", "TP", "FP",
-"FN", "TN", "N", "P", "POP", "TOP", "TON"] BINARY_RECOMMEND = ["ACC", "TPR",
-"PPV", "AUC", "AUCI", "TNR", "F1"] CI_CLASS_LIST = [ "TPR", "TNR", "PPV",
-"NPV", "ACC", "PLR", "NLR", "FPR", "FNR", "AUC", "PRE"] CI_OVERALL_LIST =
-["Kappa", "Overall ACC"] CURVE_PARAMS = ["TPR", "FPR", "TNR", "PPV"]
-ALPHA_TWO_SIDE_TABLE = { 0.2: 1.28, 0.1: 1.645, 0.05: 1.96, 0.02: 2.326, 0.01:
-2.576, 0.002: 3.09, 0.001: 3.29} ALPHA_ONE_SIDE_TABLE = { 0.1: 1.28, 0.05:
-1.645, 0.01: 2.326, 0.005: 2.576, 0.001: 3.09, 0.0005: 3.29}
-CI_ALPHA_TWO_SIDE_WARNING = "The alpha value is invalid, automatically set to
-0.05.\nSupported values (two-sided) : " + ",".join( map(str, sorted(list
-(ALPHA_TWO_SIDE_TABLE.keys())))) CI_ALPHA_ONE_SIDE_WARNING = "The alpha value
-is invalid, automatically set to 0.05.\nSupported values (one-sided) : " +
-",".join( map(str, sorted(list(ALPHA_ONE_SIDE_TABLE.keys())))) CI_FORMAT_ERROR
-= "The input type is supposed to be string but it's not!" CI_SUPPORT_ERROR =
-"CI calculation for this parameter is not supported on this version of
-pycm.\nSupported parameters : " + \ ",".join(CI_CLASS_LIST) + "," + ",".join
-(CI_OVERALL_LIST) MULTICLASS_RECOMMEND = [ "ERR", "TPR Micro", "TPR Macro", "F1
-Macro", "PPV Macro", "ACC", "Overall ACC", "MCC", "MCCI", "Overall MCC", "SOA6
+format is wrong, the result is for unweighted mode." COMPARE_METRICS_OFF_ERROR
+= "Compare cannot be executed while in either of matrices 'metrics_off=True'."
+COMBINE_TYPE_ERROR = "The input type is supposed to be pycm.ConfusionMatrix
+object but it's not!" COMPARE_RESULT_WARNING = "Confusion matrices are too
+close and the best one can not be recognized." WEIGHTED_KAPPA_WARNING = "The
+weight format is wrong, the result is for unweighted kappa."
+WEIGHTED_ALPHA_WARNING = "The weight format is wrong, the result is for
+unweighted alpha." AVERAGE_WEIGHT_ERROR = "The weight type must be dictionary
+and also must be specified for all of the classes." AVERAGE_INVALID_ERROR =
+"Invalid parameter!" BRIER_LOG_LOSS_CLASS_ERROR = "Actual vector contains
+string so pos_class should be explicitly specified" BRIER_LOG_LOSS_PROB_ERROR =
+"This option only works in binary probability mode" CLASS_NUMBER_WARNING = "The
+confusion matrix is a high dimension matrix and won't be demonstrated
+properly.\n" \ "If confusion matrix has too many zeros (sparse matrix) you can
+set `sparse` flag to True in printing functions "\ "otherwise by using save_csv
+method to save the confusion matrix in csv format you'll have better
+demonstration." CLASSES_WARNING = "Used classes is not a subset of classes in
+actual and predict vectors." CLASSES_TYPE_WARNING = "The classes is neither a
+list nor None so it'll be ignored." CURVE_NONE_WARNING = "The curve axes
+contain non-numerical value(s)." DISTANCE_METRIC_TYPE_ERROR = "The metric type
+must be DistanceType" CLASS_NUMBER_THRESHOLD = 10 BALANCE_RATIO_THRESHOLD = 3
+CLASS_PARAMS = { "TPR": "TPR", "TNR": "TNR", "PPV": "PPV", "NPV": "NPV", "FNR":
+"FNR", "FPR": "FPR", "FDR": "FDR", "FOR": "FOR", "ACC": "ACC", "F1": "F1",
+"MCC": "MCC", "BM": "BM", "MK": "MK", "PLR": "PLR", "NLR": "NLR", "DOR": "DOR",
+"TP": "TP", "TN": "TN", "FP": "FP", "FN": "FN", "POP": "POP", "P": "P", "N":
+"N", "TOP": "TOP", "TON": "TON", "PRE": "PRE", "G": "G", "RACC": "RACC",
+"F0.5": "F05", "F2": "F2", "ERR": "ERR", "RACCU": "RACCU", "J": "J", "IS":
+"IS", "CEN": "CEN", "MCEN": "MCEN", "AUC": "AUC", "sInd": "sInd", "dInd":
+"dInd", "DP": "DP", "Y": "Y", "PLRI": "PLRI", "DPI": "DPI", "AUCI": "AUCI",
+"GI": "GI", "LS": "LS", "AM": "AM", "BCD": "BCD", "OP": "OP", "IBA": "IBA",
+"GM": "GM", "Q": "Q", "AGM": "AGM", "NLRI": "NLRI", "MCCI": "MCCI", "AGF":
+"AGF", "OC": "OC", "OOC": "OOC", "AUPR": "AUPR", "ICSI": "ICSI", "QI": "QI",
+"HD": "HD", "BB": "BB", } OVERALL_PARAMS = { 'Overall ACC': 'Overall_ACC',
+'Overall RACCU': 'Overall_RACCU', 'Overall RACC': 'Overall_RACC', 'Kappa':
+'Kappa', 'Gwet AC1': 'AC1', 'Bennett S': 'S', 'Kappa Standard Error':
+'Kappa_SE', 'Kappa Unbiased': 'KappaUnbiased', 'Scott PI': 'PI', 'Kappa No
+Prevalence': 'KappaNoPrevalence', 'Kappa 95% CI': 'Kappa_CI', 'Standard Error':
+'SE', '95% CI': 'CI95', 'Chi-Squared': 'Chi_Squared', 'Phi-Squared':
+'Phi_Squared', 'Cramer V': 'V', 'Response Entropy': 'ResponseEntropy',
+'Reference Entropy': 'ReferenceEntropy', 'Cross Entropy': 'CrossEntropy',
+'Joint Entropy': 'JointEntropy', 'Conditional Entropy': 'ConditionalEntropy',
+'Mutual Information': 'MutualInformation', 'KL Divergence': 'KL', 'Lambda B':
+'LambdaB', 'Lambda A': 'LambdaA', 'Chi-Squared DF': 'DF', 'Overall J':
+'Overall_J', 'Hamming Loss': 'HammingLoss', 'Zero-one Loss': 'ZeroOneLoss',
+'NIR': 'NIR', 'P-Value': 'PValue', 'Overall CEN': 'Overall_CEN', 'Overall
+MCEN': 'Overall_MCEN', 'Overall MCC': 'Overall_MCC', 'RR': 'RR', 'CBA': 'CBA',
+'AUNU': 'AUNU', 'AUNP': 'AUNP', 'RCI': 'RCI', 'Pearson C': 'C', 'TPR Micro':
+'TPR_Micro', 'TPR Macro': 'TPR_Macro', 'CSI': 'CSI', 'ARI': 'ARI', 'TNR Micro':
+'TNR_Micro', 'TNR Macro': 'TNR_Macro', 'Bangdiwala B': 'B', 'Krippendorff
+Alpha': 'Alpha', 'SOA1(Landis & Koch)': 'SOA1', 'SOA2(Fleiss)': 'SOA2', 'SOA3
+(Altman)': 'SOA3', 'SOA4(Cicchetti)': 'SOA4', 'SOA5(Cramer)': 'SOA5', 'SOA6
+(Matthews)': 'SOA6', 'SOA7(Lambda A)': 'SOA7', 'SOA8(Lambda B)': 'SOA8', 'SOA9
+(Krippendorff Alpha)': 'SOA9', 'SOA10(Pearson C)': 'SOA10', 'FPR Macro':
+'FPR_Macro', 'FNR Macro': 'FNR_Macro', 'PPV Macro': 'PPV_Macro', 'NPV Macro':
+'NPV_Macro', 'ACC Macro': 'ACC_Macro', 'F1 Macro': 'F1_Macro', 'FPR Micro':
+'FPR_Micro', 'FNR Micro': 'FNR_Micro', 'PPV Micro': 'PPV_Micro', 'NPV Micro':
+'NPV_Micro', 'F1 Micro': 'F1_Micro', } SUMMARY_OVERALL = [ "ACC Macro",
+"Kappa", "Overall ACC", "SOA1(Landis & Koch)", "Zero-one Loss", "F1 Macro",
+"TPR Macro", "PPV Macro", "NPV Macro", "FPR Macro"] SUMMARY_CLASS = [ "ACC",
+"AUC", "AUCI", "F1", "TPR", "FPR", "PPV", "TP", "FP", "FN", "TN", "N", "P",
+"POP", "TOP", "TON"] BINARY_RECOMMEND = ["ACC", "TPR", "PPV", "AUC", "AUCI",
+"TNR", "F1"] CI_CLASS_LIST = [ "TPR", "TNR", "PPV", "NPV", "ACC", "PLR", "NLR",
+"FPR", "FNR", "AUC", "PRE"] CI_OVERALL_LIST = ["Kappa", "Overall ACC"]
+CURVE_PARAMS = ["TPR", "FPR", "TNR", "PPV"] ALPHA_TWO_SIDE_TABLE = { 0.2: 1.28,
+0.1: 1.645, 0.05: 1.96, 0.02: 2.326, 0.01: 2.576, 0.002: 3.09, 0.001: 3.29}
+ALPHA_ONE_SIDE_TABLE = { 0.1: 1.28, 0.05: 1.645, 0.01: 2.326, 0.005: 2.576,
+0.001: 3.09, 0.0005: 3.29} CI_ALPHA_TWO_SIDE_WARNING = "The alpha value is
+invalid, automatically set to 0.05.\nSupported values (two-sided) : " +
+",".join( map(str, sorted(list(ALPHA_TWO_SIDE_TABLE.keys()))))
+CI_ALPHA_ONE_SIDE_WARNING = "The alpha value is invalid, automatically set to
+0.05.\nSupported values (one-sided) : " + ",".join( map(str, sorted(list
+(ALPHA_ONE_SIDE_TABLE.keys())))) CI_FORMAT_ERROR = "The input type is supposed
+to be string but it's not!" CI_SUPPORT_ERROR = "CI calculation for this
+parameter is not supported on this version of pycm.\nSupported parameters : " +
+\ ",".join(CI_CLASS_LIST) + "," + ",".join(CI_OVERALL_LIST)
+MULTICLASS_RECOMMEND = [ "ERR", "TPR Micro", "TPR Macro", "F1 Macro", "PPV
+Macro", "NPV Macro", "ACC", "Overall ACC", "MCC", "MCCI", "Overall MCC", "SOA6
 (Matthews)", "BCD", "Hamming Loss", "Zero-one Loss"] IMBALANCED_RECOMMEND =
 [ "Kappa", "SOA1(Landis & Koch)", "SOA2(Fleiss)", "SOA3(Altman)", "SOA4
 (Cicchetti)", "CEN", "MCEN", "MCC", "MCCI", "J", "Overall J", "Overall MCC",
 "SOA6(Matthews)", "Overall CEN", "Overall MCEN", "OP", "G", "GI", "DP", "DPI",
 "GI"] PLRI_SCORE = {"Good": 4, "Fair": 3, "Poor": 2, "Negligible": 1, "None":
 "None"} NLRI_SCORE = {"Good": 4, "Fair": 3, "Poor": 2, "Negligible": 1, "None":
 "None"} DPI_SCORE = {"Good": 4, "Fair": 3, "Limited": 2, "Poor": 1, "None":
@@ -200,27 +233,28 @@
 (Test-outcome-negative)", "G": "G-(G-measure)", "ERR": "ERR-(Error-rate)",
 "RACC": "RACC-(Random-accuracy)", "RACCU": "RACCU-(Random-accuracy-unbiased)",
 "PRE": "PRE-(Prevalence)", "Overall ACC": "Overall_ACC", "Kappa": "Kappa",
 "Overall RACC": "Overall_RACC", "SOA1(Landis & Koch)": "SOA1-(Landis-&-Koch's-
 benchmark)", "SOA2(Fleiss)": "SOA2-(Fleiss'-benchmark)", "SOA3(Altman)": "SOA3-
 (Altman's-benchmark)", "SOA4(Cicchetti)": "SOA4-(Cicchetti's-benchmark)", "TPR
 Macro": "TPR_Macro", "FNR Macro": "FNR_Macro", "TNR Macro": "TNR_Macro", "FPR
-Macro": "FPR_Macro", "PPV Macro": "PPV_Macro", "F1 Macro": "F1_Macro", "F1
-Micro": "F1_Micro", "ACC Macro": "ACC_Macro", "TPR Micro": "TPR_Micro", "FNR
-Micro": "FNR_Micro", "TNR Micro": "TNR_Micro", "FPR Micro": "FPR_Micro", "PPV
-Micro": "PPV_Micro", "Scott PI": "Scott's-Pi", "Gwet AC1": "Gwet's-AC1",
-"Bennett S": "Bennett's-S", "Kappa 95% CI": "Kappa-95%25-CI", "Kappa Standard
-Error": "Kappa-standard-error", "Chi-Squared": "Chi-squared", "Phi-Squared":
-"Phi-squared", "Cramer V": "Cramer's-V", "Chi-Squared DF": "Chi-squared-DF",
-"95% CI": "95%25-CI", "Standard Error": "Standard-error", "Response Entropy":
-"Response-entropy", "Reference Entropy": "Reference-entropy", "Cross Entropy":
-"Cross-entropy", "Joint Entropy": "Joint-entropy", "Conditional Entropy":
-"Conditional-entropy", "KL Divergence": "Kullback-Leibler-divergence", "Lambda
-B": "Goodman-&-Kruskal's-lambda-B", "Lambda A": "Goodman-&-Kruskal's-lambda-A",
-"Kappa Unbiased": "Kappa-unbiased", "Overall RACCU": "Overall_RACCU", "Kappa No
+Macro": "FPR_Macro", "PPV Macro": "PPV_Macro", "NPV Macro": "NPV_Macro", "F1
+Macro": "F1_Macro", "F1 Micro": "F1_Micro", "ACC Macro": "ACC_Macro", "TPR
+Micro": "TPR_Micro", "FNR Micro": "FNR_Micro", "TNR Micro": "TNR_Micro", "FPR
+Micro": "FPR_Micro", "PPV Micro": "PPV_Micro", "NPV Micro": "NPV_Micro", "Scott
+PI": "Scott's-Pi", "Gwet AC1": "Gwet's-AC1", "Bennett S": "Bennett's-S", "Kappa
+95% CI": "Kappa-95%25-CI", "Kappa Standard Error": "Kappa-standard-error",
+"Chi-Squared": "Chi-squared", "Phi-Squared": "Phi-squared", "Cramer V":
+"Cramer's-V", "Chi-Squared DF": "Chi-squared-DF", "95% CI": "95%25-CI",
+"Standard Error": "Standard-error", "Response Entropy": "Response-entropy",
+"Reference Entropy": "Reference-entropy", "Cross Entropy": "Cross-entropy",
+"Joint Entropy": "Joint-entropy", "Conditional Entropy": "Conditional-entropy",
+"KL Divergence": "Kullback-Leibler-divergence", "Lambda B": "Goodman-&-
+Kruskal's-lambda-B", "Lambda A": "Goodman-&-Kruskal's-lambda-A", "Kappa
+Unbiased": "Kappa-unbiased", "Overall RACCU": "Overall_RACCU", "Kappa No
 Prevalence": "Kappa-no-prevalence", "Mutual Information": "Mutual-information",
 "J": "J-(Jaccard-index)", "Overall J": "Overall_J", "Hamming Loss": "Hamming-
 loss", "Zero-one Loss": "Zero-one-loss", "NIR": "NIR-(No-information-rate)",
 "P-Value": "P-Value", "IS": "IS-(Information-score)", "CEN": "CEN-(Confusion-
 entropy)", "Overall CEN": "Overall_CEN", "MCEN": "MCEN-(Modified-confusion-
 entropy)", "Overall MCEN": "Overall_MCEN", "Overall MCC": "Overall_MCC", "RR":
 "RR-(Global-performance-index)", "CBA": "CBA-(Class-balance-accuracy)", "AUC":
```

### Comparing `pycm-3.8/pycm/pycm_test.py` & `pycm-3.9/pycm/pycm_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 >>> y_actu = [2, 0, 2, 2, 0, 1, 1, 2, 2, 0, 1, 2]
 >>> y_pred = [0, 0, 2, 1, 0, 2, 1, 0, 2, 0, 2, 2]
 >>> cm = ConfusionMatrix(y_actu, y_pred)
 >>> cm
 pycm.ConfusionMatrix(classes: [0, 1, 2])
 >>> len(cm)
 3
->>> cm = ConfusionMatrix(matrix={"Class1":{"Class1":9,"Class2":3,"Class3":0},"Class2":{"Class1":3,"Class2":5,"Class3":1},"Class3":{"Class1":1,"Class2":1,"Class3":4}})
+>>> cm = ConfusionMatrix(matrix={"Class1": {"Class1": 9, "Class2": 3, "Class3": 0}, "Class2": {"Class1": 3, "Class2": 5, "Class3": 1}, "Class3": {"Class1": 1, "Class2": 1, "Class3": 4}})
 >>> cm
 pycm.ConfusionMatrix(classes: ['Class1', 'Class2', 'Class3'])
->>> cm2 = ConfusionMatrix(matrix={"Class1":{"Class1":9,"Class2":3,"Class3":0},"Class2":{"Class1":3,"Class2":5,"Class3":1},"Class3":{"Class1":0,"Class2":0,"Class3":6}})
->>> cp = Compare({"cm1":cm,"cm2":cm2})
+>>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 9, "Class2": 3, "Class3": 0}, "Class2": {"Class1": 3, "Class2": 5, "Class3": 1}, "Class3": {"Class1": 0, "Class2": 0, "Class3": 6}})
+>>> cp = Compare({"cm1": cm, "cm2": cm2})
 >>> cp
 pycm.Compare(classes: ['Class1', 'Class2', 'Class3'])
->>> crv = Curve(actual_vector = [1, 1, 2, 2], probs = [[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]], classes=[2, 1])
+>>> crv = Curve(actual_vector=[1, 1, 2, 2], probs=[[0.1, 0.9], [0.4, 0.6], [0.35, 0.65], [0.8, 0.2]], classes=[2, 1])
 >>> crv.classes
 [2, 1]
 >>> crv.thresholds
 [0.1, 0.2, 0.35, 0.4, 0.6, 0.65, 0.8, 0.9]
 >>> crv.data[2]["TPR"]
 [1.0, 1.0, 1.0, 0.5, 0.5, 0.5, 0.5, 0.0]
 >>> crv.data[2]["FPR"]
```

### Comparing `pycm-3.8/pycm/pycm_util.py` & `pycm-3.9/pycm/pycm_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import math
 import numpy
 import re
 from .pycm_param import *
 from .pycm_error import pycmMatrixError
 from warnings import warn
+from functools import wraps
 
 
 def list_check_equal(input_list):
     """
     Check equality of the input list items.
 
     :param input_list: input list
@@ -715,20 +716,68 @@
     :return: thresholds as list
     """
     thresholds = numpy.ravel(probs)
     thresholds = sorted(set(thresholds))
     return thresholds
 
 
+def char_num_transformer(input_item):
+    """
+    Transform the input string to a proper key for char-num sorting.
+
+    :param input_item: input item
+    :type input_item: str
+    :return: key as tuple
+    """
+    return [(input_item, False, False) if not re.findall(r'\d+', input_item)
+            else (input_item[:re.search(r'\d+', input_item).start()],
+                  int(re.findall(r'\d+', input_item)[0]),
+                  input_item[re.search(r'\d+', input_item).end():])]
+
+
 def sort_char_num(input_list):
     """
     Sort a list of strings first alphabetically and then numerically.
 
     :param input_list: input list of strings
     :type input_list: iterable
     :return: a sorted list of strings
     """
-    sort_by = lambda x: [(x, False, False) if not re.findall(r'\d+', x)
-                         else (x[:re.search(r'\d+', x).start()],
-                               int(re.findall(r'\d+', x)[0]),
-                               x[re.search(r'\d+', x).end():])]
-    return sorted(input_list, key=sort_by)
+    return sorted(input_list, key=char_num_transformer)
+
+
+def vector_serializer(vector):
+    """
+    Return given vector in serializable mode.
+
+    :param vector: the given vector
+    :type: list or numpy array
+    :retun: a serializable format of vector
+    """
+    if isinstance(vector, numpy.ndarray):
+        vector = vector.tolist()
+    return vector
+
+
+def metrics_off_check(func):
+    """
+    Check metrics_off flag decorator.
+
+    :param func: input function
+    :type func: function
+    :return: inner function
+    """
+    @wraps(func)
+    def inner_function(*args, **kwargs):
+        """
+        Inner function.
+
+        :param args: non-keyword arguments
+        :type args: list
+        :param kwargs: keyword arguments
+        :type kwargs: dict
+        :return: None
+        """
+        if args[0].metrics_off:
+            raise pycmMatrixError(METRICS_OFF_ERROR)
+        return func(*args, **kwargs)
+    return inner_function
```

### Comparing `pycm-3.8/pycm.egg-info/PKG-INFO` & `pycm-3.9/pycm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pycm
-Version: 3.8
+Version: 3.9
 Summary: Multi-class confusion matrix library in Python
 Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.8
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9
 Author: PyCM Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Webpage, https://www.pycm.io
 Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f
 Keywords: confusion-matrix python3 python machine_learning ML
@@ -133,22 +133,22 @@
 ## Installation
 
 ⚠️  PyCM 2.4 is the last version to support **Python 2.7** & **Python 3.4**
 
 ⚠️  Plotting capability requires **Matplotlib (>= 3.0.0)** or **Seaborn (>= 0.9.1)**
 
 ### Source code
-- Download [Version 3.8](https://github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
+- Download [Version 3.9](https://github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://github.com/sepandhaghighi/pycm/archive/dev.zip)
 - Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt` (Need root access)
 - Run `python3 setup.py install` or `python setup.py install` (Need root access)
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need root access)
+- Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need root access)
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda` (Need root access)
 - Run `conda install -c sepandhaghighi pycm` (Need root access)
 
@@ -237,15 +237,15 @@
 
 ```
 
 ### Direct CM
 
 ```pycon
 >>> from pycm import *
->>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2": {"Class1": 0, "Class2": 5}})
+>>> cm2 = ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2": {"Class1": 0, "Class2": 5}})
 >>> cm2
 pycm.ConfusionMatrix(classes: ['Class1', 'Class2'])
 >>> cm2.classes
 ['Class1', 'Class2']
 >>> cm2.print_matrix()
 Predict      Class1       Class2       
 Actual
@@ -319,15 +319,15 @@
 `transpose` is added in `version 1.2` in order to transpose input matrix (only in `Direct CM` mode)
 
 ### Relabel
 
 `relabel` method is added in `version 1.5` in order to change ConfusionMatrix classnames.
 
 ```pycon
->>> cm.relabel(mapping={0:"L1",1:"L2",2:"L3"})
+>>> cm.relabel(mapping={0: "L1", 1: "L2", 2: "L3"})
 >>> cm
 pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3'])
 ```
 
 ### Position
 
 `position` method is added in `version 2.8` in order to find the indexes of observations in `predict_vector` which made TP, TN, FP, FN.
@@ -439,34 +439,34 @@
 ['MCC', 'TPR Micro', 'ACC', 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one Loss', 'ERR', 'PPV Micro', 'Overall ACC']
 
 ```
 
 `is_imbalanced` parameter has been added in `version 3.3`, so the user can indicate whether the concerned dataset is imbalanced or not. As long as the user does not provide any information in this regard, the automatic detection algorithm will be used.
 
 ```pycon
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True)
 >>> cm.imbalance
 True
->>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = False)
+>>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
 >>> cm.imbalance
 False
 ```
 
 ### Compare
 
 In `version 2.0`, a method for comparing several confusion matrices is introduced. This option is a combination of several overall and class-based benchmarks. Each of the benchmarks evaluates the performance of the classification algorithm from good to poor and give them a numeric score. The score of good and poor performances are 1 and 0, respectively.
 
 After that, two scores are calculated for each confusion matrices, overall and class-based. The overall score is the average of the score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based score is the average of the score of six class-based benchmarks which are Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power Interpretation, AUC value Interpretation, Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It should be noticed that if one of the benchmarks returns none for one of the classes, that benchmarks will be eliminated in total averaging. If the user sets weights for the classes, the averaging over the value of class-based benchmark scores will transform to a weighted average.
 
 If the user sets the value of `by_class` boolean input `True`, the best confusion matrix is the one with the maximum class-based score. Otherwise, if a confusion matrix obtains the maximum of both overall and class-based scores, that will be reported as the best confusion matrix, but in any other case, the compared object doesn’t select the best confusion matrix.
 
 ```pycon
->>> cm2 = ConfusionMatrix(matrix={0:{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}})
->>> cm3 = ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55, 2:2}})
->>> cp = Compare({"cm2":cm2, "cm3":cm3})
+>>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1: 50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}})
+>>> cm3 = ConfusionMatrix(matrix={0: {0: 50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}})
+>>> cp = Compare({"cm2": cm2, "cm3": cm3})
 >>> print(cp)
 Best : cm2
 
 Rank  Name   Class-Score       Overall-Score
 1     cm2    0.50278           0.58095
 2     cm3    0.33611           0.52857
 
@@ -502,14 +502,15 @@
 4. `digit`: `int`
 5. `threshold` : `FunctionType (function or lambda)`
 6. `file` : `File object`
 7. `sample_weight` : python `list` or numpy `array` of numbers
 8. `transpose` : `bool`
 9. `classes` : python `list`
 10. `is_imbalanced` : `bool`
+11. `metrics_off` : `bool`
 
 * Run `help(ConfusionMatrix)` for `ConfusionMatrix` object details
 
 **Compare**
 
 1. `cm_dict` : python `dict` of `ConfusionMatrix` object (`str` : `ConfusionMatrix`)
 2. `by_class` : `bool`
@@ -629,14 +630,54 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [3.9] - 2023-05-01
+### Added
+- `OVERALL_PARAMS` dictionary
+- `__imbalancement_handler__` function
+- `vector_serializer` function
+- NPV micro/macro
+- `log_loss` method
+- 23 new distance/similarity
+	1. Dennis 
+	2. Digby
+	3. Dispersion
+	4. Doolittle
+	5. Eyraud
+	6. Fager & McGowan
+	7. Faith
+	8. Fleiss-Levin-Paik
+	9. Forbes I
+	10. Forbes II
+	11. Fossum
+	12. Gilbert & Wells
+	13. Goodall
+	14. Goodman & Kruskal's Lambda
+	15. Goodman & Kruskal Lambda-r
+	16. Guttman's Lambda A
+	17. Guttman's Lambda B
+	18. Hamann
+	19. Harris & Lahey
+	20. Hawkins & Dotson
+	21. Kendall's Tau
+	22. Kent & Foster I
+	23. Kent & Foster II
+### Changed
+- `metrics_off` parameter added to ConfusionMatrix `__init__` method
+- `CLASS_PARAMS` changed to a dictionary
+- Code style modified
+- `sort` parameter added to `relabel` method
+- Document modified
+- `CONTRIBUTING.md` updated
+- `codecov` removed from `dev-requirements.txt`
+- Test system modified
 ## [3.8] - 2023-02-01
 ### Added
 - `distance` method
 - `__contains__` method
 - `__getitem__` method
 - Goodman-Kruskal's Lambda A benchmark
 - Goodman-Kruskal's Lambda B benchmark
@@ -1276,15 +1317,16 @@
 - MK
 - NPV
 - PPV
 - TNR
 - TPR
 - documents and `README.md`
 
-[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.8...dev
+[Unreleased]: https://github.com/sepandhaghighi/pycm/compare/v3.9...dev
+[3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
 [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
 [3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7
 [3.6]: https://github.com/sepandhaghighi/pycm/compare/v3.5...v3.6
 [3.5]: https://github.com/sepandhaghighi/pycm/compare/v3.4...v3.5
 [3.4]: https://github.com/sepandhaghighi/pycm/compare/v3.3...v3.4
 [3.3]: https://github.com/sepandhaghighi/pycm/compare/v3.2...v3.3
 [3.2]: https://github.com/sepandhaghighi/pycm/compare/v3.1...v3.2
@@ -1318,10 +1360,7 @@
 [0.7]: https://github.com/sepandhaghighi/pycm/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/pycm/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/pycm/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/pycm/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/pycm/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/pycm/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/pycm/compare/1e238cd...v0.1
-
-
-
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pycm Version: 3.8 Summary: Multi-class confusion
+Metadata-Version: 2.1 Name: pycm Version: 3.9 Summary: Multi-class confusion
 matrix library in Python Home-page: https://github.com/sepandhaghighi/pycm
-Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.8 Author: PyCM
+Download-URL: https://github.com/sepandhaghighi/pycm/tarball/v3.9 Author: PyCM
 Development Team Author-email: info@pycm.io License: MIT Project-URL: Webpage,
 https://www.pycm.io Project-URL: Source, https://github.com/sepandhaghighi/pycm
 Project-URL: Discord, https://discord.com/invite/zqpU2b3J3f Keywords:
 confusion-matrix python3 python machine_learning ML Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -64,21 +64,21 @@
    CI          pycm/workflows/CI/                  pycm/workflows/CI/
             badge.svg?branch=master]              badge.svg?branch=dev]
              [https://api.codacy.com/project/
 Code Quality           badge/Grade/            [CodeFactor] [codebeat_badge]
              5d9463998a0040d09afc2b80c389365c]
 ## Installation â ï¸ PyCM 2.4 is the last version to support **Python 2.7** &
 **Python 3.4** â ï¸ Plotting capability requires **Matplotlib (>= 3.0.0)** or
-**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.8](https://
-github.com/sepandhaghighi/pycm/archive/v3.8.zip) or [Latest Source ](https://
+**Seaborn (>= 0.9.1)** ### Source code - Download [Version 3.9](https://
+github.com/sepandhaghighi/pycm/archive/v3.9.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/pycm/archive/dev.zip) - Run `pip install -
 r requirements.txt` or `pip3 install -r requirements.txt` (Need root access) -
 Run `python3 setup.py install` or `python setup.py install` (Need root access)
 ### PyPI - Check [Python Packaging User Guide](https://packaging.python.org/
-installing/) - Run `pip install pycm==3.8` or `pip3 install pycm==3.8` (Need
+installing/) - Run `pip install pycm==3.9` or `pip3 install pycm==3.9` (Need
 root access) ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` (Need root access) - Run `conda install
 -c sepandhaghighi pycm` (Need root access) ### Easy install - Run `easy_install
 --upgrade pycm` (Need root access) ### MATLAB - Download and install [MATLAB]
 (https://www.mathworks.com/products/matlab.html) (>=8.5, 64/32 bit) - Download
 and install [Python3.x](https://www.python.org/downloads/) (>=3.5, 64/32 bit) -
 [x] Select `Add to PATH` option - [x] Select `Install pip` option - Run `pip
@@ -101,15 +101,15 @@
 error) 0 2 3 FP(False positive/type 1 error/false alarm) 2 1 2 FPR(Fall-out or
 false positive rate) 0.22222 0.11111 0.33333 N(Condition negative) 9 9 6 P
 (Condition positive or support) 3 3 6 POP(Population) 12 12 12 PPV(Precision or
 positive predictive value) 0.6 0.5 0.6 TN(True negative/correct rejection) 7 8
 4 TON(Test outcome negative) 7 10 7 TOP(Test outcome positive) 5 2 5 TP(True
 positive/hit) 3 1 3 TPR(Sensitivity, recall, hit rate, or true positive rate)
 1.0 0.33333 0.5 ``` ### Direct CM ```pycon >>> from pycm import * >>> cm2 =
-ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2":2}, "Class2":
+ConfusionMatrix(matrix={"Class1": {"Class1": 1, "Class2": 2}, "Class2":
 {"Class1": 0, "Class2": 5}}) >>> cm2 pycm.ConfusionMatrix(classes: ['Class1',
 'Class2']) >>> cm2.classes ['Class1', 'Class2'] >>> cm2.print_matrix() Predict
 Class1 Class2 Actual Class1 1 2 Class2 0 5 >>> cm2.print_normalized_matrix()
 Predict Class1 Class2 Actual Class1 0.33333 0.66667 Class2 0.0 1.0 >>> cm2.stat
 (summary=True) Overall Statistics : ACC Macro 0.75 F1 Macro 0.66667 FPR Macro
 0.33333 Kappa 0.38462 Overall ACC 0.75 PPV Macro 0.85714 SOA1(Landis & Koch)
 Fair TPR Macro 0.66667 Zero-one Loss 2 Class Statistics : Classes Class1 Class2
@@ -129,16 +129,16 @@
 `version 0.9.5` in order to load saved confusion matrix with `.obj` format
 generated by `save_obj` method. For more information visit [Example4](http://
 www.pycm.io/doc/Example4.html "Example4") ### Sample weights `sample_weight` is
 added in `version 1.2` For more information visit [Example5](http://
 www.pycm.io/doc/Example5.html "Example5") ### Transpose `transpose` is added in
 `version 1.2` in order to transpose input matrix (only in `Direct CM` mode) ###
 Relabel `relabel` method is added in `version 1.5` in order to change
-ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0:"L1",1:"L2",2:
-"L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
+ConfusionMatrix classnames. ```pycon >>> cm.relabel(mapping={0: "L1", 1: "L2",
+2: "L3"}) >>> cm pycm.ConfusionMatrix(classes: ['L1', 'L2', 'L3']) ``` ###
 Position `position` method is added in `version 2.8` in order to find the
 indexes of observations in `predict_vector` which made TP, TN, FP, FN. ```pycon
 >>> cm.position() {0: {'FN': [], 'FP': [0, 7], 'TP': [1, 4, 9], 'TN': [2, 3, 5,
 6, 8, 10, 11]}, 1: {'FN': [5, 10], 'FP': [3], 'TP': [6], 'TN': [0, 1, 2, 4, 7,
 8, 9, 11]}, 2: {'FN': [0, 3, 7], 'FP': [5, 10], 'TP': [2, 8, 11], 'TN': [1, 4,
 6, 9]}} ``` ### To array `to_array` method is added in `version 2.9` in order
 to returns the confusion matrix in the form of a NumPy array. This can be
@@ -200,72 +200,72 @@
 capabilities which had been claimed by the paper. ```pycon >>> cm.imbalance
 False >>> cm.binary False >>> cm.recommended_list ['MCC', 'TPR Micro', 'ACC',
 'PPV Macro', 'BCD', 'Overall MCC', 'Hamming Loss', 'TPR Macro', 'Zero-one
 Loss', 'ERR', 'PPV Micro', 'Overall ACC'] ``` `is_imbalanced` parameter has
 been added in `version 3.3`, so the user can indicate whether the concerned
 dataset is imbalanced or not. As long as the user does not provide any
 information in this regard, the automatic detection algorithm will be used.
-```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced = True) >>>
-cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced =
-False) >>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for
-comparing several confusion matrices is introduced. This option is a
-combination of several overall and class-based benchmarks. Each of the
-benchmarks evaluates the performance of the classification algorithm from good
-to poor and give them a numeric score. The score of good and poor performances
-are 1 and 0, respectively. After that, two scores are calculated for each
-confusion matrices, overall and class-based. The overall score is the average
-of the score of seven overall benchmarks which are Landis & Koch, Cramer,
-Matthews, Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B,
-Krippendorff's Alpha, and Pearson's C. In the same manner, the class-based
-score is the average of the score of six class-based benchmarks which are
-Positive Likelihood Ratio Interpretation, Negative Likelihood Ratio
-Interpretation, Discriminant Power Interpretation, AUC value Interpretation,
-Matthews Correlation Coefficient Interpretation and Yule's Q Interpretation. It
-should be noticed that if one of the benchmarks returns none for one of the
-classes, that benchmarks will be eliminated in total averaging. If the user
-sets weights for the classes, the averaging over the value of class-based
-benchmark scores will transform to a weighted average. If the user sets the
-value of `by_class` boolean input `True`, the best confusion matrix is the one
-with the maximum class-based score. Otherwise, if a confusion matrix obtains
-the maximum of both overall and class-based scores, that will be reported as
-the best confusion matrix, but in any other case, the compared object doesnât
-select the best confusion matrix. ```pycon >>> cm2 = ConfusionMatrix(matrix={0:
-{0:2, 1:50, 2:6}, 1:{0:5, 1:50, 2:3}, 2:{0:1, 1:7, 2:50}}) >>> cm3 =
-ConfusionMatrix(matrix={0:{0:50, 1:2, 2:6}, 1:{0:50, 1:5, 2:3}, 2:{0:1, 1:55,
-2:2}}) >>> cp = Compare({"cm2":cm2, "cm3":cm3}) >>> print(cp) Best : cm2 Rank
-Name Class-Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>>
-cp.best pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3']
->>> cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
+```pycon >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=True) >>>
+cm.imbalance True >>> cm = ConfusionMatrix(y_actu, y_pred, is_imbalanced=False)
+>>> cm.imbalance False ``` ### Compare In `version 2.0`, a method for comparing
+several confusion matrices is introduced. This option is a combination of
+several overall and class-based benchmarks. Each of the benchmarks evaluates
+the performance of the classification algorithm from good to poor and give them
+a numeric score. The score of good and poor performances are 1 and 0,
+respectively. After that, two scores are calculated for each confusion
+matrices, overall and class-based. The overall score is the average of the
+score of seven overall benchmarks which are Landis & Koch, Cramer, Matthews,
+Goodman-Kruskal's Lambda A, Goodman-Kruskal's Lambda B, Krippendorff's Alpha,
+and Pearson's C. In the same manner, the class-based score is the average of
+the score of six class-based benchmarks which are Positive Likelihood Ratio
+Interpretation, Negative Likelihood Ratio Interpretation, Discriminant Power
+Interpretation, AUC value Interpretation, Matthews Correlation Coefficient
+Interpretation and Yule's Q Interpretation. It should be noticed that if one of
+the benchmarks returns none for one of the classes, that benchmarks will be
+eliminated in total averaging. If the user sets weights for the classes, the
+averaging over the value of class-based benchmark scores will transform to a
+weighted average. If the user sets the value of `by_class` boolean input
+`True`, the best confusion matrix is the one with the maximum class-based
+score. Otherwise, if a confusion matrix obtains the maximum of both overall and
+class-based scores, that will be reported as the best confusion matrix, but in
+any other case, the compared object doesnât select the best confusion matrix.
+```pycon >>> cm2 = ConfusionMatrix(matrix={0: {0: 2, 1: 50, 2: 6}, 1: {0: 5, 1:
+50, 2: 3}, 2: {0: 1, 1: 7, 2: 50}}) >>> cm3 = ConfusionMatrix(matrix={0: {0:
+50, 1: 2, 2: 6}, 1: {0: 50, 1: 5, 2: 3}, 2: {0: 1, 1: 55, 2: 2}}) >>> cp =
+Compare({"cm2": cm2, "cm3": cm3}) >>> print(cp) Best : cm2 Rank Name Class-
+Score Overall-Score 1 cm2 0.50278 0.58095 2 cm3 0.33611 0.52857 >>> cp.best
+pycm.ConfusionMatrix(classes: [0, 1, 2]) >>> cp.sorted ['cm2', 'cm3'] >>>
+cp.best_name 'cm2' ``` ### Online help `online_help` function is added in
 `version 1.1` in order to open each statistics definition in web browser
 ```pycon >>> from pycm import online_help >>> online_help("J") >>> online_help
 ("SOA1(Landis & Koch)") >>> online_help(2) ``` * List of items are available by
 calling `online_help()` (without argument) * If PyCM website is not available,
 set `alt_link = True` (new in `version 2.4`) ### Acceptable data types
 **ConfusionMatrix** 1. `actual_vector` : python `list` or numpy `array` of any
 stringable objects 2. `predict_vector` : python `list` or numpy `array` of any
 stringable objects 3. `matrix` : `dict` 4. `digit`: `int` 5. `threshold` :
 `FunctionType (function or lambda)` 6. `file` : `File object` 7.
 `sample_weight` : python `list` or numpy `array` of numbers 8. `transpose` :
-`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` * Run `help
-(ConfusionMatrix)` for `ConfusionMatrix` object details **Compare** 1.
-`cm_dict` : python `dict` of `ConfusionMatrix` object (`str` :
-`ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` : python `dict` of
-class weights (`class_name` : `float`) 4. `class_benchmark_weight`: python
-`dict` of class benchmark weights (`class_benchmark_name` : `float`) 5.
-`overall_benchmark_weight`: python `dict` of overall benchmark weights
-(`overall_benchmark_name` : `float`) 6. `digit`: `int` * Run `help(Compare)`
-for `Compare` object details **ROCCurve** 1. `actual_vector` : python `list` or
-numpy `array` of any stringable objects 2. `probs` : python `list` or numpy
-`array` 3. `classes` : python `list` 4. `thresholds`: python `list` or numpy
-`array` 5. `sample_weight`: python `list` or numpy `array` **PRCurve** 1.
+`bool` 9. `classes` : python `list` 10. `is_imbalanced` : `bool` 11.
+`metrics_off` : `bool` * Run `help(ConfusionMatrix)` for `ConfusionMatrix`
+object details **Compare** 1. `cm_dict` : python `dict` of `ConfusionMatrix`
+object (`str` : `ConfusionMatrix`) 2. `by_class` : `bool` 3. `class_weight` :
+python `dict` of class weights (`class_name` : `float`) 4.
+`class_benchmark_weight`: python `dict` of class benchmark weights
+(`class_benchmark_name` : `float`) 5. `overall_benchmark_weight`: python `dict`
+of overall benchmark weights (`overall_benchmark_name` : `float`) 6. `digit`:
+`int` * Run `help(Compare)` for `Compare` object details **ROCCurve** 1.
 `actual_vector` : python `list` or numpy `array` of any stringable objects 2.
 `probs` : python `list` or numpy `array` 3. `classes` : python `list` 4.
 `thresholds`: python `list` or numpy `array` 5. `sample_weight`: python `list`
-or numpy `array` For more information visit [here](https://github.com/
-sepandhaghighi/pycm/tree/master/Document "Document")
+or numpy `array` **PRCurve** 1. `actual_vector` : python `list` or numpy
+`array` of any stringable objects 2. `probs` : python `list` or numpy `array`
+3. `classes` : python `list` 4. `thresholds`: python `list` or numpy `array` 5.
+`sample_weight`: python `list` or numpy `array` For more information visit
+[here](https://github.com/sepandhaghighi/pycm/tree/master/Document "Document")
                      [https://asciinema.org/a/171863.png]
 ## Try PyCM in your browser! PyCM can be used online in interactive Jupyter
 Notebooks via the Binder or Colab services! Try it out now! : [![Binder](https:
 //mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sepandhaghighi/pycm/
 master) [![Google Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/sepandhaghighi/pycm/blob/
 master) * Check `Examples` in `Document` folder ## Issues & bug reports 1. Fill
@@ -313,17 +313,29 @@
 ## Show your support ### Star this repo Give a â­ï¸ if this project helped
 you! ### Donate to our project If you do like our project and we hope that you
 do, can you please support us? Our project is not and is never going to be
 working for profit. We need the money just so we can continue doing what we do
 ;-) . [PyCM_Donation] # Changelog All notable changes to this project will be
 documented in this file. The format is based on [Keep a Changelog](http://
 keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.8] - 2023-02-01 ###
-Added - `distance` method - `__contains__` method - `__getitem__` method -
-Goodman-Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [3.9] - 2023-05-01 ###
+Added - `OVERALL_PARAMS` dictionary - `__imbalancement_handler__` function -
+`vector_serializer` function - NPV micro/macro - `log_loss` method - 23 new
+distance/similarity 1. Dennis 2. Digby 3. Dispersion 4. Doolittle 5. Eyraud 6.
+Fager & McGowan 7. Faith 8. Fleiss-Levin-Paik 9. Forbes I 10. Forbes II 11.
+Fossum 12. Gilbert & Wells 13. Goodall 14. Goodman & Kruskal's Lambda 15.
+Goodman & Kruskal Lambda-r 16. Guttman's Lambda A 17. Guttman's Lambda B 18.
+Hamann 19. Harris & Lahey 20. Hawkins & Dotson 21. Kendall's Tau 22. Kent &
+Foster I 23. Kent & Foster II ### Changed - `metrics_off` parameter added to
+ConfusionMatrix `__init__` method - `CLASS_PARAMS` changed to a dictionary -
+Code style modified - `sort` parameter added to `relabel` method - Document
+modified - `CONTRIBUTING.md` updated - `codecov` removed from `dev-
+requirements.txt` - Test system modified ## [3.8] - 2023-02-01 ### Added -
+`distance` method - `__contains__` method - `__getitem__` method - Goodman-
+Kruskal's Lambda A benchmark - Goodman-Kruskal's Lambda B benchmark -
 Krippendorff's Alpha benchmark - Pearson's C benchmark - 30 new distance/
 similarity 1. AMPLE 2. Anderberg's D 3. Andres & Marzo's Delta 4. Baroni-Urbani
 & Buser I 5. Baroni-Urbani & Buser II 6. Batagelj & Bren 7. Baulieu I 8.
 Baulieu II 9. Baulieu III 10. Baulieu IV 11. Baulieu V 12. Baulieu VI 13.
 Baulieu VII 14. Baulieu VIII 15. Baulieu IX 16. Baulieu X 17. Baulieu XI 18.
 Baulieu XII 19. Baulieu XIII 20. Baulieu XIV 21. Baulieu XV 22. Benini I 23.
 Benini II 24. Canberra 25. Clement 26. Consonni & Todeschini I 27. Consonni &
@@ -520,17 +532,18 @@
 benchmark - `overall_stat` ## [0.2] - 2018-01-24 ### Added - Population -
 Condition positive - Condition negative - Test outcome positive - Test outcome
 negative - Prevalence - G-measure - Matrix method - Normalized matrix method -
 Params method ### Changed - `statistic_result` to `class_stat` - `params` to
 `stat` ## [0.1] - 2018-01-22 ### Added - ACC - BM - DOR - F1-Score - FDR - FNR
 - FOR - FPR - LR+ - LR- - MCC - MK - NPV - PPV - TNR - TPR - documents and
 `README.md` [Unreleased]: https://github.com/sepandhaghighi/pycm/compare/
-v3.8...dev [3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8
-[3.7]: https://github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https:
-//github.com/sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
+v3.9...dev [3.9]: https://github.com/sepandhaghighi/pycm/compare/v3.8...v3.9
+[3.8]: https://github.com/sepandhaghighi/pycm/compare/v3.7...v3.8 [3.7]: https:
+//github.com/sepandhaghighi/pycm/compare/v3.6...v3.7 [3.6]: https://github.com/
+sepandhaghighi/pycm/compare/v3.5...v3.6 [3.5]: https://github.com/
 sepandhaghighi/pycm/compare/v3.4...v3.5 [3.4]: https://github.com/
 sepandhaghighi/pycm/compare/v3.3...v3.4 [3.3]: https://github.com/
 sepandhaghighi/pycm/compare/v3.2...v3.3 [3.2]: https://github.com/
 sepandhaghighi/pycm/compare/v3.1...v3.2 [3.1]: https://github.com/
 sepandhaghighi/pycm/compare/v3.0...v3.1 [3.0]: https://github.com/
 sepandhaghighi/pycm/compare/v2.9...v3.0 [2.9]: https://github.com/
 sepandhaghighi/pycm/compare/v2.8...v2.9 [2.8]: https://github.com/
```

### Comparing `pycm-3.8/pycm.egg-info/SOURCES.txt` & `pycm-3.9/pycm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycm-3.8/setup.py` & `pycm-3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
    data scientists that need a broad array of metrics for predictive models
    and an accurate evaluation of large variety of classifiers.'''
 
 
 setup(
     name='pycm',
     packages=['pycm'],
-    version='3.8',
+    version='3.9',
     description='Multi-class confusion matrix library in Python',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyCM Development Team',
     author_email='info@pycm.io',
     url='https://github.com/sepandhaghighi/pycm',
-    download_url='https://github.com/sepandhaghighi/pycm/tarball/v3.8',
+    download_url='https://github.com/sepandhaghighi/pycm/tarball/v3.9',
     keywords="confusion-matrix python3 python machine_learning ML",
     project_urls={
         'Webpage': 'https://www.pycm.io',
         'Source': 'https://github.com/sepandhaghighi/pycm',
         'Discord': 'https://discord.com/invite/zqpU2b3J3f',
     },
     install_requires=get_requires(),
```

