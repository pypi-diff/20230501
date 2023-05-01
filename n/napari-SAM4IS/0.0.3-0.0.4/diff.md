# Comparing `tmp/napari-SAM4IS-0.0.3.tar.gz` & `tmp/napari-SAM4IS-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-SAM4IS-0.0.3.tar", last modified: Fri Apr 28 22:37:29 2023, max compression
+gzip compressed data, was "napari-SAM4IS-0.0.4.tar", last modified: Mon May  1 06:31:34 2023, max compression
```

## Comparing `napari-SAM4IS-0.0.3.tar` & `napari-SAM4IS-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242872 napari-SAM4IS-0.0.3/
--rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/LICENSE
--rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/MANIFEST.in
--rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 22:37:29.242940 napari-SAM4IS-0.0.3/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     2700 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/README.md
--rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/pyproject.toml
--rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-04-28 22:37:29.243270 napari-SAM4IS-0.0.3/setup.cfg
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.239608 napari-SAM4IS-0.0.3/src/
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.241261 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/
--rw-r--r--   0 hiroki     (501) staff       (20)     3985 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/SOURCES.txt
--rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/dependency_links.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/entry_points.txt
--rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/requires.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-04-28 22:37:29.000000 napari-SAM4IS-0.0.3/src/napari_SAM4IS.egg-info/top_level.txt
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242298 napari-SAM4IS-0.0.3/src/napari_sam4is/
--rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-04-28 22:37:12.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/__init__.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-28 22:37:29.242650 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/test_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4660 2023-04-28 05:37:46.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_utils.py
--rw-r--r--   0 hiroki     (501) staff       (20)    12040 2023-04-28 22:36:38.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.3/src/napari_sam4is/napari.yaml
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.798148 napari-SAM4IS-0.0.4/
+-rw-r--r--   0 hiroki     (501) staff       (20)    11358 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/LICENSE
+-rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/MANIFEST.in
+-rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-05-01 06:31:34.798259 napari-SAM4IS-0.0.4/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     6202 2023-04-30 03:47:39.000000 napari-SAM4IS-0.0.4/README.md
+-rw-r--r--   0 hiroki     (501) staff       (20)     1177 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/pyproject.toml
+-rw-r--r--   0 hiroki     (501) staff       (20)     1764 2023-05-01 06:31:34.798689 napari-SAM4IS-0.0.4/setup.cfg
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.795024 napari-SAM4IS-0.0.4/src/
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.796532 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/
+-rw-r--r--   0 hiroki     (501) staff       (20)     7487 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)      496 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/entry_points.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)      107 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/requires.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-05-01 06:31:34.000000 napari-SAM4IS-0.0.4/src/napari_SAM4IS.egg-info/top_level.txt
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.797407 napari-SAM4IS-0.0.4/src/napari_sam4is/
+-rw-r--r--   0 hiroki     (501) staff       (20)       85 2023-05-01 06:31:21.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/__init__.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-05-01 06:31:34.797803 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     1246 2023-04-23 07:36:32.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/test_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4710 2023-05-01 06:20:29.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_utils.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    12071 2023-05-01 06:27:14.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      282 2023-04-24 04:30:49.000000 napari-SAM4IS-0.0.4/src/napari_sam4is/napari.yaml
```

### Comparing `napari-SAM4IS-0.0.3/LICENSE` & `napari-SAM4IS-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.3/pyproject.toml` & `napari-SAM4IS-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.3/setup.cfg` & `napari-SAM4IS-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.3/src/napari_sam4is/_tests/test_widget.py` & `napari-SAM4IS-0.0.4/src/napari_sam4is/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-SAM4IS-0.0.3/src/napari_sam4is/_utils.py` & `napari-SAM4IS-0.0.4/src/napari_sam4is/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     else:
         pass
     return np.array(image)
 
 
 def check_image_type(viewer, layer_name):
     image = viewer.layers[layer_name].data
+    print(f'current image shape = {image.shape}')
     if len(image.shape) == 2: # Gray
         return "Gray"
     elif len(image.shape) > 4:
         return "Not supported"
     elif (len(image.shape) == 3)&(image.shape[-1] == 4):
         return "RGBA"
     elif (len(image.shape) == 3)&(image.shape[-1] == 1): # Gray
```

### Comparing `napari-SAM4IS-0.0.3/src/napari_sam4is/_widget.py` & `napari-SAM4IS-0.0.4/src/napari_sam4is/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,17 @@
                 self._save_btn.setEnabled(False)
 
     def _load_model(self):
         model_name = self._model_selection.currentText()
         self._sam_model = load_model(model_name)
         self._sam_model.to(device=self.device)
         self.sam_predictor = SamPredictor(self._sam_model)
+        print("model loaded")
         if self._image_layer_selection.currentText() != "":
-            self._on_layer_list_changed(None)
+            self._on_image_layer_changed(None)
 
     def _on_image_layer_changed(self, index):
         print("image_layer_changed")
         if self.sam_predictor is not None:
             self._image_type = check_image_type(self._viewer, self._image_layer_selection.currentText())
             if "stack" in self._image_type:
                 self._current_slice, _, _ = self._viewer.dims.current_step
```

