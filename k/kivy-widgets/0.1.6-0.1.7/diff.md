# Comparing `tmp/kivy_widgets-0.1.6.tar.gz` & `tmp/kivy_widgets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_widgets-0.1.6.tar", max compression
+gzip compressed data, was "kivy_widgets-0.1.7.tar", max compression
```

## Comparing `kivy_widgets-0.1.6.tar` & `kivy_widgets-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.6/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.6/kivy_widgets/__init__.py
--rw-r--r--   0        0        0     2723 2023-04-25 01:47:03.092367 kivy_widgets-0.1.6/kivy_widgets/buttons.py
--rw-r--r--   0        0        0     7716 2023-03-29 09:08:00.598752 kivy_widgets-0.1.6/kivy_widgets/color_definitions.py
--rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.6/kivy_widgets/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.6/kivy_widgets/icon_definitions.py
--rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.6/kivy_widgets/icons.py
--rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.6/kivy_widgets/inspector.py
--rw-r--r--   0        0        0       61 2023-03-24 03:42:53.850005 kivy_widgets-0.1.6/kivy_widgets/test.py
--rw-r--r--   0        0        0      994 2023-04-25 01:50:50.658374 kivy_widgets-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.7/kivy_widgets/__init__.py
+-rw-r--r--   0        0        0     3686 2023-05-01 20:55:55.093542 kivy_widgets-0.1.7/kivy_widgets/buttons.py
+-rw-r--r--   0        0        0     7716 2023-04-27 06:16:20.787339 kivy_widgets-0.1.7/kivy_widgets/color_definitions.py
+-rw-r--r--   0        0        0     4854 2023-05-01 20:55:55.096542 kivy_widgets-0.1.7/kivy_widgets/dropdown.py
+-rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.7/kivy_widgets/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.7/kivy_widgets/icon_definitions.py
+-rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.7/kivy_widgets/icons.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.7/kivy_widgets/inspector.py
+-rw-r--r--   0        0        0       62 2023-04-27 06:16:14.173339 kivy_widgets-0.1.7/kivy_widgets/test.py
+-rw-r--r--   0        0        0      994 2023-05-01 21:12:00.279571 kivy_widgets-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.7/PKG-INFO
```

### Comparing `kivy_widgets-0.1.6/LICENSE` & `kivy_widgets-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/README.md` & `kivy_widgets-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/kivy_widgets/buttons.py` & `kivy_widgets-0.1.7/kivy_widgets/buttons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from kivy.lang import Builder
 from kivy.metrics import dp, sp
 from kivy.properties import (
+    AliasProperty,
     ColorProperty,
     ListProperty,
     NumericProperty,
     StringProperty,
-    OptionProperty,
-    AliasProperty,
 )
 from kivy.uix.behaviors import ButtonBehavior
 from kivy.uix.boxlayout import BoxLayout
+from kivy.uix.label import Label
+from kivy.uix.widget import Widget
 
 
 class CButton(ButtonBehavior, BoxLayout):
     """
     Custom button with icon and text
     """
 
-    text = StringProperty("Button")
+    text = StringProperty()
     font_size = NumericProperty(sp(18))
     icon = StringProperty()
     bg_color = ColorProperty([1, 1, 1, 1])
     color = ColorProperty([0, 0, 0, 1])
     icon_color = ColorProperty([0, 0, 0, 1])
     radius = ListProperty([dp(5)])
     icon_size = NumericProperty(dp(24))
@@ -37,39 +38,69 @@
                 self.bg_color[1] * 0.8,
                 self.bg_color[2] * 0.8,
                 self.bg_color[3] * 1,
             ]
 
     current_color = AliasProperty(
         get_current_color,
-        bind=["state"],
+        bind=["state", "bg_color"],
     )
 
+    def get_current_mode(self):
+        if self.text and self.icon:
+            return "both"
+        elif self.text:
+            return "text"
+        elif self.icon:
+            return "icon"
+
+    current_mode = AliasProperty(
+        get_current_mode,
+        bind=["text", "icon"],
+    )
+
+    def on_current_mode(self, *args):
+        if len(self.children) > 2:
+            children_to_remove = [
+                child for child in self.children if not isinstance(child, Label)
+            ]
+            for child in children_to_remove:
+                self.remove_widget(child)
+
+        if self.current_mode in ["icon", "text"]:
+            self.add_widget(Widget(), index=2)
+            self.add_widget(Widget(), index=0)
+        else:
+            self.add_widget(Widget(), index=0)
+            self.add_widget(Widget(), index=2)
+            self.add_widget(Widget(), index=4)
+
+    def on_kv_post(self, *args):
+        if not self.text and not self.icon:
+            self.text = "Button"
+
 
 # fmt: off
 Builder.load_string("""
 <-CButton>:
     size_hint: None, None
     _width: None
-    width: (label.texture_size[0] + icon.size[0] + dp(30) if icon.size[0] < dp(50) and icon.icon and label.text else label.texture_size[0] + icon.size[0]+ dp(20)) if not self._width else self._width
+    width: (label.texture_size[0] + icon.size[0] + dp(35) if icon.size[0] < dp(50) and icon.icon and label.text else label.texture_size[0] + icon.size[0]+ dp(20)) if not self._width else self._width
 
     _height: None
     height: (dp(50) if icon.size[1] < dp(50) else icon.size[1]) if not self._height else self._height
 
-    padding: dp(10)
-    spacing: dp(10) if icon.icon and label.text else 0
-
     canvas.before:
         Color:
             rgba: root.current_color
         RoundedRectangle:
             size: self.size
             pos: self.pos
             radius: root.radius
-        
+
     Label:
         id: icon
         text: u"{}".format(unicode[root.icon]) if root.icon in unicode else "blank"
         icon: root.icon
         font_name: icon_font
         size_hint: (None, None)
         size: self.texture_size if self.icon else (dp(0), dp(0))
```

### Comparing `kivy_widgets-0.1.6/kivy_widgets/color_definitions.py` & `kivy_widgets-0.1.7/kivy_widgets/color_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/kivy_widgets/fonts/materialdesignicons-webfont.ttf` & `kivy_widgets-0.1.7/kivy_widgets/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/kivy_widgets/icon_definitions.py` & `kivy_widgets-0.1.7/kivy_widgets/icon_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/kivy_widgets/icons.py` & `kivy_widgets-0.1.7/kivy_widgets/icons.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.6/pyproject.toml` & `kivy_widgets-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kivy-widgets"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["filipemarch <filipe.marchesini@gmail.com>", "ShootingStarDragon <rppapamaths@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kivy_widgets"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kivy_widgets-0.1.6/PKG-INFO` & `kivy_widgets-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-widgets
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: filipemarch
 Author-email: filipe.marchesini@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

