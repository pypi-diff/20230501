# Comparing `tmp/werpy-0.0.1.tar.gz` & `tmp/werpy-0.0.2.tar.gz`

## Comparing `werpy-0.0.1.tar` & `werpy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 werpy-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.1/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
--rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.1/.github/assets/images/werpy-logo-word-error-rate.png
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.1/LICENSES/NUMPY_LICENSE
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.1/LICENSES/PANDAS_LICENSE
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/__init__.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/metrics.py
--rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/normalize.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/summary.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/wer.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/werp.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/werps.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 werpy-0.0.1/werpy/wers.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 werpy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.1/LICENSE
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 werpy-0.0.1/README.md
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 werpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 werpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 werpy-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    27165 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png
+-rw-r--r--   0        0        0    93938 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/assets/images/werpy-logo-word-error-rate.png
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/workflows/codacy.yml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 werpy-0.0.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSES/PANDAS_LICENSE
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/__init__.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/metrics.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/normalize.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/summary.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/wer.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/werp.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/werps.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 werpy-0.0.2/werpy/wers.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 werpy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 werpy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 werpy-0.0.2/README.md
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 werpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 werpy-0.0.2/PKG-INFO
```

### Comparing `werpy-0.0.1/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png` & `werpy-0.0.2/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.1/.github/assets/images/werpy-logo-word-error-rate.png` & `werpy-0.0.2/.github/assets/images/werpy-logo-word-error-rate.png`

 * *Files identical despite different names*

### Comparing `werpy-0.0.1/LICENSES/NUMPY_LICENSE` & `werpy-0.0.2/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.1/LICENSES/PANDAS_LICENSE` & `werpy-0.0.2/LICENSES/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.1/werpy/metrics.py` & `werpy-0.0.2/werpy/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+"""
+This module contains two functions: calculations and metrics. The calculations function takes two input sequences (
+reference and hypothesis) and returns a ragged array containing the word error rate (WER), Levenshtein distance (LD), 
+number of words in the reference sequence, counts of insertions, deletions and substitutions, as well as lists of 
+inserted, deleted and substituted words. The metrics function applies vectorization to the calculations function, 
+enabling it to take in multiple values for reference and hypothesis in the form of lists or numpy arrays.
+
+Functions:
+- calculations(reference, hypothesis) -> np.ndarray: Calculates WER and related metrics for two input sequences and 
+returns a ragged array containing the metrics.
+- metrics(reference, hypothesis) -> np.ndarray: Applies vectorization to the calculations function to calculate WER 
+and related metrics for multiple pairs of input sequences.
+"""
+
 import numpy as np
 
 
 def calculations(reference, hypothesis) -> np.ndarray:
     """
     This function calculates the word error rate and provides a breakdown of the word edits (inserts, deletions and
     substitutions) required to minimally transform one text sequence into another.
```

### Comparing `werpy-0.0.1/werpy/normalize.py` & `werpy-0.0.2/werpy/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+The Normalize module provides preprocessing methods for normalizing text input to be optimal for the Word Error Rate
+(WER) function. The class contains methods for removing punctuation, converting text to lowercase, replacing double
+spaces with a single space, and removing leading and trailing spaces. The apply_normalization method applies all the 
+normalization methods and returns the normalized input as a numpy array.
+"""
+
 import numpy as np
 
 
 class Normalize:
     """
     A class that provides the preprocessing methods for normalizing a text input.
     This class transforms text data into the optimal input format for the Word Error Rate (WER) function.
```

### Comparing `werpy-0.0.1/werpy/summary.py` & `werpy-0.0.2/werpy/summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+This module provides a summary function to display a complete breakdown of the calculated results, returned in a 
+DataFrame.
+
+This module defines the following function:
+    - summary(reference, hypothesis)
+"""
+
 import pandas as pd
 import werpy
 
 
 def summary(reference, hypothesis):
     """
     This function provides a comprehensive breakdown of the calculated results including the WER, Levenshtein
```

### Comparing `werpy-0.0.1/werpy/wer.py` & `werpy-0.0.2/werpy/wer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+This module provides a function for calculating the Word Error Rate (WER) between a reference text and a hypothesis 
+text. The WER is calculated as the number of edits (insertions, deletions, and substitutions) needed to transform 
+the hypothesis text into the reference text, divided by the number of words in the reference text.
+
+This module defines the following function:
+    - wer(reference, hypothesis): Calculate the WER between a reference text and a hypothesis text.
+"""
+
 import numpy as np
 import werpy
 
 
 def wer(reference, hypothesis) -> float:
     """
     This function will calculate the overall Word Error Rate for the entire reference and hypothesis texts.
@@ -42,14 +51,14 @@
         word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print("AttributeError: All text should be in a string format. Please check your input does not include any "
               "Numeric data types.")
     else:
-        if type(word_error_rate_breakdown[0]) == np.ndarray:
+        if isinstance(word_error_rate_breakdown[0], np.ndarray):
             transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
             wer_result = (np.sum(transform_word_error_rate_breakdown[1])) / (np.sum(transform_word_error_rate_breakdown[
                                                                                      2]))
         else:
             wer_result = word_error_rate_breakdown[0]
         return wer_result
```

### Comparing `werpy-0.0.1/werpy/werp.py` & `werpy-0.0.2/werpy/werp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+This module provides a function to calculate a weighted Word Error Rate for the entire reference and hypothesis 
+texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
+
+This module defines the following function:
+    - werp(reference, hypothesis)
+"""
+
 import numpy as np
 import werpy
 
 
 def werp(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a weighted Word Error Rate for the entire reference and hypothesis texts. It allows the
@@ -58,15 +66,15 @@
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print(
             "AttributeError: All text should be in a string format. Please check your input does not include any "
             "Numeric data types.")
     else:
-        if type(word_error_rate_breakdown[0]) == np.ndarray:
+        if isinstance(word_error_rate_breakdown[0], np.ndarray):
             transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
             weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
             weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
             weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
             m = np.sum(transform_word_error_rate_breakdown[2])
         else:
             weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
```

### Comparing `werpy-0.0.1/werpy/werps.py` & `werpy-0.0.2/werpy/werps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+This module provides a function for calculating a list of weighted Word Error Rate for each of the reference and
+hypothesis texts. It allows varying weights to be assigned to the insertion, deletion and substitution errors.
+
+This module defines the following function:
+    - werps(reference, hypothesis)
+"""
+
 import numpy as np
 import werpy
 
 
 def werps(reference, hypothesis, insertions_weight=1, deletions_weight=1, substitutions_weight=1):
     """
     This function calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. It
@@ -52,15 +60,15 @@
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print(
             "AttributeError: All text should be in a string format. Please check your input does not include any "
             "Numeric data types.")
     else:
-        if type(word_error_rate_breakdown[0]) == np.ndarray:
+        if isinstance(word_error_rate_breakdown[0], np.ndarray):
             transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
             weighted_insertions = transform_word_error_rate_breakdown[3] * insertions_weight
             weighted_deletions = transform_word_error_rate_breakdown[4] * deletions_weight
             weighted_substitutions = transform_word_error_rate_breakdown[5] * substitutions_weight
             m = transform_word_error_rate_breakdown[2]
         else:
             weighted_insertions = word_error_rate_breakdown[3] * insertions_weight
```

### Comparing `werpy-0.0.1/werpy/wers.py` & `werpy-0.0.2/werpy/wers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+This module provides a function for calculating a list of the Word Error Rates for each of the reference and
+hypothesis texts.
+
+This module defines the following function:
+    - wers(reference, hypothesis)
+"""
+
+
 import numpy as np
 import werpy
 
 
 def wers(reference, hypothesis):
     """
     This function calculates a list of the Word Error Rates for each of the reference and hypothesis texts.
@@ -39,13 +48,13 @@
         word_error_rate_breakdown = werpy.metrics(reference, hypothesis)
     except ValueError:
         print("ValueError: The Reference and Hypothesis input parameters must have the same number of elements.")
     except AttributeError:
         print("AttributeError: All text should be in a string format. Please check your input does not include any "
               "Numeric data types.")
     else:
-        if type(word_error_rate_breakdown[0]) == np.ndarray:
+        if isinstance(word_error_rate_breakdown[0], np.ndarray):
             transform_word_error_rate_breakdown = np.transpose(word_error_rate_breakdown.tolist())
             wers_result = transform_word_error_rate_breakdown[0].tolist()
         else:
             wers_result = word_error_rate_breakdown[0].tolist()
         return wers_result
```

### Comparing `werpy-0.0.1/.gitignore` & `werpy-0.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -154,7 +154,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# VSCode
+.vscode/
```

### Comparing `werpy-0.0.1/LICENSE` & `werpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `werpy-0.0.1/README.md` & `werpy-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
-# werpy - Word Error Rate for Python
+# werpy (Word Error Rate for Python)
 <!-- badges: start -->
 [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp;
 [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;
 ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;
+[![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp;
+[![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp;
 <!-- badges: end -->
 
-## What is it?
+## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
 It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
 Additionally, the summary function provides a comprehensive breakdown of the calculated results to assist in analyzing the specific errors quickly and in more detail.
 <br />
 
 ## Installation
 You can install the latest **werpy** release with Python's pip package manager:
 
 ```python
-# install werpy via PyPi
+# Install werpy from PyPi
 pip install werpy
 ```
 
 ## Main Functions
 The following table provides an overview of the functions that can be used in werpy.
 
 | Function  | Description | 
@@ -34,91 +36,140 @@
 | werp(reference, hypothesis)  | Calculates a weighted Word Error Rate for the entire reference and hypothesis texts. |
 | werps(reference, hypothesis)  | Calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. |
 | summary(reference, hypothesis)  | Provides a comprehensive breakdown of the calculated results including the WER, Levenshtein Distance and all the insertion, deletion and substitution errors. |
 
 
 ## Usage
 **Import the werpy package**
+
+*Python Code:*
 ```python
->>> import werpy
+import werpy
 ```
+<br />
 
 **Example 1 - Normalize a list of text**
+
+*Python Code:*
 ```python
->>> input_data = ["It's very popular in Antarctica.","The Sugar Bear character"]
->>> reference = werpy.normalize(input_data)
->>> print(reference)
+input_data = ["It's very popular in Antarctica.","The Sugar Bear character"]
+reference = werpy.normalize(input_data)
+print(reference)
+```
+
+*Results Output:*
+```
 ['its very popular in antarctica', 'the sugar bear character']
 ```
+<br />
 
 **Example 2 - Calculate the overall Word Error Rate on a set of strings**
+
+*Python Code:*
 ```python
->>> wer = werpy.wer('i love cold pizza', 'i love pizza')
->>> print(wer)
+wer = werpy.wer('i love cold pizza', 'i love pizza')
+print(wer)
+```
+
+*Results Output:*
+```
 0.25
 ```
+<br />
 
 **Example 3 - Calculate the overall Word Error Rate on a set of lists**
+
+*Python Code:*
 ```python
->>> ref = ['i love cold pizza','the sugar bear character was popular']
->>> hyp = ['i love pizza','the sugar bare character was popular']
->>> wer = werpy.wer(ref, hyp)
->>> print(wer)
+ref = ['i love cold pizza','the sugar bear character was popular']
+hyp = ['i love pizza','the sugar bare character was popular']
+wer = werpy.wer(ref, hyp)
+print(wer)
+```
+
+*Results Output:*
+```
 0.2
 ```
+<br />
 
 **Example 4 - Calculate the Word Error Rates for each set of texts**
+
+*Python Code:*
 ```python
->>> ref = ['no one else could claim that','she cited multiple reasons why']
->>> hyp = ['no one else could claim that','she sighted multiple reasons why']
->>> wers = werpy.wers(ref, hyp)
->>> print(wers)
+ref = ['no one else could claim that','she cited multiple reasons why']
+hyp = ['no one else could claim that','she sighted multiple reasons why']
+wers = werpy.wers(ref, hyp)
+print(wers)
+```
+
+*Results Output:*
+```
 [0.0, 0.2]
 ```
+<br />
 
 **Example 5 - Calculate the weighted Word Error Rates for the entire set of text**
+
+*Python Code:*
 ```python
->>> ref = ['it was beautiful and sunny today']
->>> hyp = ['it was a beautiful and sunny day']
->>> werp = werpy.werp(ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1)
->>> print(werp)
+ref = ['it was beautiful and sunny today']
+hyp = ['it was a beautiful and sunny day']
+werp = werpy.werp(ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1)
+print(werp)
+```
+
+*Results Output:*
+```
 0.25
 ```
+<br />
 
 **Example 6 - Calculate a list of weighted Word Error Rates for each of the reference and hypothesis texts**
+
+*Python Code:*
 ```python
->>> ref = ['it blocked sight lines of central park', 'her father was an alderman in the city government']
->>> hyp = ['it blocked sightlines of central park', 'our father was an elder man in the city government']
->>> werps = werpy.werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
->>> print(werps)
+ref = ['it blocked sight lines of central park', 'her father was an alderman in the city government']
+hyp = ['it blocked sightlines of central park', 'our father was an elder man in the city government']
+werps = werpy.werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
+print(werps)
+```
+
+*Results Output:*
+```
 [0.21428571428571427, 0.2777777777777778]
 ```
+<br />
 
 **Example 7 - Provide a complete breakdown of the Word Error Rate calculations for each of the reference and hypothesis texts**
+
+*Python Code:*
 ```python
->>> ref = ['it is consumed domestically and exported to other countries', 'rufino street in makati right inside the makati central business district', 'its estuary is considered to have abnormally low rates of dissolved oxygen', 'he later cited his first wife anita as the inspiration for the song', 'no one else could claim that']
->>> hyp = ['it is consumed domestically and exported to other countries', 'rofino street in mccauti right inside the macasi central business district', 'its estiary is considered to have a normally low rates of dissolved oxygen', 'he later sighted his first wife anita as the inspiration for the song', 'no one else could claim that']
->>> summary = werpy.summary(ref, hyp)
->>> print(summary)
+ref = ['it is consumed domestically and exported to other countries', 'rufino street in makati right inside the makati central business district', 'its estuary is considered to have abnormally low rates of dissolved oxygen', 'he later cited his first wife anita as the inspiration for the song', 'no one else could claim that']
+hyp = ['it is consumed domestically and exported to other countries', 'rofino street in mccauti right inside the macasi central business district', 'its estiary is considered to have a normally low rates of dissolved oxygen', 'he later sighted his first wife anita as the inspiration for the song', 'no one else could claim that']
+summary = werpy.summary(ref, hyp)
+print(summary)
 ```
+
+*Results Output:*
 <!-- <img src=".github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png" width=100% height=100%> -->
 <!-- <img src="https://github.com/analyticsinmotion/werpy/blob/main/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png" width=100% height=100%> -->
 <!-- ![werpy summary DataFrame](.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png)-->
 
 ![werpy-example-summary-results-word-error-rate-breakdown](https://user-images.githubusercontent.com/52817125/234950114-7efcce9b-7a76-4413-830f-7deda20cad75.png)
-
+<br />
 
 
 ## Dependencies
  - <a href="https://www.numpy.org">NumPy</a> - Provides an assortment of routines for fast operations on arrays
  - <a href="https://pandas.pydata.org/">Pandas</a> - Powerful data structures for data analysis, time series, and statistics
 
 ## Licensing
 
-``werpy`` is released under the terms of the BSD 3-Clause License. Please refer to the LICENSE file for full details.
+``werpy`` is released under the terms of the BSD 3-Clause License. Please refer to the <a href="https://github.com/analyticsinmotion/werpy/blob/main/LICENSE">LICENSE</a> file for full details.
 
 This project also includes third-party packages distributed under the BSD-3-Clause license, including NumPy and Pandas.
 
 The full NumPy and Pandas licenses can be found in the <a href="https://github.com/analyticsinmotion/werpy/tree/main/LICENSES">LICENSES</a> directory in this repository. 
 
 They can also be found directly in the following source codes:
```

### Comparing `werpy-0.0.1/pyproject.toml` & `werpy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "werpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ross Armstrong", email="ross.armstrong@analyticsinmotion.com" },
 ]
 description = "A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER)."
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
```

### Comparing `werpy-0.0.1/PKG-INFO` & `werpy-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A powerful yet lightweight Python package to calculate and analyze the Word Error Rate (WER).
 Project-URL: Homepage, https://github.com/analyticsinmotion/werpy
 Project-URL: Bug Tracker, https://github.com/analyticsinmotion/werpy/issues
 Author-email: Ross Armstrong <ross.armstrong@analyticsinmotion.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: levenshtein distance,nlp,python,python package,speech to text,stt,wer,word error rate
@@ -16,34 +16,36 @@
 Requires-Dist: numpy>=1.21.6; python_version < '3.11'
 Requires-Dist: numpy>=1.23.2; python_version >= '3.11'
 Requires-Dist: pandas>=1.3.0
 Description-Content-Type: text/markdown
 
 
 ![werpy-logo-word-error-rate](https://user-images.githubusercontent.com/52817125/235063664-2f21629c-0fad-46b6-a487-c2b5ef6f80e9.png)
-# werpy - Word Error Rate for Python
+# werpy (Word Error Rate for Python)
 <!-- badges: start -->
 [![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10%7C3.11-blue?logo=python&logoColor=ffdd54)](https://www.python.org/downloads/)&nbsp;&nbsp;
 [![werpy License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/analyticsinmotion/werpy/blob/main/LICENSE)&nbsp;&nbsp;
 ![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)&nbsp;&nbsp;
+[![CodeQL](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codeql.yml)&nbsp;&nbsp;
+[![Codacy Security Scan](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml/badge.svg)](https://github.com/analyticsinmotion/werpy/actions/workflows/codacy.yml)&nbsp;&nbsp;
 <!-- badges: end -->
 
-## What is it?
+## What is werpy?
 **werpy** is a powerful yet lightweight Python package that rapidly calculates and analyzes the Word Error Rate (WER) between two sets of text. 
 It has been designed with the flexibility to handle multiple input data types such as strings, lists and numpy arrays.<br />
 
 The package also includes a full set of features such as normalizing the input text to account for data collection variability and the capability to easily assign different weights/penalties to specific error classifications (insertions, deletions, and substitutions).
 Additionally, the summary function provides a comprehensive breakdown of the calculated results to assist in analyzing the specific errors quickly and in more detail.
 <br />
 
 ## Installation
 You can install the latest **werpy** release with Python's pip package manager:
 
 ```python
-# install werpy via PyPi
+# Install werpy from PyPi
 pip install werpy
 ```
 
 ## Main Functions
 The following table provides an overview of the functions that can be used in werpy.
 
 | Function  | Description | 
@@ -54,91 +56,140 @@
 | werp(reference, hypothesis)  | Calculates a weighted Word Error Rate for the entire reference and hypothesis texts. |
 | werps(reference, hypothesis)  | Calculates a list of weighted Word Error Rates for each of the reference and hypothesis texts. |
 | summary(reference, hypothesis)  | Provides a comprehensive breakdown of the calculated results including the WER, Levenshtein Distance and all the insertion, deletion and substitution errors. |
 
 
 ## Usage
 **Import the werpy package**
+
+*Python Code:*
 ```python
->>> import werpy
+import werpy
 ```
+<br />
 
 **Example 1 - Normalize a list of text**
+
+*Python Code:*
 ```python
->>> input_data = ["It's very popular in Antarctica.","The Sugar Bear character"]
->>> reference = werpy.normalize(input_data)
->>> print(reference)
+input_data = ["It's very popular in Antarctica.","The Sugar Bear character"]
+reference = werpy.normalize(input_data)
+print(reference)
+```
+
+*Results Output:*
+```
 ['its very popular in antarctica', 'the sugar bear character']
 ```
+<br />
 
 **Example 2 - Calculate the overall Word Error Rate on a set of strings**
+
+*Python Code:*
 ```python
->>> wer = werpy.wer('i love cold pizza', 'i love pizza')
->>> print(wer)
+wer = werpy.wer('i love cold pizza', 'i love pizza')
+print(wer)
+```
+
+*Results Output:*
+```
 0.25
 ```
+<br />
 
 **Example 3 - Calculate the overall Word Error Rate on a set of lists**
+
+*Python Code:*
 ```python
->>> ref = ['i love cold pizza','the sugar bear character was popular']
->>> hyp = ['i love pizza','the sugar bare character was popular']
->>> wer = werpy.wer(ref, hyp)
->>> print(wer)
+ref = ['i love cold pizza','the sugar bear character was popular']
+hyp = ['i love pizza','the sugar bare character was popular']
+wer = werpy.wer(ref, hyp)
+print(wer)
+```
+
+*Results Output:*
+```
 0.2
 ```
+<br />
 
 **Example 4 - Calculate the Word Error Rates for each set of texts**
+
+*Python Code:*
 ```python
->>> ref = ['no one else could claim that','she cited multiple reasons why']
->>> hyp = ['no one else could claim that','she sighted multiple reasons why']
->>> wers = werpy.wers(ref, hyp)
->>> print(wers)
+ref = ['no one else could claim that','she cited multiple reasons why']
+hyp = ['no one else could claim that','she sighted multiple reasons why']
+wers = werpy.wers(ref, hyp)
+print(wers)
+```
+
+*Results Output:*
+```
 [0.0, 0.2]
 ```
+<br />
 
 **Example 5 - Calculate the weighted Word Error Rates for the entire set of text**
+
+*Python Code:*
 ```python
->>> ref = ['it was beautiful and sunny today']
->>> hyp = ['it was a beautiful and sunny day']
->>> werp = werpy.werp(ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1)
->>> print(werp)
+ref = ['it was beautiful and sunny today']
+hyp = ['it was a beautiful and sunny day']
+werp = werpy.werp(ref, hyp, insertions_weight=0.5, deletions_weight=0.5, substitutions_weight=1)
+print(werp)
+```
+
+*Results Output:*
+```
 0.25
 ```
+<br />
 
 **Example 6 - Calculate a list of weighted Word Error Rates for each of the reference and hypothesis texts**
+
+*Python Code:*
 ```python
->>> ref = ['it blocked sight lines of central park', 'her father was an alderman in the city government']
->>> hyp = ['it blocked sightlines of central park', 'our father was an elder man in the city government']
->>> werps = werpy.werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
->>> print(werps)
+ref = ['it blocked sight lines of central park', 'her father was an alderman in the city government']
+hyp = ['it blocked sightlines of central park', 'our father was an elder man in the city government']
+werps = werpy.werps(ref, hyp, insertions_weight = 0.5, deletions_weight = 0.5, substitutions_weight = 1)
+print(werps)
+```
+
+*Results Output:*
+```
 [0.21428571428571427, 0.2777777777777778]
 ```
+<br />
 
 **Example 7 - Provide a complete breakdown of the Word Error Rate calculations for each of the reference and hypothesis texts**
+
+*Python Code:*
 ```python
->>> ref = ['it is consumed domestically and exported to other countries', 'rufino street in makati right inside the makati central business district', 'its estuary is considered to have abnormally low rates of dissolved oxygen', 'he later cited his first wife anita as the inspiration for the song', 'no one else could claim that']
->>> hyp = ['it is consumed domestically and exported to other countries', 'rofino street in mccauti right inside the macasi central business district', 'its estiary is considered to have a normally low rates of dissolved oxygen', 'he later sighted his first wife anita as the inspiration for the song', 'no one else could claim that']
->>> summary = werpy.summary(ref, hyp)
->>> print(summary)
+ref = ['it is consumed domestically and exported to other countries', 'rufino street in makati right inside the makati central business district', 'its estuary is considered to have abnormally low rates of dissolved oxygen', 'he later cited his first wife anita as the inspiration for the song', 'no one else could claim that']
+hyp = ['it is consumed domestically and exported to other countries', 'rofino street in mccauti right inside the macasi central business district', 'its estiary is considered to have a normally low rates of dissolved oxygen', 'he later sighted his first wife anita as the inspiration for the song', 'no one else could claim that']
+summary = werpy.summary(ref, hyp)
+print(summary)
 ```
+
+*Results Output:*
 <!-- <img src=".github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png" width=100% height=100%> -->
 <!-- <img src="https://github.com/analyticsinmotion/werpy/blob/main/.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png" width=100% height=100%> -->
 <!-- ![werpy summary DataFrame](.github/assets/images/werpy-example-summary-results-word-error-rate-breakdown.png)-->
 
 ![werpy-example-summary-results-word-error-rate-breakdown](https://user-images.githubusercontent.com/52817125/234950114-7efcce9b-7a76-4413-830f-7deda20cad75.png)
-
+<br />
 
 
 ## Dependencies
  - <a href="https://www.numpy.org">NumPy</a> - Provides an assortment of routines for fast operations on arrays
  - <a href="https://pandas.pydata.org/">Pandas</a> - Powerful data structures for data analysis, time series, and statistics
 
 ## Licensing
 
-``werpy`` is released under the terms of the BSD 3-Clause License. Please refer to the LICENSE file for full details.
+``werpy`` is released under the terms of the BSD 3-Clause License. Please refer to the <a href="https://github.com/analyticsinmotion/werpy/blob/main/LICENSE">LICENSE</a> file for full details.
 
 This project also includes third-party packages distributed under the BSD-3-Clause license, including NumPy and Pandas.
 
 The full NumPy and Pandas licenses can be found in the <a href="https://github.com/analyticsinmotion/werpy/tree/main/LICENSES">LICENSES</a> directory in this repository. 
 
 They can also be found directly in the following source codes:
```

