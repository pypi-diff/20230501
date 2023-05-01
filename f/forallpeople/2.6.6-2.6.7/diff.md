# Comparing `tmp/forallpeople-2.6.6.tar.gz` & `tmp/forallpeople-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forallpeople-2.6.6.tar", last modified: Tue Dec 27 20:47:35 2022, max compression
+gzip compressed data, was "forallpeople-2.6.7.tar", last modified: Mon May  1 05:08:31 2023, max compression
```

## Comparing `forallpeople-2.6.6.tar` & `forallpeople-2.6.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2022-12-23 01:36:12.117560 forallpeople-2.6.6/.github/workflows/sphinx_to_gh_pages.yaml
--rw-r--r--   0        0        0     2225 2022-12-23 01:36:12.117560 forallpeople-2.6.6/.gitignore
--rw-r--r--   0        0        0       46 2022-12-23 01:36:12.118561 forallpeople-2.6.6/.travis.yml
--rw-r--r--   0        0        0   116974 2022-12-23 01:36:12.119566 forallpeople-2.6.6/Jupyter.PNG
--rw-r--r--   0        0        0   116974 2022-12-23 01:36:12.120564 forallpeople-2.6.6/Jupyter_example.PNG
--rw-r--r--   0        0        0    11560 2022-12-23 01:36:12.120564 forallpeople-2.6.6/LICENSE.TXT
--rw-r--r--   0        0        0       27 2022-12-23 01:36:12.120564 forallpeople-2.6.6/MANIFEST.in
--rw-r--r--   0        0        0    16486 2022-12-23 01:36:12.121503 forallpeople-2.6.6/README.md
--rw-r--r--   0        0        0      632 2022-12-23 01:36:12.121560 forallpeople-2.6.6/docs/Makefile
--rw-r--r--   0        0        0   924752 2022-12-23 01:36:12.126560 forallpeople-2.6.6/docs/images/basic_usage1.gif
--rw-r--r--   0        0        0   373011 2022-12-23 01:36:12.128560 forallpeople-2.6.6/docs/images/basic_usage2.gif
--rwxr-xr-x   0        0        0      820 2022-12-23 01:36:12.129560 forallpeople-2.6.6/docs/make.bat
--rw-r--r--   0        0        0    12288 2022-12-23 01:36:12.129560 forallpeople-2.6.6/docs/source/.index.rst.swp
--rw-r--r--   0        0        0     8958 2022-12-23 01:36:12.129560 forallpeople-2.6.6/docs/source/background.ipynb
--rw-r--r--   0        0        0     9369 2022-12-23 01:36:12.130560 forallpeople-2.6.6/docs/source/basic_usage.ipynb
--rw-r--r--   0        0        0     5200 2022-12-23 01:36:12.130560 forallpeople-2.6.6/docs/source/conf.py
--rw-r--r--   0        0        0    11305 2022-12-23 01:36:12.130560 forallpeople-2.6.6/docs/source/empiricals.ipynb
--rw-r--r--   0        0        0     4148 2022-12-23 01:36:12.131566 forallpeople-2.6.6/docs/source/environments.ipynb
--rw-r--r--   0        0        0     3920 2022-12-23 01:36:12.131566 forallpeople-2.6.6/docs/source/index.ipynb
--rw-r--r--   0        0        0     2216 2022-12-23 01:36:12.132115 forallpeople-2.6.6/docs/source/interface.ipynb
--rw-r--r--   0        0        0    16531 2022-12-23 01:36:12.132115 forallpeople-2.6.6/docs/source/standard_behaviours.ipynb
--rw-r--r--   0        0        0      222 2022-12-23 01:36:12.132561 forallpeople-2.6.6/docs_env.yml
--rw-r--r--   0        0        0    24954 2022-12-27 20:47:22.536758 forallpeople-2.6.6/forallpeople/__init__.py
--rw-r--r--   0        0        0      835 2022-12-23 01:36:12.133177 forallpeople-2.6.6/forallpeople/dimensions.py
--rw-r--r--   0        0        0     8218 2022-12-23 01:36:12.133561 forallpeople-2.6.6/forallpeople/environment.py
--rw-r--r--   0        0        0     1169 2022-12-23 01:36:12.133561 forallpeople-2.6.6/forallpeople/environments/default.json
--rw-r--r--   0        0        0      747 2022-12-23 01:36:12.133561 forallpeople-2.6.6/forallpeople/environments/electrical.json
--rw-r--r--   0        0        0     4039 2022-12-23 01:36:12.134560 forallpeople-2.6.6/forallpeople/environments/structural.json
--rw-r--r--   0        0        0     2073 2022-12-23 01:36:12.134560 forallpeople-2.6.6/forallpeople/environments/test_definitions.json
--rw-r--r--   0        0        0     2253 2022-12-23 01:36:12.134560 forallpeople-2.6.6/forallpeople/environments/thermal.json
--rw-r--r--   0        0        0     2723 2022-12-23 01:36:12.135559 forallpeople-2.6.6/forallpeople/environments/us_customary.json
--rw-r--r--   0        0        0    18233 2022-12-27 20:47:22.537753 forallpeople-2.6.6/forallpeople/physical_helper_functions.py
--rw-r--r--   0        0        0    15951 2022-12-23 05:53:04.776759 forallpeople-2.6.6/forallpeople/tests/test_forallpeople.py
--rw-r--r--   0        0        0     4758 2022-12-23 01:36:12.136560 forallpeople-2.6.6/forallpeople/tests/test_tuplevector.py
--rw-r--r--   0        0        0    10086 2022-12-23 01:36:12.136560 forallpeople-2.6.6/forallpeople/tuplevector.py
--rw-r--r--   0        0        0      554 2022-12-23 01:36:12.136560 forallpeople-2.6.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-23 01:36:12.136560 forallpeople-2.6.6/requirements.txt
--rw-r--r--   0        0        0    16791 1970-01-01 00:00:00.000000 forallpeople-2.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-12-23 01:36:12.117560 forallpeople-2.6.7/.github/workflows/sphinx_to_gh_pages.yaml
+-rw-r--r--   0        0        0     2225 2022-12-23 01:36:12.117560 forallpeople-2.6.7/.gitignore
+-rw-r--r--   0        0        0       46 2022-12-23 01:36:12.118561 forallpeople-2.6.7/.travis.yml
+-rw-r--r--   0        0        0   116974 2022-12-23 01:36:12.119566 forallpeople-2.6.7/Jupyter.PNG
+-rw-r--r--   0        0        0   116974 2022-12-23 01:36:12.120564 forallpeople-2.6.7/Jupyter_example.PNG
+-rw-r--r--   0        0        0    11560 2022-12-23 01:36:12.120564 forallpeople-2.6.7/LICENSE.TXT
+-rw-r--r--   0        0        0       27 2022-12-23 01:36:12.120564 forallpeople-2.6.7/MANIFEST.in
+-rw-r--r--   0        0        0    16486 2022-12-23 01:36:12.121503 forallpeople-2.6.7/README.md
+-rw-r--r--   0        0        0      632 2022-12-23 01:36:12.121560 forallpeople-2.6.7/docs/Makefile
+-rw-r--r--   0        0        0   924752 2022-12-23 01:36:12.126560 forallpeople-2.6.7/docs/images/basic_usage1.gif
+-rw-r--r--   0        0        0   373011 2022-12-23 01:36:12.128560 forallpeople-2.6.7/docs/images/basic_usage2.gif
+-rwxr-xr-x   0        0        0      820 2022-12-23 01:36:12.129560 forallpeople-2.6.7/docs/make.bat
+-rw-r--r--   0        0        0    12288 2022-12-23 01:36:12.129560 forallpeople-2.6.7/docs/source/.index.rst.swp
+-rw-r--r--   0        0        0     8958 2022-12-23 01:36:12.129560 forallpeople-2.6.7/docs/source/background.ipynb
+-rw-r--r--   0        0        0     9369 2022-12-23 01:36:12.130560 forallpeople-2.6.7/docs/source/basic_usage.ipynb
+-rw-r--r--   0        0        0     5200 2022-12-23 01:36:12.130560 forallpeople-2.6.7/docs/source/conf.py
+-rw-r--r--   0        0        0    11305 2022-12-23 01:36:12.130560 forallpeople-2.6.7/docs/source/empiricals.ipynb
+-rw-r--r--   0        0        0     4148 2022-12-23 01:36:12.131566 forallpeople-2.6.7/docs/source/environments.ipynb
+-rw-r--r--   0        0        0     3920 2022-12-23 01:36:12.131566 forallpeople-2.6.7/docs/source/index.ipynb
+-rw-r--r--   0        0        0     2216 2022-12-23 01:36:12.132115 forallpeople-2.6.7/docs/source/interface.ipynb
+-rw-r--r--   0        0        0    16531 2022-12-23 01:36:12.132115 forallpeople-2.6.7/docs/source/standard_behaviours.ipynb
+-rw-r--r--   0        0        0      222 2022-12-23 01:36:12.132561 forallpeople-2.6.7/docs_env.yml
+-rw-r--r--   0        0        0    24954 2023-05-01 05:08:21.398170 forallpeople-2.6.7/forallpeople/__init__.py
+-rw-r--r--   0        0        0      835 2022-12-23 01:36:12.133177 forallpeople-2.6.7/forallpeople/dimensions.py
+-rw-r--r--   0        0        0     8218 2022-12-23 01:36:12.133561 forallpeople-2.6.7/forallpeople/environment.py
+-rw-r--r--   0        0        0     1169 2022-12-23 01:36:12.133561 forallpeople-2.6.7/forallpeople/environments/default.json
+-rw-r--r--   0        0        0      747 2022-12-23 01:36:12.133561 forallpeople-2.6.7/forallpeople/environments/electrical.json
+-rw-r--r--   0        0        0     3952 2023-05-01 05:08:21.399103 forallpeople-2.6.7/forallpeople/environments/structural.json
+-rw-r--r--   0        0        0     2073 2022-12-23 01:36:12.134560 forallpeople-2.6.7/forallpeople/environments/test_definitions.json
+-rw-r--r--   0        0        0     2253 2022-12-23 01:36:12.134560 forallpeople-2.6.7/forallpeople/environments/thermal.json
+-rw-r--r--   0        0        0     2723 2022-12-23 01:36:12.135559 forallpeople-2.6.7/forallpeople/environments/us_customary.json
+-rw-r--r--   0        0        0    18233 2022-12-27 20:47:22.537753 forallpeople-2.6.7/forallpeople/physical_helper_functions.py
+-rw-r--r--   0        0        0    15951 2022-12-23 05:53:04.776759 forallpeople-2.6.7/forallpeople/tests/test_forallpeople.py
+-rw-r--r--   0        0        0     4758 2022-12-23 01:36:12.136560 forallpeople-2.6.7/forallpeople/tests/test_tuplevector.py
+-rw-r--r--   0        0        0    10086 2022-12-23 01:36:12.136560 forallpeople-2.6.7/forallpeople/tuplevector.py
+-rw-r--r--   0        0        0      554 2022-12-23 01:36:12.136560 forallpeople-2.6.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-23 01:36:12.136560 forallpeople-2.6.7/requirements.txt
+-rw-r--r--   0        0        0    16791 1970-01-01 00:00:00.000000 forallpeople-2.6.7/PKG-INFO
```

### Comparing `forallpeople-2.6.6/.github/workflows/sphinx_to_gh_pages.yaml` & `forallpeople-2.6.7/.github/workflows/sphinx_to_gh_pages.yaml`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/.gitignore` & `forallpeople-2.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/Jupyter.PNG` & `forallpeople-2.6.7/Jupyter.PNG`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/Jupyter_example.PNG` & `forallpeople-2.6.7/Jupyter_example.PNG`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/LICENSE.TXT` & `forallpeople-2.6.7/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/README.md` & `forallpeople-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/Makefile` & `forallpeople-2.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/images/basic_usage1.gif` & `forallpeople-2.6.7/docs/images/basic_usage1.gif`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/images/basic_usage2.gif` & `forallpeople-2.6.7/docs/images/basic_usage2.gif`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/make.bat` & `forallpeople-2.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/.index.rst.swp` & `forallpeople-2.6.7/docs/source/.index.rst.swp`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/background.ipynb` & `forallpeople-2.6.7/docs/source/background.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/basic_usage.ipynb` & `forallpeople-2.6.7/docs/source/basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/conf.py` & `forallpeople-2.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/empiricals.ipynb` & `forallpeople-2.6.7/docs/source/empiricals.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/environments.ipynb` & `forallpeople-2.6.7/docs/source/environments.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/index.ipynb` & `forallpeople-2.6.7/docs/source/index.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/interface.ipynb` & `forallpeople-2.6.7/docs/source/interface.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/docs/source/standard_behaviours.ipynb` & `forallpeople-2.6.7/docs/source/standard_behaviours.ipynb`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/__init__.py` & `forallpeople-2.6.7/forallpeople/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 from __future__ import annotations
 
-__version__ = "2.6.6"
+__version__ = "2.6.7"
 
 from fractions import Fraction
 from typing import Union, Optional
 from forallpeople.dimensions import Dimensions
 import forallpeople.physical_helper_functions as phf
 import forallpeople.tuplevector as vec
 from forallpeople.environment import Environment
```

### Comparing `forallpeople-2.6.6/forallpeople/dimensions.py` & `forallpeople-2.6.7/forallpeople/dimensions.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environment.py` & `forallpeople-2.6.7/forallpeople/environment.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environments/default.json` & `forallpeople-2.6.7/forallpeople/environments/default.json`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environments/electrical.json` & `forallpeople-2.6.7/forallpeople/environments/electrical.json`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environments/structural.json` & `forallpeople-2.6.7/forallpeople/environments/structural.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972972972972973%*

 * *Differences: {'delete': "['J_m2']"}*

```diff
@@ -19,26 +19,14 @@
             0,
             0,
             0,
             0
         ],
         "Symbol": "J"
     },
-    "J_m2": {
-        "Dimension": [
-            1,
-            0,
-            -2,
-            0,
-            0,
-            0,
-            0
-        ],
-        "Symbol": "J*m\u207b\u00b2"
-    },
     "MJ": {
         "Dimension": [
             1,
             2,
             -2,
             0,
             0,
```

### Comparing `forallpeople-2.6.6/forallpeople/environments/test_definitions.json` & `forallpeople-2.6.7/forallpeople/environments/test_definitions.json`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environments/thermal.json` & `forallpeople-2.6.7/forallpeople/environments/thermal.json`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/environments/us_customary.json` & `forallpeople-2.6.7/forallpeople/environments/us_customary.json`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/physical_helper_functions.py` & `forallpeople-2.6.7/forallpeople/physical_helper_functions.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/tests/test_forallpeople.py` & `forallpeople-2.6.7/forallpeople/tests/test_forallpeople.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/tests/test_tuplevector.py` & `forallpeople-2.6.7/forallpeople/tests/test_tuplevector.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/forallpeople/tuplevector.py` & `forallpeople-2.6.7/forallpeople/tuplevector.py`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/pyproject.toml` & `forallpeople-2.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forallpeople-2.6.6/PKG-INFO` & `forallpeople-2.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forallpeople
-Version: 2.6.6
+Version: 2.6.7
 Summary: The SI Units: "For all people, for all time"
 Home-page: https://github.com/connorferster/forallpeople
 Author: Connor Ferster
 Author-email: connorferster@gmail.com
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: black >= 22.3.0 ; extra == "dev"
```

