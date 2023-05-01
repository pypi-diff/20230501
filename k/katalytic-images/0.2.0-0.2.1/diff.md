# Comparing `tmp/katalytic-images-0.2.0.tar.gz` & `tmp/katalytic-images-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.2.0.tar", last modified: Mon May  1 11:06:19 2023, max compression
+gzip compressed data, was "katalytic-images-0.2.1.tar", last modified: Mon May  1 12:22:23 2023, max compression
```

## Comparing `katalytic-images-0.2.0.tar` & `katalytic-images-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.2.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.2.0/.gitignore
--rw-r--r--   0        0        0     3324 2023-04-30 14:15:39.110597 katalytic-images-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1198 2023-05-01 11:06:00.384195 katalytic-images-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.2.0/README.md
--rw-r--r--   0        0        0     1503 2023-05-01 11:06:00.368194 katalytic-images-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-05-01 10:57:08.769254 katalytic-images-0.2.0/src/katalytic/images.py
--rw-r--r--   0        0        0    11945 2023-05-01 11:00:26.823672 katalytic-images-0.2.0/tests/test_images.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 katalytic-images-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-05-01 07:17:35.782858 katalytic-images-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 12:19:15.021593 katalytic-images-0.2.1/.gitignore
+-rw-r--r--   0        0        0     3324 2023-05-01 07:17:35.782858 katalytic-images-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1395 2023-05-01 12:22:12.820063 katalytic-images-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-05-01 07:17:35.782858 katalytic-images-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2130 2023-05-01 07:17:35.782858 katalytic-images-0.2.1/README.md
+-rw-r--r--   0        0        0     1503 2023-05-01 12:22:12.820063 katalytic-images-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6780 2023-05-01 12:19:33.562095 katalytic-images-0.2.1/src/katalytic/images.py
+-rw-r--r--   0        0        0    11945 2023-05-01 12:19:15.021593 katalytic-images-0.2.1/tests/test_images.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 katalytic-images-0.2.1/PKG-INFO
```

### Comparing `katalytic-images-0.2.0/.gitignore` & `katalytic-images-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.0/.gitlab-ci.yml` & `katalytic-images-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.0/CHANGELOG.md` & `katalytic-images-0.2.1/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.2.1 (2023-05-01)
+### fix
+- [[`16b0fd1`](https://gitlab.com/katalytic/katalytic-images/commit/16b0fd1d66f06dff08afbdb22b4f319d7831db1e)] **draw:** change default font_scale from 1.75 to 1.25
+
+
 ## 0.2.0 (2023-05-01)
 ### feat
 - [[`0088b92`](https://gitlab.com/katalytic/katalytic-images/commit/0088b92ebc8afcddde775357a57006c4ae492195)] add bhwc, hwc, hw
 - [[`d33f595`](https://gitlab.com/katalytic/katalytic-images/commit/d33f595243f80d0ae5673622b5b4f6792786d63d)] add draw() and draw_inplace(); fix are_arrays_equal() when the shape is different
 - [[`e7fb20b`](https://gitlab.com/katalytic/katalytic-images/commit/e7fb20b238ef1f63dc8ea79db2260271ca9f79a9)] add load_image and save_image to the universal functions
```

### Comparing `katalytic-images-0.2.0/LICENSE.txt` & `katalytic-images-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.0/README.md` & `katalytic-images-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.0/pyproject.toml` & `katalytic-images-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.2.0"
+version = "0.2.1"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-images-0.2.0/src/katalytic/images.py` & `katalytic-images-0.2.1/src/katalytic/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,18 +149,18 @@
     }
 
     return {conversion.get(k, k): v for k, v in shape.items()}
 
 
 def _pick_draw_function(shape_type):
     fn = {
-        'circle': cv2.circle,  # cv.circle(img,(447,63), 63, (0,0,255), -1)
+        'circle': cv2.circle,
         'line': cv2.line,
-        'rectangle': cv2.rectangle,  # cv.rectangle(img,(384,0),(510,128),(0,255,0),3)
-        'text': cv2.putText, # cv.putText(img, text, org, fontFace, fontScale, color
+        'rectangle': cv2.rectangle,
+        'text': cv2.putText,
     }
 
     if shape_type not in fn:
         raise ValueError(f'Unknown shape: {shape_type!r}')
     else:
         return fn[shape_type]
 
@@ -168,15 +168,15 @@
 def _insert_defaults(shape):
     defaults = {
         'circle': {'thickness': -1},
         'line': {},
         'rectangle': {'thickness': -1},
         'text': {
             'font': cv2.FONT_HERSHEY_SIMPLEX,
-            'font_scale': 1.75,
+            'font_scale': 1.25,
             'thickness': 3,
         },
         'polygon': {},
     }
 
     return {**defaults.get(shape['type'], {}), **shape}
```

### Comparing `katalytic-images-0.2.0/tests/test_images.py` & `katalytic-images-0.2.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.2.0/PKG-INFO` & `katalytic-images-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.2.0
+Version: 0.2.1
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

