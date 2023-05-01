# Comparing `tmp/streamlit-vizzu-0.1.2.tar.gz` & `tmp/streamlit-vizzu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-vizzu-0.1.2.tar", last modified: Thu Feb 23 14:41:59 2023, max compression
+gzip compressed data, was "streamlit-vizzu-0.1.3.tar", last modified: Mon May  1 17:21:48 2023, max compression
```

## Comparing `streamlit-vizzu-0.1.2.tar` & `streamlit-vizzu-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/src/streamlit_vizzu/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/ipyvizzu.js
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:47.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:41:59.571554 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 14:41:59.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-23 14:41:59.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 14:41:59.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 14:41:59.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-23 14:41:59.000000 streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:48.594154 streamlit-vizzu-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 17:21:48.590154 streamlit-vizzu-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:21:48.594154 streamlit-vizzu-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:48.586154 streamlit-vizzu-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:48.590154 streamlit-vizzu-0.1.3/src/streamlit_vizzu/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:48.590154 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:30.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:21:48.590154 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 17:21:48.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 17:21:48.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:21:48.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 17:21:48.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 17:21:48.000000 streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/top_level.txt
```

### Comparing `streamlit-vizzu-0.1.2/LICENSE` & `streamlit-vizzu-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-vizzu-0.1.2/PKG-INFO` & `streamlit-vizzu-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-vizzu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bidirectional streamlit component for interacting with vizzu animations
 Author: Zachary Blackwoood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-vizzu-0.1.2/README.md` & `streamlit-vizzu-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-vizzu-0.1.2/setup.py` & `streamlit-vizzu-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-vizzu",
-    version="0.1.2",
+    version="0.1.3",
     author="Zachary Blackwoood",
     author_email="zachary@streamlit.io",
     description=(
         "Bidirectional streamlit component for interacting with vizzu animations"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `streamlit-vizzu-0.1.2/src/streamlit_vizzu/chart.py` & `streamlit-vizzu-0.1.3/src/streamlit_vizzu/chart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
+from importlib_metadata import version
+from distutils.version import StrictVersion
+import uuid
 
 import streamlit as st
 import streamlit.components.v1 as components
 from ipyvizzu.chart import Chart
 from ipyvizzu.method import Animate
 from ipyvizzu.template import DisplayTarget, DisplayTemplate
 
@@ -46,23 +49,25 @@
         self.chart_id = f"{self.key}_vizzu_chart"
         self.animations: list[str] = []
         self.return_clicks = return_clicks
         self.height = height
         self.chart_height = height - 20
         self.rerun_on_click = rerun_on_click
         self.default_duration = default_duration
+        self.ipyvizzu_version = StrictVersion(version("ipyvizzu"))
 
         super().__init__(
             width=f"{width}px",
             height=f"{self.chart_height}px",
             display=DisplayTarget.MANUAL,
             **kwargs,
         )
 
-        self._chart_id
+        if self.ipyvizzu_version >= StrictVersion("0.15.0"):
+            self.initializing()
 
     def show(self):
         """
         Render your chart within your streamlit app. Note that any animations
         applied after your chart is shown will not affect the chart.
         """
         component_value = _component_func(
@@ -117,19 +122,33 @@
 
         return script
 
     def _repr_html_(self) -> str:
         return f'<div id="{self.chart_id}"><script>{self._get_script()}</script></div>'
 
     def _animation_to_js(self, *animations: Any, **options: Any):
-        animation = self._merge_animations(animations)
+        if self.ipyvizzu_version < StrictVersion("0.15.0"):
+            animation = self._merge_animations(animations)
+            animate = Animate(animation, options)
+            return DisplayTemplate.ANIMATE.format(
+                display_target=self._display_target.value,
+                chart_id=self._chart_id,
+                scroll=str(self._scroll_into_view).lower(),
+                **animate.dump(),
+            )
+
+        from ipyvizzu.animation import AnimationMerger
+
+        animation = AnimationMerger.merge_animations(animations)
         animate = Animate(animation, options)
+        self._last_anim = uuid.uuid4().hex[:7]
         return DisplayTemplate.ANIMATE.format(
             display_target=self._display_target.value,
             chart_id=self._chart_id,
+            anim_id=self._last_anim,
             scroll=str(self._scroll_into_view).lower(),
             **animate.dump(),
         )
 
     def animate(self, *animations: Any, **options: Any):
         """
         Pass any number of Animation objects (e.g. Data, Config, or Style objects), and
```

### Comparing `streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/main.js` & `streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-vizzu-0.1.2/src/streamlit_vizzu/frontend/streamlit-component-lib.js` & `streamlit-vizzu-0.1.3/src/streamlit_vizzu/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-vizzu-0.1.2/src/streamlit_vizzu.egg-info/PKG-INFO` & `streamlit-vizzu-0.1.3/src/streamlit_vizzu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-vizzu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bidirectional streamlit component for interacting with vizzu animations
 Author: Zachary Blackwoood
 Author-email: zachary@streamlit.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

