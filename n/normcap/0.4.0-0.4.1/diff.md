# Comparing `tmp/normcap-0.4.0.tar.gz` & `tmp/normcap-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normcap-0.4.0.tar", max compression
+gzip compressed data, was "normcap-0.4.1.tar", max compression
```

## Comparing `normcap-0.4.0.tar` & `normcap-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0    12852 2023-01-29 20:47:57.900429 normcap-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      724 2023-01-29 20:47:57.900429 normcap-0.4.0/LICENSE
--rw-r--r--   0        0        0     6709 2023-01-29 20:47:57.900429 normcap-0.4.0/README.md
--rw-r--r--   0        0        0       46 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/__init__.py
--rw-r--r--   0        0        0      113 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/__main__.py
--rw-r--r--   0        0        0     1659 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/app.py
--rw-r--r--   0        0        0      450 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     1183 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/clipboard/linux.py
--rw-r--r--   0        0        0      560 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/clipboard/macos.py
--rw-r--r--   0        0        0      284 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/clipboard/qt.py
--rw-r--r--   0        0        0     5922 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/clipboard/windows.py
--rw-r--r--   0        0        0        0 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/__init__.py
--rw-r--r--   0        0        0     8906 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/constants.py
--rw-r--r--   0        0        0     1848 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/downloader.py
--rw-r--r--   0        0        0     8209 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     2753 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0     9465 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     3439 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/models.py
--rw-r--r--   0        0        0     3935 2023-01-29 20:47:58.264432 normcap-0.4.0/normcap/gui/notifier.py
--rw-r--r--   0        0        0   217598 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/resources.py
--rw-r--r--   0        0        0     3525 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/settings.py
--rw-r--r--   0        0        0     6175 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/system_info.py
--rw-r--r--   0        0        0    17902 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/tray.py
--rw-r--r--   0        0        0     5333 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/update_check.py
--rw-r--r--   0        0        0    11925 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/gui/window.py
--rw-r--r--   0        0        0       97 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     2999 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/enhance.py
--rw-r--r--   0        0        0       46 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/__init__.py
--rw-r--r--   0        0        0      940 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/base_magic.py
--rw-r--r--   0        0        0     1856 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/email_magic.py
--rw-r--r--   0        0        0     2602 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/magic.py
--rw-r--r--   0        0        0     1141 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/multi_line_magic.py
--rw-r--r--   0        0        0     1644 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/paragraph_magic.py
--rw-r--r--   0        0        0     1062 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/single_line_magic.py
--rw-r--r--   0        0        0     2738 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/magics/url_magic.py
--rw-r--r--   0        0        0     4912 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/models.py
--rw-r--r--   0        0        0     1805 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     2106 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/ocr/utils.py
--rw-r--r--   0        0        0        0 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0    24936 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/normcap.svg
--rw-r--r--   0        0        0     9267 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0    16576 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/notification.svg
--rw-r--r--   0        0        0     9267 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0    16576 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/parse.svg
--rw-r--r--   0        0        0     2982 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0    14953 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/raw.svg
--rw-r--r--   0        0        0      528 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    13793 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/settings.svg
--rw-r--r--   0        0        0    17311 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16523 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/icons/tray.svg
--rw-r--r--   0        0        0       79 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0     1649 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     7145 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/dbus_portal.py
--rw-r--r--   0        0        0     4245 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/dbus_portal_legacy.py
--rw-r--r--   0        0        0     1816 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/dbus_shell.py
--rw-r--r--   0        0        0      461 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/qt.py
--rw-r--r--   0        0        0     5472 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/screengrab/utils.py
--rw-r--r--   0        0        0     7363 2023-01-29 20:47:58.268432 normcap-0.4.0/normcap/utils.py
--rw-r--r--   0        0        0     5694 2023-01-29 20:47:58.268432 normcap-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7971 1970-01-01 00:00:00.000000 normcap-0.4.0/setup.py
--rw-r--r--   0        0        0     8282 1970-01-01 00:00:00.000000 normcap-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13604 2023-05-01 12:30:54.612167 normcap-0.4.1/CHANGELOG
+-rw-r--r--   0        0        0      724 2023-05-01 12:30:54.612167 normcap-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7062 2023-05-01 12:30:54.612167 normcap-0.4.1/README.md
+-rw-r--r--   0        0        0       46 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/__main__.py
+-rw-r--r--   0        0        0     1659 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/app.py
+-rw-r--r--   0        0        0      450 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/linux.py
+-rw-r--r--   0        0        0      588 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/macos.py
+-rw-r--r--   0        0        0      284 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/qt.py
+-rw-r--r--   0        0        0     5885 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/windows.py
+-rw-r--r--   0        0        0        0 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     8955 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/constants.py
+-rw-r--r--   0        0        0     2356 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     8359 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     2753 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0    10006 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     3481 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/models.py
+-rw-r--r--   0        0        0     3949 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/notifier.py
+-rw-r--r--   0        0        0   217598 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/resources.py
+-rw-r--r--   0        0        0     3552 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6205 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    20812 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/tray.py
+-rw-r--r--   0        0        0     4568 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      758 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/utils.py
+-rw-r--r--   0        0        0    11944 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/window.py
+-rw-r--r--   0        0        0       93 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3603 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0       46 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/base_magic.py
+-rw-r--r--   0        0        0     1807 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/email_magic.py
+-rw-r--r--   0        0        0     2463 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/magic.py
+-rw-r--r--   0        0        0     1048 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/multi_line_magic.py
+-rw-r--r--   0        0        0     1546 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/paragraph_magic.py
+-rw-r--r--   0        0        0      964 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/single_line_magic.py
+-rw-r--r--   0        0        0     2699 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/url_magic.py
+-rw-r--r--   0        0        0     5121 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/models.py
+-rw-r--r--   0        0        0     1535 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     3305 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0    24936 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/normcap.svg
+-rw-r--r--   0        0        0     9267 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0    16576 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/notification.svg
+-rw-r--r--   0        0        0     9267 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0    16576 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/parse.svg
+-rw-r--r--   0        0        0     2982 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0    14953 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/raw.svg
+-rw-r--r--   0        0        0      528 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    13793 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/settings.svg
+-rw-r--r--   0        0        0    17311 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16523 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/tray.svg
+-rw-r--r--   0        0        0       79 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0     1623 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     7202 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_portal.py
+-rw-r--r--   0        0        0     4239 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_portal_legacy.py
+-rw-r--r--   0        0        0     1816 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_shell.py
+-rw-r--r--   0        0        0      461 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/qt.py
+-rw-r--r--   0        0        0     5512 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/utils.py
+-rw-r--r--   0        0        0     7463 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/utils.py
+-rw-r--r--   0        0        0     7764 2023-05-01 12:30:54.980166 normcap-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8263 1970-01-01 00:00:00.000000 normcap-0.4.1/setup.py
+-rw-r--r--   0        0        0     8543 1970-01-01 00:00:00.000000 normcap-0.4.1/PKG-INFO
```

### Comparing `normcap-0.4.0/CHANGELOG.md` & `normcap-0.4.1/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 # Changelog
 
-## v0.4.0 (2022-01-29)
+## v0.4.1 (2023-05-01)
 
-- All: Remove support for Tesseract \< 5.0
+**All:**
+
+- Enlarge settings button a bit to make it easier to spot.
+  ([#254](https://github.com/dynobo/normcap/issues/254))
+- Prevent running multiple instances and start capture in original instance instead.
+  ([#306](https://github.com/dynobo/normcap/issues/306))
+- Fix unintended re-capture if tray icon is disabled.
+  ([#254](https://github.com/dynobo/normcap/issues/254))
+- Fix occasional crashes after use of Language Manager.
+- Add experimental `--cli-mode` switch to print NormCap's detection to STDOUT and exit
+  immediately. This is useful if you want to use the detected text as input for other
+  programs or commands. E.g.:
+  ```sh
+  normcap --cli-mode | xargs -I {} firefox "http://duckduckgo.com/?q={}"`
+  ```
+
+## v0.4.0 (2023-01-29)
+
+- All: Remove support for Tesseract \< 5.0.
 - All: Faster startup if "Check for updates" is enabled.
 - All: Refactor icon handling. Fixes a bug in the AUR package.
   ([#353](https://github.com/dynobo/normcap/issues/353))
 - All: Fix crash if tesseract data for English is missing.
   ([#353](https://github.com/dynobo/normcap/issues/353))
 - Linux: Fix FlatPak crashes due to missing permissions
   ([#320](https://github.com/dynobo/normcap/issues/320)).
```

### Comparing `normcap-0.4.0/LICENSE` & `normcap-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/README.md` & `normcap-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -72,349 +72,371 @@
 00000470: 5b41 5552 5d28 6874 7470 733a 2f2f 696d  [AUR](https://im
 00000480: 672e 7368 6965 6c64 732e 696f 2f61 7572  g.shields.io/aur
 00000490: 2f76 6f74 6573 2f6e 6f72 6d63 6170 3f6c  /votes/normcap?l
 000004a0: 6162 656c 3d41 5552 2532 3076 6f74 6573  abel=AUR%20votes
 000004b0: 2663 6f6c 6f72 3d62 6c75 6529 5d28 6874  &color=blue)](ht
 000004c0: 7470 733a 2f2f 6175 722e 6172 6368 6c69  tps://aur.archli
 000004d0: 6e75 782e 6f72 672f 7061 636b 6167 6573  nux.org/packages
-000004e0: 2f6e 6f72 6d63 6170 290a 0a2a 2a4c 696e  /normcap)..**Lin
-000004f0: 6b73 3a2a 2a20 5b53 6f75 7263 6520 436f  ks:** [Source Co
-00000500: 6465 5d28 6874 7470 733a 2f2f 6769 7468  de](https://gith
-00000510: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
-00000520: 726d 6361 7029 207c 0a5b 446f 6375 6d65  rmcap) |.[Docume
-00000530: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000540: 2f64 796e 6f62 6f2e 6769 7468 7562 2e69  /dynobo.github.i
-00000550: 6f2f 6e6f 726d 6361 702f 2920 7c0a 5b46  o/normcap/) |.[F
-00000560: 4151 735d 2868 7474 7073 3a2f 2f64 796e  AQs](https://dyn
-00000570: 6f62 6f2e 6769 7468 7562 2e69 6f2f 6e6f  obo.github.io/no
-00000580: 726d 6361 702f 2366 6171 7329 207c 0a5b  rmcap/#faqs) |.[
-00000590: 5265 6c65 6173 6573 5d28 6874 7470 733a  Releases](https:
-000005a0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796e  //github.com/dyn
-000005b0: 6f62 6f2f 6e6f 726d 6361 702f 7265 6c65  obo/normcap/rele
-000005c0: 6173 6573 2920 7c0a 5b43 6861 6e67 656c  ases) |.[Changel
-000005d0: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-000005e0: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
-000005f0: 726d 6361 702f 626c 6f62 2f6d 6169 6e2f  rmcap/blob/main/
-00000600: 4348 414e 4745 4c4f 472e 6d64 290a 0a5b  CHANGELOG.md)..[
-00000610: 215b 5363 7265 656e 6361 7374 5d28 6874  ![Screencast](ht
-00000620: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
-00000630: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
-00000640: 656e 742e 636f 6d2f 3131 3037 3138 3736  ent.com/11071876
-00000650: 2f31 3839 3736 3735 3835 2d38 6263 3435  /189767585-8bc45
-00000660: 6331 382d 3833 3932 2d34 3131 642d 3834  c18-8392-411d-84
-00000670: 6463 2d63 6566 3163 6235 6462 6334 372e  dc-cef1cb5dbc47.
-00000680: 6769 6629 5d28 6874 7470 733a 2f2f 7261  gif)](https://ra
-00000690: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000006a0: 656e 742e 636f 6d2f 6479 6e6f 626f 2f6e  ent.com/dynobo/n
-000006b0: 6f72 6d63 6170 2f6d 6169 6e2f 6173 7365  ormcap/main/asse
-000006c0: 7473 2f6e 6f72 6d63 6170 2e67 6966 290a  ts/normcap.gif).
-000006d0: 0a23 2320 5175 6963 6b73 7461 7274 0a0a  .## Quickstart..
-000006e0: 496e 7374 616c 6c20 6120 7072 6562 7569  Install a prebui
-000006f0: 6c74 2072 656c 6561 7365 3a0a 0a2d 202a  lt release:..- *
-00000700: 2a57 696e 646f 7773 2a2a 3a0a 2020 5b4e  *Windows**:.  [N
-00000710: 6f72 6d43 6170 2d30 2e34 2e30 2d78 3836  ormCap-0.4.0-x86
-00000720: 5f36 342d 5769 6e64 6f77 732e 6d73 695d  _64-Windows.msi]
-00000730: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000740: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
-00000750: 6170 2f72 656c 6561 7365 732f 646f 776e  ap/releases/down
-00000760: 6c6f 6164 2f76 302e 342e 302f 4e6f 726d  load/v0.4.0/Norm
-00000770: 4361 702d 302e 342e 302d 7838 365f 3634  Cap-0.4.0-x86_64
-00000780: 2d57 696e 646f 7773 2e6d 7369 290a 2d20  -Windows.msi).- 
-00000790: 2a2a 4c69 6e75 782a 2a3a 0a20 205b 4e6f  **Linux**:.  [No
-000007a0: 726d 4361 702d 302e 342e 302d 7838 365f  rmCap-0.4.0-x86_
-000007b0: 3634 2e41 7070 496d 6167 655d 2868 7474  64.AppImage](htt
-000007c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000007d0: 6479 6e6f 626f 2f6e 6f72 6d63 6170 2f72  dynobo/normcap/r
-000007e0: 656c 6561 7365 732f 646f 776e 6c6f 6164  eleases/download
-000007f0: 2f76 302e 342e 302f 4e6f 726d 4361 702d  /v0.4.0/NormCap-
-00000800: 302e 342e 302d 7838 365f 3634 2e41 7070  0.4.0-x86_64.App
-00000810: 496d 6167 6529 0a2d 202a 2a6d 6163 4f53  Image).- **macOS
-00000820: 2a2a 2028 7838 3629 20c2 b93a 0a20 205b  ** (x86) ..:.  [
-00000830: 4e6f 726d 4361 702d 302e 342e 302d 7838  NormCap-0.4.0-x8
-00000840: 365f 3634 2d6d 6163 4f53 2e64 6d67 5d28  6_64-macOS.dmg](
-00000850: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000860: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
-00000870: 702f 7265 6c65 6173 6573 2f64 6f77 6e6c  p/releases/downl
-00000880: 6f61 642f 7630 2e34 2e30 2f4e 6f72 6d43  oad/v0.4.0/NormC
-00000890: 6170 2d30 2e34 2e30 2d78 3836 5f36 342d  ap-0.4.0-x86_64-
-000008a0: 6d61 634f 532e 646d 6729 0a2d 202a 2a6d  macOS.dmg).- **m
-000008b0: 6163 4f53 2a2a 2028 4d31 2920 c2b9 c2b7  acOS** (M1) ....
-000008c0: c2b2 3a0a 2020 5b4e 6f72 6d43 6170 2d30  ..:.  [NormCap-0
-000008d0: 2e34 2e30 2d61 726d 3634 2d6d 6163 4f53  .4.0-arm64-macOS
-000008e0: 2e64 6d67 5d28 6874 7470 733a 2f2f 6769  .dmg](https://gi
-000008f0: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
-00000900: 6e6f 726d 6361 702f 7265 6c65 6173 6573  normcap/releases
-00000910: 2f64 6f77 6e6c 6f61 642f 7630 2e34 2e30  /download/v0.4.0
-00000920: 2f4e 6f72 6d43 6170 2d30 2e34 2e30 2d61  /NormCap-0.4.0-a
-00000930: 726d 3634 2d6d 6163 4f53 2e64 6d67 290a  rm64-macOS.dmg).
-00000940: 2020 5c0a 2020 3c73 7562 3e31 3a20 4f6e    \.  <sub>1: On
-00000950: 206d 6163 4f53 2c20 616c 6c6f 7720 7468   macOS, allow th
-00000960: 6520 756e 7369 676e 6564 2061 7070 6c69  e unsigned appli
-00000970: 6361 7469 6f6e 206f 6e20 6669 7273 7420  cation on first 
-00000980: 7374 6172 743a 2022 5379 7374 656d 0a20  start: "System. 
-00000990: 2050 7265 6665 7265 6e63 6573 2220 e286   Preferences" ..
-000009a0: 9220 2253 6563 7572 6974 7920 2620 5072  . "Security & Pr
-000009b0: 6976 6163 7922 20e2 8692 2022 4765 6e65  ivacy" ... "Gene
-000009c0: 7261 6c22 20e2 8692 2022 4f70 656e 2061  ral" ... "Open a
-000009d0: 6e79 7761 7922 2e20 596f 7520 6d69 6768  nyway". You migh
-000009e0: 7420 616c 736f 206e 6565 640a 2020 746f  t also need.  to
-000009f0: 2061 6c6c 6f77 204e 6f72 6d43 6170 2074   allow NormCap t
-00000a00: 6f20 7461 6b65 2073 6372 6565 6e73 686f  o take screensho
-00000a10: 7473 2e0a 2020 5b23 3133 355d 2868 7474  ts..  [#135](htt
-00000a20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000a30: 6479 6e6f 626f 2f6e 6f72 6d63 6170 2f69  dynobo/normcap/i
-00000a40: 7373 7565 732f 3133 3529 3c62 723e 2032  ssues/135)<br> 2
-00000a50: 3a20 4d69 6768 7420 6265 2061 7661 696c  : Might be avail
-00000a60: 6162 6c65 2061 2062 6974 0a20 2064 656c  able a bit.  del
-00000a70: 6179 6564 2c20 6173 2069 7420 6973 2063  ayed, as it is c
-00000a80: 7572 7265 6e74 6c79 2062 7569 6c64 206d  urrently build m
-00000a90: 616e 7561 6c6c 792e 2028 5468 782c 0a20  anually. (Thx,. 
-00000aa0: 205b 4054 616b 7269 6e5d 2868 7474 7073   [@Takrin](https
-00000ab0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5461  ://github.com/Ta
-00000ac0: 6b72 696e 2921 293c 2f73 7562 3e0a 0a49  krin)!)</sub>..I
-00000ad0: 6e73 7461 6c6c 2066 726f 6d20 7265 706f  nstall from repo
-00000ae0: 7369 746f 7269 6573 3a0a 0a2d 202a 2a41  sitories:..- **A
-00000af0: 7263 6820 2f20 4d61 6e6a 6172 6f2a 2a3a  rch / Manjaro**:
-00000b00: 2049 6e73 7461 6c6c 2074 6865 0a20 205b   Install the.  [
-00000b10: 606e 6f72 6d63 6170 605d 2868 7474 7073  `normcap`](https
-00000b20: 3a2f 2f61 7572 2e61 7263 686c 696e 7578  ://aur.archlinux
-00000b30: 2e6f 7267 2f70 6163 6b61 6765 732f 6e6f  .org/packages/no
-00000b40: 726d 6361 7029 2070 6163 6b61 6765 2066  rmcap) package f
-00000b50: 726f 6d20 4155 522e 0a2d 202a 2a46 6c61  rom AUR..- **Fla
-00000b60: 7450 616b 2028 4c69 6e75 7829 2a2a 3a20  tPak (Linux)**: 
-00000b70: 496e 7374 616c 6c0a 2020 5b63 6f6d 2e67  Install.  [com.g
-00000b80: 6974 6875 622e 6479 6e6f 626f 2e6e 6f72  ithub.dynobo.nor
-00000b90: 6d63 6170 5d28 6874 7470 733a 2f2f 666c  mcap](https://fl
-00000ba0: 6174 6875 622e 6f72 672f 6170 7073 2f64  athub.org/apps/d
-00000bb0: 6574 6169 6c73 2f63 6f6d 2e67 6974 6875  etails/com.githu
-00000bc0: 622e 6479 6e6f 626f 2e6e 6f72 6d63 6170  b.dynobo.normcap
-00000bd0: 290a 2020 6672 6f6d 2046 6c61 7448 7562  ).  from FlatHub
-00000be0: 2e0a 0a49 6620 796f 7520 6578 7065 7269  ...If you experi
-00000bf0: 656e 6365 2069 7373 7565 7320 706c 6561  ence issues plea
-00000c00: 7365 206c 6f6f 6b20 6174 2074 6865 0a5b  se look at the.[
-00000c10: 4641 5173 5d28 6874 7470 733a 2f2f 6479  FAQs](https://dy
-00000c20: 6e6f 626f 2e67 6974 6875 622e 696f 2f6e  nobo.github.io/n
-00000c30: 6f72 6d63 6170 2f23 6661 7173 2920 6f72  ormcap/#faqs) or
-00000c40: 0a5b 6f70 656e 2061 6e20 6973 7375 655d  .[open an issue]
-00000c50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000c60: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
-00000c70: 6170 2f69 7373 7565 7329 2e0a 0a23 2320  ap/issues)...## 
-00000c80: 5079 7468 6f6e 2070 6163 6b61 6765 0a0a  Python package..
-00000c90: 4173 2061 6e20 5f61 6c74 6572 6e61 7469  As an _alternati
-00000ca0: 7665 5f20 746f 2061 2070 7265 6275 696c  ve_ to a prebuil
-00000cb0: 7420 7061 636b 6167 6520 796f 7520 6361  t package you ca
-00000cc0: 6e20 696e 7374 616c 6c20 7468 650a 5b4e  n install the.[N
-00000cd0: 6f72 6d43 6170 2050 7974 686f 6e20 7061  ormCap Python pa
-00000ce0: 636b 6167 655d 2868 7474 7073 3a2f 2f70  ckage](https://p
-00000cf0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000d00: 6e6f 726d 6361 702f 2920 666f 7220 2a2a  normcap/) for **
-00000d10: 5079 7468 6f6e 203e 3d33 2e39 2a2a 3a0a  Python >=3.9**:.
-00000d20: 0a23 2323 2320 4f6e 204c 696e 7578 0a0a  .#### On Linux..
-00000d30: 6060 6073 680a 2320 496e 7374 616c 6c20  ```sh.# Install 
-00000d40: 6465 7065 6e64 656e 6369 6573 2028 5562  dependencies (Ub
-00000d50: 756e 7475 2f44 6562 6961 6e29 0a73 7564  untu/Debian).sud
-00000d60: 6f20 6170 7420 696e 7374 616c 6c20 6275  o apt install bu
-00000d70: 696c 642d 6573 7365 6e74 6961 6c20 7465  ild-essential te
-00000d80: 7373 6572 6163 742d 6f63 7220 7465 7373  sseract-ocr tess
-00000d90: 6572 6163 742d 6f63 722d 656e 6720 6c69  eract-ocr-eng li
-00000da0: 6274 6573 7365 7261 6374 2d64 6576 206c  btesseract-dev l
-00000db0: 6962 6c65 7074 6f6e 6963 612d 6465 7620  ibleptonica-dev 
-00000dc0: 776c 2d63 6c69 7062 6f61 7264 0a0a 2323  wl-clipboard..##
-00000dd0: 2049 6e73 7461 6c6c 2064 6570 656e 6465   Install depende
-00000de0: 6e63 6965 7320 2841 7263 6829 0a73 7564  ncies (Arch).sud
-00000df0: 6f20 7061 636d 616e 202d 5320 7465 7373  o pacman -S tess
-00000e00: 6572 6163 7420 7465 7373 6572 6163 742d  eract tesseract-
-00000e10: 6461 7461 2d65 6e67 2077 6c2d 636c 6970  data-eng wl-clip
-00000e20: 626f 6172 640a 0a23 2320 496e 7374 616c  board..## Instal
-00000e30: 6c20 6465 7065 6e64 656e 6369 6573 2028  l dependencies (
-00000e40: 4665 646f 7261 290a 7375 646f 2064 6e66  Fedora).sudo dnf
-00000e50: 2069 6e73 7461 6c6c 2074 6573 7365 7261   install tessera
-00000e60: 6374 2077 6c2d 636c 6970 626f 6172 640a  ct wl-clipboard.
-00000e70: 0a23 2320 496e 7374 616c 6c20 6465 7065  .## Install depe
-00000e80: 6e64 656e 6369 6573 2028 6f70 656e 5355  ndencies (openSU
-00000e90: 5345 290a 7375 646f 207a 7970 7065 7220  SE).sudo zypper 
-00000ea0: 696e 7374 616c 6c20 7079 7468 6f6e 332d  install python3-
-00000eb0: 6465 7665 6c20 7465 7373 6572 6163 742d  devel tesseract-
-00000ec0: 6f63 7220 7465 7373 6572 6163 742d 6f63  ocr tesseract-oc
-00000ed0: 722d 6465 7665 6c20 776c 2d63 6c69 7062  r-devel wl-clipb
-00000ee0: 6f61 7264 0a0a 2320 496e 7374 616c 6c20  oard..# Install 
-00000ef0: 6e6f 726d 6361 700a 7069 7020 696e 7374  normcap.pip inst
-00000f00: 616c 6c20 6e6f 726d 6361 700a 0a23 2052  all normcap..# R
-00000f10: 756e 0a2e 2f6e 6f72 6d63 6170 0a60 6060  un../normcap.```
-00000f20: 0a0a 2323 2323 204f 6e20 6d61 634f 530a  ..#### On macOS.
-00000f30: 0a60 6060 7368 0a23 2049 6e73 7461 6c6c  .```sh.# Install
-00000f40: 2064 6570 656e 6465 6e63 6965 730a 6272   dependencies.br
-00000f50: 6577 2069 6e73 7461 6c6c 2074 6573 7365  ew install tesse
-00000f60: 7261 6374 2074 6573 7365 7261 6374 2d6c  ract tesseract-l
-00000f70: 616e 670a 0a23 2049 6e73 7461 6c6c 206e  ang..# Install n
-00000f80: 6f72 6d63 6170 0a70 6970 2069 6e73 7461  ormcap.pip insta
-00000f90: 6c6c 206e 6f72 6d63 6170 0a0a 2320 5275  ll normcap..# Ru
-00000fa0: 6e0a 2e2f 6e6f 726d 6361 700a 6060 600a  n../normcap.```.
-00000fb0: 0a23 2323 2320 4f6e 2057 696e 646f 7773  .#### On Windows
-00000fc0: 0a0a 315c 2e20 496e 7374 616c 6c20 6054  ..1\. Install `T
-00000fd0: 6573 7365 7261 6374 2035 6020 6279 2075  esseract 5` by u
-00000fe0: 7369 6e67 2074 6865 0a5b 696e 7374 616c  sing the.[instal
-00000ff0: 6c65 7220 7072 6f76 6964 6564 2062 7920  ler provided by 
-00001000: 5542 204d 616e 6e68 6569 6d5d 2868 7474  UB Mannheim](htt
-00001010: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001020: 5542 2d4d 616e 6e68 6569 6d2f 7465 7373  UB-Mannheim/tess
-00001030: 6572 6163 742f 7769 6b69 292e 0a0a 325c  eract/wiki)...2\
-00001040: 2e20 4164 6a75 7374 2065 6e76 6972 6f6e  . Adjust environ
-00001050: 6d65 6e74 2076 6172 6961 626c 6573 3a0a  ment variables:.
-00001060: 0a2d 2043 7265 6174 6520 616e 2065 6e76  .- Create an env
-00001070: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00001080: 6520 6054 4553 5344 4154 415f 5052 4546  e `TESSDATA_PREF
-00001090: 4958 6020 616e 6420 7365 7420 6974 2074  IX` and set it t
-000010a0: 6f20 5465 7373 6572 6163 7427 7320 6461  o Tesseract's da
-000010b0: 7461 0a20 2066 6f6c 6465 722c 2065 2e67  ta.  folder, e.g
-000010c0: 2e3a 0a0a 2020 6060 6063 6d64 0a20 2073  .:..  ```cmd.  s
-000010d0: 6574 7820 5445 5353 4441 5441 5f50 5245  etx TESSDATA_PRE
-000010e0: 4649 5820 2243 3a5c 5072 6f67 7261 6d20  FIX "C:\Program 
-000010f0: 4669 6c65 735c 5465 7373 6572 6163 742d  Files\Tesseract-
-00001100: 4f43 525c 7465 7373 6461 7461 220a 2020  OCR\tessdata".  
-00001110: 6060 600a 0a2d 2041 7070 656e 6420 5465  ```..- Append Te
-00001120: 7373 6572 6163 7427 7320 6c6f 6361 7469  sseract's locati
-00001130: 6f6e 2074 6f20 7468 6520 656e 7669 726f  on to the enviro
-00001140: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
-00001150: 5061 7468 602c 2065 2e67 2e3a 0a0a 2020  Path`, e.g.:..  
-00001160: 6060 6063 6d64 0a20 2073 6574 7820 5061  ```cmd.  setx Pa
-00001170: 7468 2022 2550 6174 6825 3b43 3a5c 5072  th "%Path%;C:\Pr
-00001180: 6f67 7261 6d20 4669 6c65 735c 5465 7373  ogram Files\Tess
-00001190: 6572 6163 742d 4f43 5222 0a20 2060 6060  eract-OCR".  ```
-000011a0: 0a0a 2d20 4d61 6b65 2073 7572 6520 746f  ..- Make sure to
-000011b0: 2063 6c6f 7365 2061 6e64 2072 656f 7065   close and reope
-000011c0: 6e20 796f 7572 2063 7572 7265 6e74 2074  n your current t
-000011d0: 6572 6d69 6e61 6c20 7769 6e64 6f77 2074  erminal window t
-000011e0: 6f20 6170 706c 7920 7468 6520 6e65 7720  o apply the new 
-000011f0: 7661 7269 6162 6c65 732e 0a20 2054 6573  variables..  Tes
-00001200: 7420 6974 2062 7920 7275 6e6e 696e 673a  t it by running:
-00001210: 0a0a 2020 6060 6063 6d64 0a20 2074 6573  ..  ```cmd.  tes
-00001220: 7365 7261 6374 202d 2d6c 6973 742d 6c61  seract --list-la
-00001230: 6e67 730a 2020 6060 600a 0a33 5c2e 2049  ngs.  ```..3\. I
-00001240: 6e73 7461 6c6c 2061 6e64 2072 756e 204e  nstall and run N
-00001250: 6f72 6d43 6170 3a0a 0a60 6060 6261 7368  ormCap:..```bash
-00001260: 0a23 2049 6e73 7461 6c6c 206e 6f72 6d63  .# Install normc
-00001270: 6170 0a70 6970 2069 6e73 7461 6c6c 206e  ap.pip install n
-00001280: 6f72 6d63 6170 0a0a 2320 5275 6e0a 6e6f  ormcap..# Run.no
-00001290: 726d 6361 700a 6060 600a 0a23 2320 5768  rmcap.```..## Wh
-000012a0: 7920 224e 6f72 6d43 6170 223f 0a0a 5365  y "NormCap"?..Se
-000012b0: 6520 5b58 4b43 445d 2868 7474 7073 3a2f  e [XKCD](https:/
-000012c0: 2f78 6b63 642e 636f 6d29 3a0a 0a5b 215b  /xkcd.com):..[![
-000012d0: 436f 6d69 635d 2868 7474 7073 3a2f 2f69  Comic](https://i
-000012e0: 6d67 732e 786b 6364 2e63 6f6d 2f63 6f6d  mgs.xkcd.com/com
-000012f0: 6963 732f 6e6f 726d 5f6e 6f72 6d61 6c5f  ics/norm_normal_
-00001300: 6669 6c65 5f66 6f72 6d61 742e 706e 6729  file_format.png)
-00001310: 5d28 6874 7470 733a 2f2f 786b 6364 2e63  ](https://xkcd.c
-00001320: 6f6d 2f32 3131 362f 290a 0a23 2320 4465  om/2116/)..## De
-00001330: 7665 6c6f 706d 656e 740a 0a50 7265 7265  velopment..Prere
-00001340: 7175 6973 6974 6573 2066 6f72 2073 6574  quisites for set
-00001350: 7469 6e67 2075 7020 6120 6465 7665 6c6f  ting up a develo
-00001360: 706d 656e 7420 656e 7669 726f 6e6d 656e  pment environmen
-00001370: 7420 6172 653a 202a 2a50 7974 686f 6e20  t are: **Python 
-00001380: 3e3d 332e 392a 2a2c 0a2a 2a50 6f65 7472  >=3.9**,.**Poetr
-00001390: 793e 3d31 2e33 2e32 2a2a 2061 6e64 202a  y>=1.3.2** and *
-000013a0: 2a54 6573 7365 7261 6374 2a2a 2028 696e  *Tesseract** (in
-000013b0: 636c 2e20 2a2a 6c61 6e67 7561 6765 2064  cl. **language d
-000013c0: 6174 612a 2a29 2e0a 0a60 6060 7368 0a23  ata**)...```sh.#
-000013d0: 2043 6c6f 6e65 2072 6570 6f73 6974 6f72   Clone repositor
-000013e0: 790a 6769 7420 636c 6f6e 6520 6874 7470  y.git clone http
-000013f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00001400: 796e 6f62 6f2f 6e6f 726d 6361 702e 6769  ynobo/normcap.gi
-00001410: 740a 0a23 2043 6861 6e67 6520 696e 746f  t..# Change into
-00001420: 2070 726f 6a65 6374 2064 6972 6563 746f   project directo
-00001430: 7279 0a63 6420 6e6f 726d 6361 700a 0a23  ry.cd normcap..#
-00001440: 2043 7265 6174 6520 7669 7274 7561 6c20   Create virtual 
-00001450: 656e 7620 616e 6420 696e 7374 616c 6c20  env and install 
-00001460: 6465 7065 6e64 656e 6369 6573 0a70 6f65  dependencies.poe
-00001470: 7472 7920 696e 7374 616c 6c0a 0a23 2052  try install..# R
-00001480: 6567 6973 7465 7220 7072 652d 636f 6d6d  egister pre-comm
-00001490: 6974 2068 6f6f 6b0a 706f 6574 7279 2072  it hook.poetry r
-000014a0: 756e 2070 7265 2d63 6f6d 6d69 7420 696e  un pre-commit in
-000014b0: 7374 616c 6c0a 0a23 2052 756e 204e 6f72  stall..# Run Nor
-000014c0: 6d43 6170 2069 6e20 7669 7274 7561 6c20  mCap in virtual 
-000014d0: 656e 760a 706f 6574 7279 2072 756e 2070  env.poetry run p
-000014e0: 7974 686f 6e20 2d6d 206e 6f72 6d63 6170  ython -m normcap
-000014f0: 0a60 6060 0a0a 2323 2043 7265 6469 7473  .```..## Credits
-00001500: 0a0a 5468 6973 2070 726f 6a65 6374 2075  ..This project u
-00001510: 7365 7320 7468 6520 666f 6c6c 6f77 696e  ses the followin
-00001520: 6720 6e6f 6e2d 7374 616e 6461 7264 206c  g non-standard l
-00001530: 6962 7261 7269 6573 3a0a 0a2d 205b 7079  ibraries:..- [py
-00001540: 7369 6465 365d 2868 7474 7073 3a2f 2f70  side6](https://p
-00001550: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00001560: 5079 5369 6465 362f 2920 5f2d 2062 696e  PySide6/) _- bin
-00001570: 6469 6e67 7320 666f 7220 5174 2055 4920  dings for Qt UI 
-00001580: 4672 616d 6577 6f72 6b5f 0a2d 205b 7079  Framework_.- [py
-00001590: 7465 7373 6572 6163 745d 2868 7474 7073  tesseract](https
-000015a0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-000015b0: 6563 742f 7079 7465 7373 6572 6163 742f  ect/pytesseract/
-000015c0: 2920 5f2d 2077 7261 7070 6572 2066 6f72  ) _- wrapper for
-000015d0: 2074 6573 7365 7261 6374 2773 2041 5049   tesseract's API
-000015e0: 5f0a 2d20 5b6a 6565 706e 6579 5d28 6874  _.- [jeepney](ht
-000015f0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00001600: 726f 6a65 6374 2f6a 6565 706e 6579 2f29  roject/jeepney/)
-00001610: 205f 2d20 4442 5553 2063 6c69 656e 745f   _- DBUS client_
-00001620: 0a0a 416e 6420 6974 2064 6570 656e 6473  ..And it depends
-00001630: 206f 6e20 6578 7465 726e 616c 2073 6f66   on external sof
-00001640: 7477 6172 653a 0a0a 2d20 5b74 6573 7365  tware:..- [tesse
-00001650: 7261 6374 5d28 6874 7470 733a 2f2f 6769  ract](https://gi
-00001660: 7468 7562 2e63 6f6d 2f74 6573 7365 7261  thub.com/tessera
-00001670: 6374 2d6f 6372 2f74 6573 7365 7261 6374  ct-ocr/tesseract
-00001680: 2920 2d20 5f4f 4352 2065 6e67 696e 655f  ) - _OCR engine_
-00001690: 0a2d 205b 776c 2d63 6c69 7062 6f61 7264  .- [wl-clipboard
-000016a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000016b0: 2e63 6f6d 2f62 7567 6165 7663 2f77 6c2d  .com/bugaevc/wl-
-000016c0: 636c 6970 626f 6172 6429 202d 205f 5761  clipboard) - _Wa
-000016d0: 796c 616e 6420 636c 6970 626f 6172 640a  yland clipboard.
-000016e0: 2020 7574 696c 6974 6965 735f 0a0a 5061    utilities_..Pa
-000016f0: 636b 6167 696e 6720 6973 2064 6f6e 6520  ckaging is done 
-00001700: 7769 7468 3a0a 0a2d 205b 6272 6965 6663  with:..- [briefc
-00001710: 6173 655d 2868 7474 7073 3a2f 2f70 7970  ase](https://pyp
-00001720: 692e 6f72 672f 7072 6f6a 6563 742f 6272  i.org/project/br
-00001730: 6965 6663 6173 652f 2920 5f2d 2063 6f6e  iefcase/) _- con
-00001740: 7665 7274 696e 6720 5079 7468 6f6e 2070  verting Python p
-00001750: 726f 6a65 6374 7320 696e 746f 5f0a 2020  rojects into_.  
-00001760: 5f73 7461 6e64 616c 6f6e 6520 6170 7073  _standalone apps
-00001770: 5f0a 0a54 6861 6e6b 7320 746f 2074 6865  _..Thanks to the
-00001780: 206d 6169 6e74 6169 6e65 7273 206f 6620   maintainers of 
-00001790: 7468 6f73 6520 6e69 6365 2074 6f6f 6c73  those nice tools
-000017a0: 210a 0a23 2320 5369 6d69 6c61 7220 6f70  !..## Similar op
-000017b0: 656e 2073 6f75 7263 6520 746f 6f6c 730a  en source tools.
-000017c0: 0a49 6620 4e6f 726d 4361 7020 646f 6573  .If NormCap does
-000017d0: 6e27 7420 6669 7420 796f 7572 206e 6565  n't fit your nee
-000017e0: 6473 2c20 7472 7920 7468 6f73 6520 616c  ds, try those al
-000017f0: 7465 726e 6174 6976 6573 2028 6e6f 2070  ternatives (no p
-00001800: 6172 7469 6375 6c61 7220 6f72 6465 7229  articular order)
-00001810: 3a0a 0a2d 205b 5465 7874 536e 6174 6368  :..- [TextSnatch
-00001820: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00001830: 7562 2e63 6f6d 2f52 616a 536f 6c61 692f  ub.com/RajSolai/
-00001840: 5465 7874 536e 6174 6368 6572 2920 284c  TextSnatcher) (L
-00001850: 696e 7578 290a 2d20 5b47 7265 656e 5368  inux).- [GreenSh
-00001860: 6f74 5d28 6874 7470 733a 2f2f 6765 7467  ot](https://getg
-00001870: 7265 656e 7368 6f74 2e6f 7267 2f29 2028  reenshot.org/) (
-00001880: 4c69 6e75 782c 206d 6163 4f53 290a 2d20  Linux, macOS).- 
-00001890: 5b54 6578 7453 686f 745d 2868 7474 7073  [TextShot](https
-000018a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6961  ://github.com/ia
-000018b0: 6e7a 6861 6f30 352f 7465 7874 7368 6f74  nzhao05/textshot
-000018c0: 2920 2857 696e 646f 7773 290a 2d20 5b67  ) (Windows).- [g
-000018d0: 496d 6167 6552 6561 6465 725d 2868 7474  ImageReader](htt
-000018e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000018f0: 6d61 6e69 7361 6e64 726f 2f67 496d 6167  manisandro/gImag
-00001900: 6552 6561 6465 7229 2028 4c69 6e75 782c  eReader) (Linux,
-00001910: 2057 696e 646f 7773 290a 2d20 5b43 6170   Windows).- [Cap
-00001920: 7475 7265 3254 6578 745d 2868 7474 7073  ture2Text](https
-00001930: 3a2f 2f73 6f75 7263 6566 6f72 6765 2e6e  ://sourceforge.n
-00001940: 6574 2f70 726f 6a65 6374 732f 6361 7074  et/projects/capt
-00001950: 7572 6532 7465 7874 2920 2857 696e 646f  ure2text) (Windo
-00001960: 7773 290a 2d20 5b46 726f 675d 2868 7474  ws).- [Frog](htt
-00001970: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001980: 5465 6e64 6572 4f77 6c2f 4672 6f67 2920  TenderOwl/Frog) 
-00001990: 284c 696e 7578 290a 2d20 5b54 6578 7469  (Linux).- [Texti
-000019a0: 6e61 746f 725d 2868 7474 7073 3a2f 2f67  nator](https://g
-000019b0: 6974 6875 622e 636f 6d2f 5268 6574 5462  ithub.com/RhetTb
-000019c0: 756c 6c2f 7465 7874 696e 6174 6f72 2920  ull/textinator) 
-000019d0: 286d 6163 4f53 290a 0a23 2320 4365 7274  (macOS)..## Cert
-000019e0: 6966 6963 6174 696f 6e0a 0a21 5b57 4f4d  ification..![WOM
-000019f0: 4d5d 2868 7474 7073 3a2f 2f72 6177 2e67  M](https://raw.g
-00001a00: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001a10: 2e63 6f6d 2f64 796e 6f62 6f2f 6c6d 6469  .com/dynobo/lmdi
-00001a20: 6167 2f6d 6173 7465 722f 6261 6467 652e  ag/master/badge.
-00001a30: 706e 6729 0a                             png).
+000004e0: 2f6e 6f72 6d63 6170 290a 0a3c 6120 6872  /normcap)..<a hr
+000004f0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
+00000500: 6275 796d 6561 636f 6666 6565 2e63 6f6d  buymeacoffee.com
+00000510: 2f64 796e 6f62 6f22 2074 6172 6765 743d  /dynobo" target=
+00000520: 225f 626c 616e 6b22 3e3c 696d 6720 7372  "_blank"><img sr
+00000530: 633d 2268 7474 7073 3a2f 2f63 646e 2e62  c="https://cdn.b
+00000540: 7579 6d65 6163 6f66 6665 652e 636f 6d2f  uymeacoffee.com/
+00000550: 6275 7474 6f6e 732f 7632 2f64 6566 6175  buttons/v2/defau
+00000560: 6c74 2d79 656c 6c6f 772e 706e 6722 2061  lt-yellow.png" a
+00000570: 6c74 3d22 4275 7920 4d65 2041 2043 6f66  lt="Buy Me A Cof
+00000580: 6665 6522 2073 7479 6c65 3d22 6865 6967  fee" style="heig
+00000590: 6874 3a20 3430 7078 2021 696d 706f 7274  ht: 40px !import
+000005a0: 616e 743b 2220 3e3c 2f61 3e0a 0a2a 2a4c  ant;" ></a>..**L
+000005b0: 696e 6b73 3a2a 2a20 5b53 6f75 7263 6520  inks:** [Source 
+000005c0: 436f 6465 5d28 6874 7470 733a 2f2f 6769  Code](https://gi
+000005d0: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
+000005e0: 6e6f 726d 6361 7029 207c 0a5b 446f 6375  normcap) |.[Docu
+000005f0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+00000600: 3a2f 2f64 796e 6f62 6f2e 6769 7468 7562  ://dynobo.github
+00000610: 2e69 6f2f 6e6f 726d 6361 702f 2920 7c0a  .io/normcap/) |.
+00000620: 5b46 4151 735d 2868 7474 7073 3a2f 2f64  [FAQs](https://d
+00000630: 796e 6f62 6f2e 6769 7468 7562 2e69 6f2f  ynobo.github.io/
+00000640: 6e6f 726d 6361 702f 2366 6171 7329 207c  normcap/#faqs) |
+00000650: 0a5b 5265 6c65 6173 6573 5d28 6874 7470  .[Releases](http
+00000660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000670: 796e 6f62 6f2f 6e6f 726d 6361 702f 7265  ynobo/normcap/re
+00000680: 6c65 6173 6573 2920 7c0a 5b43 6861 6e67  leases) |.[Chang
+00000690: 656c 6f67 5d28 6874 7470 733a 2f2f 6769  elog](https://gi
+000006a0: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
+000006b0: 6e6f 726d 6361 702f 626c 6f62 2f6d 6169  normcap/blob/mai
+000006c0: 6e2f 4348 414e 4745 4c4f 4729 0a0a 5b21  n/CHANGELOG)..[!
+000006d0: 5b53 6372 6565 6e63 6173 745d 2868 7474  [Screencast](htt
+000006e0: 7073 3a2f 2f75 7365 722d 696d 6167 6573  ps://user-images
+000006f0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000700: 6e74 2e63 6f6d 2f31 3130 3731 3837 362f  nt.com/11071876/
+00000710: 3138 3937 3637 3538 352d 3862 6334 3563  189767585-8bc45c
+00000720: 3138 2d38 3339 322d 3431 3164 2d38 3464  18-8392-411d-84d
+00000730: 632d 6365 6631 6362 3564 6263 3437 2e67  c-cef1cb5dbc47.g
+00000740: 6966 295d 2868 7474 7073 3a2f 2f72 6177  if)](https://raw
+00000750: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000760: 6e74 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  nt.com/dynobo/no
+00000770: 726d 6361 702f 6d61 696e 2f61 7373 6574  rmcap/main/asset
+00000780: 732f 6e6f 726d 6361 702e 6769 6629 0a0a  s/normcap.gif)..
+00000790: 2323 2051 7569 636b 7374 6172 740a 0a49  ## Quickstart..I
+000007a0: 6e73 7461 6c6c 2061 2070 7265 6275 696c  nstall a prebuil
+000007b0: 7420 7265 6c65 6173 653a 0a0a 2d20 2a2a  t release:..- **
+000007c0: 5769 6e64 6f77 732a 2a3a 0a20 205b 4e6f  Windows**:.  [No
+000007d0: 726d 4361 702d 302e 342e 312d 7838 365f  rmCap-0.4.1-x86_
+000007e0: 3634 2d57 696e 646f 7773 2e6d 7369 5d28  64-Windows.msi](
+000007f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000800: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
+00000810: 702f 7265 6c65 6173 6573 2f64 6f77 6e6c  p/releases/downl
+00000820: 6f61 642f 7630 2e34 2e31 2f4e 6f72 6d43  oad/v0.4.1/NormC
+00000830: 6170 2d30 2e34 2e31 2d78 3836 5f36 342d  ap-0.4.1-x86_64-
+00000840: 5769 6e64 6f77 732e 6d73 6929 0a2d 202a  Windows.msi).- *
+00000850: 2a4c 696e 7578 2a2a 3a0a 2020 5b4e 6f72  *Linux**:.  [Nor
+00000860: 6d43 6170 2d30 2e34 2e31 2d78 3836 5f36  mCap-0.4.1-x86_6
+00000870: 342e 4170 7049 6d61 6765 5d28 6874 7470  4.AppImage](http
+00000880: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000890: 796e 6f62 6f2f 6e6f 726d 6361 702f 7265  ynobo/normcap/re
+000008a0: 6c65 6173 6573 2f64 6f77 6e6c 6f61 642f  leases/download/
+000008b0: 7630 2e34 2e31 2f4e 6f72 6d43 6170 2d30  v0.4.1/NormCap-0
+000008c0: 2e34 2e31 2d78 3836 5f36 342e 4170 7049  .4.1-x86_64.AppI
+000008d0: 6d61 6765 290a 2d20 2a2a 6d61 634f 532a  mage).- **macOS*
+000008e0: 2a20 2878 3836 2920 c2b9 3a0a 2020 5b4e  * (x86) ..:.  [N
+000008f0: 6f72 6d43 6170 2d30 2e34 2e31 2d78 3836  ormCap-0.4.1-x86
+00000900: 5f36 342d 6d61 634f 532e 646d 675d 2868  _64-macOS.dmg](h
+00000910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000920: 6d2f 6479 6e6f 626f 2f6e 6f72 6d63 6170  m/dynobo/normcap
+00000930: 2f72 656c 6561 7365 732f 646f 776e 6c6f  /releases/downlo
+00000940: 6164 2f76 302e 342e 312f 4e6f 726d 4361  ad/v0.4.1/NormCa
+00000950: 702d 302e 342e 312d 7838 365f 3634 2d6d  p-0.4.1-x86_64-m
+00000960: 6163 4f53 2e64 6d67 290a 2d20 2a2a 6d61  acOS.dmg).- **ma
+00000970: 634f 532a 2a20 284d 3129 20c2 b9c2 b7c2  cOS** (M1) .....
+00000980: b23a 0a20 205b 4e6f 726d 4361 702d 302e  .:.  [NormCap-0.
+00000990: 342e 312d 6172 6d36 342d 6d61 634f 532e  4.1-arm64-macOS.
+000009a0: 646d 675d 2868 7474 7073 3a2f 2f67 6974  dmg](https://git
+000009b0: 6875 622e 636f 6d2f 6479 6e6f 626f 2f6e  hub.com/dynobo/n
+000009c0: 6f72 6d63 6170 2f72 656c 6561 7365 732f  ormcap/releases/
+000009d0: 646f 776e 6c6f 6164 2f76 302e 342e 312f  download/v0.4.1/
+000009e0: 4e6f 726d 4361 702d 302e 342e 312d 6172  NormCap-0.4.1-ar
+000009f0: 6d36 342d 6d61 634f 532e 646d 6729 0a20  m64-macOS.dmg). 
+00000a00: 205c 0a20 203c 7375 623e 313a 204f 6e20   \.  <sub>1: On 
+00000a10: 6d61 634f 532c 2061 6c6c 6f77 2074 6865  macOS, allow the
+00000a20: 2075 6e73 6967 6e65 6420 6170 706c 6963   unsigned applic
+00000a30: 6174 696f 6e20 6f6e 2066 6972 7374 2073  ation on first s
+00000a40: 7461 7274 3a20 2253 7973 7465 6d0a 2020  tart: "System.  
+00000a50: 5072 6566 6572 656e 6365 7322 20e2 8692  Preferences" ...
+00000a60: 2022 5365 6375 7269 7479 2026 2050 7269   "Security & Pri
+00000a70: 7661 6379 2220 e286 9220 2247 656e 6572  vacy" ... "Gener
+00000a80: 616c 2220 e286 9220 224f 7065 6e20 616e  al" ... "Open an
+00000a90: 7977 6179 222e 2059 6f75 206d 6967 6874  yway". You might
+00000aa0: 2061 6c73 6f20 6e65 6564 0a20 2074 6f20   also need.  to 
+00000ab0: 616c 6c6f 7720 4e6f 726d 4361 7020 746f  allow NormCap to
+00000ac0: 2074 616b 6520 7363 7265 656e 7368 6f74   take screenshot
+00000ad0: 732e 0a20 205b 2331 3335 5d28 6874 7470  s..  [#135](http
+00000ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000af0: 796e 6f62 6f2f 6e6f 726d 6361 702f 6973  ynobo/normcap/is
+00000b00: 7375 6573 2f31 3335 293c 6272 3e20 323a  sues/135)<br> 2:
+00000b10: 204d 6967 6874 2062 6520 6176 6169 6c61   Might be availa
+00000b20: 626c 6520 6120 6269 740a 2020 6465 6c61  ble a bit.  dela
+00000b30: 7965 642c 2061 7320 6974 2069 7320 6375  yed, as it is cu
+00000b40: 7272 656e 746c 7920 6275 696c 6420 6d61  rrently build ma
+00000b50: 6e75 616c 6c79 2e20 2854 6878 2c0a 2020  nually. (Thx,.  
+00000b60: 5b40 5461 6b72 696e 5d28 6874 7470 733a  [@Takrin](https:
+00000b70: 2f2f 6769 7468 7562 2e63 6f6d 2f54 616b  //github.com/Tak
+00000b80: 7269 6e29 2129 3c2f 7375 623e 0a0a 496e  rin)!)</sub>..In
+00000b90: 7374 616c 6c20 6672 6f6d 2072 6570 6f73  stall from repos
+00000ba0: 6974 6f72 6965 733a 0a0a 2d20 2a2a 5769  itories:..- **Wi
+00000bb0: 6e64 6f77 732a 2a3a 2049 6e73 7461 6c6c  ndows**: Install
+00000bc0: 2066 726f 6d0a 2020 5b4d 6963 726f 736f   from.  [Microso
+00000bd0: 6674 2053 746f 7265 5d28 6874 7470 733a  ft Store](https:
+00000be0: 2f2f 6170 7073 2e6d 6963 726f 736f 6674  //apps.microsoft
+00000bf0: 2e63 6f6d 2f73 746f 7265 2f64 6574 6169  .com/store/detai
+00000c00: 6c2f 6e6f 726d 6361 702f 5850 444c 4a4e  l/normcap/XPDLJN
+00000c10: 4234 4236 4332 5a52 292e 0a2d 202a 2a41  B4B6C2ZR)..- **A
+00000c20: 7263 6820 2f20 4d61 6e6a 6172 6f2a 2a3a  rch / Manjaro**:
+00000c30: 2049 6e73 7461 6c6c 2074 6865 0a20 205b   Install the.  [
+00000c40: 606e 6f72 6d63 6170 605d 2868 7474 7073  `normcap`](https
+00000c50: 3a2f 2f61 7572 2e61 7263 686c 696e 7578  ://aur.archlinux
+00000c60: 2e6f 7267 2f70 6163 6b61 6765 732f 6e6f  .org/packages/no
+00000c70: 726d 6361 7029 2070 6163 6b61 6765 2066  rmcap) package f
+00000c80: 726f 6d20 4155 522e 0a2d 202a 2a46 6c61  rom AUR..- **Fla
+00000c90: 7450 616b 2028 4c69 6e75 7829 2a2a 3a20  tPak (Linux)**: 
+00000ca0: 496e 7374 616c 6c0a 2020 5b63 6f6d 2e67  Install.  [com.g
+00000cb0: 6974 6875 622e 6479 6e6f 626f 2e6e 6f72  ithub.dynobo.nor
+00000cc0: 6d63 6170 5d28 6874 7470 733a 2f2f 666c  mcap](https://fl
+00000cd0: 6174 6875 622e 6f72 672f 6170 7073 2f64  athub.org/apps/d
+00000ce0: 6574 6169 6c73 2f63 6f6d 2e67 6974 6875  etails/com.githu
+00000cf0: 622e 6479 6e6f 626f 2e6e 6f72 6d63 6170  b.dynobo.normcap
+00000d00: 290a 2020 6672 6f6d 2046 6c61 7448 7562  ).  from FlatHub
+00000d10: 2e0a 0a49 6620 796f 7520 6578 7065 7269  ...If you experi
+00000d20: 656e 6365 2069 7373 7565 7320 706c 6561  ence issues plea
+00000d30: 7365 206c 6f6f 6b20 6174 2074 6865 0a5b  se look at the.[
+00000d40: 4641 5173 5d28 6874 7470 733a 2f2f 6479  FAQs](https://dy
+00000d50: 6e6f 626f 2e67 6974 6875 622e 696f 2f6e  nobo.github.io/n
+00000d60: 6f72 6d63 6170 2f23 6661 7173 2920 6f72  ormcap/#faqs) or
+00000d70: 0a5b 6f70 656e 2061 6e20 6973 7375 655d  .[open an issue]
+00000d80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000d90: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
+00000da0: 6170 2f69 7373 7565 7329 2e0a 0a23 2320  ap/issues)...## 
+00000db0: 5079 7468 6f6e 2070 6163 6b61 6765 0a0a  Python package..
+00000dc0: 4173 2061 6e20 5f61 6c74 6572 6e61 7469  As an _alternati
+00000dd0: 7665 5f20 746f 2061 2070 7265 6275 696c  ve_ to a prebuil
+00000de0: 7420 7061 636b 6167 6520 796f 7520 6361  t package you ca
+00000df0: 6e20 696e 7374 616c 6c20 7468 650a 5b4e  n install the.[N
+00000e00: 6f72 6d43 6170 2050 7974 686f 6e20 7061  ormCap Python pa
+00000e10: 636b 6167 655d 2868 7474 7073 3a2f 2f70  ckage](https://p
+00000e20: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000e30: 6e6f 726d 6361 702f 2920 666f 7220 2a2a  normcap/) for **
+00000e40: 5079 7468 6f6e 203e 3d33 2e39 2a2a 3a0a  Python >=3.9**:.
+00000e50: 0a23 2323 2320 4f6e 204c 696e 7578 0a0a  .#### On Linux..
+00000e60: 6060 6073 680a 2320 496e 7374 616c 6c20  ```sh.# Install 
+00000e70: 6465 7065 6e64 656e 6369 6573 2028 5562  dependencies (Ub
+00000e80: 756e 7475 2f44 6562 6961 6e29 0a73 7564  untu/Debian).sud
+00000e90: 6f20 6170 7420 696e 7374 616c 6c20 6275  o apt install bu
+00000ea0: 696c 642d 6573 7365 6e74 6961 6c20 7465  ild-essential te
+00000eb0: 7373 6572 6163 742d 6f63 7220 7465 7373  sseract-ocr tess
+00000ec0: 6572 6163 742d 6f63 722d 656e 6720 6c69  eract-ocr-eng li
+00000ed0: 6274 6573 7365 7261 6374 2d64 6576 206c  btesseract-dev l
+00000ee0: 6962 6c65 7074 6f6e 6963 612d 6465 7620  ibleptonica-dev 
+00000ef0: 776c 2d63 6c69 7062 6f61 7264 0a0a 2323  wl-clipboard..##
+00000f00: 2049 6e73 7461 6c6c 2064 6570 656e 6465   Install depende
+00000f10: 6e63 6965 7320 2841 7263 6829 0a73 7564  ncies (Arch).sud
+00000f20: 6f20 7061 636d 616e 202d 5320 7465 7373  o pacman -S tess
+00000f30: 6572 6163 7420 7465 7373 6572 6163 742d  eract tesseract-
+00000f40: 6461 7461 2d65 6e67 2077 6c2d 636c 6970  data-eng wl-clip
+00000f50: 626f 6172 640a 0a23 2320 496e 7374 616c  board..## Instal
+00000f60: 6c20 6465 7065 6e64 656e 6369 6573 2028  l dependencies (
+00000f70: 4665 646f 7261 290a 7375 646f 2064 6e66  Fedora).sudo dnf
+00000f80: 2069 6e73 7461 6c6c 2074 6573 7365 7261   install tessera
+00000f90: 6374 2077 6c2d 636c 6970 626f 6172 640a  ct wl-clipboard.
+00000fa0: 0a23 2320 496e 7374 616c 6c20 6465 7065  .## Install depe
+00000fb0: 6e64 656e 6369 6573 2028 6f70 656e 5355  ndencies (openSU
+00000fc0: 5345 290a 7375 646f 207a 7970 7065 7220  SE).sudo zypper 
+00000fd0: 696e 7374 616c 6c20 7079 7468 6f6e 332d  install python3-
+00000fe0: 6465 7665 6c20 7465 7373 6572 6163 742d  devel tesseract-
+00000ff0: 6f63 7220 7465 7373 6572 6163 742d 6f63  ocr tesseract-oc
+00001000: 722d 6465 7665 6c20 776c 2d63 6c69 7062  r-devel wl-clipb
+00001010: 6f61 7264 0a0a 2320 496e 7374 616c 6c20  oard..# Install 
+00001020: 6e6f 726d 6361 700a 7069 7020 696e 7374  normcap.pip inst
+00001030: 616c 6c20 6e6f 726d 6361 700a 0a23 2052  all normcap..# R
+00001040: 756e 0a2e 2f6e 6f72 6d63 6170 0a60 6060  un../normcap.```
+00001050: 0a0a 2323 2323 204f 6e20 6d61 634f 530a  ..#### On macOS.
+00001060: 0a60 6060 7368 0a23 2049 6e73 7461 6c6c  .```sh.# Install
+00001070: 2064 6570 656e 6465 6e63 6965 730a 6272   dependencies.br
+00001080: 6577 2069 6e73 7461 6c6c 2074 6573 7365  ew install tesse
+00001090: 7261 6374 2074 6573 7365 7261 6374 2d6c  ract tesseract-l
+000010a0: 616e 670a 0a23 2049 6e73 7461 6c6c 206e  ang..# Install n
+000010b0: 6f72 6d63 6170 0a70 6970 2069 6e73 7461  ormcap.pip insta
+000010c0: 6c6c 206e 6f72 6d63 6170 0a0a 2320 5275  ll normcap..# Ru
+000010d0: 6e0a 2e2f 6e6f 726d 6361 700a 6060 600a  n../normcap.```.
+000010e0: 0a23 2323 2320 4f6e 2057 696e 646f 7773  .#### On Windows
+000010f0: 0a0a 315c 2e20 496e 7374 616c 6c20 6054  ..1\. Install `T
+00001100: 6573 7365 7261 6374 2035 6020 6279 2075  esseract 5` by u
+00001110: 7369 6e67 2074 6865 0a5b 696e 7374 616c  sing the.[instal
+00001120: 6c65 7220 7072 6f76 6964 6564 2062 7920  ler provided by 
+00001130: 5542 204d 616e 6e68 6569 6d5d 2868 7474  UB Mannheim](htt
+00001140: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001150: 5542 2d4d 616e 6e68 6569 6d2f 7465 7373  UB-Mannheim/tess
+00001160: 6572 6163 742f 7769 6b69 292e 0a0a 325c  eract/wiki)...2\
+00001170: 2e20 4164 6a75 7374 2065 6e76 6972 6f6e  . Adjust environ
+00001180: 6d65 6e74 2076 6172 6961 626c 6573 3a0a  ment variables:.
+00001190: 0a2d 2043 7265 6174 6520 616e 2065 6e76  .- Create an env
+000011a0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+000011b0: 6520 6054 4553 5344 4154 415f 5052 4546  e `TESSDATA_PREF
+000011c0: 4958 6020 616e 6420 7365 7420 6974 2074  IX` and set it t
+000011d0: 6f20 5465 7373 6572 6163 7427 7320 6461  o Tesseract's da
+000011e0: 7461 0a20 2066 6f6c 6465 722c 2065 2e67  ta.  folder, e.g
+000011f0: 2e3a 0a0a 2020 6060 6063 6d64 0a20 2073  .:..  ```cmd.  s
+00001200: 6574 7820 5445 5353 4441 5441 5f50 5245  etx TESSDATA_PRE
+00001210: 4649 5820 2243 3a5c 5072 6f67 7261 6d20  FIX "C:\Program 
+00001220: 4669 6c65 735c 5465 7373 6572 6163 742d  Files\Tesseract-
+00001230: 4f43 525c 7465 7373 6461 7461 220a 2020  OCR\tessdata".  
+00001240: 6060 600a 0a2d 2041 7070 656e 6420 5465  ```..- Append Te
+00001250: 7373 6572 6163 7427 7320 6c6f 6361 7469  sseract's locati
+00001260: 6f6e 2074 6f20 7468 6520 656e 7669 726f  on to the enviro
+00001270: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
+00001280: 5061 7468 602c 2065 2e67 2e3a 0a0a 2020  Path`, e.g.:..  
+00001290: 6060 6063 6d64 0a20 2073 6574 7820 5061  ```cmd.  setx Pa
+000012a0: 7468 2022 2550 6174 6825 3b43 3a5c 5072  th "%Path%;C:\Pr
+000012b0: 6f67 7261 6d20 4669 6c65 735c 5465 7373  ogram Files\Tess
+000012c0: 6572 6163 742d 4f43 5222 0a20 2060 6060  eract-OCR".  ```
+000012d0: 0a0a 2d20 4d61 6b65 2073 7572 6520 746f  ..- Make sure to
+000012e0: 2063 6c6f 7365 2061 6e64 2072 656f 7065   close and reope
+000012f0: 6e20 796f 7572 2063 7572 7265 6e74 2074  n your current t
+00001300: 6572 6d69 6e61 6c20 7769 6e64 6f77 2074  erminal window t
+00001310: 6f20 6170 706c 7920 7468 6520 6e65 7720  o apply the new 
+00001320: 7661 7269 6162 6c65 732e 0a20 2054 6573  variables..  Tes
+00001330: 7420 6974 2062 7920 7275 6e6e 696e 673a  t it by running:
+00001340: 0a0a 2020 6060 6063 6d64 0a20 2074 6573  ..  ```cmd.  tes
+00001350: 7365 7261 6374 202d 2d6c 6973 742d 6c61  seract --list-la
+00001360: 6e67 730a 2020 6060 600a 0a33 5c2e 2049  ngs.  ```..3\. I
+00001370: 6e73 7461 6c6c 2061 6e64 2072 756e 204e  nstall and run N
+00001380: 6f72 6d43 6170 3a0a 0a60 6060 6261 7368  ormCap:..```bash
+00001390: 0a23 2049 6e73 7461 6c6c 206e 6f72 6d63  .# Install normc
+000013a0: 6170 0a70 6970 2069 6e73 7461 6c6c 206e  ap.pip install n
+000013b0: 6f72 6d63 6170 0a0a 2320 5275 6e0a 6e6f  ormcap..# Run.no
+000013c0: 726d 6361 700a 6060 600a 0a23 2320 5768  rmcap.```..## Wh
+000013d0: 7920 224e 6f72 6d43 6170 223f 0a0a 5365  y "NormCap"?..Se
+000013e0: 6520 5b58 4b43 445d 2868 7474 7073 3a2f  e [XKCD](https:/
+000013f0: 2f78 6b63 642e 636f 6d29 3a0a 0a5b 215b  /xkcd.com):..[![
+00001400: 436f 6d69 635d 2868 7474 7073 3a2f 2f69  Comic](https://i
+00001410: 6d67 732e 786b 6364 2e63 6f6d 2f63 6f6d  mgs.xkcd.com/com
+00001420: 6963 732f 6e6f 726d 5f6e 6f72 6d61 6c5f  ics/norm_normal_
+00001430: 6669 6c65 5f66 6f72 6d61 742e 706e 6729  file_format.png)
+00001440: 5d28 6874 7470 733a 2f2f 786b 6364 2e63  ](https://xkcd.c
+00001450: 6f6d 2f32 3131 362f 290a 0a23 2320 4465  om/2116/)..## De
+00001460: 7665 6c6f 706d 656e 740a 0a50 7265 7265  velopment..Prere
+00001470: 7175 6973 6974 6573 2066 6f72 2073 6574  quisites for set
+00001480: 7469 6e67 2075 7020 6120 6465 7665 6c6f  ting up a develo
+00001490: 706d 656e 7420 656e 7669 726f 6e6d 656e  pment environmen
+000014a0: 7420 6172 653a 202a 2a50 7974 686f 6e20  t are: **Python 
+000014b0: 3e3d 332e 392a 2a2c 0a2a 2a50 6f65 7472  >=3.9**,.**Poetr
+000014c0: 793e 3d31 2e33 2e32 2a2a 2061 6e64 202a  y>=1.3.2** and *
+000014d0: 2a54 6573 7365 7261 6374 2a2a 2028 696e  *Tesseract** (in
+000014e0: 636c 2e20 2a2a 6c61 6e67 7561 6765 2064  cl. **language d
+000014f0: 6174 612a 2a29 2e0a 0a60 6060 7368 0a23  ata**)...```sh.#
+00001500: 2043 6c6f 6e65 2072 6570 6f73 6974 6f72   Clone repositor
+00001510: 790a 6769 7420 636c 6f6e 6520 6874 7470  y.git clone http
+00001520: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001530: 796e 6f62 6f2f 6e6f 726d 6361 702e 6769  ynobo/normcap.gi
+00001540: 740a 0a23 2043 6861 6e67 6520 696e 746f  t..# Change into
+00001550: 2070 726f 6a65 6374 2064 6972 6563 746f   project directo
+00001560: 7279 0a63 6420 6e6f 726d 6361 700a 0a23  ry.cd normcap..#
+00001570: 2043 7265 6174 6520 7669 7274 7561 6c20   Create virtual 
+00001580: 656e 7620 616e 6420 696e 7374 616c 6c20  env and install 
+00001590: 6465 7065 6e64 656e 6369 6573 0a70 6f65  dependencies.poe
+000015a0: 7472 7920 696e 7374 616c 6c0a 0a23 2052  try install..# R
+000015b0: 6567 6973 7465 7220 7072 652d 636f 6d6d  egister pre-comm
+000015c0: 6974 2068 6f6f 6b0a 706f 6574 7279 2072  it hook.poetry r
+000015d0: 756e 2070 7265 2d63 6f6d 6d69 7420 696e  un pre-commit in
+000015e0: 7374 616c 6c0a 0a23 2052 756e 204e 6f72  stall..# Run Nor
+000015f0: 6d43 6170 2069 6e20 7669 7274 7561 6c20  mCap in virtual 
+00001600: 656e 760a 706f 6574 7279 2072 756e 2070  env.poetry run p
+00001610: 7974 686f 6e20 2d6d 206e 6f72 6d63 6170  ython -m normcap
+00001620: 0a60 6060 0a0a 2323 2043 7265 6469 7473  .```..## Credits
+00001630: 0a0a 5468 6973 2070 726f 6a65 6374 2075  ..This project u
+00001640: 7365 7320 7468 6520 666f 6c6c 6f77 696e  ses the followin
+00001650: 6720 6e6f 6e2d 7374 616e 6461 7264 206c  g non-standard l
+00001660: 6962 7261 7269 6573 3a0a 0a2d 205b 7079  ibraries:..- [py
+00001670: 7369 6465 365d 2868 7474 7073 3a2f 2f70  side6](https://p
+00001680: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00001690: 5079 5369 6465 362f 2920 5f2d 2062 696e  PySide6/) _- bin
+000016a0: 6469 6e67 7320 666f 7220 5174 2055 4920  dings for Qt UI 
+000016b0: 4672 616d 6577 6f72 6b5f 0a2d 205b 6a65  Framework_.- [je
+000016c0: 6570 6e65 795d 2868 7474 7073 3a2f 2f70  epney](https://p
+000016d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000016e0: 6a65 6570 6e65 792f 2920 5f2d 2044 4255  jeepney/) _- DBU
+000016f0: 5320 636c 6965 6e74 5f0a 0a41 6e64 2069  S client_..And i
+00001700: 7420 6465 7065 6e64 7320 6f6e 2065 7874  t depends on ext
+00001710: 6572 6e61 6c20 736f 6674 7761 7265 3a0a  ernal software:.
+00001720: 0a2d 205b 7465 7373 6572 6163 745d 2868  .- [tesseract](h
+00001730: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001740: 6d2f 7465 7373 6572 6163 742d 6f63 722f  m/tesseract-ocr/
+00001750: 7465 7373 6572 6163 7429 202d 205f 4f43  tesseract) - _OC
+00001760: 5220 656e 6769 6e65 5f0a 2d20 5b77 6c2d  R engine_.- [wl-
+00001770: 636c 6970 626f 6172 645d 2868 7474 7073  clipboard](https
+00001780: 3a2f 2f67 6974 6875 622e 636f 6d2f 6275  ://github.com/bu
+00001790: 6761 6576 632f 776c 2d63 6c69 7062 6f61  gaevc/wl-clipboa
+000017a0: 7264 2920 2d20 5f57 6179 6c61 6e64 2063  rd) - _Wayland c
+000017b0: 6c69 7062 6f61 7264 0a20 2075 7469 6c69  lipboard.  utili
+000017c0: 7469 6573 5f0a 0a50 6163 6b61 6769 6e67  ties_..Packaging
+000017d0: 2069 7320 646f 6e65 2077 6974 683a 0a0a   is done with:..
+000017e0: 2d20 5b62 7269 6566 6361 7365 5d28 6874  - [briefcase](ht
+000017f0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00001800: 726f 6a65 6374 2f62 7269 6566 6361 7365  roject/briefcase
+00001810: 2f29 205f 2d20 636f 6e76 6572 7469 6e67  /) _- converting
+00001820: 2050 7974 686f 6e20 7072 6f6a 6563 7473   Python projects
+00001830: 2069 6e74 6f5f 0a20 205f 7374 616e 6461   into_.  _standa
+00001840: 6c6f 6e65 2061 7070 735f 0a0a 5468 616e  lone apps_..Than
+00001850: 6b73 2074 6f20 7468 6520 6d61 696e 7461  ks to the mainta
+00001860: 696e 6572 7320 6f66 2074 686f 7365 206e  iners of those n
+00001870: 6963 6520 746f 6f6c 7321 0a0a 2323 2053  ice tools!..## S
+00001880: 696d 696c 6172 206f 7065 6e20 736f 7572  imilar open sour
+00001890: 6365 2074 6f6f 6c73 0a0a 4966 204e 6f72  ce tools..If Nor
+000018a0: 6d43 6170 2064 6f65 736e 2774 2066 6974  mCap doesn't fit
+000018b0: 2079 6f75 7220 6e65 6564 732c 2074 7279   your needs, try
+000018c0: 2074 686f 7365 2061 6c74 6572 6e61 7469   those alternati
+000018d0: 7665 7320 286e 6f20 7061 7274 6963 756c  ves (no particul
+000018e0: 6172 206f 7264 6572 293a 0a0a 2d20 5b54  ar order):..- [T
+000018f0: 6578 7453 6e61 7463 6865 725d 2868 7474  extSnatcher](htt
+00001900: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001910: 5261 6a53 6f6c 6169 2f54 6578 7453 6e61  RajSolai/TextSna
+00001920: 7463 6865 7229 2028 4c69 6e75 7829 0a2d  tcher) (Linux).-
+00001930: 205b 4772 6565 6e53 686f 745d 2868 7474   [GreenShot](htt
+00001940: 7073 3a2f 2f67 6574 6772 6565 6e73 686f  ps://getgreensho
+00001950: 742e 6f72 672f 2920 284c 696e 7578 2c20  t.org/) (Linux, 
+00001960: 6d61 634f 5329 0a2d 205b 5465 7874 5368  macOS).- [TextSh
+00001970: 6f74 5d28 6874 7470 733a 2f2f 6769 7468  ot](https://gith
+00001980: 7562 2e63 6f6d 2f69 616e 7a68 616f 3035  ub.com/ianzhao05
+00001990: 2f74 6578 7473 686f 7429 2028 5769 6e64  /textshot) (Wind
+000019a0: 6f77 7329 0a2d 205b 6749 6d61 6765 5265  ows).- [gImageRe
+000019b0: 6164 6572 5d28 6874 7470 733a 2f2f 6769  ader](https://gi
+000019c0: 7468 7562 2e63 6f6d 2f6d 616e 6973 616e  thub.com/manisan
+000019d0: 6472 6f2f 6749 6d61 6765 5265 6164 6572  dro/gImageReader
+000019e0: 2920 284c 696e 7578 2c20 5769 6e64 6f77  ) (Linux, Window
+000019f0: 7329 0a2d 205b 4361 7074 7572 6532 5465  s).- [Capture2Te
+00001a00: 7874 5d28 6874 7470 733a 2f2f 736f 7572  xt](https://sour
+00001a10: 6365 666f 7267 652e 6e65 742f 7072 6f6a  ceforge.net/proj
+00001a20: 6563 7473 2f63 6170 7475 7265 3274 6578  ects/capture2tex
+00001a30: 7429 2028 5769 6e64 6f77 7329 0a2d 205b  t) (Windows).- [
+00001a40: 4672 6f67 5d28 6874 7470 733a 2f2f 6769  Frog](https://gi
+00001a50: 7468 7562 2e63 6f6d 2f54 656e 6465 724f  thub.com/TenderO
+00001a60: 776c 2f46 726f 6729 2028 4c69 6e75 7829  wl/Frog) (Linux)
+00001a70: 0a2d 205b 5465 7874 696e 6174 6f72 5d28  .- [Textinator](
+00001a80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001a90: 6f6d 2f52 6865 7454 6275 6c6c 2f74 6578  om/RhetTbull/tex
+00001aa0: 7469 6e61 746f 7229 2028 6d61 634f 5329  tinator) (macOS)
+00001ab0: 0a2d 205b 5465 7874 2d47 7261 625d 2868  .- [Text-Grab](h
+00001ac0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001ad0: 6d2f 5468 654a 6f65 4669 6e2f 5465 7874  m/TheJoeFin/Text
+00001ae0: 2d47 7261 6229 2028 5769 6e64 6f77 7329  -Grab) (Windows)
+00001af0: 0a2d 205b 6470 5363 7265 656e 4f43 525d  .- [dpScreenOCR]
+00001b00: 2868 7474 7073 3a2f 2f64 616e 706c 612e  (https://danpla.
+00001b10: 6769 7468 7562 2e69 6f2f 6470 7363 7265  github.io/dpscre
+00001b20: 656e 6f63 722f 2920 284c 696e 7578 2c20  enocr/) (Linux, 
+00001b30: 5769 6e64 6f77 7329 0a0a 2323 2043 6572  Windows)..## Cer
+00001b40: 7469 6669 6361 7469 6f6e 0a0a 215b 574f  tification..![WO
+00001b50: 4d4d 5d28 6874 7470 733a 2f2f 7261 772e  MM](https://raw.
+00001b60: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001b70: 742e 636f 6d2f 6479 6e6f 626f 2f6c 6d64  t.com/dynobo/lmd
+00001b80: 6961 672f 6d61 7374 6572 2f62 6164 6765  iag/master/badge
+00001b90: 2e70 6e67 290a                           .png).
```

### Comparing `normcap-0.4.0/normcap/app.py` & `normcap-0.4.1/normcap/app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/clipboard/linux.py` & `normcap-0.4.1/normcap/clipboard/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def _wl_copy(text: str) -> None:
     """Use wl-clipboard package to copy text to system clipboard."""
     subprocess.run(
-        ["wl-copy"],
+        args=["wl-copy"],
         shell=False,
         input=text,
         encoding="utf-8",
         check=True,
         timeout=30,
     )
 
@@ -24,15 +24,14 @@
 def _is_wayland_display_manager() -> bool:
     wayland_display = os.environ.get("WAYLAND_DISPLAY", "")
     xdg_session_type = os.environ.get("XDG_SESSION_TYPE", "")
     return "wayland" in wayland_display.lower() or "wayland" in xdg_session_type.lower()
 
 
 def get_copy_func() -> Callable:
-
     if _is_wayland_display_manager():
         if shutil.which("wl-copy") is not None:
             logger.debug("Select clipboard method wl-copy")
             return _wl_copy
 
         logger.warning(
             "Your display manager uses Wayland. Please install the system "
```

### Comparing `normcap-0.4.0/normcap/clipboard/macos.py` & `normcap-0.4.1/normcap/clipboard/macos.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from normcap.clipboard import qt
 
 logger = logging.getLogger(__name__)
 
 
 def pbcopy(text: str) -> None:
     subprocess.run(
-        ["pbcopy", "w"],
-        shell=False,
+        ["pbcopy", "w"],  # noqa: S607
+        shell=False,  # noqa: S603
         input=text,
         encoding="utf-8",
         check=True,
         timeout=30,
     )
```

### Comparing `normcap-0.4.0/normcap/clipboard/windows.py` & `normcap-0.4.1/normcap/clipboard/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 """
 
 import contextlib
 import ctypes
 import logging
 import sys
 import time
+from collections.abc import Generator, Iterator
 from ctypes import c_size_t, c_wchar, c_wchar_p, get_errno, sizeof
-from typing import Any, Callable, Generator, Iterator
+from typing import Any, Callable
 
 logger = logging.getLogger(__name__)
 
 
 class CheckedCall:
     def __init__(self, f: Any) -> None:  # noqa: ANN401
         self.argtypes: list
@@ -32,15 +33,15 @@
             raise RuntimeError(f"Error calling {self.f.__name__}")
         return ret
 
     def __setattr__(self, key: str, value: Any) -> None:  # noqa: ANN401
         setattr(self.f, key, value)
 
 
-def _windll_copy(text: str) -> None:
+def _windll_copy(text: str) -> None:  # noqa: PLR0915
     if sys.platform != "win32":
         raise RuntimeError("Windows clipboard only available on Windows OS.")
 
     from ctypes.wintypes import (
         BOOL,
         DWORD,
         HANDLE,
@@ -148,40 +149,39 @@
 
         try:
             yield
         finally:
             safeCloseClipboard()
 
     def copy_windows(text: str) -> None:
-        with window() as hwnd:
+        with window() as hwnd, clipboard(hwnd):
             # http://msdn.com/ms649048
             # If an application calls OpenClipboard with hwnd set to NULL,
             # EmptyClipboard sets the clipboard owner to NULL;
             # this causes SetClipboardData to fail.
             # => We need a valid hwnd to copy something.
-            with clipboard(hwnd):
-                safeEmptyClipboard()
+            safeEmptyClipboard()
 
-                if text:
-                    # http://msdn.com/ms649051
-                    # If the hMem parameter identifies a memory object,
-                    # the object must have been allocated using the
-                    # function with the GMEM_MOVEABLE flag.
-                    count = wcslen(text) + 1
-                    handle = safeGlobalAlloc(GMEM_MOVEABLE, count * sizeof(c_wchar))
-                    locked_handle = safeGlobalLock(handle)
-
-                    ctypes.memmove(
-                        c_wchar_p(locked_handle),
-                        c_wchar_p(text),
-                        count * sizeof(c_wchar),
-                    )
+            if text:
+                # http://msdn.com/ms649051
+                # If the hMem parameter identifies a memory object,
+                # the object must have been allocated using the
+                # function with the GMEM_MOVEABLE flag.
+                count = wcslen(text) + 1
+                handle = safeGlobalAlloc(GMEM_MOVEABLE, count * sizeof(c_wchar))
+                locked_handle = safeGlobalLock(handle)
+
+                ctypes.memmove(
+                    c_wchar_p(locked_handle),
+                    c_wchar_p(text),
+                    count * sizeof(c_wchar),
+                )
 
-                    safeGlobalUnlock(handle)
-                    safeSetClipboardData(CF_UNICODETEXT, handle)
+                safeGlobalUnlock(handle)
+                safeSetClipboardData(CF_UNICODETEXT, handle)
 
     copy_windows(text)
 
 
 def get_copy_func() -> Callable:
     logger.debug("Select clipboard method windll")
     return _windll_copy
```

### Comparing `normcap-0.4.0/normcap/gui/constants.py` & `normcap-0.4.1/normcap/gui/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,21 @@
     "You are not using the prebuild package version of NormCap. "
     "Please refer to the documentation of Tesseract for your "
     "operating system on how to install additional languages."
 )
 
 URLS = Urls(
     releases="https://github.com/dynobo/normcap/releases",
-    changelog="https://github.com/dynobo/normcap/blob/main/CHANGELOG.md",
+    changelog="https://github.com/dynobo/normcap/blob/main/CHANGELOG",
     pypi="https://pypi.org/pypi/normcap",
     github="https://github.com/dynobo/normcap",
     issues="https://github.com/dynobo/normcap/issues",
     faqs="https://dynobo.github.io/normcap/#faqs",
     website="https://dynobo.github.io/normcap",
+    buymeacoffee="https://buymeacoffee.com/dynobo",
 )
 
 TESSDATA_REPO = "https://github.com/tesseract-ocr/tessdata_fast"
 TESSDATA_BASE_URL = f"{TESSDATA_REPO}/raw/4.1.0/"
 
 LANGUAGES = (
     ("afr", "2.5 MB", "Afrikaans", "Afrikaans"),
```

### Comparing `normcap-0.4.0/normcap/gui/downloader.py` & `normcap-0.4.1/normcap/gui/downloader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """Find new version on github or pypi."""
 import logging
-import ssl
-from urllib.request import urlopen
 
-import certifi
 from PySide6 import QtCore
 
 logger = logging.getLogger(__name__)
 
 
 class Communicate(QtCore.QObject):
     """TrayMenus' communication bus."""
 
     on_download_finished = QtCore.Signal(bytes, str)  # response, url
     on_download_failed = QtCore.Signal(str, str)  # msg, url
 
 
 class Worker(QtCore.QRunnable):
-    def __init__(self, url: str) -> None:
+    def __init__(self, url: str, timeout: int = 30) -> None:
         super().__init__()
         self.url = url
+        self.timeout = timeout
         self.com = Communicate()
 
     @QtCore.Slot()
     def run(self) -> None:
         try:
-            context = ssl.create_default_context(cafile=certifi.where())
-            with urlopen(self.url, context=context) as response:  # nosec B310
+            import ssl
+            from urllib.request import urlopen
+
+            context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLS_CLIENT)
+            context.load_default_certs()
+            if not context.get_ca_certs():
+                context = ssl._create_unverified_context()  # noqa: S323
+                logger.debug("Fallback to ssl without verification")
+            if not self.url.startswith("http"):
+                raise ValueError(f"Downloading from {self.url[:9]}... is not allowed.")
+            with urlopen(  # noqa: S310
+                self.url, context=context, timeout=self.timeout
+            ) as response:
                 raw_data = response.read()
         except Exception as e:
             msg = f"Exception '{e}' during download of '{self.url}'"
             logger.error(msg)
             self.com.on_download_failed.emit(msg, self.url)
         else:
             self.com.on_download_finished.emit(raw_data, self.url)
@@ -44,14 +53,14 @@
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.com = Communicate()
         self.threadpool = QtCore.QThreadPool()
 
-    def get(self, url: str) -> None:
+    def get(self, url: str, timeout: int = 30) -> None:
         """Start downloading url. Emits signal, when done."""
         logger.debug("Download %s", url)
-        worker = Worker(url=url)
+        worker = Worker(url=url, timeout=timeout)
         worker.com.on_download_finished.connect(self.com.on_download_finished)
         worker.com.on_download_failed.connect(self.com.on_download_failed)
         self.threadpool.start(worker)
```

### Comparing `normcap-0.4.0/normcap/gui/language_manager.py` & `normcap-0.4.1/normcap/gui/language_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 
 
 class LanguageManager(QtWidgets.QDialog):
     def __init__(
         self, tessdata_path: Path, parent: Optional[QtWidgets.QWidget] = None
     ) -> None:
         super().__init__(parent)
-        # TODO: Avoid unnecessary properties
 
         self.setModal(True)
-        self.setWindowTitle("Manage Languages (experimental)")
+        self.setWindowTitle("Manage Languages")
         self.setMinimumSize(800, 600)
 
         self.tessdata_path = tessdata_path
 
         self.com = Communicate()
         self.downloader = Downloader()
         self.downloader.com.on_download_failed.connect(self._on_download_error)
@@ -54,49 +53,49 @@
         )
         self.available_layout.button.pressed.connect(self._download)
 
         h_layout = QtWidgets.QHBoxLayout()
         h_layout.addLayout(self.installed_layout)
         h_layout.addLayout(self.available_layout)
 
-        self.close_button = QtWidgets.QPushButton("&Close")
-        self.close_button.pressed.connect(self.close)
+        close_button = QtWidgets.QPushButton("&Close")
+        close_button.pressed.connect(self.close)
 
         self.tessdata_label = QtWidgets.QLabel(
             f"<a href='file:///{self.tessdata_path.resolve()}'>"
-            "View tessdata folder in file manager...</a>"
+            "Close and view tessdata folder in file manager...</a>"
         )
         self.tessdata_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
         self.tessdata_label.linkActivated.connect(self.com.on_open_url)
         self.com.on_open_url.connect(self.close)
 
         layout = QtWidgets.QVBoxLayout()
         layout.addLayout(h_layout)
-        layout.addWidget(self.close_button)
+        layout.addWidget(close_button)
         layout.addWidget(self.tessdata_label)
 
         self.setLayout(layout)
 
         self.loading_indicator = LoadingIndicator(self, size=256)
 
         self._update_models()
-        self.close_button.setFocus()
+        close_button.setFocus()
 
     @QtCore.Slot(str, str)
     def _on_download_error(self, reason: str, url: str) -> None:
         self._set_in_progress(False)
         QtWidgets.QMessageBox.critical(
             self, "Error", f"<b>Language download failed!</b><br><br>{reason}"
         )
 
     @QtCore.Slot(bytes, str)
     def _on_download_finished(self, data: bytes, url: str) -> None:
         """Save language to tessdata folder."""
         file_name = url.split("/")[-1]
-        with open(self.tessdata_path / file_name, "wb") as fh:
+        with Path(self.tessdata_path / file_name).open(mode="wb") as fh:
             fh.write(data)
         self._update_models()
         self._set_in_progress(False)
 
     def _update_models(self) -> None:
         installed = self._get_installed_languages()
         self.installed_layout.model.languages = [
@@ -128,27 +127,32 @@
         if not indexes:
             return
 
         if len(self.installed_layout.model.languages) <= 1:
             QtWidgets.QMessageBox.information(
                 self,
                 "Information",
-                "It is not possible to delete all languages. "
-                + "NormCap needs at least one to function correctly.",
+                (
+                    "It is not possible to delete all languages. "
+                    "NormCap needs at least one to function correctly."
+                ),
             )
             return
 
         index = indexes[0]
         language = self.installed_layout.model.languages[index.row()][0]
         Path(self.tessdata_path / f"{language}.traineddata").unlink()
         self._update_models()
 
     def _set_in_progress(self, value: bool) -> None:
         self.available_layout.view.setEnabled(not value)
+        self.available_layout.button.setEnabled(not value)
         self.installed_layout.view.setEnabled(not value)
+        self.installed_layout.button.setEnabled(not value)
+        self.tessdata_label.setEnabled(not value)
         self.loading_indicator.setVisible(value)
 
 
 class IconLabel(QtWidgets.QWidget):
     """Label with icon in front."""
 
     def __init__(self, icon: str, text: str) -> None:
```

### Comparing `normcap-0.4.0/normcap/gui/loading_indicator.py` & `normcap-0.4.1/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/gui/menu_button.py` & `normcap-0.4.1/normcap/gui/menu_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Create the settings button and its menu."""
 
 from typing import Any, Optional
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-from normcap import __version__, ocr
-from normcap.gui import system_info
+from normcap import __version__
 from normcap.gui.constants import MESSAGE_LANGUAGES, URLS
 
 _MENU_STYLE = """
 QMenu {
     background-color: rgba(0,0,0,0.8);
     color: white;
 }
@@ -48,122 +47,109 @@
 
 _BUTTON_STYLE = """
 QToolButton { border:0px; }
 QToolButton::hover {
     background: qradialgradient(
         cx: 0.5, cy: 0.5,
         fx: 0.5, fy: 0.5,
-        radius: 0.5,
-        stop: 0 rgba(0,0,0,0) stop: 0.25 rgba(255,255,255,80) stop: 0.95 rgba(0,0,0,0)
+        radius: 0.55,
+        stop: 0 rgba(0,0,0,0) stop: 0.25 rgba(255,255,255,120) stop: 0.95 rgba(0,0,0,0)
     );
 }
 QToolButton::menu-indicator { image: none; }
 """
 
 
 class Communicate(QtCore.QObject):
     """SettingsMenu' communication bus."""
 
     on_open_url = QtCore.Signal(str)
     on_close_in_settings = QtCore.Signal(str)
     on_manage_languages = QtCore.Signal()
+    on_setting_change = QtCore.Signal(str)
 
 
 class MenuButton(QtWidgets.QToolButton):
     """Button to adjust setting on main window top right."""
 
     title_font = QtGui.QFont(QtGui.QFont().family(), pointSize=10, weight=600)
 
     def __init__(
         self,
         settings: QtCore.QSettings,
+        installed_languages: list[str],
         language_manager: bool = False,
         parent: Optional[QtWidgets.QWidget] = None,
     ) -> None:
         super().__init__(parent)
+        self.languages = installed_languages
         self.setObjectName("settings_icon")
         self.settings = settings
         self.has_language_manager = language_manager
 
         self.setCursor(QtCore.Qt.CursorShape.ArrowCursor)
-        self.setFixedSize(38, 38)
+        self.setFixedSize(44, 44)
         self.setToolButtonStyle(QtCore.Qt.ToolButtonStyle.ToolButtonIconOnly)
 
         self.setIcon(QtGui.QIcon(":settings"))
-        self.setIconSize(QtCore.QSize(26, 26))
+        self.setIconSize(QtCore.QSize(32, 32))
         self.setPopupMode(QtWidgets.QToolButton.ToolButtonPopupMode.InstantPopup)
         self.setAutoRaise(True)
 
         self.message_box = QtWidgets.QMessageBox()
         self.message_box.setIconPixmap(QtGui.QIcon(":normcap").pixmap(48, 48))
         # Necessary on wayland for main window to regain focus:
         self.message_box.setWindowFlags(QtCore.Qt.WindowType.Popup)
 
-        self._add_menu()
+        self.setMenu(self._create_menu())
 
         self.setStyleSheet(_BUTTON_STYLE)
         self.com = Communicate()
 
-    def _add_menu(self) -> None:
+    def _create_menu(self) -> QtWidgets.QMenu:
         menu = QtWidgets.QMenu(self)
         menu.setObjectName("settings_menu")
         menu.setStyleSheet(
             _MENU_STYLE.replace("$COLOR", str(self.settings.value("color")))
         )
         menu.setAttribute(QtCore.Qt.WidgetAttribute.WA_TranslucentBackground, True)
-
-        self._add_title(menu, "Settings")
-        self._add_settings_section(menu)
-        menu.addSeparator()
-        self._add_title(menu, "Capture mode")
-        self._add_mode_section(menu)
-        menu.addSeparator()
-        self._add_title(menu, "Languages")
-        languages = ocr.utils.get_tesseract_languages(
-            tesseract_cmd=system_info.get_tesseract_path(),
-            tessdata_path=system_info.get_tessdata_path(),
-        )
-        self._add_languages_section(menu, languages=languages)
-        menu.addSeparator()
-        self._add_title(menu, "Application")
-        self._add_application_section(menu)
-        menu.triggered.connect(self._on_item_click)
-
-        self.setMenu(menu)
-
-    def _add_title(
-        self,
-        menu: QtWidgets.QMenu,
-        text: str,
-        action_parent: Optional[QtGui.QAction] = None,
-    ) -> None:
-        action = QtGui.QAction(text, action_parent or menu)
-        action.setEnabled(False)
-        action.setFont(self.title_font)
-        menu.addAction(action)
+        menu.triggered.connect(self.on_item_click)
+        menu.aboutToShow.connect(self.populate_menu_entries)
+        return menu
+
+    @QtCore.Slot(list)
+    def on_languages_changed(self, installed_languages: list[str]) -> None:
+        self.languages = installed_languages
 
     @QtCore.Slot(QtGui.QAction)
-    def _on_item_click(self, action: QtGui.QAction) -> None:
+    def on_item_click(self, action: QtGui.QAction) -> None:
         action_name = action.objectName()
         group = action.actionGroup()
         group_name = group.objectName() if group else None
         value: Optional[Any] = None
         setting = None
 
         if action_name == "close":
             self.com.on_close_in_settings.emit("Clicked close in settings")
-        elif action_name == "message_languages":
+            return
+
+        if action_name == "show_help_languages":
             self.message_box.setText(MESSAGE_LANGUAGES)
             self.message_box.exec_()
-        elif action_name == "manage_languages":
+            return
+
+        if action_name == "manage_languages":
             self.com.on_manage_languages.emit()
-        elif group_name == "website_group" or action_name.startswith("file:/"):
-            url = action_name
-            self.com.on_open_url.emit(url)
-        elif group_name == "settings_group":
+            return
+
+        if group_name == "website_group" or action_name.startswith("file:/"):
+            self.com.on_open_url.emit(action_name)
+            return
+
+        if group_name == "settings_group":
             setting = action_name
             value = action.isChecked()
         elif group_name == "mode_group":
             setting = "mode"
             value = action_name
         elif group_name == "language_group":
             setting = "language"
@@ -171,14 +157,43 @@
             if not languages:
                 languages = [action_name]
                 action.setChecked(True)
             value = languages
 
         if None not in (setting, value):
             self.settings.setValue(str(setting), value)
+            self.com.on_setting_change.emit(str(setting))
+
+    @QtCore.Slot()
+    def populate_menu_entries(self) -> None:
+        menu = self.menu()
+        menu.clear()
+
+        self._add_title(menu, "Settings")
+        self._add_settings_section(menu)
+        menu.addSeparator()
+        self._add_title(menu, "Capture mode")
+        self._add_mode_section(menu)
+        menu.addSeparator()
+        self._add_title(menu, "Languages")
+        self._add_languages_section(menu)
+        menu.addSeparator()
+        self._add_title(menu, "Application")
+        self._add_application_section(menu)
+
+    def _add_title(
+        self,
+        menu: QtWidgets.QMenu,
+        text: str,
+        action_parent: Optional[QtGui.QAction] = None,
+    ) -> None:
+        action = QtGui.QAction(text, action_parent or menu)
+        action.setEnabled(False)
+        action.setFont(self.title_font)
+        menu.addAction(action)
 
     def _add_settings_section(
         self, menu: QtWidgets.QMenu
     ) -> None:  # sourcery skip: class-extract-method
         settings_group = QtGui.QActionGroup(menu)
         settings_group.setObjectName("settings_group")
         settings_group.setExclusive(False)
@@ -214,18 +229,18 @@
 
         action = QtGui.QAction("raw", mode_group)
         action.setObjectName("raw")
         action.setCheckable(True)
         action.setChecked(self.settings.value("mode") == "raw")
         menu.addAction(action)
 
-    def _add_languages_section(
-        self, menu: QtWidgets.QMenu, languages: list[str]
-    ) -> None:
-        if len(languages) <= 7:
+    def _add_languages_section(self, menu: QtWidgets.QMenu) -> None:
+        languages = self.languages
+        overflow_languages_count = 7
+        if len(languages) <= overflow_languages_count:
             language_menu = menu
         else:
             language_menu = QtWidgets.QMenu("select", menu)
             language_menu.setObjectName("language_menu")
             menu.addMenu(language_menu)
 
         language_group = QtGui.QActionGroup(language_menu)
@@ -239,15 +254,15 @@
             language_menu.addAction(action)
 
         if self.has_language_manager:
             action = QtGui.QAction("add/remove...", menu)
             action.setObjectName("manage_languages")
         else:
             action = QtGui.QAction("... need more?", menu)
-            action.setObjectName("message_languages")
+            action.setObjectName("show_help_languages")
 
         menu.addAction(action)
 
     def _add_application_section(self, menu: QtWidgets.QMenu) -> None:
         submenu = QtWidgets.QMenu(menu)
         submenu.setObjectName("settings_menu_website")
         submenu.setTitle("About")
@@ -273,12 +288,16 @@
         action.setObjectName(URLS.releases)
         submenu.addAction(action)
 
         action = QtGui.QAction("Report a problem", about_group)
         action.setObjectName(URLS.issues)
         submenu.addAction(action)
 
+        action = QtGui.QAction("Buy me a coffee", about_group)
+        action.setObjectName(URLS.buymeacoffee)
+        submenu.addAction(action)
+
         menu.addMenu(submenu)
 
         action = QtGui.QAction("Close", menu)
         action.setObjectName("close")
         menu.addAction(action)
```

### Comparing `normcap-0.4.0/normcap/gui/models.py` & `normcap-0.4.1/normcap/gui/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Various Data Models."""
-from __future__ import annotations
-
 import enum
 import logging
 from collections import namedtuple
 from dataclasses import dataclass, field
 from typing import Optional
 
 from PySide6 import QtGui
@@ -40,14 +38,15 @@
     releases: str
     changelog: str
     pypi: str
     github: str
     issues: str
     website: str
     faqs: str
+    buymeacoffee: str
 
     @property
     def releases_atom(self) -> str:
         """URL to github releases rss feed."""
         return f"{self.releases}.atom"
 
     @property
@@ -92,15 +91,16 @@
         return self.bottom - self.top
 
     @property
     def size(self) -> tuple[int, int]:
         """Width and height of rect."""
         return (self.width, self.height)
 
-    def scaled(self, scale_factor: float) -> Rect:
+    # ONHOLD: Annotate as Self with Python 3.11
+    def scaled(self, scale_factor: float):  # noqa: ANN201
         """Create an integer-scaled copy of the Rect."""
         return Rect(
             top=int(self.top * scale_factor),
             bottom=int(self.bottom * scale_factor),
             left=int(self.left * scale_factor),
             right=int(self.right * scale_factor),
         )
```

### Comparing `normcap-0.4.0/normcap/gui/notifier.py` & `normcap-0.4.1/normcap/gui/notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             f"--icon={icon_path.resolve()}",
             "--app-name=NormCap",
             f"{title}",
             f"{message}",
         ]
 
         # Left detached on purpose!
-        subprocess.Popen(cmds, start_new_session=True)
+        subprocess.Popen(cmds, start_new_session=True)  # noqa: S603
 
     def send_via_qt_tray(self, title: str, message: str) -> None:
         """Send via QT trayicon.
 
         Used for:
             - Windows
             - macOS
```

### Comparing `normcap-0.4.0/normcap/gui/resources.py` & `normcap-0.4.1/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/gui/settings.py` & `normcap-0.4.1/normcap/gui/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Any, Iterable, Optional
+from collections.abc import Iterable
+from typing import Any, Optional
 
 from PySide6 import QtCore
 
 from normcap.gui.models import Setting
 
 logger = logging.getLogger(__name__)
```

### Comparing `normcap-0.4.0/normcap/gui/system_info.py` & `normcap-0.4.1/normcap/gui/system_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,47 +57,49 @@
 def get_tesseract_path() -> Path:
     if is_briefcase_package():
         if sys.platform == "linux":
             binary_path = Path(__file__).parent.parent.parent.parent / "bin"
         elif sys.platform == "win32":
             binary_path = Path(__file__).parent.parent / "resources" / "tesseract"
         elif sys.platform == "darwin":
-            binary_path = Path(__file__).parent.parent.parent.parent / "bin"
+            binary_path = (
+                Path(__file__).parent.parent.parent.parent / "app_packages" / "bin"
+            )
         else:
-            raise ValueError(f"Platform {sys.platform} is currently not supported")
+            raise ValueError(f"Platform {sys.platform} is not supported")
         extension = ".exe" if sys.platform == "win32" else ""
         tesseract_path = binary_path / f"tesseract{extension}"
         if not tesseract_path.exists():
-            raise RuntimeError(f"Couldn't locate tesseract binary in {tesseract_path}!")
+            raise RuntimeError(f"Could not locate Tesseract binary {tesseract_path}!")
         return tesseract_path
 
     # Then try to find tesseract on system
     if tesseract_bin := shutil.which("tesseract"):
         tesseract_path = Path(tesseract_bin)
         if tesseract_path.exists():
             return tesseract_path
 
     raise RuntimeError(
         "No Tesseract binary found! Tesseract has to be installed and added "
-        + "to PATH environment variable."
+        "to PATH environment variable."
     )
 
 
 def get_tessdata_path() -> Optional[os.PathLike]:
     """Deside which path for tesseract language files to use."""
     if is_briefcase_package() or is_flatpak_package():
         tessdata_path = config_directory() / "tessdata"
         return tessdata_path.resolve()
 
     if prefix := os.environ.get("TESSDATA_PREFIX", None):
         tessdata_path = Path(prefix) / "tessdata"
         if tessdata_path.is_dir() and list(tessdata_path.glob("*.traineddata")):
             return tessdata_path.resolve()
 
-    if sys.platform == "win32":
+    if sys.platform.startswith("win"):
         logger.warning("Missing tessdata directory. (Is TESSDATA_PREFIX variable set?)")
 
     return None
 
 
 @functools.cache
 def display_manager_is_wayland() -> bool:
@@ -113,17 +115,17 @@
     kde_full_session = os.environ.get("KDE_FULL_SESSION", "").lower()
     xdg_current_desktop = os.environ.get("XDG_CURRENT_DESKTOP", "").lower()
     desktop_session = os.environ.get("DESKTOP_SESSION", "").lower()
     gnome_desktop_session_id = os.environ.get("GNOME_DESKTOP_SESSION_ID", "")
     if gnome_desktop_session_id == "this-is-deprecated":
         gnome_desktop_session_id = ""
 
-    if gnome_desktop_session_id != "" or "gnome" in xdg_current_desktop:
+    if gnome_desktop_session_id or "gnome" in xdg_current_desktop:
         return DesktopEnvironment.GNOME
-    if kde_full_session != "" or "kde-plasma" in desktop_session:
+    if kde_full_session or "kde-plasma" in desktop_session:
         return DesktopEnvironment.KDE
     if "sway" in xdg_current_desktop:
         return DesktopEnvironment.SWAY
     if "unity" in xdg_current_desktop:
         return DesktopEnvironment.UNITY
 
     return DesktopEnvironment.OTHER
```

### Comparing `normcap-0.4.0/normcap/gui/tray.py` & `normcap-0.4.1/normcap/gui/tray.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,33 @@
 """Create system tray and its menu."""
-import datetime
-import io
 import logging
 import os
 import sys
-import tempfile
 import time
+from collections.abc import Iterable
 from functools import partial
-from pathlib import Path
-from typing import Any, Iterable, NoReturn
+from typing import Any, NoReturn, Optional
 
-from PIL import Image
-from PySide6 import QtCore, QtGui, QtWidgets
+from PySide6 import QtCore, QtGui, QtNetwork, QtWidgets
 
 from normcap import __version__, clipboard, ocr, screengrab
-from normcap.gui import resources, system_info
+from normcap.gui import resources, system_info, utils  # noqa: F401 (loads resources!)
 from normcap.gui.language_manager import LanguageManager
 from normcap.gui.menu_button import MenuButton
 from normcap.gui.models import Capture, CaptureMode, DesktopEnvironment, Rect, Screen
 from normcap.gui.notifier import Notifier
 from normcap.gui.settings import Settings
 from normcap.gui.update_check import UpdateChecker
 from normcap.gui.window import Window
 
-if not resources.qt_resource_data:
-    raise ValueError("Couldn't load QT resources")
-
 logger = logging.getLogger(__name__)
 
 UPDATE_CHECK_INTERVAL_DAYS = 7
 
 
-def _save_image_in_tempfolder(
-    image: Image.Image, postfix: str = "", log_level: int = logging.DEBUG
-) -> None:
-    """For debugging it can be useful to store the cropped image."""
-    if logger.getEffectiveLevel() == log_level:
-        file_dir = Path(tempfile.gettempdir()) / "normcap"
-        file_dir.mkdir(exist_ok=True)
-        now = datetime.datetime.now()
-        file_name = f"{now:%Y-%m-%d_%H-%M-%S_%f}{postfix}.png"
-        logger.debug("Save debug image as %s", file_dir / file_name)
-        image.save(str(file_dir / file_name))
-
-
 class Communicate(QtCore.QObject):
     """TrayMenus' communication bus."""
 
     on_close_or_exit = QtCore.Signal(str)
     on_copied_to_clipboard = QtCore.Signal()
     on_image_cropped = QtCore.Signal()
     on_manage_languages = QtCore.Signal()
@@ -55,270 +35,160 @@
     on_open_url_and_hide = QtCore.Signal(str)
     on_quit = QtCore.Signal()
     on_region_selected = QtCore.Signal(Rect)
     on_screenshots_updated = QtCore.Signal()
     on_send_notification = QtCore.Signal(Capture)
     on_tray_menu_capture_clicked = QtCore.Signal()
     on_window_positioned = QtCore.Signal()
+    on_languages_changed = QtCore.Signal(list)
 
 
 class SystemTray(QtWidgets.QSystemTrayIcon):
     """System tray icon with menu."""
 
     capture = Capture()
     windows: dict[int, Window] = {}
+    installed_languages: list[str] = []
+    _debug_language_manager = False
+    _socket_name = f"v{__version__}-normcap"
+    _socket_out: Optional[QtNetwork.QLocalSocket] = None
+    _socket_in: Optional[QtNetwork.QLocalSocket] = None
+    _socket_server: Optional[QtNetwork.QLocalServer] = None
 
     def __init__(self, parent: QtCore.QObject, args: dict[str, Any]) -> None:
         logger.debug("System info:\n%s", system_info.to_dict())
         super().__init__(parent)
 
         self.com = Communicate()
 
+        self._socket_out = QtNetwork.QLocalSocket(self)
+        self._socket_out.connectToServer(self._socket_name)
+        if self._socket_out.waitForConnected():
+            logger.debug("Another instance is already running. Sending capture signal.")
+            self._socket_out.write(b"capture")
+            self._socket_out.waitForBytesWritten(1000)
+            self._exit_application("NormCap already running")
+        else:
+            self._create_socket_server()
+
         self.settings = Settings("normcap", "settings", init_settings=args)
-        self._sanatize_active_language(self.settings)
+        self.installed_languages: list[str] = []
 
         if args.get("reset", False):
             self.settings.reset()
 
+        self.cli_mode = args.get("cli_mode", False)
+
         self.capture.mode = (
             CaptureMode.PARSE
             if self.settings.value("mode") == "parse"
             else CaptureMode.RAW
         )
 
         self.screens: list[Screen] = system_info.screens()
 
-        self._set_tray_icon()
-        self._add_tray_menu()
         self._ensure_screenshot_permission()
-        self._add_update_checker()
-        self._add_notifier()
         self._set_signals()
         self._update_screenshots(delayed=False)
-
-    def _ensure_screenshot_permission(self) -> None:
-        if screengrab.has_screenshot_permission():
-            return
-
-        if sys.platform == "darwin":
-            # Reset privacy permission in case of new NormCap version. This is necessary
-            # because somehow the setting is associated with the binary and won't work
-            # after it got updated.
-            if self.settings.value("version") != __version__:
-                self.settings.setValue("version", __version__)
-                screengrab.macos_reset_screenshot_permission()
-
-            # Trigger permission request to make the NormCap entry available in settings
-            screengrab.macos_request_screenshot_permission()
-
-            # Message box to explain what's happening and open the preferences
-            app = "NormCap" if system_info.is_prebuild_package() else "Terminal"
-            button = QtWidgets.QMessageBox.critical(
-                None,
-                "Error!",
-                f"{app} is missing permissions for 'Screen Recording'.\n\n"
-                + "Grant the permissions via 'Privacy & Security' settings "
-                + "and restart NormCap.\n\nClick OK to exit.",
-                buttons=QtWidgets.QMessageBox.Open | QtWidgets.QMessageBox.Cancel,
-            )
-            if button == QtWidgets.QMessageBox.Open:
-                logger.debug("Open macOS privacy settings")
-                screengrab.macos_open_privacy_settings()
-
-            self._exit_application("Screen Recording permissions missing on macOS")
-
-    def _set_tray_icon(self) -> None:
-        self.setIcon(QtGui.QIcon.fromTheme("tool-magic-symbolic", QtGui.QIcon(":tray")))
+        self.setContextMenu(QtWidgets.QMenu())
+        self._populate_context_menu_entries()
+        self.contextMenu().aboutToShow.connect(self._populate_context_menu_entries)
+        QtCore.QTimer.singleShot(100, self._delayed_init)
 
     @QtCore.Slot()
     def _color_tray_icon(self) -> None:
         if sizes := self.icon().availableSizes():
             pixmap = self.icon().pixmap(sizes[-1])
             mask = pixmap.createMaskFromColor(
                 QtGui.QColor("transparent"), QtCore.Qt.MaskMode.MaskInColor
             )
             pixmap.fill(QtGui.QColor(str(self.settings.value("color"))))
             pixmap.setMask(mask)
             self.setIcon(QtGui.QIcon(pixmap))
 
             QtCore.QTimer.singleShot(5000, self._set_tray_icon)
 
-    def _set_signals(self) -> None:
-        """Set up signals to trigger program logic."""
-        self.activated.connect(self._handle_tray_click)
-        self.com.on_tray_menu_capture_clicked.connect(self._update_screenshots)
-        self.com.on_screenshots_updated.connect(self._show_windows)
-        self.com.on_quit.connect(lambda: self._exit_application("clicked exit in tray"))
-        self.com.on_region_selected.connect(self._close_windows)
-        self.com.on_region_selected.connect(self._crop_image)
-        self.com.on_image_cropped.connect(self._capture_to_ocr)
-        self.com.on_ocr_performed.connect(self._copy_to_clipboard)
-        self.com.on_copied_to_clipboard.connect(self._notify_or_close)
-        self.com.on_copied_to_clipboard.connect(self._color_tray_icon)
-        self.com.on_close_or_exit.connect(self._close_or_exit)
-        self.com.on_open_url_and_hide.connect(self._open_url_and_hide)
-        self.com.on_manage_languages.connect(self._open_language_manager)
+    @QtCore.Slot()
+    def _on_new_connection(self) -> None:
+        """Open incoming socket to listen for messages from other NormCap instances."""
+        if not self._socket_server:
+            return
+        self._socket_in = self._socket_server.nextPendingConnection()
+        if self._socket_in:
+            logger.debug("Connect to incoming socket.")
+            self._socket_in.readyRead.connect(self._on_ready_read)
+
+    @QtCore.Slot()
+    def _on_ready_read(self) -> None:
+        """Process messages received from other NormCap instances."""
+        if not self._socket_in:
+            return
+        message = self._socket_in.readAll()
+        if message and bytes(message).decode("utf-8", errors="ignore") == "capture":
+            logger.info("Received socket signal to capture.")
+            self._update_screenshots()
 
     @QtCore.Slot(QtWidgets.QSystemTrayIcon.ActivationReason)
     def _handle_tray_click(
         self, reason: QtWidgets.QSystemTrayIcon.ActivationReason
     ) -> None:
         logger.debug("Tray event: %s", reason)
-        if reason == QtWidgets.QSystemTrayIcon.ActivationReason.Trigger:
+        if (
+            reason == QtWidgets.QSystemTrayIcon.ActivationReason.Trigger
+            and self.settings.value("tray", False, type=bool)
+        ):
             self._update_screenshots()
 
-    def _add_update_checker(self) -> None:
-        if self.settings.value("update", type=bool) is False:
-            return
-
-        interval = datetime.timedelta(days=UPDATE_CHECK_INTERVAL_DAYS)
-        today_sub_interval = f"{datetime.datetime.now() - interval:%Y-%m-%d}"
-        if str(self.settings.value("last-update-check", type=str)) > today_sub_interval:
-            return
-
-        checker = UpdateChecker(self, packaged=system_info.is_prebuild_package())
-        checker.com.on_version_checked.connect(self._update_time_of_last_update_check)
-        checker.com.on_click_get_new_version.connect(self.com.on_open_url_and_hide)
-        QtCore.QTimer.singleShot(500, checker.check)
-
-    def _update_time_of_last_update_check(self, newest_version: str) -> None:
-        if newest_version is not None:
-            today = f"{datetime.datetime.now():%Y-%m-%d}"
-            self.settings.setValue("last-update-check", today)
-
-    def _add_notifier(self) -> None:
-        self.notifier = Notifier(self)
-        self.com.on_send_notification.connect(self.notifier.send_notification)
-        self.notifier.com.on_notification_sent.connect(
-            lambda: self.com.on_close_or_exit.emit("notification sent")
-        )
-
-    def _update_screenshots(self, delayed: bool = True) -> None:
-        """Get new screenshots and cache them."""
-        if delayed:
-            time.sleep(0.15)
-
-        capture = screengrab.get_capture_func()
-        screens = capture()
-
-        if not screens:
-            logger.error("Could not grab screenshot.")
-            return
-
-        for idx, screenshot in enumerate(screens):
-            _save_image_in_tempfolder(screenshot, postfix=f"_raw_screen{idx}")
-            self.screens[idx].screenshot = screenshot
-
-        self.com.on_screenshots_updated.emit()
-
-    def _add_tray_menu(self) -> None:
-        """Create menu for system tray."""
-        menu = QtWidgets.QMenu()
-
-        action = QtGui.QAction("Capture", menu)
-        action.triggered.connect(self.com.on_tray_menu_capture_clicked.emit)
-        menu.addAction(action)
-
-        action = QtGui.QAction("Exit", menu)
-        action.triggered.connect(self.com.on_quit.emit)
-        menu.addAction(action)
-
-        self.setContextMenu(menu)
-
     @QtCore.Slot()
     def _show_windows(self) -> None:
         """Initialize child windows with method depending on system."""
         if not system_info.display_manager_is_wayland():
             for index in range(len(system_info.screens())):
                 self._create_window(index)
 
         elif system_info.desktop_environment() in (
             DesktopEnvironment.GNOME,
             DesktopEnvironment.KDE,
         ):
             self.com.on_window_positioned.connect(self._create_next_window)
             self._create_next_window()
 
-    def _create_next_window(self) -> None:
-        """Open child window only for next display."""
-        if len(system_info.screens()) > len(self.windows):
-            index = len(self.windows.keys())
-            self._create_window(index)
-
-    def _create_window(self, index: int) -> None:
-        """Open a child window for the specified screen."""
-        new_window = Window(screen=self.screens[index], settings=self.settings)
-        new_window.com.on_esc_key_pressed.connect(
-            lambda: self.com.on_close_or_exit.emit("esc button pressed")
-        )
-        new_window.com.on_region_selected.connect(self.com.on_region_selected)
-        new_window.com.on_window_positioned.connect(self.com.on_window_positioned)
-        if index == 0:
-            new_window.ui_layer.setLayout(self._create_menu_button())
-
-        new_window.set_fullscreen()
-        self.windows[index] = new_window
-
-    def _create_menu_button(self) -> QtWidgets.QLayout:
-        # system_info.is_briefcase_package = lambda: True  # LanguageManager debugging
-        settings_menu = MenuButton(
-            settings=self.settings,
-            language_manager=system_info.is_prebuild_package(),
-        )
-        settings_menu.com.on_open_url.connect(self.com.on_open_url_and_hide)
-        settings_menu.com.on_manage_languages.connect(self.com.on_manage_languages)
-        settings_menu.com.on_close_in_settings.connect(
-            lambda: self.com.on_close_or_exit.emit("clicked close in menu")
-        )
-        layout = QtWidgets.QGridLayout()
-        layout.setContentsMargins(26, 26, 26, 26)
-        layout.setRowStretch(1, 1)
-        layout.setColumnStretch(0, 1)
-        layout.addWidget(settings_menu, 0, 1)
-        return layout
-
-    def _update_settings_menu(self, installed_languages: list[str]) -> None:
-        """After Language settings changed, recreate menu button the update menus."""
-        self._sanatize_active_language(self.settings)
-
-        # TODO: Implement clean way to update the menu than delete & recreate
-        menu_layout = self.windows[0].ui_layer.layout()
-        if menu_layout:
-            while menu_layout.count():
-                menu_layout.takeAt(0).widget().deleteLater()
-            menu_layout.deleteLater()
-
-        QtCore.QTimer.singleShot(
-            5, lambda: self.windows[0].ui_layer.setLayout(self._create_menu_button())
-        )
+    @QtCore.Slot(str)
+    def _apply_setting_change(self, setting: str) -> None:
+        if setting == "tray":
+            capture_action = self.contextMenu().findChild(QtGui.QAction, name="capture")
+            if capture_action:
+                capture_action.setVisible(
+                    self.settings.value(setting, False, type=bool)
+                )
 
-    @staticmethod
-    def _sanatize_active_language(settings: QtCore.QSettings) -> None:
+    @QtCore.Slot(list)
+    def _sanatize_language_setting(self, installed_languages: list[str]) -> None:
         """Verify that languages selected in the settings exist.
 
         If one doesn't, remove it. If none does, autoselect the first in list.
         """
-        installed_languages = ocr.utils.get_tesseract_languages(
-            tesseract_cmd=system_info.get_tesseract_path(),
-            tessdata_path=system_info.get_tessdata_path(),
-        )
-
-        active_languages = settings.value("language")
+        active_languages = self.settings.value("language")
         if not isinstance(active_languages, list):
             active_languages = [active_languages]
 
         active_languages = [a for a in active_languages if a in installed_languages]
         if not active_languages:
             active_languages = [installed_languages[0]]
 
-        settings.setValue("language", active_languages)
+        self.settings.setValue("language", active_languages)
 
-    #####################
-    # OCR Functionality #
-    #####################
+    @QtCore.Slot(list)
+    def _update_installed_languages(self, installed_languages: list[str]) -> None:
+        """Update instance attribute to reflect changes.
+
+        the instance attribute is used e.g. to create a menu_button with an up to
+        date language menu.
+        """
+        self.installed_languages = installed_languages
 
     @QtCore.Slot(Rect)
     def _crop_image(self, grab_info: tuple[Rect, int]) -> None:
         """Crop image to selected region."""
         logger.info("Crop image to region %s", grab_info[0].points)
         rect, screen_idx = grab_info
 
@@ -327,86 +197,87 @@
             raise TypeError("Screenshot is None!")
 
         self.capture.mode = CaptureMode[str(self.settings.value("mode")).upper()]
         self.capture.rect = rect
         self.capture.screen = self.screens[screen_idx]
         self.capture.image = screenshot.copy(QtCore.QRect(*rect.geometry))
 
-        _save_image_in_tempfolder(self.capture.image, postfix="_cropped")
+        utils._save_image_in_tempfolder(self.capture.image, postfix="_cropped")
 
         self.com.on_image_cropped.emit()
 
-    @staticmethod
-    def _qimage_to_pil_image(image: QtGui.QImage) -> Image.Image:
-        """Cast QImage to pillow Image type."""
-        ba = QtCore.QByteArray()
-        buffer = QtCore.QBuffer(ba)
-        buffer.open(QtCore.QIODevice.ReadWrite)
-        image.save(buffer, "PNG")  # type:ignore
-        return Image.open(io.BytesIO(buffer.data()))
-
     @QtCore.Slot()
     def _capture_to_ocr(self) -> None:
         """Perform content recognition on grabed image."""
-        if self.capture.image_area < 25:
+        minimum_image_area = 25
+        if self.capture.image_area < minimum_image_area:
             logger.warning("Area of %s too small. Skip OCR", self.capture.image_area)
             self.com.on_close_or_exit.emit("selection too small")
             return
 
         logger.debug("Start OCR")
         language = self.settings.value("language")
         if not isinstance(language, str) and not isinstance(language, Iterable):
             raise TypeError()
         ocr_result = ocr.recognize(
             tesseract_cmd=system_info.get_tesseract_path(),
             languages=language,
-            image=self._qimage_to_pil_image(self.capture.image),
+            image=self.capture.image,
             tessdata_path=system_info.get_tessdata_path(),
             parse=self.capture.mode is CaptureMode.PARSE,
             resize_factor=3.2,
             padding_size=80,
         )
-        _save_image_in_tempfolder(ocr_result.image, postfix="_enhanced")
+        utils._save_image_in_tempfolder(ocr_result.image, postfix="_enhanced")
 
         self.capture.ocr_text = ocr_result.text
         self.capture.ocr_applied_magic = ocr_result.best_scored_magic
 
         logger.info("Text from OCR:\n%s", self.capture.ocr_text)
         self.com.on_ocr_performed.emit()
 
     @QtCore.Slot(str)
     def _open_url_and_hide(self, url: str) -> None:
         """Open url in default browser, then hide to tray or exit."""
         logger.debug("Open %s", url)
-        QtGui.QDesktopServices.openUrl(url)
-        self.com.on_close_or_exit.emit("opened web browser")
+        result = QtGui.QDesktopServices.openUrl(
+            QtCore.QUrl(url, QtCore.QUrl.ParsingMode.TolerantMode)
+        )
+        self.com.on_close_or_exit.emit(f"opened uri with result={result}")
 
     @QtCore.Slot()
     def _open_language_manager(self) -> None:
         """Open url in default browser, then hide to tray or exit."""
         logger.debug("Loading language manager...")
         self.language_window = LanguageManager(
             tessdata_path=system_info.config_directory() / "tessdata",
             parent=self.windows[0],
         )
         self.language_window.com.on_open_url.connect(self._open_url_and_hide)
         self.language_window.com.on_change_installed_languages.connect(
-            self._update_settings_menu
+            self.com.on_languages_changed
         )
         self.language_window.exec_()
 
     @QtCore.Slot()
     def _copy_to_clipboard(self) -> None:
         """Copy results to clipboard."""
         copy_to_clipboard = clipboard.get_copy_func()
         logger.debug("Copy text to clipboard")
         copy_to_clipboard(self.capture.ocr_text)
         self.com.on_copied_to_clipboard.emit()
 
     @QtCore.Slot()
+    def _print_to_stdout(self) -> None:
+        """Print results to stdout ."""
+        logger.debug("Print text to stdout")
+        print(self.capture.ocr_text, file=sys.stdout)  # noqa: T201
+        self._exit_application(reason="printed to stdout")
+
+    @QtCore.Slot()
     def _notify_or_close(self) -> None:
         if self.settings.value("notification", type=bool):
             self.com.on_send_notification.emit(self.capture)
         else:
             self.com.on_close_or_exit.emit("detection completed")
 
     @QtCore.Slot()
@@ -432,16 +303,201 @@
             delayed_exit = partial(
                 self._exit_application, reason="notification sent delaying exit"
             )
             QtCore.QTimer.singleShot(5000, delayed_exit)
         else:
             self._exit_application(reason)
 
+    def _delayed_init(self) -> None:
+        self.installed_languages = ocr.tesseract.get_languages(
+            tesseract_cmd=system_info.get_tesseract_path(),
+            tessdata_path=system_info.get_tessdata_path(),
+        )
+        self.com.on_languages_changed.emit(self.installed_languages)
+        self._add_update_checker()
+        self._add_notifier()
+        self._set_tray_icon()
+
+    def _set_tray_icon(self) -> None:
+        self.setIcon(QtGui.QIcon.fromTheme("tool-magic-symbolic", QtGui.QIcon(":tray")))
+
+    def _create_socket_server(self) -> None:
+        """Open socket server to listen for other NormCap instances."""
+        if self._socket_out:
+            self._socket_out.close()
+            self._socket_out = None
+        QtNetwork.QLocalServer().removeServer(self._socket_name)
+        self._socket_server = QtNetwork.QLocalServer(self)
+        self._socket_server.newConnection.connect(self._on_new_connection)
+        self._socket_server.listen(self._socket_name)
+        logger.debug("Listen on local socket %s.", self._socket_server.serverName())
+
+    def _ensure_screenshot_permission(self) -> None:
+        if screengrab.has_screenshot_permission():
+            return
+
+        if sys.platform == "darwin":
+            # Reset privacy permission in case of new NormCap version. This is necessary
+            # because somehow the setting is associated with the binary and won't work
+            # after it got updated.
+            if self.settings.value("version") != __version__:
+                self.settings.setValue("version", __version__)
+                screengrab.macos_reset_screenshot_permission()
+
+            # Trigger permission request to make the NormCap entry available in settings
+            screengrab.macos_request_screenshot_permission()
+
+            # Message box to explain what's happening and open the preferences
+            app = "NormCap" if system_info.is_prebuild_package() else "Terminal"
+            button = QtWidgets.QMessageBox.critical(
+                None,
+                "Error!",
+                (
+                    f"{app} is missing permissions for 'Screen Recording'.\n\n"
+                    "Grant the permissions via 'Privacy & Security' settings "
+                    "and restart NormCap.\n\nClick OK to exit."
+                ),
+                buttons=QtWidgets.QMessageBox.Open | QtWidgets.QMessageBox.Cancel,
+            )
+            if button == QtWidgets.QMessageBox.Open:
+                logger.debug("Open macOS privacy settings")
+                screengrab.macos_open_privacy_settings()
+
+            self._exit_application("Screen Recording permissions missing on macOS")
+
+    def _set_signals(self) -> None:
+        """Set up signals to trigger program logic."""
+        self.activated.connect(self._handle_tray_click)
+        self.com.on_tray_menu_capture_clicked.connect(self._update_screenshots)
+        self.com.on_screenshots_updated.connect(self._show_windows)
+        self.com.on_quit.connect(lambda: self._exit_application("clicked exit in tray"))
+        self.com.on_region_selected.connect(self._close_windows)
+        self.com.on_region_selected.connect(self._crop_image)
+        self.com.on_image_cropped.connect(self._capture_to_ocr)
+        self.com.on_ocr_performed.connect(
+            self._print_to_stdout if self.cli_mode else self._copy_to_clipboard
+        )
+        self.com.on_copied_to_clipboard.connect(self._notify_or_close)
+        self.com.on_copied_to_clipboard.connect(self._color_tray_icon)
+        self.com.on_close_or_exit.connect(self._close_or_exit)
+        self.com.on_open_url_and_hide.connect(self._open_url_and_hide)
+        self.com.on_manage_languages.connect(self._open_language_manager)
+        self.com.on_languages_changed.connect(self._sanatize_language_setting)
+        self.com.on_languages_changed.connect(self._update_installed_languages)
+
+    def _add_update_checker(self) -> None:
+        if not self.settings.value("update", type=bool):
+            return
+
+        now_sub_interval_sec = time.time() - (60 * 60 * 24 * UPDATE_CHECK_INTERVAL_DAYS)
+        now_sub_interval = time.strftime("%Y-%m-%d", time.gmtime(now_sub_interval_sec))
+        if str(self.settings.value("last-update-check", type=str)) > now_sub_interval:
+            return
+
+        checker = UpdateChecker(self, packaged=system_info.is_prebuild_package())
+        checker.com.on_version_checked.connect(self._update_time_of_last_update_check)
+        checker.com.on_click_get_new_version.connect(self.com.on_open_url_and_hide)
+        QtCore.QTimer.singleShot(500, checker.check)
+
+    def _update_time_of_last_update_check(self, newest_version: str) -> None:
+        if newest_version is not None:
+            today = time.strftime("%Y-%m-%d", time.gmtime())
+            self.settings.setValue("last-update-check", today)
+
+    def _add_notifier(self) -> None:
+        self.notifier = Notifier(self)
+        self.com.on_send_notification.connect(self.notifier.send_notification)
+        self.notifier.com.on_notification_sent.connect(
+            lambda: self.com.on_close_or_exit.emit("notification sent")
+        )
+
+    def _update_screenshots(self, delayed: bool = True) -> None:
+        """Get new screenshots and cache them."""
+        if delayed:
+            time.sleep(0.15)
+
+        capture = screengrab.get_capture_func()
+        screens = capture()
+
+        if not screens:
+            logger.error("Could not grab screenshot.")
+            return
+
+        for idx, screenshot in enumerate(screens):
+            utils._save_image_in_tempfolder(screenshot, postfix=f"_raw_screen{idx}")
+            self.screens[idx].screenshot = screenshot
+
+        self.com.on_screenshots_updated.emit()
+
+    @QtCore.Slot()
+    def _populate_context_menu_entries(self) -> None:
+        """Create menu for system tray."""
+        menu = self.contextMenu()
+        menu.clear()
+
+        if bool(self.settings.value("tray", False, type=bool)):
+            action = QtGui.QAction("Capture", menu)
+            action.setObjectName("capture")
+            action.triggered.connect(self.com.on_tray_menu_capture_clicked.emit)
+            menu.addAction(action)
+
+        action = QtGui.QAction("Exit", menu)
+        action.triggered.connect(self.com.on_quit.emit)
+        menu.addAction(action)
+
+    def _create_next_window(self) -> None:
+        """Open child window only for next display."""
+        if len(system_info.screens()) > len(self.windows):
+            index = len(self.windows.keys())
+            self._create_window(index)
+
+    def _create_window(self, index: int) -> None:
+        """Open a child window for the specified screen."""
+        new_window = Window(screen=self.screens[index], settings=self.settings)
+        new_window.com.on_esc_key_pressed.connect(
+            lambda: self.com.on_close_or_exit.emit("esc button pressed")
+        )
+        new_window.com.on_region_selected.connect(self.com.on_region_selected)
+        new_window.com.on_window_positioned.connect(self.com.on_window_positioned)
+        if index == 0:
+            new_window.ui_layer.setLayout(self._create_menu_button())
+
+        new_window.set_fullscreen()
+        self.windows[index] = new_window
+
+    def _create_menu_button(self) -> QtWidgets.QLayout:
+        if self._debug_language_manager:
+            system_info.is_briefcase_package = lambda: True
+        settings_menu = MenuButton(
+            settings=self.settings,
+            language_manager=system_info.is_prebuild_package(),
+            installed_languages=self.installed_languages,
+        )
+        settings_menu.com.on_open_url.connect(self.com.on_open_url_and_hide)
+        settings_menu.com.on_manage_languages.connect(self.com.on_manage_languages)
+        settings_menu.com.on_setting_change.connect(self._apply_setting_change)
+        settings_menu.com.on_close_in_settings.connect(
+            lambda: self.com.on_close_or_exit.emit("clicked close in menu")
+        )
+        self.com.on_languages_changed.connect(settings_menu.on_languages_changed)
+        layout = QtWidgets.QGridLayout()
+        layout.setContentsMargins(26, 26, 26, 26)
+        layout.setRowStretch(1, 1)
+        layout.setColumnStretch(0, 1)
+        layout.addWidget(settings_menu, 0, 1)
+        return layout
+
     def _exit_application(self, reason: str) -> NoReturn:
         self.hide()
+        if self._socket_server:
+            self._socket_server.close()
+            self._socket_server.removeServer(self._socket_name)
+
         QtWidgets.QApplication.processEvents()
         time.sleep(0.05)
         logger.info("Exit normcap (%s)", reason)
-        logger.debug("Debug images saved in %s%snormcap", tempfile.gettempdir(), os.sep)
+        logger.debug(
+            "Debug images saved in %s%snormcap", utils.tempfile.gettempdir(), os.sep
+        )
         # The preferable QApplication.quit() doesn't work reliably on macOS. E.g. when
         # right clicking on "close" in tray menu, NormCap process keeps running.
         sys.exit(0)
```

### Comparing `normcap-0.4.0/normcap/gui/window.py` & `normcap-0.4.1/normcap/gui/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Normcap base window.
 
 Inherited for the main window, instantiated for the child windows (which get created
 in multi display setups).
 """
 
 import logging
-import os
 import tempfile
+from pathlib import Path
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
 from normcap.gui import system_info
 from normcap.gui.models import CaptureMode, DesktopEnvironment, Rect, Screen
 from normcap.gui.settings import Settings
 
@@ -103,15 +103,15 @@
         y = shell_interface.call("start")
         if x.errorName() or y.errorName():
             logger.error("Failed move Window!")
             logger.error(x.errorMessage(), y.errorMessage())
     else:
         logger.warning("Invalid dbus interface on KDE")
 
-    os.unlink(script_file.name)
+    Path(script_file.name).unlink()
 
 
 class Communicate(QtCore.QObject):
     """Window's communication bus."""
 
     on_esc_key_pressed = QtCore.Signal()
     on_region_selected = QtCore.Signal(Rect)
```

### Comparing `normcap-0.4.0/normcap/ocr/magics/email_magic.py` & `normcap-0.4.1/normcap/ocr/magics/email_magic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 """Magic Class to handle e-mail adresses contained in the text."""
 
+import functools
 import logging
 import re
 
 from normcap.ocr.magics.base_magic import BaseMagic
 from normcap.ocr.models import OcrResult
 
 logger = logging.getLogger(__name__)
 
 
 class EmailMagic(BaseMagic):
     """Detect and extract email adress(es) in the OCR results."""
 
-    _emails: list[str] = []
+    @staticmethod
+    @functools.cache
+    def _extract_emails(text: str) -> list[str]:
+        reg_email = r"[a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9._-]+"
+        return re.findall(reg_email, text)
 
     def score(self, ocr_result: OcrResult) -> float:
         """Calc score based on chars in email adresses vs. overall chars.
 
         Arguments:
-            BaseMagic {class} -- Base class for magics
-            capture {Capture} -- NormCap's session data
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            float -- score between 0-100 (100 = more likely)
+        Returns:
+            score between 0-100 (100 = more likely).
         """
-        # Get concatenated lines
         text = ocr_result.text
-
-        # Search email addresses in line
-        reg_email = r"[a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9._-]+"
-        self._emails = re.findall(reg_email, text)
-
+        emails = self._extract_emails(text)
         logger.info(
-            "%s emails found %s",
-            len(self._emails),
-            [": " + " ".join(self._emails) if self._emails else ""],
+            "%s emails found %s", len(emails), f": {' '.join(emails)}" if emails else ""
         )
 
         # Calc chars & ratio
-        email_chars = sum(len(e) for e in self._emails)
-        all_chars = max([len(text), 1])
-        ratio = email_chars / (all_chars * 0.75)
-
-        logger.debug("%s/%s (%s) chars in emails", email_chars, all_chars, ratio)
+        email_chars = sum(len(e) for e in emails)
+        count_chars = ocr_result.num_chars
+        ratio = min(email_chars / count_chars, 1) if count_chars else 0
+        logger.debug("%s/%s (%s) chars in emails", email_chars, count_chars, ratio)
         return round(100 * ratio, 2)
 
     def transform(self, ocr_result: OcrResult) -> str:
         """Transform to comma separated string of email adresses.
 
         Other chars not contained in email adresses are discarded.
 
         Arguments:
-            capture {Capture} -- NormCap's session data
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            str -- comma separated email adresses
+        Returns:
+            Comma separated email adresses.
         """
         logger.info("Transform with Email magic")
-        return ", ".join(self._emails)
+        return ", ".join(self._extract_emails(ocr_result.text))
```

### Comparing `normcap-0.4.0/normcap/ocr/magics/magic.py` & `normcap-0.4.1/normcap/ocr/magics/magic.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,38 +13,32 @@
 
 
 class Magic:
     """Load available magics, scores, and trigger magic with highest score.
 
     Arguments:
         AbstractHandler {[type]} -- [description]
-
-    Returns
-    -------
-        [type] -- [description]
     """
 
     _magics = {
         "SingleLineMagic": SingleLineMagic(),
         "MultiLineMagic": MultiLineMagic(),
         "ParagraphMagic": ParagraphMagic(),
         "EmailMagic": EmailMagic(),
         "UrlMagic": UrlMagic(),
     }
 
     def apply(self, ocr_result: OcrResult) -> OcrResult:
         """Load magics, calculate score, execture magic with highest score.
 
-        Arguments:
-            AbstractHandler {class} -- self
-            capture {Capture} -- NormCap's session data
+        Args:
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            Capture -- Enriched NormCap's session data
+        Returns:
+            Enriched NormCap's session data.
         """
         # Get score per magic
         ocr_result.magic_scores = self._calc_scores(ocr_result)
 
         # Transform with best magic
         if best_magic_name := ocr_result.best_scored_magic:
             best_magic = self._magics[best_magic_name]
@@ -53,26 +47,25 @@
         ocr_result.parsed = self._post_process(ocr_result)
         return ocr_result
 
     @staticmethod
     def _post_process(ocr_result: OcrResult) -> str:
         """Apply postprocessing to transformed output."""
         transformed = ocr_result.parsed
-        # TODO: Check tesseract issue if whitespace workaround still necessary:
+        # ONHOLD: Check tesseract issue if whitespace workaround still necessary:
         # https://github.com/tesseract-ocr/tesseract/issues/2702
         if ocr_result.tess_args.is_language_without_spaces():
             transformed = transformed.replace(" ", "")
         return transformed
 
     def _calc_scores(self, ocr_result: OcrResult) -> dict[str, float]:
         """Calculate score for every loaded magic.
 
         Arguments:
-            capture {Capture} -- NormCap's session data
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            dict -- Scores in format {<magic Name>: <score>}
+        Returns:
+            Scores in format {<magic Name>: <score>}.
         """
         scores = {name: magic.score(ocr_result) for name, magic in self._magics.items()}
         logger.debug("Magic scores:\n%s", scores)
         return scores
```

### Comparing `normcap-0.4.0/normcap/ocr/magics/multi_line_magic.py` & `normcap-0.4.1/normcap/ocr/magics/multi_line_magic.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,33 +8,30 @@
     """Format multi line text."""
 
     def score(self, ocr_result: OcrResult) -> float:
         # sourcery skip: assign-if-exp, inline-immediately-returned-variable
         """Calc score based on amount of lines and breaks.
 
         Arguments:
-            BaseMagic {class} -- Base class for magics
-            capture {Capture} -- NormCap's session data
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            float -- score between 0-100 (100 = more likely)
+        Returns:
+            Score between 0-100 (100 = more likely)
         """
         if (ocr_result.num_lines > 1) and (
             ocr_result.num_blocks == ocr_result.num_pars == 1
         ):
             return 50.0
 
         return 0
 
     def transform(self, ocr_result: OcrResult) -> str:
         """Just transform into multiple lines of text.
 
-        Arguments:
-            capture {Capture} -- NormCap's session data
+        Args:
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            str -- Lines of text
+        Returns:
+            Lines of text.
         """
         # Just return concatenated text
         return ocr_result.lines
```

### Comparing `normcap-0.4.0/normcap/ocr/magics/paragraph_magic.py` & `normcap-0.4.1/normcap/ocr/magics/paragraph_magic.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,31 @@
 
 class ParagraphMagic(BaseMagic):
     """Detect and extract plain text formatted in paragraphs."""
 
     def score(self, ocr_result: OcrResult) -> float:
         """Calc score based on layout of amount of paragraphs and blocks.
 
-        Arguments:
-            BaseMagic {class} -- Base class for magics
-            capture {Capture} -- NormCap's session data
-
-        Returns
-        -------
-            float -- score between 0-100 (100 = more likely)
+        Arg:
+            ocr_result: Recognized text and meta information.
+
+        Returns:
+            Score between 0-100 (100 = more likely).
         """
         breaks = ocr_result.num_blocks + ocr_result.num_pars - 1
         return 100 - (100 / (breaks))
 
     def transform(self, ocr_result: OcrResult) -> str:
         """Transform wordboxes into nicely formatted paragraphs.
 
-        Arguments:
-            capture {Capture} -- NormCap's session data
+        Args:
+            ocr_result: Recognized text and meta information.
 
-        Returns
-        -------
-            str -- Transformed text
+        Returns:
+            Transformed text.
         """
         result = ""
         current_par_num = 1
         current_block_num = 1
         for word in ocr_result.words:
             breaks = 0
             if word["par_num"] != current_par_num:
```

### Comparing `normcap-0.4.0/normcap/ocr/models.py` & `normcap-0.4.1/normcap/ocr/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,70 @@
 import os
 from dataclasses import dataclass, field
 from enum import IntEnum
 from os import PathLike
 from typing import Optional
 
-from PIL import Image
+from PySide6.QtGui import QImage
+
+
+class PSM(IntEnum):
+    """Available tesseract mode options."""
+
+    OSD_ONLY = 0  # Orientation and script detection (OSD) only.
+    AUTO_OSD = 1  # Automatic page segmentation with orientation & script detection.
+    AUTO_ONLY = 2  # Automatic page segmentation, but no OSD, or OCR.
+    AUTO = 3  # Fully automatic page segmentation, but no OSD. (`tesserocr` default)
+    SINGLE_COLUMN = 4  # Assume a single column of text of variable sizes.
+    SINGLE_BLOCK_VERT_TEXT = 5  # Assume a  uniform block of vertically aligned text.
+    SINGLE_BLOCK = 6  # Assume a single uniform block of text.
+    SINGLE_LINE = 7  # Treat the image as a single text line.
+    SINGLE_WORD = 8  # Treat the image as a single word.
+    CIRCLE_WORD = 9  # Treat the image as a single word in a circle.
+    SINGLE_CHAR = 10  # Treat the image as a single character.
+    SPARSE_TEXT = 11  # Find as much text as possible in no particular order.
+    SPARSE_TEXT_OSD = 12  # Sparse text with orientation and script det.
+    RAW_LINE = 13  # Treat the image as a single text line, bypassing Tesseract hacks.
+    COUNT = 14  # Number of enum entries.
+
+
+class OEM(IntEnum):
+    """Available tesseract model options."""
+
+    TESSERACT_ONLY = 0  # Run Tesseract only - fastest
+    LSTM_ONLY = 1  # Run just the LSTM line recognizer. (>=v4.00)
+    TESSERACT_LSTM_COMBINED = 2  # Run the LSTM recognizer, but allow fallback
+    # to Tesseract when things get difficult. (>=v4.00)
+    DEFAULT = 3  # Run both and combine results - best accuracy.
 
 
 @dataclass
 class TessArgs:
     """Arguments used when envoking tesseract."""
 
-    path: Optional[PathLike]
+    tessdata_path: Optional[PathLike]
     lang: str
-    oem: int
-    psm: int
-    version: str
-
-    def to_config_str(self) -> str:
-        """Generate command line args for pytesseract/tesseract.
-
-        The language is ommited, as pytesseract takes an extra argument for that.
-        """
-        config_str = f"--oem {self.oem} --psm {self.psm}"
-        if self.path:
-            config_str += f' --tessdata-dir "{self.path}"'
+    oem: OEM
+    psm: PSM
+
+    def as_list(self) -> list[str]:
+        """Generate command line args for tesseract."""
+        arg_list = [
+            "-l",
+            self.lang,
+            "--oem",
+            str(self.oem.value),
+            "--psm",
+            str(self.psm.value),
+        ]
+        if self.tessdata_path:
+            arg_list.extend(["--tessdata-dir", str(self.tessdata_path)])
         if self.is_language_without_spaces():
-            config_str += " -c preserve_interword_spaces=1"
-        return config_str
+            arg_list.extend(["-c", "preserve_interword_spaces=1"])
+        return arg_list
 
     def is_language_without_spaces(self) -> bool:
         """Check if selected languages are only languages w/o spaces between words."""
         languages_without_spaces = {
             "chi_sim",
             "chi_sim_vert",
             "chi_tra",
@@ -46,15 +79,15 @@
 
 @dataclass
 class OcrResult:
     """Encapsulate recognized text and meta information."""
 
     tess_args: TessArgs
     words: list[dict]  # Words+metadata detected by OCR
-    image: Image.Image
+    image: QImage
     magic_scores: dict[str, float] = field(default_factory=dict)  # magics with scores
     parsed: str = ""  # Transformed result
 
     def _count_unique_sections(self, level: str) -> int:
         postfix = "_num"
         unique_sections = {w[level + postfix] for w in self.words}
         return len(unique_sections)
@@ -91,50 +124,25 @@
             else:
                 all_lines[-1] += f' {word["text"]}'
 
         all_lines = list(filter(None, all_lines))  # Remove empty
         return os.linesep.join(all_lines)
 
     @property
+    def num_chars(self) -> int:
+        """Provide number of chars without word separators."""
+        return sum(len(w["text"]) for w in self.words)
+
+    @property
     def num_lines(self) -> int:
         """Provide number of lines in OCR text."""
         return self._count_unique_sections("line")
 
     @property
     def num_pars(self) -> int:
         """Provide number of paragraphs in OCR text."""
         return self._count_unique_sections("par")
 
     @property
     def num_blocks(self) -> int:
         """Provide number of text blocks in OCR text."""
         return self._count_unique_sections("block")
-
-
-class PSM(IntEnum):
-    """Available tesseract mode options."""
-
-    OSD_ONLY = 0  # Orientation and script detection (OSD) only.
-    AUTO_OSD = 1  # Automatic page segmentation with orientation & script detection.
-    AUTO_ONLY = 2  # Automatic page segmentation, but no OSD, or OCR.
-    AUTO = 3  # Fully automatic page segmentation, but no OSD. (`tesserocr` default)
-    SINGLE_COLUMN = 4  # Assume a single column of text of variable sizes.
-    SINGLE_BLOCK_VERT_TEXT = 5  # Assume a  uniform block of vertically aligned text.
-    SINGLE_BLOCK = 6  # Assume a single uniform block of text.
-    SINGLE_LINE = 7  # Treat the image as a single text line.
-    SINGLE_WORD = 8  # Treat the image as a single word.
-    CIRCLE_WORD = 9  # Treat the image as a single word in a circle.
-    SINGLE_CHAR = 10  # Treat the image as a single character.
-    SPARSE_TEXT = 11  # Find as much text as possible in no particular order.
-    SPARSE_TEXT_OSD = 12  # Sparse text with orientation and script det.
-    RAW_LINE = 13  # Treat the image as a single text line, bypassing Tesseract hacks.
-    COUNT = 14  # Number of enum entries.
-
-
-class OEM(IntEnum):
-    """Available tesseract model options."""
-
-    TESSERACT_ONLY = 0  # Run Tesseract only - fastest
-    LSTM_ONLY = 1  # Run just the LSTM line recognizer. (>=v4.00)
-    TESSERACT_LSTM_COMBINED = 2  # Run the LSTM recognizer, but allow fallback
-    # to Tesseract when things get difficult. (>=v4.00)
-    DEFAULT = 3  # Run both and combine results - best accuracy.
```

### Comparing `normcap-0.4.0/normcap/ocr/recognize.py` & `normcap-0.4.1/normcap/ocr/recognize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,50 @@
 """Detect OCR tool & language and perform OCR on selected part of image."""
 
 import logging
+from collections.abc import Iterable
 from os import PathLike
-from typing import Iterable, Optional, Union
+from typing import Optional, Union
 
-from PIL import Image
-from pytesseract import pytesseract
+from PySide6.QtGui import QImage
 
-from normcap.ocr import enhance, utils
+from normcap.ocr import enhance, tesseract
 from normcap.ocr.magics import Magic
 from normcap.ocr.models import OEM, PSM, OcrResult, TessArgs
 
 logger = logging.getLogger(__name__)
 
 
-def recognize(
+def recognize(  # noqa: PLR0913
     tesseract_cmd: PathLike,
     languages: Union[str, Iterable[str]],
-    image: Image.Image,
+    image: QImage,
     tessdata_path: Optional[PathLike] = None,
     parse: bool = True,
     resize_factor: Optional[float] = None,
     padding_size: Optional[int] = None,
 ) -> OcrResult:
     """Apply OCR on selected image section."""
     image = enhance.preprocess(image, resize_factor=resize_factor, padding=padding_size)
 
     tess_args = TessArgs(
-        path=tessdata_path,
+        tessdata_path=tessdata_path,
         lang=languages if isinstance(languages, str) else "+".join(languages),
         oem=OEM.DEFAULT,
         psm=PSM.AUTO_OSD,
-        version=utils.get_tesseract_version(tesseract_cmd),  # type: ignore
-        # For the type ignore, see: https://github.com/python/mypy/issues/5107
     )
     logger.debug(
-        "Run Tesseract on image of size %s with args:\n%s", image.size, tess_args
+        "Run Tesseract on image of size %s with args:\n%s",
+        image.size().toTuple(),
+        tess_args,
     )
-
-    pytesseract.tesseract_cmd = str(tesseract_cmd)
-    tsv_data = pytesseract.image_to_data(
-        image,
-        lang=tess_args.lang,
-        output_type=pytesseract.Output.DICT,
-        timeout=30,
-        config=tess_args.to_config_str(),
-    )
-
-    result = OcrResult(
-        tess_args=tess_args, words=utils.tsv_to_list_of_dicts(tsv_data), image=image
+    ocr_result_data = tesseract.perform_ocr(
+        cmd=tesseract_cmd, image=image, args=tess_args.as_list()
     )
+    result = OcrResult(tess_args=tess_args, words=ocr_result_data, image=image)
     logger.debug("OCR result:\n%s", result)
 
     if parse:
         result = Magic().apply(result)
         logger.debug("Parsed text:\n%s", result.parsed)
 
     return result
```

### Comparing `normcap-0.4.0/normcap/resources/icons/normcap.png` & `normcap-0.4.1/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/normcap.svg` & `normcap-0.4.1/normcap/resources/icons/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/notification.png` & `normcap-0.4.1/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/notification.svg` & `normcap-0.4.1/normcap/resources/icons/notification.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/parse.png` & `normcap-0.4.1/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/parse.svg` & `normcap-0.4.1/normcap/resources/icons/parse.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/raw.png` & `normcap-0.4.1/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/raw.svg` & `normcap-0.4.1/normcap/resources/icons/raw.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/resources.qrc` & `normcap-0.4.1/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/settings.png` & `normcap-0.4.1/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/settings.svg` & `normcap-0.4.1/normcap/resources/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/tray.png` & `normcap-0.4.1/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/icons/tray.svg` & `normcap-0.4.1/normcap/resources/icons/tray.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.4.1/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/resources/tessdata/README.txt` & `normcap-0.4.1/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/screengrab/__init__.py` & `normcap-0.4.1/normcap/screengrab/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,29 @@
     import PySide6
 
     version_tuple = PySide6.__version__.split(".")
     return version_tuple[0] >= "6" and version_tuple[1] >= "4"
 
 
 def get_capture_func() -> Callable:
-
     # fmt: off
     if sys.platform != "linux" or not utils.has_wayland_display_manager():
         logger.debug("Select capture method QT")
         from normcap.screengrab import qt
         return qt.capture
 
     if utils.has_dbus_portal_support():
         if _is_pyside6_64plus():
             logger.debug("Select capture method DBUS portal")
             from normcap.screengrab import dbus_portal
             return dbus_portal.capture
-        else:
-            logger.debug("Select capture method DBUS portal legacy")
-            from normcap.screengrab import dbus_portal_legacy
-            return dbus_portal_legacy.capture
+
+        logger.debug("Select capture method DBUS portal legacy")
+        from normcap.screengrab import dbus_portal_legacy
+        return dbus_portal_legacy.capture
 
     logger.debug("Select capture method DBUS shell")
     from normcap.screengrab import dbus_shell
 
     return dbus_shell.capture
     # fmt: on
```

### Comparing `normcap-0.4.0/normcap/screengrab/dbus_portal.py` & `normcap-0.4.1/normcap/screengrab/dbus_portal.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 logger = logging.getLogger(__name__)
 
 TIMEOUT_SECONDS = 7
 
 
 class OrgFreedesktopPortalRequestInterface(QtDBus.QDBusAbstractInterface):
-
     Response = QtCore.Signal(QtDBus.QDBusMessage)
 
     def __init__(
         self, path: str, connection: QtDBus.QDBusConnection, parent: QtCore.QObject
     ) -> None:
         super().__init__(
             "org.freedesktop.portal.Desktop",
@@ -48,16 +47,16 @@
         self.timeout_timer = self._get_timeout_timer(timeout_sec)
 
     def grab_full_desktop(self) -> None:
         bus = QtDBus.QDBusConnection.sessionBus()
 
         base = bus.baseService()[1:].replace(".", "_")
 
-        pseudo_unique_str = "".join(random.choice("abcdefghijklmnop") for _ in range(8))
-        token = f"normcap_{pseudo_unique_str}"
+        random_str = "".join(random.choice("abcdefghi") for _ in range(8))  # noqa: S311
+        token = f"normcap_{random_str}"
         object_path = f"/org/freedesktop/portal/desktop/request/{base}/{token}"
 
         request = OrgFreedesktopPortalRequestInterface(object_path, bus, self)
         request.Response.connect(self.got_signal)
 
         interface = QtDBus.QDBusInterface(
             "org.freedesktop.portal.Desktop",
@@ -101,23 +100,24 @@
             msg = f"Error code {code} received from xdg-portal!"
             logger.error(msg)
             self.on_exception.emit(ScreenshotResponseError(msg))
 
         logger.debug("Parse response")
         uri = str(message).split('[Variant(QString): "')[1]
         uri = uri.split('"]}')[0]
-        # TODO: Parse from arguments instead?
+        # ONHOLD: Extracting DBusArgument as below should work, but it doesn't.
+        # _, arg = message.arguments()
+        # QtDBus.QDBusMessage()
         # arg.beginArray()
         # while not arg.atEnd():
         #     arg.beginMap()
         #     while not arg.atEnd():
         #         arg.beginMapEntry()
         #         key = arg.asVariant()
         #         value = arg.asVariant()
-        #         # v = value.variant()
         #         arg.endMapEntry()
         #     arg.endMap()
         # arg.endArray()
         self.on_response.emit(uri)
 
 
 def _synchronized_capture(interactive: bool) -> list[QtGui.QImage]:
```

### Comparing `normcap-0.4.0/normcap/screengrab/dbus_portal_legacy.py` & `normcap-0.4.1/normcap/screengrab/dbus_portal_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Capture screenshots for all screens using org.freedesktop.portal.Desktop.
 
 Legacy version using jeepney.
 
-# FIXME: Not working with Gnome 43 in FlatPak (If new version doesnt work their, either)
-# TODO: Remove legacy dbus portal module once it is deprecated. Check in 2023-05-01.
+# FIXME: Not working with Gnome 43 in FlatPak (If new version doesnt work there, too)
+# ONHOLD: Remove legacy dbus portal module once it is deprecated. Check in 2023-05-01.
 
 AppImage related dependency chain necessary to be resolved before removal:
 
 - PySide6 v6.1+
   Currently, only v6.2 can be installed, in which the new implementatio (dbus_portal.py)
   doesn't receive any response for unknown reasons.
 
 - glibc 2.28+
   PySide6 packaging got changed between 6.2 and 6.4 to actually check for glibc2.28+.
   As this is not present on Ubuntu 16.04 AppImage, PySide6 v6.4+ won't install.
   Sidenote: the missing glibc 2.28+ probably also is the reason for some failures on old
   host distributions and during the appimage.github.io checks.
-  TODO: Let's retry appimage.github.io submission
+  ONHOLD: Let's retry appimage.github.io submission
   Details see https://lists.qt-project.org/pipermail/pyside/2022-December/003253.html
 
 - Briefcase support image on Ubuntu 18.04.6 LTS
   This versions ships with the Glib required. The current minimal required version for
   AppImages (16.04) should be retired around April 2023 https://wiki.ubuntu.com/Releases
 """
 
@@ -61,16 +61,16 @@
 
 
 def grab_full_desktop() -> Optional[QtGui.QImage]:
     """Capture rect of screen on gnome systems using wayland."""
     image = None
     try:
         connection = open_dbus_connection(bus="SESSION")
-        pseudo_unique_str = "".join(random.choice("abcdefghijklmnop") for _ in range(8))
-        token = f"normcap_{pseudo_unique_str}"
+        random_str = "".join(random.choice("abcdefghi") for _ in range(8))  # noqa: S311
+        token = f"normcap_{random_str}"
         sender_name = connection.unique_name[1:].replace(".", "_")
         handle = f"/org/freedesktop/portal/desktop/request/{sender_name}/{token}"
 
         response_rule = MatchRule(
             type="signal", interface="org.freedesktop.portal.Request", path=handle
         )
         Proxy(message_bus, connection).AddMatch(response_rule)
```

### Comparing `normcap-0.4.0/normcap/screengrab/dbus_shell.py` & `normcap-0.4.1/normcap/screengrab/dbus_shell.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.0/normcap/screengrab/utils.py` & `normcap-0.4.1/normcap/screengrab/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,57 +47,58 @@
     if sys.platform != "linux":
         return False
     xdg_session_type = os.environ.get("XDG_SESSION_TYPE", "").lower()
     wayland_display = os.environ.get("WAYLAND_DISPLAY", "").lower()
     return "wayland" in wayland_display or "wayland" in xdg_session_type
 
 
-@functools.lru_cache
+@functools.cache
 def get_gnome_version() -> Optional[str]:
     """Get gnome-shell version (Linux, Gnome)."""
     if sys.platform != "linux":
         return None
 
     if (
-        os.environ.get("GNOME_DESKTOP_SESSION_ID", "") == ""
+        not os.environ.get("GNOME_DESKTOP_SESSION_ID", "")
         and "gnome" not in os.environ.get("XDG_CURRENT_DESKTOP", "").lower()
     ):
         return None
 
     if not shutil.which("gnome-shell"):
         return None
 
     try:
-        output_raw = subprocess.check_output(["gnome-shell", "--version"], shell=False)
-        output = output_raw.decode().strip()
-        if result := re.search(r"\s+([\d.]+)", output):
+        output = subprocess.check_output(
+            ["gnome-shell", "--version"], shell=False, text=True  # noqa: S607, S603
+        )
+        if result := re.search(r"\s+([\d.]+)", output.strip()):
             gnome_version = result.groups()[0]
     except Exception as e:
         logger.warning("Exception when trying to get gnome version from cli %s", e)
         return None
     else:
         logger.debug("Detected Gnome Version: %s", gnome_version)
         return gnome_version
 
 
 def has_dbus_portal_support() -> bool:
-    if gnome_version := get_gnome_version():
-        if gnome_version < "41":
-            return False
+    gnome_version = get_gnome_version()
+    if gnome_version and gnome_version < "41":
+        return False
     return True
 
 
 def macos_reset_screenshot_permission() -> None:
     """Use tccutil to reset permissions for current application."""
     logger.info("Reset screen recording permissions for eu.dynobo.normcap")
     cmd = ["tccutil", "reset", "ScreenCapture", "eu.dynobo.normcap"]
     try:
         completed_proc = subprocess.run(
             cmd,
-            shell=False,
+            shell=False,  # noqa: S603
             encoding="utf-8",
             check=False,
             timeout=10,
         )
         if completed_proc.returncode != 0:
             logger.error(
                 "Failed resetting screen recording permissions: %s %s",
@@ -117,16 +118,15 @@
         return True
     raise RuntimeError("Unknown platform")
 
 
 def _macos_has_screenshot_permission() -> bool:
     """Use CoreGraphics to check if application has screen recording permissions.
 
-    Returns
-    -------
+    Returns:
         True if permissions are available or can't be detected.
     """
     try:
         core_graphics = ctypes.util.find_library("CoreGraphics")
         if not core_graphics:
             raise RuntimeError("Couldn't load CoreGraphics")
         cg = ctypes.cdll.LoadLibrary(core_graphics)
@@ -150,20 +150,20 @@
     except Exception as e:
         logger.warning("Couldn't request screen recording permission: %s", e)
 
 
 def macos_open_privacy_settings() -> None:
     link_to_preferences = (
         "x-apple.systempreferences:com.apple.preference.security"
-        + "?Privacy_ScreenCapture"
+        "?Privacy_ScreenCapture"
     )
     try:
         if sys.platform != "darwin":
             raise RuntimeError(f"Tried opening macOS settings on {sys.platform}")
         subprocess.run(
-            ["open", link_to_preferences],
-            shell=False,
+            ["open", link_to_preferences],  # noqa: S607
+            shell=False,  # noqa: S603
             check=True,
             timeout=30,
         )
     except Exception as e:
         logger.error("Couldn't open privacy settings: %s", e)
```

### Comparing `normcap-0.4.0/normcap/utils.py` & `normcap-0.4.1/normcap/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 logger = logging.getLogger("normcap")
 
 
 _ISSUES_URLS = "https://github.com/dynobo/normcap/issues"
 _XCB_ERROR_URL = (
     "https://github.com/dynobo/normcap/blob/main/FAQ.md"
-    + "#linux-could-not-load-the-qt-platform-plugin-xcb",
+    "#linux-could-not-load-the-qt-platform-plugin-xcb",
 )
 
 
 def create_argparser() -> argparse.ArgumentParser:
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         prog="normcap",
@@ -61,40 +61,43 @@
         help="Set level of detail for console output (default: %(default)s)",
     )
     parser.add_argument(
         "--version",
         action="store_true",
         help="Print NormCap version and exit",
     )
+    parser.add_argument(
+        "--cli-mode",
+        action="store_true",
+        help="Print text after detection to stdout and exits immediately",
+    )
     return parser
 
 
 def set_environ_for_wayland() -> None:
     # QT has 32 as default cursor size on wayland, while it should be 24
     if "XCURSOR_SIZE" not in os.environ:
         logger.debug("Set XCURSOR_SIZE=24")
         os.environ["XCURSOR_SIZE"] = "24"
 
     # Select wayland extension for better rendering
-
     if "QT_QPA_PLATFORM" not in os.environ:
         logger.debug("Set QT_QPA_PLATFORM=wayland")
         os.environ["QT_QPA_PLATFORM"] = "wayland"
 
     # Adopt PATH to find wl-copy if not installed on system (FlatPak brings its own)
     if system_info.is_briefcase_package() and not shutil.which("wl-copy"):
         binary_path = str((Path(__file__).parent.parent.parent / "bin").resolve())
         logger.debug("Append path to wl-copy to PATH+=%s", binary_path)
-        os.environ["PATH"] = binary_path + ":" + os.environ["PATH"]
+        os.environ["PATH"] = binary_path + os.pathsep + os.environ.get("PATH", "")
 
 
 def set_environ_for_flatpak() -> None:
     # Unity DE (and maybe others) use gtk-nocsd to remove client side decorations.
-    # It doesn't work within FlatPak, and the error message make pytesseract crash.
-    # Therefore we deactivate it within the Flatpak.
+    # It doesn't work within FlatPak, therefore we deactivate it.
     # See: https://github.com/dynobo/normcap/issues/290#issuecomment-1289629427
     ld_preload = os.environ.get("LD_PRELOAD", "")
     if "nocsd" in ld_preload.lower():
         logger.warning(
             "Found LD_PRELOAD='%s'. Setting to LD_PRELOAD='' to avoid issues.",
             ld_preload,
         )
@@ -146,15 +149,15 @@
 def hook_exceptions(
     exc_type: type[BaseException],
     exc_value: BaseException,
     exc_traceback: Optional[TracebackType],
 ) -> None:  # sourcery skip: extract-method
     """Print traceback and quit application.
 
-    TODO: Think about removing/simplifying exception hook after switch to Python 3.11
+    ONHOLD: Think about removing/simplifying exception hook after switch to Python 3.11
     """
     try:
         logger.critical("Uncaught exception! Quitting NormCap!")
 
         formatted_exc = "".join(
             f"  {e}" for e in traceback.format_exception_only(exc_type, exc_value)
         )
```

### Comparing `normcap-0.4.0/setup.py` & `normcap-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,486 +14,504 @@
 000000d0: 655f 6461 7461 203d 205c 0a7b 2727 3a20  e_data = \.{'': 
 000000e0: 5b27 2a27 5d2c 2027 6e6f 726d 6361 702e  ['*'], 'normcap.
 000000f0: 7265 736f 7572 6365 7327 3a20 5b27 6963  resources': ['ic
 00000100: 6f6e 732f 2a27 2c20 2774 6573 7364 6174  ons/*', 'tessdat
 00000110: 612f 2a27 5d7d 0a0a 696e 7374 616c 6c5f  a/*']}..install_
 00000120: 7265 7175 6972 6573 203d 205c 0a5b 2750  requires = \.['P
 00000130: 7953 6964 6536 2d45 7373 656e 7469 616c  ySide6-Essential
-00000140: 733e 3d36 2e34 2e31 2c3c 372e 302e 3027  s>=6.4.1,<7.0.0'
-00000150: 2c0a 2027 6365 7274 6966 693e 3d32 3032  ,. 'certifi>=202
-00000160: 322e 3132 2e37 2c3c 3230 3233 2e30 2e30  2.12.7,<2023.0.0
-00000170: 272c 0a20 276a 6565 706e 6579 3e3d 302e  ',. 'jeepney>=0.
-00000180: 382e 302c 3c30 2e39 2e30 272c 0a20 2770  8.0,<0.9.0',. 'p
-00000190: 7974 6573 7365 7261 6374 3e3d 302e 332e  ytesseract>=0.3.
-000001a0: 3130 275d 0a0a 656e 7472 795f 706f 696e  10']..entry_poin
-000001b0: 7473 203d 205c 0a7b 2763 6f6e 736f 6c65  ts = \.{'console
-000001c0: 5f73 6372 6970 7473 273a 205b 276e 6f72  _scripts': ['nor
-000001d0: 6d63 6170 203d 206e 6f72 6d63 6170 2e61  mcap = normcap.a
-000001e0: 7070 3a6d 6169 6e27 5d7d 0a0a 7365 7475  pp:main']}..setu
-000001f0: 705f 6b77 6172 6773 203d 207b 0a20 2020  p_kwargs = {.   
-00000200: 2027 6e61 6d65 273a 2027 6e6f 726d 6361   'name': 'normca
-00000210: 7027 2c0a 2020 2020 2776 6572 7369 6f6e  p',.    'version
-00000220: 273a 2027 302e 342e 3027 2c0a 2020 2020  ': '0.4.0',.    
-00000230: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
-00000240: 4f43 522d 706f 7765 7265 6420 7363 7265  OCR-powered scre
-00000250: 656e 2d63 6170 7475 7265 2074 6f6f 6c20  en-capture tool 
-00000260: 746f 2063 6170 7475 7265 2069 6e66 6f72  to capture infor
-00000270: 6d61 7469 6f6e 2069 6e73 7465 6164 206f  mation instead o
-00000280: 6620 696d 6167 6573 2e27 2c0a 2020 2020  f images.',.    
-00000290: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
-000002a0: 6e27 3a20 273c 212d 2d20 6d61 726b 646f  n': '<!-- markdo
-000002b0: 776e 6c69 6e74 2d64 6973 6162 6c65 204d  wnlint-disable M
-000002c0: 4430 3133 204d 4430 3236 204d 4430 3333  D013 MD026 MD033
-000002d0: 202d 2d3e 5c6e 5c6e 2320 4e6f 726d 4361   -->\n\n# NormCa
-000002e0: 705c 6e5c 6e2a 2a5f 4f43 5220 706f 7765  p\n\n**_OCR powe
-000002f0: 7265 6420 7363 7265 656e 2d63 6170 7475  red screen-captu
-00000300: 7265 2074 6f6f 6c20 746f 2063 6170 7475  re tool to captu
-00000310: 7265 2069 6e66 6f72 6d61 7469 6f6e 2069  re information i
-00000320: 6e73 7465 6164 206f 6620 696d 6167 6573  nstead of images
-00000330: 2e20 466f 7220 4c69 6e75 782c 5c6e 6d61  . For Linux,\nma
-00000340: 634f 5320 616e 6420 5769 6e64 6f77 732e  cOS and Windows.
-00000350: 5f2a 2a5c 6e5c 6e5b 215b 4275 696c 645d  _**\n\n[![Build]
-00000360: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000370: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
-00000380: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
-00000390: 7374 6174 7573 2f64 796e 6f62 6f2f 6e6f  status/dynobo/no
-000003a0: 726d 6361 702f 7079 7468 6f6e 2e79 616d  rmcap/python.yam
-000003b0: 6c3f 6272 616e 6368 3d6d 6169 6e29 5d28  l?branch=main)](
-000003c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003d0: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
-000003e0: 702f 7265 6c65 6173 6573 295c 6e5b 215b  p/releases)\n[![
-000003f0: 436f 7665 7261 6765 2053 7461 7475 735d  Coverage Status]
-00000400: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000410: 656c 6473 2e69 6f2f 636f 7665 7261 6c6c  elds.io/coverall
-00000420: 7343 6f76 6572 6167 652f 6769 7468 7562  sCoverage/github
-00000430: 2f64 796e 6f62 6f2f 6e6f 726d 6361 703f  /dynobo/normcap?
-00000440: 6c61 6265 6c3d 5465 7374 2532 3063 6f76  label=Test%20cov
-00000450: 6572 6167 6526 6272 616e 6368 3d6d 6169  erage&branch=mai
-00000460: 6e29 5d28 6874 7470 733a 2f2f 636f 7665  n)](https://cove
-00000470: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
-00000480: 6479 6e6f 626f 2f6e 6f72 6d63 6170 295c  dynobo/normcap)\
-00000490: 6e5b 215b 436f 6465 514c 5d28 6874 7470  n[![CodeQL](http
-000004a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000004b0: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
-000004c0: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
-000004d0: 732f 6479 6e6f 626f 2f6e 6f72 6d63 6170  s/dynobo/normcap
-000004e0: 2f63 6f64 6571 6c2d 616e 616c 7973 6973  /codeql-analysis
-000004f0: 2e79 6d6c 3f62 7261 6e63 683d 6d61 696e  .yml?branch=main
-00000500: 266c 6162 656c 3d43 6f64 6551 4c29 5d28  &label=CodeQL)](
-00000510: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000520: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
-00000530: 702f 6163 7469 6f6e 732f 776f 726b 666c  p/actions/workfl
-00000540: 6f77 732f 636f 6465 716c 2d61 6e61 6c79  ows/codeql-analy
-00000550: 7369 732e 796d 6c29 5c6e 5c6e 5b21 5b47  sis.yml)\n\n[![G
-00000560: 6974 4875 625d 2868 7474 7073 3a2f 2f69  itHub](https://i
-00000570: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000580: 7468 7562 2f64 6f77 6e6c 6f61 6473 2f64  thub/downloads/d
-00000590: 796e 6f62 6f2f 6e6f 726d 6361 702f 746f  ynobo/normcap/to
-000005a0: 7461 6c3f 6c61 6265 6c3d 4769 7468 7562  tal?label=Github
-000005b0: 2532 3064 6f77 6e6c 6f61 6473 2663 6f6c  %20downloads&col
-000005c0: 6f72 3d62 6c75 6529 5d28 6874 7470 733a  or=blue)](https:
-000005d0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796e  //github.com/dyn
-000005e0: 6f62 6f2f 6e6f 726d 6361 702f 7265 6c65  obo/normcap/rele
-000005f0: 6173 6573 295c 6e5b 215b 5079 5069 5d28  ases)\n[![PyPi](
-00000600: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000610: 6c64 732e 696f 2f70 7970 692f 646d 2f6e  lds.io/pypi/dm/n
-00000620: 6f72 6d63 6170 3f6c 6162 656c 3d50 7950  ormcap?label=PyP
-00000630: 6925 3230 646f 776e 6c6f 6164 7326 636f  i%20downloads&co
-00000640: 6c6f 723d 626c 7565 295d 2868 7474 7073  lor=blue)](https
-00000650: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000660: 6563 742f 6e6f 726d 6361 7029 5c6e 5b21  ect/normcap)\n[!
-00000670: 5b46 6c61 7468 7562 5d28 6874 7470 733a  [Flathub](https:
-00000680: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000690: 2f66 6c61 7468 7562 2f64 6f77 6e6c 6f61  /flathub/downloa
-000006a0: 6473 2f63 6f6d 2e67 6974 6875 622e 6479  ds/com.github.dy
-000006b0: 6e6f 626f 2e6e 6f72 6d63 6170 3f6c 6162  nobo.normcap?lab
-000006c0: 656c 3d46 6c61 7468 7562 2532 3064 6f77  el=Flathub%20dow
-000006d0: 6e6c 6f61 6473 2663 6f6c 6f72 3d62 6c75  nloads&color=blu
-000006e0: 6529 5d28 6874 7470 733a 2f2f 666c 6174  e)](https://flat
-000006f0: 6875 622e 6f72 672f 6170 7073 2f64 6574  hub.org/apps/det
-00000700: 6169 6c73 2f63 6f6d 2e67 6974 6875 622e  ails/com.github.
-00000710: 6479 6e6f 626f 2e6e 6f72 6d63 6170 295c  dynobo.normcap)\
-00000720: 6e5b 215b 4155 525d 2868 7474 7073 3a2f  n[![AUR](https:/
-00000730: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000740: 6175 722f 766f 7465 732f 6e6f 726d 6361  aur/votes/normca
-00000750: 703f 6c61 6265 6c3d 4155 5225 3230 766f  p?label=AUR%20vo
-00000760: 7465 7326 636f 6c6f 723d 626c 7565 295d  tes&color=blue)]
-00000770: 2868 7474 7073 3a2f 2f61 7572 2e61 7263  (https://aur.arc
-00000780: 686c 696e 7578 2e6f 7267 2f70 6163 6b61  hlinux.org/packa
-00000790: 6765 732f 6e6f 726d 6361 7029 5c6e 5c6e  ges/normcap)\n\n
-000007a0: 2a2a 4c69 6e6b 733a 2a2a 205b 536f 7572  **Links:** [Sour
-000007b0: 6365 2043 6f64 655d 2868 7474 7073 3a2f  ce Code](https:/
-000007c0: 2f67 6974 6875 622e 636f 6d2f 6479 6e6f  /github.com/dyno
-000007d0: 626f 2f6e 6f72 6d63 6170 2920 7c5c 6e5b  bo/normcap) |\n[
-000007e0: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-000007f0: 7474 7073 3a2f 2f64 796e 6f62 6f2e 6769  ttps://dynobo.gi
-00000800: 7468 7562 2e69 6f2f 6e6f 726d 6361 702f  thub.io/normcap/
-00000810: 2920 7c5c 6e5b 4641 5173 5d28 6874 7470  ) |\n[FAQs](http
-00000820: 733a 2f2f 6479 6e6f 626f 2e67 6974 6875  s://dynobo.githu
-00000830: 622e 696f 2f6e 6f72 6d63 6170 2f23 6661  b.io/normcap/#fa
-00000840: 7173 2920 7c5c 6e5b 5265 6c65 6173 6573  qs) |\n[Releases
-00000850: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000860: 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f 726d  .com/dynobo/norm
-00000870: 6361 702f 7265 6c65 6173 6573 2920 7c5c  cap/releases) |\
-00000880: 6e5b 4368 616e 6765 6c6f 675d 2868 7474  n[Changelog](htt
-00000890: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000008a0: 6479 6e6f 626f 2f6e 6f72 6d63 6170 2f62  dynobo/normcap/b
-000008b0: 6c6f 622f 6d61 696e 2f43 4841 4e47 454c  lob/main/CHANGEL
-000008c0: 4f47 2e6d 6429 5c6e 5c6e 5b21 5b53 6372  OG.md)\n\n[![Scr
-000008d0: 6565 6e63 6173 745d 2868 7474 7073 3a2f  eencast](https:/
-000008e0: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-000008f0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000900: 6f6d 2f31 3130 3731 3837 362f 3138 3937  om/11071876/1897
-00000910: 3637 3538 352d 3862 6334 3563 3138 2d38  67585-8bc45c18-8
-00000920: 3339 322d 3431 3164 2d38 3464 632d 6365  392-411d-84dc-ce
-00000930: 6631 6362 3564 6263 3437 2e67 6966 295d  f1cb5dbc47.gif)]
-00000940: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000950: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000960: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
-00000970: 702f 6d61 696e 2f61 7373 6574 732f 6e6f  p/main/assets/no
-00000980: 726d 6361 702e 6769 6629 5c6e 5c6e 2323  rmcap.gif)\n\n##
-00000990: 2051 7569 636b 7374 6172 745c 6e5c 6e49   Quickstart\n\nI
-000009a0: 6e73 7461 6c6c 2061 2070 7265 6275 696c  nstall a prebuil
-000009b0: 7420 7265 6c65 6173 653a 5c6e 5c6e 2d20  t release:\n\n- 
-000009c0: 2a2a 5769 6e64 6f77 732a 2a3a 5c6e 2020  **Windows**:\n  
-000009d0: 5b4e 6f72 6d43 6170 2d30 2e34 2e30 2d78  [NormCap-0.4.0-x
-000009e0: 3836 5f36 342d 5769 6e64 6f77 732e 6d73  86_64-Windows.ms
-000009f0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
-00000a00: 622e 636f 6d2f 6479 6e6f 626f 2f6e 6f72  b.com/dynobo/nor
-00000a10: 6d63 6170 2f72 656c 6561 7365 732f 646f  mcap/releases/do
-00000a20: 776e 6c6f 6164 2f76 302e 342e 302f 4e6f  wnload/v0.4.0/No
-00000a30: 726d 4361 702d 302e 342e 302d 7838 365f  rmCap-0.4.0-x86_
-00000a40: 3634 2d57 696e 646f 7773 2e6d 7369 295c  64-Windows.msi)\
-00000a50: 6e2d 202a 2a4c 696e 7578 2a2a 3a5c 6e20  n- **Linux**:\n 
-00000a60: 205b 4e6f 726d 4361 702d 302e 342e 302d   [NormCap-0.4.0-
-00000a70: 7838 365f 3634 2e41 7070 496d 6167 655d  x86_64.AppImage]
-00000a80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000a90: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
-00000aa0: 6170 2f72 656c 6561 7365 732f 646f 776e  ap/releases/down
-00000ab0: 6c6f 6164 2f76 302e 342e 302f 4e6f 726d  load/v0.4.0/Norm
-00000ac0: 4361 702d 302e 342e 302d 7838 365f 3634  Cap-0.4.0-x86_64
-00000ad0: 2e41 7070 496d 6167 6529 5c6e 2d20 2a2a  .AppImage)\n- **
-00000ae0: 6d61 634f 532a 2a20 2878 3836 2920 c2b9  macOS** (x86) ..
-00000af0: 3a5c 6e20 205b 4e6f 726d 4361 702d 302e  :\n  [NormCap-0.
-00000b00: 342e 302d 7838 365f 3634 2d6d 6163 4f53  4.0-x86_64-macOS
-00000b10: 2e64 6d67 5d28 6874 7470 733a 2f2f 6769  .dmg](https://gi
-00000b20: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
-00000b30: 6e6f 726d 6361 702f 7265 6c65 6173 6573  normcap/releases
-00000b40: 2f64 6f77 6e6c 6f61 642f 7630 2e34 2e30  /download/v0.4.0
-00000b50: 2f4e 6f72 6d43 6170 2d30 2e34 2e30 2d78  /NormCap-0.4.0-x
-00000b60: 3836 5f36 342d 6d61 634f 532e 646d 6729  86_64-macOS.dmg)
-00000b70: 5c6e 2d20 2a2a 6d61 634f 532a 2a20 284d  \n- **macOS** (M
-00000b80: 3129 20c2 b9c2 b7c2 b23a 5c6e 2020 5b4e  1) ......:\n  [N
-00000b90: 6f72 6d43 6170 2d30 2e34 2e30 2d61 726d  ormCap-0.4.0-arm
-00000ba0: 3634 2d6d 6163 4f53 2e64 6d67 5d28 6874  64-macOS.dmg](ht
-00000bb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000bc0: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
-00000bd0: 7265 6c65 6173 6573 2f64 6f77 6e6c 6f61  releases/downloa
-00000be0: 642f 7630 2e34 2e30 2f4e 6f72 6d43 6170  d/v0.4.0/NormCap
-00000bf0: 2d30 2e34 2e30 2d61 726d 3634 2d6d 6163  -0.4.0-arm64-mac
-00000c00: 4f53 2e64 6d67 295c 6e20 205c 5c5c 6e20  OS.dmg)\n  \\\n 
-00000c10: 203c 7375 623e 313a 204f 6e20 6d61 634f   <sub>1: On macO
-00000c20: 532c 2061 6c6c 6f77 2074 6865 2075 6e73  S, allow the uns
-00000c30: 6967 6e65 6420 6170 706c 6963 6174 696f  igned applicatio
-00000c40: 6e20 6f6e 2066 6972 7374 2073 7461 7274  n on first start
-00000c50: 3a20 2253 7973 7465 6d5c 6e20 2050 7265  : "System\n  Pre
-00000c60: 6665 7265 6e63 6573 2220 e286 9220 2253  ferences" ... "S
-00000c70: 6563 7572 6974 7920 2620 5072 6976 6163  ecurity & Privac
-00000c80: 7922 20e2 8692 2022 4765 6e65 7261 6c22  y" ... "General"
-00000c90: 20e2 8692 2022 4f70 656e 2061 6e79 7761   ... "Open anywa
-00000ca0: 7922 2e20 596f 7520 6d69 6768 7420 616c  y". You might al
-00000cb0: 736f 206e 6565 645c 6e20 2074 6f20 616c  so need\n  to al
-00000cc0: 6c6f 7720 4e6f 726d 4361 7020 746f 2074  low NormCap to t
-00000cd0: 616b 6520 7363 7265 656e 7368 6f74 732e  ake screenshots.
-00000ce0: 5c6e 2020 5b23 3133 355d 2868 7474 7073  \n  [#135](https
-00000cf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6479  ://github.com/dy
-00000d00: 6e6f 626f 2f6e 6f72 6d63 6170 2f69 7373  nobo/normcap/iss
-00000d10: 7565 732f 3133 3529 3c62 723e 2032 3a20  ues/135)<br> 2: 
-00000d20: 4d69 6768 7420 6265 2061 7661 696c 6162  Might be availab
-00000d30: 6c65 2061 2062 6974 5c6e 2020 6465 6c61  le a bit\n  dela
-00000d40: 7965 642c 2061 7320 6974 2069 7320 6375  yed, as it is cu
-00000d50: 7272 656e 746c 7920 6275 696c 6420 6d61  rrently build ma
-00000d60: 6e75 616c 6c79 2e20 2854 6878 2c5c 6e20  nually. (Thx,\n 
-00000d70: 205b 4054 616b 7269 6e5d 2868 7474 7073   [@Takrin](https
-00000d80: 3a2f 2f67 6974 6875 622e 636f 6d2f 5461  ://github.com/Ta
-00000d90: 6b72 696e 2921 293c 2f73 7562 3e5c 6e5c  krin)!)</sub>\n\
-00000da0: 6e49 6e73 7461 6c6c 2066 726f 6d20 7265  nInstall from re
-00000db0: 706f 7369 746f 7269 6573 3a5c 6e5c 6e2d  positories:\n\n-
-00000dc0: 202a 2a41 7263 6820 2f20 4d61 6e6a 6172   **Arch / Manjar
-00000dd0: 6f2a 2a3a 2049 6e73 7461 6c6c 2074 6865  o**: Install the
-00000de0: 5c6e 2020 5b60 6e6f 726d 6361 7060 5d28  \n  [`normcap`](
-00000df0: 6874 7470 733a 2f2f 6175 722e 6172 6368  https://aur.arch
-00000e00: 6c69 6e75 782e 6f72 672f 7061 636b 6167  linux.org/packag
-00000e10: 6573 2f6e 6f72 6d63 6170 2920 7061 636b  es/normcap) pack
-00000e20: 6167 6520 6672 6f6d 2041 5552 2e5c 6e2d  age from AUR.\n-
-00000e30: 202a 2a46 6c61 7450 616b 2028 4c69 6e75   **FlatPak (Linu
-00000e40: 7829 2a2a 3a20 496e 7374 616c 6c5c 6e20  x)**: Install\n 
-00000e50: 205b 636f 6d2e 6769 7468 7562 2e64 796e   [com.github.dyn
-00000e60: 6f62 6f2e 6e6f 726d 6361 705d 2868 7474  obo.normcap](htt
-00000e70: 7073 3a2f 2f66 6c61 7468 7562 2e6f 7267  ps://flathub.org
-00000e80: 2f61 7070 732f 6465 7461 696c 732f 636f  /apps/details/co
-00000e90: 6d2e 6769 7468 7562 2e64 796e 6f62 6f2e  m.github.dynobo.
-00000ea0: 6e6f 726d 6361 7029 5c6e 2020 6672 6f6d  normcap)\n  from
-00000eb0: 2046 6c61 7448 7562 2e5c 6e5c 6e49 6620   FlatHub.\n\nIf 
-00000ec0: 796f 7520 6578 7065 7269 656e 6365 2069  you experience i
-00000ed0: 7373 7565 7320 706c 6561 7365 206c 6f6f  ssues please loo
-00000ee0: 6b20 6174 2074 6865 5c6e 5b46 4151 735d  k at the\n[FAQs]
-00000ef0: 2868 7474 7073 3a2f 2f64 796e 6f62 6f2e  (https://dynobo.
-00000f00: 6769 7468 7562 2e69 6f2f 6e6f 726d 6361  github.io/normca
-00000f10: 702f 2366 6171 7329 206f 725c 6e5b 6f70  p/#faqs) or\n[op
-00000f20: 656e 2061 6e20 6973 7375 655d 2868 7474  en an issue](htt
-00000f30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000f40: 6479 6e6f 626f 2f6e 6f72 6d63 6170 2f69  dynobo/normcap/i
-00000f50: 7373 7565 7329 2e5c 6e5c 6e23 2320 5079  ssues).\n\n## Py
-00000f60: 7468 6f6e 2070 6163 6b61 6765 5c6e 5c6e  thon package\n\n
-00000f70: 4173 2061 6e20 5f61 6c74 6572 6e61 7469  As an _alternati
-00000f80: 7665 5f20 746f 2061 2070 7265 6275 696c  ve_ to a prebuil
-00000f90: 7420 7061 636b 6167 6520 796f 7520 6361  t package you ca
-00000fa0: 6e20 696e 7374 616c 6c20 7468 655c 6e5b  n install the\n[
-00000fb0: 4e6f 726d 4361 7020 5079 7468 6f6e 2070  NormCap Python p
-00000fc0: 6163 6b61 6765 5d28 6874 7470 733a 2f2f  ackage](https://
-00000fd0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000fe0: 2f6e 6f72 6d63 6170 2f29 2066 6f72 202a  /normcap/) for *
-00000ff0: 2a50 7974 686f 6e20 3e3d 332e 392a 2a3a  *Python >=3.9**:
-00001000: 5c6e 5c6e 2323 2323 204f 6e20 4c69 6e75  \n\n#### On Linu
-00001010: 785c 6e5c 6e60 6060 7368 5c6e 2320 496e  x\n\n```sh\n# In
-00001020: 7374 616c 6c20 6465 7065 6e64 656e 6369  stall dependenci
-00001030: 6573 2028 5562 756e 7475 2f44 6562 6961  es (Ubuntu/Debia
-00001040: 6e29 5c6e 7375 646f 2061 7074 2069 6e73  n)\nsudo apt ins
-00001050: 7461 6c6c 2062 7569 6c64 2d65 7373 656e  tall build-essen
-00001060: 7469 616c 2074 6573 7365 7261 6374 2d6f  tial tesseract-o
-00001070: 6372 2074 6573 7365 7261 6374 2d6f 6372  cr tesseract-ocr
-00001080: 2d65 6e67 206c 6962 7465 7373 6572 6163  -eng libtesserac
-00001090: 742d 6465 7620 6c69 626c 6570 746f 6e69  t-dev libleptoni
-000010a0: 6361 2d64 6576 2077 6c2d 636c 6970 626f  ca-dev wl-clipbo
-000010b0: 6172 645c 6e5c 6e23 2320 496e 7374 616c  ard\n\n## Instal
-000010c0: 6c20 6465 7065 6e64 656e 6369 6573 2028  l dependencies (
-000010d0: 4172 6368 295c 6e73 7564 6f20 7061 636d  Arch)\nsudo pacm
-000010e0: 616e 202d 5320 7465 7373 6572 6163 7420  an -S tesseract 
-000010f0: 7465 7373 6572 6163 742d 6461 7461 2d65  tesseract-data-e
-00001100: 6e67 2077 6c2d 636c 6970 626f 6172 645c  ng wl-clipboard\
-00001110: 6e5c 6e23 2320 496e 7374 616c 6c20 6465  n\n## Install de
-00001120: 7065 6e64 656e 6369 6573 2028 4665 646f  pendencies (Fedo
-00001130: 7261 295c 6e73 7564 6f20 646e 6620 696e  ra)\nsudo dnf in
-00001140: 7374 616c 6c20 7465 7373 6572 6163 7420  stall tesseract 
-00001150: 776c 2d63 6c69 7062 6f61 7264 5c6e 5c6e  wl-clipboard\n\n
-00001160: 2323 2049 6e73 7461 6c6c 2064 6570 656e  ## Install depen
-00001170: 6465 6e63 6965 7320 286f 7065 6e53 5553  dencies (openSUS
-00001180: 4529 5c6e 7375 646f 207a 7970 7065 7220  E)\nsudo zypper 
-00001190: 696e 7374 616c 6c20 7079 7468 6f6e 332d  install python3-
-000011a0: 6465 7665 6c20 7465 7373 6572 6163 742d  devel tesseract-
-000011b0: 6f63 7220 7465 7373 6572 6163 742d 6f63  ocr tesseract-oc
-000011c0: 722d 6465 7665 6c20 776c 2d63 6c69 7062  r-devel wl-clipb
-000011d0: 6f61 7264 5c6e 5c6e 2320 496e 7374 616c  oard\n\n# Instal
-000011e0: 6c20 6e6f 726d 6361 705c 6e70 6970 2069  l normcap\npip i
-000011f0: 6e73 7461 6c6c 206e 6f72 6d63 6170 5c6e  nstall normcap\n
-00001200: 5c6e 2320 5275 6e5c 6e2e 2f6e 6f72 6d63  \n# Run\n./normc
-00001210: 6170 5c6e 6060 605c 6e5c 6e23 2323 2320  ap\n```\n\n#### 
-00001220: 4f6e 206d 6163 4f53 5c6e 5c6e 6060 6073  On macOS\n\n```s
-00001230: 685c 6e23 2049 6e73 7461 6c6c 2064 6570  h\n# Install dep
-00001240: 656e 6465 6e63 6965 735c 6e62 7265 7720  endencies\nbrew 
-00001250: 696e 7374 616c 6c20 7465 7373 6572 6163  install tesserac
-00001260: 7420 7465 7373 6572 6163 742d 6c61 6e67  t tesseract-lang
-00001270: 5c6e 5c6e 2320 496e 7374 616c 6c20 6e6f  \n\n# Install no
-00001280: 726d 6361 705c 6e70 6970 2069 6e73 7461  rmcap\npip insta
-00001290: 6c6c 206e 6f72 6d63 6170 5c6e 5c6e 2320  ll normcap\n\n# 
-000012a0: 5275 6e5c 6e2e 2f6e 6f72 6d63 6170 5c6e  Run\n./normcap\n
-000012b0: 6060 605c 6e5c 6e23 2323 2320 4f6e 2057  ```\n\n#### On W
-000012c0: 696e 646f 7773 5c6e 5c6e 315c 5c2e 2049  indows\n\n1\\. I
-000012d0: 6e73 7461 6c6c 2060 5465 7373 6572 6163  nstall `Tesserac
-000012e0: 7420 3560 2062 7920 7573 696e 6720 7468  t 5` by using th
-000012f0: 655c 6e5b 696e 7374 616c 6c65 7220 7072  e\n[installer pr
-00001300: 6f76 6964 6564 2062 7920 5542 204d 616e  ovided by UB Man
-00001310: 6e68 6569 6d5d 2868 7474 7073 3a2f 2f67  nheim](https://g
-00001320: 6974 6875 622e 636f 6d2f 5542 2d4d 616e  ithub.com/UB-Man
-00001330: 6e68 6569 6d2f 7465 7373 6572 6163 742f  nheim/tesseract/
-00001340: 7769 6b69 292e 5c6e 5c6e 325c 5c2e 2041  wiki).\n\n2\\. A
-00001350: 646a 7573 7420 656e 7669 726f 6e6d 656e  djust environmen
-00001360: 7420 7661 7269 6162 6c65 733a 5c6e 5c6e  t variables:\n\n
-00001370: 2d20 4372 6561 7465 2061 6e20 656e 7669  - Create an envi
-00001380: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00001390: 2060 5445 5353 4441 5441 5f50 5245 4649   `TESSDATA_PREFI
-000013a0: 5860 2061 6e64 2073 6574 2069 7420 746f  X` and set it to
-000013b0: 2054 6573 7365 7261 6374 5c27 7320 6461   Tesseract\'s da
-000013c0: 7461 5c6e 2020 666f 6c64 6572 2c20 652e  ta\n  folder, e.
-000013d0: 672e 3a5c 6e5c 6e20 2060 6060 636d 645c  g.:\n\n  ```cmd\
-000013e0: 6e20 2073 6574 7820 5445 5353 4441 5441  n  setx TESSDATA
-000013f0: 5f50 5245 4649 5820 2243 3a5c 5c50 726f  _PREFIX "C:\\Pro
-00001400: 6772 616d 2046 696c 6573 5c5c 5465 7373  gram Files\\Tess
-00001410: 6572 6163 742d 4f43 525c 5c74 6573 7364  eract-OCR\\tessd
-00001420: 6174 6122 5c6e 2020 6060 605c 6e5c 6e2d  ata"\n  ```\n\n-
-00001430: 2041 7070 656e 6420 5465 7373 6572 6163   Append Tesserac
-00001440: 745c 2773 206c 6f63 6174 696f 6e20 746f  t\'s location to
-00001450: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
-00001460: 2076 6172 6961 626c 6520 6050 6174 6860   variable `Path`
-00001470: 2c20 652e 672e 3a5c 6e5c 6e20 2060 6060  , e.g.:\n\n  ```
-00001480: 636d 645c 6e20 2073 6574 7820 5061 7468  cmd\n  setx Path
-00001490: 2022 2550 6174 6825 3b43 3a5c 5c50 726f   "%Path%;C:\\Pro
-000014a0: 6772 616d 2046 696c 6573 5c5c 5465 7373  gram Files\\Tess
-000014b0: 6572 6163 742d 4f43 5222 5c6e 2020 6060  eract-OCR"\n  ``
-000014c0: 605c 6e5c 6e2d 204d 616b 6520 7375 7265  `\n\n- Make sure
-000014d0: 2074 6f20 636c 6f73 6520 616e 6420 7265   to close and re
-000014e0: 6f70 656e 2079 6f75 7220 6375 7272 656e  open your curren
-000014f0: 7420 7465 726d 696e 616c 2077 696e 646f  t terminal windo
-00001500: 7720 746f 2061 7070 6c79 2074 6865 206e  w to apply the n
-00001510: 6577 2076 6172 6961 626c 6573 2e5c 6e20  ew variables.\n 
-00001520: 2054 6573 7420 6974 2062 7920 7275 6e6e   Test it by runn
-00001530: 696e 673a 5c6e 5c6e 2020 6060 6063 6d64  ing:\n\n  ```cmd
-00001540: 5c6e 2020 7465 7373 6572 6163 7420 2d2d  \n  tesseract --
-00001550: 6c69 7374 2d6c 616e 6773 5c6e 2020 6060  list-langs\n  ``
-00001560: 605c 6e5c 6e33 5c5c 2e20 496e 7374 616c  `\n\n3\\. Instal
-00001570: 6c20 616e 6420 7275 6e20 4e6f 726d 4361  l and run NormCa
-00001580: 703a 5c6e 5c6e 6060 6062 6173 685c 6e23  p:\n\n```bash\n#
-00001590: 2049 6e73 7461 6c6c 206e 6f72 6d63 6170   Install normcap
-000015a0: 5c6e 7069 7020 696e 7374 616c 6c20 6e6f  \npip install no
-000015b0: 726d 6361 705c 6e5c 6e23 2052 756e 5c6e  rmcap\n\n# Run\n
-000015c0: 6e6f 726d 6361 705c 6e60 6060 5c6e 5c6e  normcap\n```\n\n
-000015d0: 2323 2057 6879 2022 4e6f 726d 4361 7022  ## Why "NormCap"
-000015e0: 3f5c 6e5c 6e53 6565 205b 584b 4344 5d28  ?\n\nSee [XKCD](
-000015f0: 6874 7470 733a 2f2f 786b 6364 2e63 6f6d  https://xkcd.com
-00001600: 293a 5c6e 5c6e 5b21 5b43 6f6d 6963 5d28  ):\n\n[![Comic](
-00001610: 6874 7470 733a 2f2f 696d 6773 2e78 6b63  https://imgs.xkc
-00001620: 642e 636f 6d2f 636f 6d69 6373 2f6e 6f72  d.com/comics/nor
-00001630: 6d5f 6e6f 726d 616c 5f66 696c 655f 666f  m_normal_file_fo
-00001640: 726d 6174 2e70 6e67 295d 2868 7474 7073  rmat.png)](https
-00001650: 3a2f 2f78 6b63 642e 636f 6d2f 3231 3136  ://xkcd.com/2116
-00001660: 2f29 5c6e 5c6e 2323 2044 6576 656c 6f70  /)\n\n## Develop
-00001670: 6d65 6e74 5c6e 5c6e 5072 6572 6571 7569  ment\n\nPrerequi
-00001680: 7369 7465 7320 666f 7220 7365 7474 696e  sites for settin
-00001690: 6720 7570 2061 2064 6576 656c 6f70 6d65  g up a developme
-000016a0: 6e74 2065 6e76 6972 6f6e 6d65 6e74 2061  nt environment a
-000016b0: 7265 3a20 2a2a 5079 7468 6f6e 203e 3d33  re: **Python >=3
-000016c0: 2e39 2a2a 2c5c 6e2a 2a50 6f65 7472 793e  .9**,\n**Poetry>
-000016d0: 3d31 2e33 2e32 2a2a 2061 6e64 202a 2a54  =1.3.2** and **T
-000016e0: 6573 7365 7261 6374 2a2a 2028 696e 636c  esseract** (incl
-000016f0: 2e20 2a2a 6c61 6e67 7561 6765 2064 6174  . **language dat
-00001700: 612a 2a29 2e5c 6e5c 6e60 6060 7368 5c6e  a**).\n\n```sh\n
-00001710: 2320 436c 6f6e 6520 7265 706f 7369 746f  # Clone reposito
-00001720: 7279 5c6e 6769 7420 636c 6f6e 6520 6874  ry\ngit clone ht
-00001730: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001740: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702e  /dynobo/normcap.
-00001750: 6769 745c 6e5c 6e23 2043 6861 6e67 6520  git\n\n# Change 
-00001760: 696e 746f 2070 726f 6a65 6374 2064 6972  into project dir
-00001770: 6563 746f 7279 5c6e 6364 206e 6f72 6d63  ectory\ncd normc
-00001780: 6170 5c6e 5c6e 2320 4372 6561 7465 2076  ap\n\n# Create v
-00001790: 6972 7475 616c 2065 6e76 2061 6e64 2069  irtual env and i
-000017a0: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
-000017b0: 6965 735c 6e70 6f65 7472 7920 696e 7374  ies\npoetry inst
-000017c0: 616c 6c5c 6e5c 6e23 2052 6567 6973 7465  all\n\n# Registe
-000017d0: 7220 7072 652d 636f 6d6d 6974 2068 6f6f  r pre-commit hoo
-000017e0: 6b5c 6e70 6f65 7472 7920 7275 6e20 7072  k\npoetry run pr
-000017f0: 652d 636f 6d6d 6974 2069 6e73 7461 6c6c  e-commit install
-00001800: 5c6e 5c6e 2320 5275 6e20 4e6f 726d 4361  \n\n# Run NormCa
-00001810: 7020 696e 2076 6972 7475 616c 2065 6e76  p in virtual env
-00001820: 5c6e 706f 6574 7279 2072 756e 2070 7974  \npoetry run pyt
-00001830: 686f 6e20 2d6d 206e 6f72 6d63 6170 5c6e  hon -m normcap\n
-00001840: 6060 605c 6e5c 6e23 2320 4372 6564 6974  ```\n\n## Credit
-00001850: 735c 6e5c 6e54 6869 7320 7072 6f6a 6563  s\n\nThis projec
-00001860: 7420 7573 6573 2074 6865 2066 6f6c 6c6f  t uses the follo
-00001870: 7769 6e67 206e 6f6e 2d73 7461 6e64 6172  wing non-standar
-00001880: 6420 6c69 6272 6172 6965 733a 5c6e 5c6e  d libraries:\n\n
-00001890: 2d20 5b70 7973 6964 6536 5d28 6874 7470  - [pyside6](http
-000018a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000018b0: 6a65 6374 2f50 7953 6964 6536 2f29 205f  ject/PySide6/) _
-000018c0: 2d20 6269 6e64 696e 6773 2066 6f72 2051  - bindings for Q
-000018d0: 7420 5549 2046 7261 6d65 776f 726b 5f5c  t UI Framework_\
-000018e0: 6e2d 205b 7079 7465 7373 6572 6163 745d  n- [pytesseract]
-000018f0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00001900: 672f 7072 6f6a 6563 742f 7079 7465 7373  g/project/pytess
-00001910: 6572 6163 742f 2920 5f2d 2077 7261 7070  eract/) _- wrapp
-00001920: 6572 2066 6f72 2074 6573 7365 7261 6374  er for tesseract
-00001930: 5c27 7320 4150 495f 5c6e 2d20 5b6a 6565  \'s API_\n- [jee
-00001940: 706e 6579 5d28 6874 7470 733a 2f2f 7079  pney](https://py
-00001950: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6a  pi.org/project/j
-00001960: 6565 706e 6579 2f29 205f 2d20 4442 5553  eepney/) _- DBUS
-00001970: 2063 6c69 656e 745f 5c6e 5c6e 416e 6420   client_\n\nAnd 
-00001980: 6974 2064 6570 656e 6473 206f 6e20 6578  it depends on ex
-00001990: 7465 726e 616c 2073 6f66 7477 6172 653a  ternal software:
-000019a0: 5c6e 5c6e 2d20 5b74 6573 7365 7261 6374  \n\n- [tesseract
-000019b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000019c0: 2e63 6f6d 2f74 6573 7365 7261 6374 2d6f  .com/tesseract-o
-000019d0: 6372 2f74 6573 7365 7261 6374 2920 2d20  cr/tesseract) - 
-000019e0: 5f4f 4352 2065 6e67 696e 655f 5c6e 2d20  _OCR engine_\n- 
-000019f0: 5b77 6c2d 636c 6970 626f 6172 645d 2868  [wl-clipboard](h
-00001a00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001a10: 6d2f 6275 6761 6576 632f 776c 2d63 6c69  m/bugaevc/wl-cli
-00001a20: 7062 6f61 7264 2920 2d20 5f57 6179 6c61  pboard) - _Wayla
-00001a30: 6e64 2063 6c69 7062 6f61 7264 5c6e 2020  nd clipboard\n  
-00001a40: 7574 696c 6974 6965 735f 5c6e 5c6e 5061  utilities_\n\nPa
-00001a50: 636b 6167 696e 6720 6973 2064 6f6e 6520  ckaging is done 
-00001a60: 7769 7468 3a5c 6e5c 6e2d 205b 6272 6965  with:\n\n- [brie
-00001a70: 6663 6173 655d 2868 7474 7073 3a2f 2f70  fcase](https://p
-00001a80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00001a90: 6272 6965 6663 6173 652f 2920 5f2d 2063  briefcase/) _- c
-00001aa0: 6f6e 7665 7274 696e 6720 5079 7468 6f6e  onverting Python
-00001ab0: 2070 726f 6a65 6374 7320 696e 746f 5f5c   projects into_\
-00001ac0: 6e20 205f 7374 616e 6461 6c6f 6e65 2061  n  _standalone a
-00001ad0: 7070 735f 5c6e 5c6e 5468 616e 6b73 2074  pps_\n\nThanks t
-00001ae0: 6f20 7468 6520 6d61 696e 7461 696e 6572  o the maintainer
-00001af0: 7320 6f66 2074 686f 7365 206e 6963 6520  s of those nice 
-00001b00: 746f 6f6c 7321 5c6e 5c6e 2323 2053 696d  tools!\n\n## Sim
-00001b10: 696c 6172 206f 7065 6e20 736f 7572 6365  ilar open source
-00001b20: 2074 6f6f 6c73 5c6e 5c6e 4966 204e 6f72   tools\n\nIf Nor
-00001b30: 6d43 6170 2064 6f65 736e 5c27 7420 6669  mCap doesn\'t fi
-00001b40: 7420 796f 7572 206e 6565 6473 2c20 7472  t your needs, tr
-00001b50: 7920 7468 6f73 6520 616c 7465 726e 6174  y those alternat
-00001b60: 6976 6573 2028 6e6f 2070 6172 7469 6375  ives (no particu
-00001b70: 6c61 7220 6f72 6465 7229 3a5c 6e5c 6e2d  lar order):\n\n-
-00001b80: 205b 5465 7874 536e 6174 6368 6572 5d28   [TextSnatcher](
-00001b90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001ba0: 6f6d 2f52 616a 536f 6c61 692f 5465 7874  om/RajSolai/Text
-00001bb0: 536e 6174 6368 6572 2920 284c 696e 7578  Snatcher) (Linux
-00001bc0: 295c 6e2d 205b 4772 6565 6e53 686f 745d  )\n- [GreenShot]
-00001bd0: 2868 7474 7073 3a2f 2f67 6574 6772 6565  (https://getgree
-00001be0: 6e73 686f 742e 6f72 672f 2920 284c 696e  nshot.org/) (Lin
-00001bf0: 7578 2c20 6d61 634f 5329 5c6e 2d20 5b54  ux, macOS)\n- [T
-00001c00: 6578 7453 686f 745d 2868 7474 7073 3a2f  extShot](https:/
-00001c10: 2f67 6974 6875 622e 636f 6d2f 6961 6e7a  /github.com/ianz
-00001c20: 6861 6f30 352f 7465 7874 7368 6f74 2920  hao05/textshot) 
-00001c30: 2857 696e 646f 7773 295c 6e2d 205b 6749  (Windows)\n- [gI
-00001c40: 6d61 6765 5265 6164 6572 5d28 6874 7470  mageReader](http
-00001c50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00001c60: 616e 6973 616e 6472 6f2f 6749 6d61 6765  anisandro/gImage
-00001c70: 5265 6164 6572 2920 284c 696e 7578 2c20  Reader) (Linux, 
-00001c80: 5769 6e64 6f77 7329 5c6e 2d20 5b43 6170  Windows)\n- [Cap
-00001c90: 7475 7265 3254 6578 745d 2868 7474 7073  ture2Text](https
-00001ca0: 3a2f 2f73 6f75 7263 6566 6f72 6765 2e6e  ://sourceforge.n
-00001cb0: 6574 2f70 726f 6a65 6374 732f 6361 7074  et/projects/capt
-00001cc0: 7572 6532 7465 7874 2920 2857 696e 646f  ure2text) (Windo
-00001cd0: 7773 295c 6e2d 205b 4672 6f67 5d28 6874  ws)\n- [Frog](ht
-00001ce0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001cf0: 2f54 656e 6465 724f 776c 2f46 726f 6729  /TenderOwl/Frog)
-00001d00: 2028 4c69 6e75 7829 5c6e 2d20 5b54 6578   (Linux)\n- [Tex
-00001d10: 7469 6e61 746f 725d 2868 7474 7073 3a2f  tinator](https:/
-00001d20: 2f67 6974 6875 622e 636f 6d2f 5268 6574  /github.com/Rhet
-00001d30: 5462 756c 6c2f 7465 7874 696e 6174 6f72  Tbull/textinator
-00001d40: 2920 286d 6163 4f53 295c 6e5c 6e23 2320  ) (macOS)\n\n## 
-00001d50: 4365 7274 6966 6963 6174 696f 6e5c 6e5c  Certification\n\
-00001d60: 6e21 5b57 4f4d 4d5d 2868 7474 7073 3a2f  n![WOMM](https:/
-00001d70: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001d80: 6f6e 7465 6e74 2e63 6f6d 2f64 796e 6f62  ontent.com/dynob
-00001d90: 6f2f 6c6d 6469 6167 2f6d 6173 7465 722f  o/lmdiag/master/
-00001da0: 6261 6467 652e 706e 6729 5c6e 272c 0a20  badge.png)\n',. 
-00001db0: 2020 2027 6175 7468 6f72 273a 2027 6479     'author': 'dy
-00001dc0: 6e6f 626f 272c 0a20 2020 2027 6175 7468  nobo',.    'auth
-00001dd0: 6f72 5f65 6d61 696c 273a 2027 6479 6e6f  or_email': 'dyno
-00001de0: 626f 406d 6169 6c62 6f78 2e6f 7267 272c  bo@mailbox.org',
-00001df0: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00001e00: 273a 2027 4e6f 6e65 272c 0a20 2020 2027  ': 'None',.    '
-00001e10: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
-00001e20: 273a 2027 4e6f 6e65 272c 0a20 2020 2027  ': 'None',.    '
-00001e30: 7572 6c27 3a20 2768 7474 7073 3a2f 2f64  url': 'https://d
-00001e40: 796e 6f62 6f2e 6769 7468 7562 2e69 6f2f  ynobo.github.io/
-00001e50: 6e6f 726d 6361 702f 272c 0a20 2020 2027  normcap/',.    '
-00001e60: 7061 636b 6167 6573 273a 2070 6163 6b61  packages': packa
-00001e70: 6765 732c 0a20 2020 2027 7061 636b 6167  ges,.    'packag
-00001e80: 655f 6461 7461 273a 2070 6163 6b61 6765  e_data': package
-00001e90: 5f64 6174 612c 0a20 2020 2027 696e 7374  _data,.    'inst
-00001ea0: 616c 6c5f 7265 7175 6972 6573 273a 2069  all_requires': i
-00001eb0: 6e73 7461 6c6c 5f72 6571 7569 7265 732c  nstall_requires,
-00001ec0: 0a20 2020 2027 656e 7472 795f 706f 696e  .    'entry_poin
-00001ed0: 7473 273a 2065 6e74 7279 5f70 6f69 6e74  ts': entry_point
-00001ee0: 732c 0a20 2020 2027 7079 7468 6f6e 5f72  s,.    'python_r
-00001ef0: 6571 7569 7265 7327 3a20 273e 3d33 2e39  equires': '>=3.9
-00001f00: 2c3c 332e 3132 272c 0a7d 0a0a 0a73 6574  ,<3.12',.}...set
-00001f10: 7570 282a 2a73 6574 7570 5f6b 7761 7267  up(**setup_kwarg
-00001f20: 7329 0a                                  s).
+00000140: 733d 3d36 2e34 2e32 272c 2027 6a65 6570  s==6.4.2', 'jeep
+00000150: 6e65 793e 3d30 2e38 2e30 2c3c 302e 392e  ney>=0.8.0,<0.9.
+00000160: 3027 5d0a 0a65 6e74 7279 5f70 6f69 6e74  0']..entry_point
+00000170: 7320 3d20 5c0a 7b27 636f 6e73 6f6c 655f  s = \.{'console_
+00000180: 7363 7269 7074 7327 3a20 5b27 6e6f 726d  scripts': ['norm
+00000190: 6361 7020 3d20 6e6f 726d 6361 702e 6170  cap = normcap.ap
+000001a0: 703a 6d61 696e 275d 7d0a 0a73 6574 7570  p:main']}..setup
+000001b0: 5f6b 7761 7267 7320 3d20 7b0a 2020 2020  _kwargs = {.    
+000001c0: 276e 616d 6527 3a20 276e 6f72 6d63 6170  'name': 'normcap
+000001d0: 272c 0a20 2020 2027 7665 7273 696f 6e27  ',.    'version'
+000001e0: 3a20 2730 2e34 2e31 272c 0a20 2020 2027  : '0.4.1',.    '
+000001f0: 6465 7363 7269 7074 696f 6e27 3a20 274f  description': 'O
+00000200: 4352 2d70 6f77 6572 6564 2073 6372 6565  CR-powered scree
+00000210: 6e2d 6361 7074 7572 6520 746f 6f6c 2074  n-capture tool t
+00000220: 6f20 6361 7074 7572 6520 696e 666f 726d  o capture inform
+00000230: 6174 696f 6e20 696e 7374 6561 6420 6f66  ation instead of
+00000240: 2069 6d61 6765 732e 272c 0a20 2020 2027   images.',.    '
+00000250: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000260: 273a 2027 3c21 2d2d 206d 6172 6b64 6f77  ': '<!-- markdow
+00000270: 6e6c 696e 742d 6469 7361 626c 6520 4d44  nlint-disable MD
+00000280: 3031 3320 4d44 3032 3620 4d44 3033 3320  013 MD026 MD033 
+00000290: 2d2d 3e5c 6e5c 6e23 204e 6f72 6d43 6170  -->\n\n# NormCap
+000002a0: 5c6e 5c6e 2a2a 5f4f 4352 2070 6f77 6572  \n\n**_OCR power
+000002b0: 6564 2073 6372 6565 6e2d 6361 7074 7572  ed screen-captur
+000002c0: 6520 746f 6f6c 2074 6f20 6361 7074 7572  e tool to captur
+000002d0: 6520 696e 666f 726d 6174 696f 6e20 696e  e information in
+000002e0: 7374 6561 6420 6f66 2069 6d61 6765 732e  stead of images.
+000002f0: 2046 6f72 204c 696e 7578 2c5c 6e6d 6163   For Linux,\nmac
+00000300: 4f53 2061 6e64 2057 696e 646f 7773 2e5f  OS and Windows._
+00000310: 2a2a 5c6e 5c6e 5b21 5b42 7569 6c64 5d28  **\n\n[![Build](
+00000320: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000330: 6c64 732e 696f 2f67 6974 6875 622f 6163  lds.io/github/ac
+00000340: 7469 6f6e 732f 776f 726b 666c 6f77 2f73  tions/workflow/s
+00000350: 7461 7475 732f 6479 6e6f 626f 2f6e 6f72  tatus/dynobo/nor
+00000360: 6d63 6170 2f70 7974 686f 6e2e 7961 6d6c  mcap/python.yaml
+00000370: 3f62 7261 6e63 683d 6d61 696e 295d 2868  ?branch=main)](h
+00000380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000390: 6d2f 6479 6e6f 626f 2f6e 6f72 6d63 6170  m/dynobo/normcap
+000003a0: 2f72 656c 6561 7365 7329 5c6e 5b21 5b43  /releases)\n[![C
+000003b0: 6f76 6572 6167 6520 5374 6174 7573 5d28  overage Status](
+000003c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000003d0: 6c64 732e 696f 2f63 6f76 6572 616c 6c73  lds.io/coveralls
+000003e0: 436f 7665 7261 6765 2f67 6974 6875 622f  Coverage/github/
+000003f0: 6479 6e6f 626f 2f6e 6f72 6d63 6170 3f6c  dynobo/normcap?l
+00000400: 6162 656c 3d54 6573 7425 3230 636f 7665  abel=Test%20cove
+00000410: 7261 6765 2662 7261 6e63 683d 6d61 696e  rage&branch=main
+00000420: 295d 2868 7474 7073 3a2f 2f63 6f76 6572  )](https://cover
+00000430: 616c 6c73 2e69 6f2f 6769 7468 7562 2f64  alls.io/github/d
+00000440: 796e 6f62 6f2f 6e6f 726d 6361 7029 5c6e  ynobo/normcap)\n
+00000450: 5b21 5b43 6f64 6551 4c5d 2868 7474 7073  [![CodeQL](https
+00000460: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000470: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
+00000480: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
+00000490: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
+000004a0: 636f 6465 716c 2d61 6e61 6c79 7369 732e  codeql-analysis.
+000004b0: 796d 6c3f 6272 616e 6368 3d6d 6169 6e26  yml?branch=main&
+000004c0: 6c61 6265 6c3d 436f 6465 514c 295d 2868  label=CodeQL)](h
+000004d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004e0: 6d2f 6479 6e6f 626f 2f6e 6f72 6d63 6170  m/dynobo/normcap
+000004f0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000500: 7773 2f63 6f64 6571 6c2d 616e 616c 7973  ws/codeql-analys
+00000510: 6973 2e79 6d6c 295c 6e5c 6e5b 215b 4769  is.yml)\n\n[![Gi
+00000520: 7448 7562 5d28 6874 7470 733a 2f2f 696d  tHub](https://im
+00000530: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000540: 6875 622f 646f 776e 6c6f 6164 732f 6479  hub/downloads/dy
+00000550: 6e6f 626f 2f6e 6f72 6d63 6170 2f74 6f74  nobo/normcap/tot
+00000560: 616c 3f6c 6162 656c 3d47 6974 6875 6225  al?label=Github%
+00000570: 3230 646f 776e 6c6f 6164 7326 636f 6c6f  20downloads&colo
+00000580: 723d 626c 7565 295d 2868 7474 7073 3a2f  r=blue)](https:/
+00000590: 2f67 6974 6875 622e 636f 6d2f 6479 6e6f  /github.com/dyno
+000005a0: 626f 2f6e 6f72 6d63 6170 2f72 656c 6561  bo/normcap/relea
+000005b0: 7365 7329 5c6e 5b21 5b50 7950 695d 2868  ses)\n[![PyPi](h
+000005c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000005d0: 6473 2e69 6f2f 7079 7069 2f64 6d2f 6e6f  ds.io/pypi/dm/no
+000005e0: 726d 6361 703f 6c61 6265 6c3d 5079 5069  rmcap?label=PyPi
+000005f0: 2532 3064 6f77 6e6c 6f61 6473 2663 6f6c  %20downloads&col
+00000600: 6f72 3d62 6c75 6529 5d28 6874 7470 733a  or=blue)](https:
+00000610: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000620: 6374 2f6e 6f72 6d63 6170 295c 6e5b 215b  ct/normcap)\n[![
+00000630: 466c 6174 6875 625d 2868 7474 7073 3a2f  Flathub](https:/
+00000640: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000650: 666c 6174 6875 622f 646f 776e 6c6f 6164  flathub/download
+00000660: 732f 636f 6d2e 6769 7468 7562 2e64 796e  s/com.github.dyn
+00000670: 6f62 6f2e 6e6f 726d 6361 703f 6c61 6265  obo.normcap?labe
+00000680: 6c3d 466c 6174 6875 6225 3230 646f 776e  l=Flathub%20down
+00000690: 6c6f 6164 7326 636f 6c6f 723d 626c 7565  loads&color=blue
+000006a0: 295d 2868 7474 7073 3a2f 2f66 6c61 7468  )](https://flath
+000006b0: 7562 2e6f 7267 2f61 7070 732f 6465 7461  ub.org/apps/deta
+000006c0: 696c 732f 636f 6d2e 6769 7468 7562 2e64  ils/com.github.d
+000006d0: 796e 6f62 6f2e 6e6f 726d 6361 7029 5c6e  ynobo.normcap)\n
+000006e0: 5b21 5b41 5552 5d28 6874 7470 733a 2f2f  [![AUR](https://
+000006f0: 696d 672e 7368 6965 6c64 732e 696f 2f61  img.shields.io/a
+00000700: 7572 2f76 6f74 6573 2f6e 6f72 6d63 6170  ur/votes/normcap
+00000710: 3f6c 6162 656c 3d41 5552 2532 3076 6f74  ?label=AUR%20vot
+00000720: 6573 2663 6f6c 6f72 3d62 6c75 6529 5d28  es&color=blue)](
+00000730: 6874 7470 733a 2f2f 6175 722e 6172 6368  https://aur.arch
+00000740: 6c69 6e75 782e 6f72 672f 7061 636b 6167  linux.org/packag
+00000750: 6573 2f6e 6f72 6d63 6170 295c 6e5c 6e3c  es/normcap)\n\n<
+00000760: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000770: 7777 772e 6275 796d 6561 636f 6666 6565  www.buymeacoffee
+00000780: 2e63 6f6d 2f64 796e 6f62 6f22 2074 6172  .com/dynobo" tar
+00000790: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+000007a0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+000007b0: 646e 2e62 7579 6d65 6163 6f66 6665 652e  dn.buymeacoffee.
+000007c0: 636f 6d2f 6275 7474 6f6e 732f 7632 2f64  com/buttons/v2/d
+000007d0: 6566 6175 6c74 2d79 656c 6c6f 772e 706e  efault-yellow.pn
+000007e0: 6722 2061 6c74 3d22 4275 7920 4d65 2041  g" alt="Buy Me A
+000007f0: 2043 6f66 6665 6522 2073 7479 6c65 3d22   Coffee" style="
+00000800: 6865 6967 6874 3a20 3430 7078 2021 696d  height: 40px !im
+00000810: 706f 7274 616e 743b 2220 3e3c 2f61 3e5c  portant;" ></a>\
+00000820: 6e5c 6e2a 2a4c 696e 6b73 3a2a 2a20 5b53  n\n**Links:** [S
+00000830: 6f75 7263 6520 436f 6465 5d28 6874 7470  ource Code](http
+00000840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000850: 796e 6f62 6f2f 6e6f 726d 6361 7029 207c  ynobo/normcap) |
+00000860: 5c6e 5b44 6f63 756d 656e 7461 7469 6f6e  \n[Documentation
+00000870: 5d28 6874 7470 733a 2f2f 6479 6e6f 626f  ](https://dynobo
+00000880: 2e67 6974 6875 622e 696f 2f6e 6f72 6d63  .github.io/normc
+00000890: 6170 2f29 207c 5c6e 5b46 4151 735d 2868  ap/) |\n[FAQs](h
+000008a0: 7474 7073 3a2f 2f64 796e 6f62 6f2e 6769  ttps://dynobo.gi
+000008b0: 7468 7562 2e69 6f2f 6e6f 726d 6361 702f  thub.io/normcap/
+000008c0: 2366 6171 7329 207c 5c6e 5b52 656c 6561  #faqs) |\n[Relea
+000008d0: 7365 735d 2868 7474 7073 3a2f 2f67 6974  ses](https://git
+000008e0: 6875 622e 636f 6d2f 6479 6e6f 626f 2f6e  hub.com/dynobo/n
+000008f0: 6f72 6d63 6170 2f72 656c 6561 7365 7329  ormcap/releases)
+00000900: 207c 5c6e 5b43 6861 6e67 656c 6f67 5d28   |\n[Changelog](
+00000910: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000920: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
+00000930: 702f 626c 6f62 2f6d 6169 6e2f 4348 414e  p/blob/main/CHAN
+00000940: 4745 4c4f 4729 5c6e 5c6e 5b21 5b53 6372  GELOG)\n\n[![Scr
+00000950: 6565 6e63 6173 745d 2868 7474 7073 3a2f  eencast](https:/
+00000960: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+00000970: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000980: 6f6d 2f31 3130 3731 3837 362f 3138 3937  om/11071876/1897
+00000990: 3637 3538 352d 3862 6334 3563 3138 2d38  67585-8bc45c18-8
+000009a0: 3339 322d 3431 3164 2d38 3464 632d 6365  392-411d-84dc-ce
+000009b0: 6631 6362 3564 6263 3437 2e67 6966 295d  f1cb5dbc47.gif)]
+000009c0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+000009d0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000009e0: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
+000009f0: 702f 6d61 696e 2f61 7373 6574 732f 6e6f  p/main/assets/no
+00000a00: 726d 6361 702e 6769 6629 5c6e 5c6e 2323  rmcap.gif)\n\n##
+00000a10: 2051 7569 636b 7374 6172 745c 6e5c 6e49   Quickstart\n\nI
+00000a20: 6e73 7461 6c6c 2061 2070 7265 6275 696c  nstall a prebuil
+00000a30: 7420 7265 6c65 6173 653a 5c6e 5c6e 2d20  t release:\n\n- 
+00000a40: 2a2a 5769 6e64 6f77 732a 2a3a 5c6e 2020  **Windows**:\n  
+00000a50: 5b4e 6f72 6d43 6170 2d30 2e34 2e31 2d78  [NormCap-0.4.1-x
+00000a60: 3836 5f36 342d 5769 6e64 6f77 732e 6d73  86_64-Windows.ms
+00000a70: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+00000a80: 622e 636f 6d2f 6479 6e6f 626f 2f6e 6f72  b.com/dynobo/nor
+00000a90: 6d63 6170 2f72 656c 6561 7365 732f 646f  mcap/releases/do
+00000aa0: 776e 6c6f 6164 2f76 302e 342e 312f 4e6f  wnload/v0.4.1/No
+00000ab0: 726d 4361 702d 302e 342e 312d 7838 365f  rmCap-0.4.1-x86_
+00000ac0: 3634 2d57 696e 646f 7773 2e6d 7369 295c  64-Windows.msi)\
+00000ad0: 6e2d 202a 2a4c 696e 7578 2a2a 3a5c 6e20  n- **Linux**:\n 
+00000ae0: 205b 4e6f 726d 4361 702d 302e 342e 312d   [NormCap-0.4.1-
+00000af0: 7838 365f 3634 2e41 7070 496d 6167 655d  x86_64.AppImage]
+00000b00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000b10: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
+00000b20: 6170 2f72 656c 6561 7365 732f 646f 776e  ap/releases/down
+00000b30: 6c6f 6164 2f76 302e 342e 312f 4e6f 726d  load/v0.4.1/Norm
+00000b40: 4361 702d 302e 342e 312d 7838 365f 3634  Cap-0.4.1-x86_64
+00000b50: 2e41 7070 496d 6167 6529 5c6e 2d20 2a2a  .AppImage)\n- **
+00000b60: 6d61 634f 532a 2a20 2878 3836 2920 c2b9  macOS** (x86) ..
+00000b70: 3a5c 6e20 205b 4e6f 726d 4361 702d 302e  :\n  [NormCap-0.
+00000b80: 342e 312d 7838 365f 3634 2d6d 6163 4f53  4.1-x86_64-macOS
+00000b90: 2e64 6d67 5d28 6874 7470 733a 2f2f 6769  .dmg](https://gi
+00000ba0: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
+00000bb0: 6e6f 726d 6361 702f 7265 6c65 6173 6573  normcap/releases
+00000bc0: 2f64 6f77 6e6c 6f61 642f 7630 2e34 2e31  /download/v0.4.1
+00000bd0: 2f4e 6f72 6d43 6170 2d30 2e34 2e31 2d78  /NormCap-0.4.1-x
+00000be0: 3836 5f36 342d 6d61 634f 532e 646d 6729  86_64-macOS.dmg)
+00000bf0: 5c6e 2d20 2a2a 6d61 634f 532a 2a20 284d  \n- **macOS** (M
+00000c00: 3129 20c2 b9c2 b7c2 b23a 5c6e 2020 5b4e  1) ......:\n  [N
+00000c10: 6f72 6d43 6170 2d30 2e34 2e31 2d61 726d  ormCap-0.4.1-arm
+00000c20: 3634 2d6d 6163 4f53 2e64 6d67 5d28 6874  64-macOS.dmg](ht
+00000c30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000c40: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
+00000c50: 7265 6c65 6173 6573 2f64 6f77 6e6c 6f61  releases/downloa
+00000c60: 642f 7630 2e34 2e31 2f4e 6f72 6d43 6170  d/v0.4.1/NormCap
+00000c70: 2d30 2e34 2e31 2d61 726d 3634 2d6d 6163  -0.4.1-arm64-mac
+00000c80: 4f53 2e64 6d67 295c 6e20 205c 5c5c 6e20  OS.dmg)\n  \\\n 
+00000c90: 203c 7375 623e 313a 204f 6e20 6d61 634f   <sub>1: On macO
+00000ca0: 532c 2061 6c6c 6f77 2074 6865 2075 6e73  S, allow the uns
+00000cb0: 6967 6e65 6420 6170 706c 6963 6174 696f  igned applicatio
+00000cc0: 6e20 6f6e 2066 6972 7374 2073 7461 7274  n on first start
+00000cd0: 3a20 2253 7973 7465 6d5c 6e20 2050 7265  : "System\n  Pre
+00000ce0: 6665 7265 6e63 6573 2220 e286 9220 2253  ferences" ... "S
+00000cf0: 6563 7572 6974 7920 2620 5072 6976 6163  ecurity & Privac
+00000d00: 7922 20e2 8692 2022 4765 6e65 7261 6c22  y" ... "General"
+00000d10: 20e2 8692 2022 4f70 656e 2061 6e79 7761   ... "Open anywa
+00000d20: 7922 2e20 596f 7520 6d69 6768 7420 616c  y". You might al
+00000d30: 736f 206e 6565 645c 6e20 2074 6f20 616c  so need\n  to al
+00000d40: 6c6f 7720 4e6f 726d 4361 7020 746f 2074  low NormCap to t
+00000d50: 616b 6520 7363 7265 656e 7368 6f74 732e  ake screenshots.
+00000d60: 5c6e 2020 5b23 3133 355d 2868 7474 7073  \n  [#135](https
+00000d70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6479  ://github.com/dy
+00000d80: 6e6f 626f 2f6e 6f72 6d63 6170 2f69 7373  nobo/normcap/iss
+00000d90: 7565 732f 3133 3529 3c62 723e 2032 3a20  ues/135)<br> 2: 
+00000da0: 4d69 6768 7420 6265 2061 7661 696c 6162  Might be availab
+00000db0: 6c65 2061 2062 6974 5c6e 2020 6465 6c61  le a bit\n  dela
+00000dc0: 7965 642c 2061 7320 6974 2069 7320 6375  yed, as it is cu
+00000dd0: 7272 656e 746c 7920 6275 696c 6420 6d61  rrently build ma
+00000de0: 6e75 616c 6c79 2e20 2854 6878 2c5c 6e20  nually. (Thx,\n 
+00000df0: 205b 4054 616b 7269 6e5d 2868 7474 7073   [@Takrin](https
+00000e00: 3a2f 2f67 6974 6875 622e 636f 6d2f 5461  ://github.com/Ta
+00000e10: 6b72 696e 2921 293c 2f73 7562 3e5c 6e5c  krin)!)</sub>\n\
+00000e20: 6e49 6e73 7461 6c6c 2066 726f 6d20 7265  nInstall from re
+00000e30: 706f 7369 746f 7269 6573 3a5c 6e5c 6e2d  positories:\n\n-
+00000e40: 202a 2a57 696e 646f 7773 2a2a 3a20 496e   **Windows**: In
+00000e50: 7374 616c 6c20 6672 6f6d 5c6e 2020 5b4d  stall from\n  [M
+00000e60: 6963 726f 736f 6674 2053 746f 7265 5d28  icrosoft Store](
+00000e70: 6874 7470 733a 2f2f 6170 7073 2e6d 6963  https://apps.mic
+00000e80: 726f 736f 6674 2e63 6f6d 2f73 746f 7265  rosoft.com/store
+00000e90: 2f64 6574 6169 6c2f 6e6f 726d 6361 702f  /detail/normcap/
+00000ea0: 5850 444c 4a4e 4234 4236 4332 5a52 292e  XPDLJNB4B6C2ZR).
+00000eb0: 5c6e 2d20 2a2a 4172 6368 202f 204d 616e  \n- **Arch / Man
+00000ec0: 6a61 726f 2a2a 3a20 496e 7374 616c 6c20  jaro**: Install 
+00000ed0: 7468 655c 6e20 205b 606e 6f72 6d63 6170  the\n  [`normcap
+00000ee0: 605d 2868 7474 7073 3a2f 2f61 7572 2e61  `](https://aur.a
+00000ef0: 7263 686c 696e 7578 2e6f 7267 2f70 6163  rchlinux.org/pac
+00000f00: 6b61 6765 732f 6e6f 726d 6361 7029 2070  kages/normcap) p
+00000f10: 6163 6b61 6765 2066 726f 6d20 4155 522e  ackage from AUR.
+00000f20: 5c6e 2d20 2a2a 466c 6174 5061 6b20 284c  \n- **FlatPak (L
+00000f30: 696e 7578 292a 2a3a 2049 6e73 7461 6c6c  inux)**: Install
+00000f40: 5c6e 2020 5b63 6f6d 2e67 6974 6875 622e  \n  [com.github.
+00000f50: 6479 6e6f 626f 2e6e 6f72 6d63 6170 5d28  dynobo.normcap](
+00000f60: 6874 7470 733a 2f2f 666c 6174 6875 622e  https://flathub.
+00000f70: 6f72 672f 6170 7073 2f64 6574 6169 6c73  org/apps/details
+00000f80: 2f63 6f6d 2e67 6974 6875 622e 6479 6e6f  /com.github.dyno
+00000f90: 626f 2e6e 6f72 6d63 6170 295c 6e20 2066  bo.normcap)\n  f
+00000fa0: 726f 6d20 466c 6174 4875 622e 5c6e 5c6e  rom FlatHub.\n\n
+00000fb0: 4966 2079 6f75 2065 7870 6572 6965 6e63  If you experienc
+00000fc0: 6520 6973 7375 6573 2070 6c65 6173 6520  e issues please 
+00000fd0: 6c6f 6f6b 2061 7420 7468 655c 6e5b 4641  look at the\n[FA
+00000fe0: 5173 5d28 6874 7470 733a 2f2f 6479 6e6f  Qs](https://dyno
+00000ff0: 626f 2e67 6974 6875 622e 696f 2f6e 6f72  bo.github.io/nor
+00001000: 6d63 6170 2f23 6661 7173 2920 6f72 5c6e  mcap/#faqs) or\n
+00001010: 5b6f 7065 6e20 616e 2069 7373 7565 5d28  [open an issue](
+00001020: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001030: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
+00001040: 702f 6973 7375 6573 292e 5c6e 5c6e 2323  p/issues).\n\n##
+00001050: 2050 7974 686f 6e20 7061 636b 6167 655c   Python package\
+00001060: 6e5c 6e41 7320 616e 205f 616c 7465 726e  n\nAs an _altern
+00001070: 6174 6976 655f 2074 6f20 6120 7072 6562  ative_ to a preb
+00001080: 7569 6c74 2070 6163 6b61 6765 2079 6f75  uilt package you
+00001090: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
+000010a0: 5c6e 5b4e 6f72 6d43 6170 2050 7974 686f  \n[NormCap Pytho
+000010b0: 6e20 7061 636b 6167 655d 2868 7474 7073  n package](https
+000010c0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000010d0: 6563 742f 6e6f 726d 6361 702f 2920 666f  ect/normcap/) fo
+000010e0: 7220 2a2a 5079 7468 6f6e 203e 3d33 2e39  r **Python >=3.9
+000010f0: 2a2a 3a5c 6e5c 6e23 2323 2320 4f6e 204c  **:\n\n#### On L
+00001100: 696e 7578 5c6e 5c6e 6060 6073 685c 6e23  inux\n\n```sh\n#
+00001110: 2049 6e73 7461 6c6c 2064 6570 656e 6465   Install depende
+00001120: 6e63 6965 7320 2855 6275 6e74 752f 4465  ncies (Ubuntu/De
+00001130: 6269 616e 295c 6e73 7564 6f20 6170 7420  bian)\nsudo apt 
+00001140: 696e 7374 616c 6c20 6275 696c 642d 6573  install build-es
+00001150: 7365 6e74 6961 6c20 7465 7373 6572 6163  sential tesserac
+00001160: 742d 6f63 7220 7465 7373 6572 6163 742d  t-ocr tesseract-
+00001170: 6f63 722d 656e 6720 6c69 6274 6573 7365  ocr-eng libtesse
+00001180: 7261 6374 2d64 6576 206c 6962 6c65 7074  ract-dev liblept
+00001190: 6f6e 6963 612d 6465 7620 776c 2d63 6c69  onica-dev wl-cli
+000011a0: 7062 6f61 7264 5c6e 5c6e 2323 2049 6e73  pboard\n\n## Ins
+000011b0: 7461 6c6c 2064 6570 656e 6465 6e63 6965  tall dependencie
+000011c0: 7320 2841 7263 6829 5c6e 7375 646f 2070  s (Arch)\nsudo p
+000011d0: 6163 6d61 6e20 2d53 2074 6573 7365 7261  acman -S tessera
+000011e0: 6374 2074 6573 7365 7261 6374 2d64 6174  ct tesseract-dat
+000011f0: 612d 656e 6720 776c 2d63 6c69 7062 6f61  a-eng wl-clipboa
+00001200: 7264 5c6e 5c6e 2323 2049 6e73 7461 6c6c  rd\n\n## Install
+00001210: 2064 6570 656e 6465 6e63 6965 7320 2846   dependencies (F
+00001220: 6564 6f72 6129 5c6e 7375 646f 2064 6e66  edora)\nsudo dnf
+00001230: 2069 6e73 7461 6c6c 2074 6573 7365 7261   install tessera
+00001240: 6374 2077 6c2d 636c 6970 626f 6172 645c  ct wl-clipboard\
+00001250: 6e5c 6e23 2320 496e 7374 616c 6c20 6465  n\n## Install de
+00001260: 7065 6e64 656e 6369 6573 2028 6f70 656e  pendencies (open
+00001270: 5355 5345 295c 6e73 7564 6f20 7a79 7070  SUSE)\nsudo zypp
+00001280: 6572 2069 6e73 7461 6c6c 2070 7974 686f  er install pytho
+00001290: 6e33 2d64 6576 656c 2074 6573 7365 7261  n3-devel tessera
+000012a0: 6374 2d6f 6372 2074 6573 7365 7261 6374  ct-ocr tesseract
+000012b0: 2d6f 6372 2d64 6576 656c 2077 6c2d 636c  -ocr-devel wl-cl
+000012c0: 6970 626f 6172 645c 6e5c 6e23 2049 6e73  ipboard\n\n# Ins
+000012d0: 7461 6c6c 206e 6f72 6d63 6170 5c6e 7069  tall normcap\npi
+000012e0: 7020 696e 7374 616c 6c20 6e6f 726d 6361  p install normca
+000012f0: 705c 6e5c 6e23 2052 756e 5c6e 2e2f 6e6f  p\n\n# Run\n./no
+00001300: 726d 6361 705c 6e60 6060 5c6e 5c6e 2323  rmcap\n```\n\n##
+00001310: 2323 204f 6e20 6d61 634f 535c 6e5c 6e60  ## On macOS\n\n`
+00001320: 6060 7368 5c6e 2320 496e 7374 616c 6c20  ``sh\n# Install 
+00001330: 6465 7065 6e64 656e 6369 6573 5c6e 6272  dependencies\nbr
+00001340: 6577 2069 6e73 7461 6c6c 2074 6573 7365  ew install tesse
+00001350: 7261 6374 2074 6573 7365 7261 6374 2d6c  ract tesseract-l
+00001360: 616e 675c 6e5c 6e23 2049 6e73 7461 6c6c  ang\n\n# Install
+00001370: 206e 6f72 6d63 6170 5c6e 7069 7020 696e   normcap\npip in
+00001380: 7374 616c 6c20 6e6f 726d 6361 705c 6e5c  stall normcap\n\
+00001390: 6e23 2052 756e 5c6e 2e2f 6e6f 726d 6361  n# Run\n./normca
+000013a0: 705c 6e60 6060 5c6e 5c6e 2323 2323 204f  p\n```\n\n#### O
+000013b0: 6e20 5769 6e64 6f77 735c 6e5c 6e31 5c5c  n Windows\n\n1\\
+000013c0: 2e20 496e 7374 616c 6c20 6054 6573 7365  . Install `Tesse
+000013d0: 7261 6374 2035 6020 6279 2075 7369 6e67  ract 5` by using
+000013e0: 2074 6865 5c6e 5b69 6e73 7461 6c6c 6572   the\n[installer
+000013f0: 2070 726f 7669 6465 6420 6279 2055 4220   provided by UB 
+00001400: 4d61 6e6e 6865 696d 5d28 6874 7470 733a  Mannheim](https:
+00001410: 2f2f 6769 7468 7562 2e63 6f6d 2f55 422d  //github.com/UB-
+00001420: 4d61 6e6e 6865 696d 2f74 6573 7365 7261  Mannheim/tessera
+00001430: 6374 2f77 696b 6929 2e5c 6e5c 6e32 5c5c  ct/wiki).\n\n2\\
+00001440: 2e20 4164 6a75 7374 2065 6e76 6972 6f6e  . Adjust environ
+00001450: 6d65 6e74 2076 6172 6961 626c 6573 3a5c  ment variables:\
+00001460: 6e5c 6e2d 2043 7265 6174 6520 616e 2065  n\n- Create an e
+00001470: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00001480: 626c 6520 6054 4553 5344 4154 415f 5052  ble `TESSDATA_PR
+00001490: 4546 4958 6020 616e 6420 7365 7420 6974  EFIX` and set it
+000014a0: 2074 6f20 5465 7373 6572 6163 745c 2773   to Tesseract\'s
+000014b0: 2064 6174 615c 6e20 2066 6f6c 6465 722c   data\n  folder,
+000014c0: 2065 2e67 2e3a 5c6e 5c6e 2020 6060 6063   e.g.:\n\n  ```c
+000014d0: 6d64 5c6e 2020 7365 7478 2054 4553 5344  md\n  setx TESSD
+000014e0: 4154 415f 5052 4546 4958 2022 433a 5c5c  ATA_PREFIX "C:\\
+000014f0: 5072 6f67 7261 6d20 4669 6c65 735c 5c54  Program Files\\T
+00001500: 6573 7365 7261 6374 2d4f 4352 5c5c 7465  esseract-OCR\\te
+00001510: 7373 6461 7461 225c 6e20 2060 6060 5c6e  ssdata"\n  ```\n
+00001520: 5c6e 2d20 4170 7065 6e64 2054 6573 7365  \n- Append Tesse
+00001530: 7261 6374 5c27 7320 6c6f 6361 7469 6f6e  ract\'s location
+00001540: 2074 6f20 7468 6520 656e 7669 726f 6e6d   to the environm
+00001550: 656e 7420 7661 7269 6162 6c65 2060 5061  ent variable `Pa
+00001560: 7468 602c 2065 2e67 2e3a 5c6e 5c6e 2020  th`, e.g.:\n\n  
+00001570: 6060 6063 6d64 5c6e 2020 7365 7478 2050  ```cmd\n  setx P
+00001580: 6174 6820 2225 5061 7468 253b 433a 5c5c  ath "%Path%;C:\\
+00001590: 5072 6f67 7261 6d20 4669 6c65 735c 5c54  Program Files\\T
+000015a0: 6573 7365 7261 6374 2d4f 4352 225c 6e20  esseract-OCR"\n 
+000015b0: 2060 6060 5c6e 5c6e 2d20 4d61 6b65 2073   ```\n\n- Make s
+000015c0: 7572 6520 746f 2063 6c6f 7365 2061 6e64  ure to close and
+000015d0: 2072 656f 7065 6e20 796f 7572 2063 7572   reopen your cur
+000015e0: 7265 6e74 2074 6572 6d69 6e61 6c20 7769  rent terminal wi
+000015f0: 6e64 6f77 2074 6f20 6170 706c 7920 7468  ndow to apply th
+00001600: 6520 6e65 7720 7661 7269 6162 6c65 732e  e new variables.
+00001610: 5c6e 2020 5465 7374 2069 7420 6279 2072  \n  Test it by r
+00001620: 756e 6e69 6e67 3a5c 6e5c 6e20 2060 6060  unning:\n\n  ```
+00001630: 636d 645c 6e20 2074 6573 7365 7261 6374  cmd\n  tesseract
+00001640: 202d 2d6c 6973 742d 6c61 6e67 735c 6e20   --list-langs\n 
+00001650: 2060 6060 5c6e 5c6e 335c 5c2e 2049 6e73   ```\n\n3\\. Ins
+00001660: 7461 6c6c 2061 6e64 2072 756e 204e 6f72  tall and run Nor
+00001670: 6d43 6170 3a5c 6e5c 6e60 6060 6261 7368  mCap:\n\n```bash
+00001680: 5c6e 2320 496e 7374 616c 6c20 6e6f 726d  \n# Install norm
+00001690: 6361 705c 6e70 6970 2069 6e73 7461 6c6c  cap\npip install
+000016a0: 206e 6f72 6d63 6170 5c6e 5c6e 2320 5275   normcap\n\n# Ru
+000016b0: 6e5c 6e6e 6f72 6d63 6170 5c6e 6060 605c  n\nnormcap\n```\
+000016c0: 6e5c 6e23 2320 5768 7920 224e 6f72 6d43  n\n## Why "NormC
+000016d0: 6170 223f 5c6e 5c6e 5365 6520 5b58 4b43  ap"?\n\nSee [XKC
+000016e0: 445d 2868 7474 7073 3a2f 2f78 6b63 642e  D](https://xkcd.
+000016f0: 636f 6d29 3a5c 6e5c 6e5b 215b 436f 6d69  com):\n\n[![Comi
+00001700: 635d 2868 7474 7073 3a2f 2f69 6d67 732e  c](https://imgs.
+00001710: 786b 6364 2e63 6f6d 2f63 6f6d 6963 732f  xkcd.com/comics/
+00001720: 6e6f 726d 5f6e 6f72 6d61 6c5f 6669 6c65  norm_normal_file
+00001730: 5f66 6f72 6d61 742e 706e 6729 5d28 6874  _format.png)](ht
+00001740: 7470 733a 2f2f 786b 6364 2e63 6f6d 2f32  tps://xkcd.com/2
+00001750: 3131 362f 295c 6e5c 6e23 2320 4465 7665  116/)\n\n## Deve
+00001760: 6c6f 706d 656e 745c 6e5c 6e50 7265 7265  lopment\n\nPrere
+00001770: 7175 6973 6974 6573 2066 6f72 2073 6574  quisites for set
+00001780: 7469 6e67 2075 7020 6120 6465 7665 6c6f  ting up a develo
+00001790: 706d 656e 7420 656e 7669 726f 6e6d 656e  pment environmen
+000017a0: 7420 6172 653a 202a 2a50 7974 686f 6e20  t are: **Python 
+000017b0: 3e3d 332e 392a 2a2c 5c6e 2a2a 506f 6574  >=3.9**,\n**Poet
+000017c0: 7279 3e3d 312e 332e 322a 2a20 616e 6420  ry>=1.3.2** and 
+000017d0: 2a2a 5465 7373 6572 6163 742a 2a20 2869  **Tesseract** (i
+000017e0: 6e63 6c2e 202a 2a6c 616e 6775 6167 6520  ncl. **language 
+000017f0: 6461 7461 2a2a 292e 5c6e 5c6e 6060 6073  data**).\n\n```s
+00001800: 685c 6e23 2043 6c6f 6e65 2072 6570 6f73  h\n# Clone repos
+00001810: 6974 6f72 795c 6e67 6974 2063 6c6f 6e65  itory\ngit clone
+00001820: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001830: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
+00001840: 6170 2e67 6974 5c6e 5c6e 2320 4368 616e  ap.git\n\n# Chan
+00001850: 6765 2069 6e74 6f20 7072 6f6a 6563 7420  ge into project 
+00001860: 6469 7265 6374 6f72 795c 6e63 6420 6e6f  directory\ncd no
+00001870: 726d 6361 705c 6e5c 6e23 2043 7265 6174  rmcap\n\n# Creat
+00001880: 6520 7669 7274 7561 6c20 656e 7620 616e  e virtual env an
+00001890: 6420 696e 7374 616c 6c20 6465 7065 6e64  d install depend
+000018a0: 656e 6369 6573 5c6e 706f 6574 7279 2069  encies\npoetry i
+000018b0: 6e73 7461 6c6c 5c6e 5c6e 2320 5265 6769  nstall\n\n# Regi
+000018c0: 7374 6572 2070 7265 2d63 6f6d 6d69 7420  ster pre-commit 
+000018d0: 686f 6f6b 5c6e 706f 6574 7279 2072 756e  hook\npoetry run
+000018e0: 2070 7265 2d63 6f6d 6d69 7420 696e 7374   pre-commit inst
+000018f0: 616c 6c5c 6e5c 6e23 2052 756e 204e 6f72  all\n\n# Run Nor
+00001900: 6d43 6170 2069 6e20 7669 7274 7561 6c20  mCap in virtual 
+00001910: 656e 765c 6e70 6f65 7472 7920 7275 6e20  env\npoetry run 
+00001920: 7079 7468 6f6e 202d 6d20 6e6f 726d 6361  python -m normca
+00001930: 705c 6e60 6060 5c6e 5c6e 2323 2043 7265  p\n```\n\n## Cre
+00001940: 6469 7473 5c6e 5c6e 5468 6973 2070 726f  dits\n\nThis pro
+00001950: 6a65 6374 2075 7365 7320 7468 6520 666f  ject uses the fo
+00001960: 6c6c 6f77 696e 6720 6e6f 6e2d 7374 616e  llowing non-stan
+00001970: 6461 7264 206c 6962 7261 7269 6573 3a5c  dard libraries:\
+00001980: 6e5c 6e2d 205b 7079 7369 6465 365d 2868  n\n- [pyside6](h
+00001990: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000019a0: 7072 6f6a 6563 742f 5079 5369 6465 362f  project/PySide6/
+000019b0: 2920 5f2d 2062 696e 6469 6e67 7320 666f  ) _- bindings fo
+000019c0: 7220 5174 2055 4920 4672 616d 6577 6f72  r Qt UI Framewor
+000019d0: 6b5f 5c6e 2d20 5b6a 6565 706e 6579 5d28  k_\n- [jeepney](
+000019e0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000019f0: 2f70 726f 6a65 6374 2f6a 6565 706e 6579  /project/jeepney
+00001a00: 2f29 205f 2d20 4442 5553 2063 6c69 656e  /) _- DBUS clien
+00001a10: 745f 5c6e 5c6e 416e 6420 6974 2064 6570  t_\n\nAnd it dep
+00001a20: 656e 6473 206f 6e20 6578 7465 726e 616c  ends on external
+00001a30: 2073 6f66 7477 6172 653a 5c6e 5c6e 2d20   software:\n\n- 
+00001a40: 5b74 6573 7365 7261 6374 5d28 6874 7470  [tesseract](http
+00001a50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00001a60: 6573 7365 7261 6374 2d6f 6372 2f74 6573  esseract-ocr/tes
+00001a70: 7365 7261 6374 2920 2d20 5f4f 4352 2065  seract) - _OCR e
+00001a80: 6e67 696e 655f 5c6e 2d20 5b77 6c2d 636c  ngine_\n- [wl-cl
+00001a90: 6970 626f 6172 645d 2868 7474 7073 3a2f  ipboard](https:/
+00001aa0: 2f67 6974 6875 622e 636f 6d2f 6275 6761  /github.com/buga
+00001ab0: 6576 632f 776c 2d63 6c69 7062 6f61 7264  evc/wl-clipboard
+00001ac0: 2920 2d20 5f57 6179 6c61 6e64 2063 6c69  ) - _Wayland cli
+00001ad0: 7062 6f61 7264 5c6e 2020 7574 696c 6974  pboard\n  utilit
+00001ae0: 6965 735f 5c6e 5c6e 5061 636b 6167 696e  ies_\n\nPackagin
+00001af0: 6720 6973 2064 6f6e 6520 7769 7468 3a5c  g is done with:\
+00001b00: 6e5c 6e2d 205b 6272 6965 6663 6173 655d  n\n- [briefcase]
+00001b10: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00001b20: 672f 7072 6f6a 6563 742f 6272 6965 6663  g/project/briefc
+00001b30: 6173 652f 2920 5f2d 2063 6f6e 7665 7274  ase/) _- convert
+00001b40: 696e 6720 5079 7468 6f6e 2070 726f 6a65  ing Python proje
+00001b50: 6374 7320 696e 746f 5f5c 6e20 205f 7374  cts into_\n  _st
+00001b60: 616e 6461 6c6f 6e65 2061 7070 735f 5c6e  andalone apps_\n
+00001b70: 5c6e 5468 616e 6b73 2074 6f20 7468 6520  \nThanks to the 
+00001b80: 6d61 696e 7461 696e 6572 7320 6f66 2074  maintainers of t
+00001b90: 686f 7365 206e 6963 6520 746f 6f6c 7321  hose nice tools!
+00001ba0: 5c6e 5c6e 2323 2053 696d 696c 6172 206f  \n\n## Similar o
+00001bb0: 7065 6e20 736f 7572 6365 2074 6f6f 6c73  pen source tools
+00001bc0: 5c6e 5c6e 4966 204e 6f72 6d43 6170 2064  \n\nIf NormCap d
+00001bd0: 6f65 736e 5c27 7420 6669 7420 796f 7572  oesn\'t fit your
+00001be0: 206e 6565 6473 2c20 7472 7920 7468 6f73   needs, try thos
+00001bf0: 6520 616c 7465 726e 6174 6976 6573 2028  e alternatives (
+00001c00: 6e6f 2070 6172 7469 6375 6c61 7220 6f72  no particular or
+00001c10: 6465 7229 3a5c 6e5c 6e2d 205b 5465 7874  der):\n\n- [Text
+00001c20: 536e 6174 6368 6572 5d28 6874 7470 733a  Snatcher](https:
+00001c30: 2f2f 6769 7468 7562 2e63 6f6d 2f52 616a  //github.com/Raj
+00001c40: 536f 6c61 692f 5465 7874 536e 6174 6368  Solai/TextSnatch
+00001c50: 6572 2920 284c 696e 7578 295c 6e2d 205b  er) (Linux)\n- [
+00001c60: 4772 6565 6e53 686f 745d 2868 7474 7073  GreenShot](https
+00001c70: 3a2f 2f67 6574 6772 6565 6e73 686f 742e  ://getgreenshot.
+00001c80: 6f72 672f 2920 284c 696e 7578 2c20 6d61  org/) (Linux, ma
+00001c90: 634f 5329 5c6e 2d20 5b54 6578 7453 686f  cOS)\n- [TextSho
+00001ca0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00001cb0: 622e 636f 6d2f 6961 6e7a 6861 6f30 352f  b.com/ianzhao05/
+00001cc0: 7465 7874 7368 6f74 2920 2857 696e 646f  textshot) (Windo
+00001cd0: 7773 295c 6e2d 205b 6749 6d61 6765 5265  ws)\n- [gImageRe
+00001ce0: 6164 6572 5d28 6874 7470 733a 2f2f 6769  ader](https://gi
+00001cf0: 7468 7562 2e63 6f6d 2f6d 616e 6973 616e  thub.com/manisan
+00001d00: 6472 6f2f 6749 6d61 6765 5265 6164 6572  dro/gImageReader
+00001d10: 2920 284c 696e 7578 2c20 5769 6e64 6f77  ) (Linux, Window
+00001d20: 7329 5c6e 2d20 5b43 6170 7475 7265 3254  s)\n- [Capture2T
+00001d30: 6578 745d 2868 7474 7073 3a2f 2f73 6f75  ext](https://sou
+00001d40: 7263 6566 6f72 6765 2e6e 6574 2f70 726f  rceforge.net/pro
+00001d50: 6a65 6374 732f 6361 7074 7572 6532 7465  jects/capture2te
+00001d60: 7874 2920 2857 696e 646f 7773 295c 6e2d  xt) (Windows)\n-
+00001d70: 205b 4672 6f67 5d28 6874 7470 733a 2f2f   [Frog](https://
+00001d80: 6769 7468 7562 2e63 6f6d 2f54 656e 6465  github.com/Tende
+00001d90: 724f 776c 2f46 726f 6729 2028 4c69 6e75  rOwl/Frog) (Linu
+00001da0: 7829 5c6e 2d20 5b54 6578 7469 6e61 746f  x)\n- [Textinato
+00001db0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00001dc0: 622e 636f 6d2f 5268 6574 5462 756c 6c2f  b.com/RhetTbull/
+00001dd0: 7465 7874 696e 6174 6f72 2920 286d 6163  textinator) (mac
+00001de0: 4f53 295c 6e2d 205b 5465 7874 2d47 7261  OS)\n- [Text-Gra
+00001df0: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
+00001e00: 622e 636f 6d2f 5468 654a 6f65 4669 6e2f  b.com/TheJoeFin/
+00001e10: 5465 7874 2d47 7261 6229 2028 5769 6e64  Text-Grab) (Wind
+00001e20: 6f77 7329 5c6e 2d20 5b64 7053 6372 6565  ows)\n- [dpScree
+00001e30: 6e4f 4352 5d28 6874 7470 733a 2f2f 6461  nOCR](https://da
+00001e40: 6e70 6c61 2e67 6974 6875 622e 696f 2f64  npla.github.io/d
+00001e50: 7073 6372 6565 6e6f 6372 2f29 2028 4c69  pscreenocr/) (Li
+00001e60: 6e75 782c 2057 696e 646f 7773 295c 6e5c  nux, Windows)\n\
+00001e70: 6e23 2320 4365 7274 6966 6963 6174 696f  n## Certificatio
+00001e80: 6e5c 6e5c 6e21 5b57 4f4d 4d5d 2868 7474  n\n\n![WOMM](htt
+00001e90: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00001ea0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00001eb0: 796e 6f62 6f2f 6c6d 6469 6167 2f6d 6173  ynobo/lmdiag/mas
+00001ec0: 7465 722f 6261 6467 652e 706e 6729 5c6e  ter/badge.png)\n
+00001ed0: 272c 0a20 2020 2027 6175 7468 6f72 273a  ',.    'author':
+00001ee0: 2027 6479 6e6f 626f 272c 0a20 2020 2027   'dynobo',.    '
+00001ef0: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
+00001f00: 6479 6e6f 626f 406d 6169 6c62 6f78 2e6f  dynobo@mailbox.o
+00001f10: 7267 272c 0a20 2020 2027 6d61 696e 7461  rg',.    'mainta
+00001f20: 696e 6572 273a 2027 4e6f 6e65 272c 0a20  iner': 'None',. 
+00001f30: 2020 2027 6d61 696e 7461 696e 6572 5f65     'maintainer_e
+00001f40: 6d61 696c 273a 2027 4e6f 6e65 272c 0a20  mail': 'None',. 
+00001f50: 2020 2027 7572 6c27 3a20 2768 7474 7073     'url': 'https
+00001f60: 3a2f 2f64 796e 6f62 6f2e 6769 7468 7562  ://dynobo.github
+00001f70: 2e69 6f2f 6e6f 726d 6361 702f 272c 0a20  .io/normcap/',. 
+00001f80: 2020 2027 7061 636b 6167 6573 273a 2070     'packages': p
+00001f90: 6163 6b61 6765 732c 0a20 2020 2027 7061  ackages,.    'pa
+00001fa0: 636b 6167 655f 6461 7461 273a 2070 6163  ckage_data': pac
+00001fb0: 6b61 6765 5f64 6174 612c 0a20 2020 2027  kage_data,.    '
+00001fc0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00001fd0: 273a 2069 6e73 7461 6c6c 5f72 6571 7569  ': install_requi
+00001fe0: 7265 732c 0a20 2020 2027 656e 7472 795f  res,.    'entry_
+00001ff0: 706f 696e 7473 273a 2065 6e74 7279 5f70  points': entry_p
+00002000: 6f69 6e74 732c 0a20 2020 2027 7079 7468  oints,.    'pyth
+00002010: 6f6e 5f72 6571 7569 7265 7327 3a20 273e  on_requires': '>
+00002020: 3d33 2e39 2c3c 332e 3132 272c 0a7d 0a0a  =3.9,<3.12',.}..
+00002030: 0a73 6574 7570 282a 2a73 6574 7570 5f6b  .setup(**setup_k
+00002040: 7761 7267 7329 0a                        wargs).
```

### Comparing `normcap-0.4.0/PKG-INFO` & `normcap-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 726d  : 2.1.Name: norm
 00000020: 6361 700a 5665 7273 696f 6e3a 2030 2e34  cap.Version: 0.4
-00000030: 2e30 0a53 756d 6d61 7279 3a20 4f43 522d  .0.Summary: OCR-
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4f43 522d  .1.Summary: OCR-
 00000040: 706f 7765 7265 6420 7363 7265 656e 2d63  powered screen-c
 00000050: 6170 7475 7265 2074 6f6f 6c20 746f 2063  apture tool to c
 00000060: 6170 7475 7265 2069 6e66 6f72 6d61 7469  apture informati
 00000070: 6f6e 2069 6e73 7465 6164 206f 6620 696d  on instead of im
 00000080: 6167 6573 2e0a 486f 6d65 2d70 6167 653a  ages..Home-page:
 00000090: 2068 7474 7073 3a2f 2f64 796e 6f62 6f2e   https://dynobo.
 000000a0: 6769 7468 7562 2e69 6f2f 6e6f 726d 6361  github.io/normca
@@ -69,450 +69,466 @@
 00000440: 6320 3a3a 204d 756c 7469 6d65 6469 6120  c :: Multimedia 
 00000450: 3a3a 2047 7261 7068 6963 7320 3a3a 2043  :: Graphics :: C
 00000460: 6170 7475 7265 203a 3a20 5363 7265 656e  apture :: Screen
 00000470: 2043 6170 7475 7265 0a43 6c61 7373 6966   Capture.Classif
 00000480: 6965 723a 2054 6f70 6963 203a 3a20 5574  ier: Topic :: Ut
 00000490: 696c 6974 6965 730a 5265 7175 6972 6573  ilities.Requires
 000004a0: 2d44 6973 743a 2050 7953 6964 6536 2d45  -Dist: PySide6-E
-000004b0: 7373 656e 7469 616c 7320 283e 3d36 2e34  ssentials (>=6.4
-000004c0: 2e31 2c3c 372e 302e 3029 0a52 6571 7569  .1,<7.0.0).Requi
-000004d0: 7265 732d 4469 7374 3a20 6365 7274 6966  res-Dist: certif
-000004e0: 6920 283e 3d32 3032 322e 3132 2e37 2c3c  i (>=2022.12.7,<
-000004f0: 3230 3233 2e30 2e30 290a 5265 7175 6972  2023.0.0).Requir
-00000500: 6573 2d44 6973 743a 206a 6565 706e 6579  es-Dist: jeepney
-00000510: 2028 3e3d 302e 382e 302c 3c30 2e39 2e30   (>=0.8.0,<0.9.0
-00000520: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000530: 2070 7974 6573 7365 7261 6374 2028 3e3d   pytesseract (>=
-00000540: 302e 332e 3130 290a 5072 6f6a 6563 742d  0.3.10).Project-
-00000550: 5552 4c3a 2046 4151 732c 2068 7474 7073  URL: FAQs, https
-00000560: 3a2f 2f64 796e 6f62 6f2e 6769 7468 7562  ://dynobo.github
-00000570: 2e69 6f2f 6e6f 726d 6361 702f 2366 6171  .io/normcap/#faq
-00000580: 730a 5072 6f6a 6563 742d 5552 4c3a 2049  s.Project-URL: I
-00000590: 7373 7565 732c 2068 7474 7073 3a2f 2f67  ssues, https://g
-000005a0: 6974 6875 622e 636f 6d2f 6479 6e6f 626f  ithub.com/dynobo
-000005b0: 2f6e 6f72 6d63 6170 2f69 7373 7565 730a  /normcap/issues.
-000005c0: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
-000005d0: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
-000005e0: 2f67 6974 6875 622e 636f 6d2f 6479 6e6f  /github.com/dyno
-000005f0: 626f 2f6e 6f72 6d63 6170 0a44 6573 6372  bo/normcap.Descr
-00000600: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000610: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000620: 776e 0a0a 3c21 2d2d 206d 6172 6b64 6f77  wn..<!-- markdow
-00000630: 6e6c 696e 742d 6469 7361 626c 6520 4d44  nlint-disable MD
-00000640: 3031 3320 4d44 3032 3620 4d44 3033 3320  013 MD026 MD033 
-00000650: 2d2d 3e0a 0a23 204e 6f72 6d43 6170 0a0a  -->..# NormCap..
-00000660: 2a2a 5f4f 4352 2070 6f77 6572 6564 2073  **_OCR powered s
-00000670: 6372 6565 6e2d 6361 7074 7572 6520 746f  creen-capture to
-00000680: 6f6c 2074 6f20 6361 7074 7572 6520 696e  ol to capture in
-00000690: 666f 726d 6174 696f 6e20 696e 7374 6561  formation instea
-000006a0: 6420 6f66 2069 6d61 6765 732e 2046 6f72  d of images. For
-000006b0: 204c 696e 7578 2c0a 6d61 634f 5320 616e   Linux,.macOS an
-000006c0: 6420 5769 6e64 6f77 732e 5f2a 2a0a 0a5b  d Windows._**..[
-000006d0: 215b 4275 696c 645d 2868 7474 7073 3a2f  ![Build](https:/
-000006e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000006f0: 6769 7468 7562 2f61 6374 696f 6e73 2f77  github/actions/w
-00000700: 6f72 6b66 6c6f 772f 7374 6174 7573 2f64  orkflow/status/d
-00000710: 796e 6f62 6f2f 6e6f 726d 6361 702f 7079  ynobo/normcap/py
-00000720: 7468 6f6e 2e79 616d 6c3f 6272 616e 6368  thon.yaml?branch
-00000730: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
-00000740: 6769 7468 7562 2e63 6f6d 2f64 796e 6f62  github.com/dynob
-00000750: 6f2f 6e6f 726d 6361 702f 7265 6c65 6173  o/normcap/releas
-00000760: 6573 290a 5b21 5b43 6f76 6572 6167 6520  es).[![Coverage 
-00000770: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-00000780: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
-00000790: 6f76 6572 616c 6c73 436f 7665 7261 6765  overallsCoverage
-000007a0: 2f67 6974 6875 622f 6479 6e6f 626f 2f6e  /github/dynobo/n
-000007b0: 6f72 6d63 6170 3f6c 6162 656c 3d54 6573  ormcap?label=Tes
-000007c0: 7425 3230 636f 7665 7261 6765 2662 7261  t%20coverage&bra
-000007d0: 6e63 683d 6d61 696e 295d 2868 7474 7073  nch=main)](https
-000007e0: 3a2f 2f63 6f76 6572 616c 6c73 2e69 6f2f  ://coveralls.io/
-000007f0: 6769 7468 7562 2f64 796e 6f62 6f2f 6e6f  github/dynobo/no
-00000800: 726d 6361 7029 0a5b 215b 436f 6465 514c  rmcap).[![CodeQL
-00000810: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000820: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000830: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000840: 2f73 7461 7475 732f 6479 6e6f 626f 2f6e  /status/dynobo/n
-00000850: 6f72 6d63 6170 2f63 6f64 6571 6c2d 616e  ormcap/codeql-an
-00000860: 616c 7973 6973 2e79 6d6c 3f62 7261 6e63  alysis.yml?branc
-00000870: 683d 6d61 696e 266c 6162 656c 3d43 6f64  h=main&label=Cod
-00000880: 6551 4c29 5d28 6874 7470 733a 2f2f 6769  eQL)](https://gi
-00000890: 7468 7562 2e63 6f6d 2f64 796e 6f62 6f2f  thub.com/dynobo/
-000008a0: 6e6f 726d 6361 702f 6163 7469 6f6e 732f  normcap/actions/
-000008b0: 776f 726b 666c 6f77 732f 636f 6465 716c  workflows/codeql
-000008c0: 2d61 6e61 6c79 7369 732e 796d 6c29 0a0a  -analysis.yml)..
-000008d0: 5b21 5b47 6974 4875 625d 2868 7474 7073  [![GitHub](https
-000008e0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000008f0: 6f2f 6769 7468 7562 2f64 6f77 6e6c 6f61  o/github/downloa
-00000900: 6473 2f64 796e 6f62 6f2f 6e6f 726d 6361  ds/dynobo/normca
-00000910: 702f 746f 7461 6c3f 6c61 6265 6c3d 4769  p/total?label=Gi
-00000920: 7468 7562 2532 3064 6f77 6e6c 6f61 6473  thub%20downloads
-00000930: 2663 6f6c 6f72 3d62 6c75 6529 5d28 6874  &color=blue)](ht
-00000940: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000950: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
-00000960: 7265 6c65 6173 6573 290a 5b21 5b50 7950  releases).[![PyP
-00000970: 695d 2868 7474 7073 3a2f 2f69 6d67 2e73  i](https://img.s
-00000980: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
-00000990: 6d2f 6e6f 726d 6361 703f 6c61 6265 6c3d  m/normcap?label=
-000009a0: 5079 5069 2532 3064 6f77 6e6c 6f61 6473  PyPi%20downloads
-000009b0: 2663 6f6c 6f72 3d62 6c75 6529 5d28 6874  &color=blue)](ht
-000009c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000009d0: 726f 6a65 6374 2f6e 6f72 6d63 6170 290a  roject/normcap).
-000009e0: 5b21 5b46 6c61 7468 7562 5d28 6874 7470  [![Flathub](http
-000009f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000a00: 696f 2f66 6c61 7468 7562 2f64 6f77 6e6c  io/flathub/downl
-00000a10: 6f61 6473 2f63 6f6d 2e67 6974 6875 622e  oads/com.github.
-00000a20: 6479 6e6f 626f 2e6e 6f72 6d63 6170 3f6c  dynobo.normcap?l
-00000a30: 6162 656c 3d46 6c61 7468 7562 2532 3064  abel=Flathub%20d
-00000a40: 6f77 6e6c 6f61 6473 2663 6f6c 6f72 3d62  ownloads&color=b
-00000a50: 6c75 6529 5d28 6874 7470 733a 2f2f 666c  lue)](https://fl
-00000a60: 6174 6875 622e 6f72 672f 6170 7073 2f64  athub.org/apps/d
-00000a70: 6574 6169 6c73 2f63 6f6d 2e67 6974 6875  etails/com.githu
-00000a80: 622e 6479 6e6f 626f 2e6e 6f72 6d63 6170  b.dynobo.normcap
-00000a90: 290a 5b21 5b41 5552 5d28 6874 7470 733a  ).[![AUR](https:
-00000aa0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000ab0: 2f61 7572 2f76 6f74 6573 2f6e 6f72 6d63  /aur/votes/normc
-00000ac0: 6170 3f6c 6162 656c 3d41 5552 2532 3076  ap?label=AUR%20v
-00000ad0: 6f74 6573 2663 6f6c 6f72 3d62 6c75 6529  otes&color=blue)
-00000ae0: 5d28 6874 7470 733a 2f2f 6175 722e 6172  ](https://aur.ar
-00000af0: 6368 6c69 6e75 782e 6f72 672f 7061 636b  chlinux.org/pack
-00000b00: 6167 6573 2f6e 6f72 6d63 6170 290a 0a2a  ages/normcap)..*
-00000b10: 2a4c 696e 6b73 3a2a 2a20 5b53 6f75 7263  *Links:** [Sourc
-00000b20: 6520 436f 6465 5d28 6874 7470 733a 2f2f  e Code](https://
-00000b30: 6769 7468 7562 2e63 6f6d 2f64 796e 6f62  github.com/dynob
-00000b40: 6f2f 6e6f 726d 6361 7029 207c 0a5b 446f  o/normcap) |.[Do
-00000b50: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00000b60: 7073 3a2f 2f64 796e 6f62 6f2e 6769 7468  ps://dynobo.gith
-00000b70: 7562 2e69 6f2f 6e6f 726d 6361 702f 2920  ub.io/normcap/) 
-00000b80: 7c0a 5b46 4151 735d 2868 7474 7073 3a2f  |.[FAQs](https:/
-00000b90: 2f64 796e 6f62 6f2e 6769 7468 7562 2e69  /dynobo.github.i
-00000ba0: 6f2f 6e6f 726d 6361 702f 2366 6171 7329  o/normcap/#faqs)
-00000bb0: 207c 0a5b 5265 6c65 6173 6573 5d28 6874   |.[Releases](ht
-00000bc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000bd0: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
-00000be0: 7265 6c65 6173 6573 2920 7c0a 5b43 6861  releases) |.[Cha
-00000bf0: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
-00000c00: 6769 7468 7562 2e63 6f6d 2f64 796e 6f62  github.com/dynob
-00000c10: 6f2f 6e6f 726d 6361 702f 626c 6f62 2f6d  o/normcap/blob/m
-00000c20: 6169 6e2f 4348 414e 4745 4c4f 472e 6d64  ain/CHANGELOG.md
-00000c30: 290a 0a5b 215b 5363 7265 656e 6361 7374  )..[![Screencast
-00000c40: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
-00000c50: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
-00000c60: 636f 6e74 656e 742e 636f 6d2f 3131 3037  content.com/1107
-00000c70: 3138 3736 2f31 3839 3736 3735 3835 2d38  1876/189767585-8
-00000c80: 6263 3435 6331 382d 3833 3932 2d34 3131  bc45c18-8392-411
-00000c90: 642d 3834 6463 2d63 6566 3163 6235 6462  d-84dc-cef1cb5db
-00000ca0: 6334 372e 6769 6629 5d28 6874 7470 733a  c47.gif)](https:
-00000cb0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000cc0: 636f 6e74 656e 742e 636f 6d2f 6479 6e6f  content.com/dyno
-00000cd0: 626f 2f6e 6f72 6d63 6170 2f6d 6169 6e2f  bo/normcap/main/
-00000ce0: 6173 7365 7473 2f6e 6f72 6d63 6170 2e67  assets/normcap.g
-00000cf0: 6966 290a 0a23 2320 5175 6963 6b73 7461  if)..## Quicksta
-00000d00: 7274 0a0a 496e 7374 616c 6c20 6120 7072  rt..Install a pr
-00000d10: 6562 7569 6c74 2072 656c 6561 7365 3a0a  ebuilt release:.
-00000d20: 0a2d 202a 2a57 696e 646f 7773 2a2a 3a0a  .- **Windows**:.
-00000d30: 2020 5b4e 6f72 6d43 6170 2d30 2e34 2e30    [NormCap-0.4.0
-00000d40: 2d78 3836 5f36 342d 5769 6e64 6f77 732e  -x86_64-Windows.
-00000d50: 6d73 695d 2868 7474 7073 3a2f 2f67 6974  msi](https://git
-00000d60: 6875 622e 636f 6d2f 6479 6e6f 626f 2f6e  hub.com/dynobo/n
-00000d70: 6f72 6d63 6170 2f72 656c 6561 7365 732f  ormcap/releases/
-00000d80: 646f 776e 6c6f 6164 2f76 302e 342e 302f  download/v0.4.0/
-00000d90: 4e6f 726d 4361 702d 302e 342e 302d 7838  NormCap-0.4.0-x8
-00000da0: 365f 3634 2d57 696e 646f 7773 2e6d 7369  6_64-Windows.msi
-00000db0: 290a 2d20 2a2a 4c69 6e75 782a 2a3a 0a20  ).- **Linux**:. 
-00000dc0: 205b 4e6f 726d 4361 702d 302e 342e 302d   [NormCap-0.4.0-
-00000dd0: 7838 365f 3634 2e41 7070 496d 6167 655d  x86_64.AppImage]
-00000de0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000df0: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
-00000e00: 6170 2f72 656c 6561 7365 732f 646f 776e  ap/releases/down
-00000e10: 6c6f 6164 2f76 302e 342e 302f 4e6f 726d  load/v0.4.0/Norm
-00000e20: 4361 702d 302e 342e 302d 7838 365f 3634  Cap-0.4.0-x86_64
-00000e30: 2e41 7070 496d 6167 6529 0a2d 202a 2a6d  .AppImage).- **m
-00000e40: 6163 4f53 2a2a 2028 7838 3629 20c2 b93a  acOS** (x86) ..:
-00000e50: 0a20 205b 4e6f 726d 4361 702d 302e 342e  .  [NormCap-0.4.
-00000e60: 302d 7838 365f 3634 2d6d 6163 4f53 2e64  0-x86_64-macOS.d
-00000e70: 6d67 5d28 6874 7470 733a 2f2f 6769 7468  mg](https://gith
-00000e80: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
-00000e90: 726d 6361 702f 7265 6c65 6173 6573 2f64  rmcap/releases/d
-00000ea0: 6f77 6e6c 6f61 642f 7630 2e34 2e30 2f4e  ownload/v0.4.0/N
-00000eb0: 6f72 6d43 6170 2d30 2e34 2e30 2d78 3836  ormCap-0.4.0-x86
-00000ec0: 5f36 342d 6d61 634f 532e 646d 6729 0a2d  _64-macOS.dmg).-
-00000ed0: 202a 2a6d 6163 4f53 2a2a 2028 4d31 2920   **macOS** (M1) 
-00000ee0: c2b9 c2b7 c2b2 3a0a 2020 5b4e 6f72 6d43  ......:.  [NormC
-00000ef0: 6170 2d30 2e34 2e30 2d61 726d 3634 2d6d  ap-0.4.0-arm64-m
-00000f00: 6163 4f53 2e64 6d67 5d28 6874 7470 733a  acOS.dmg](https:
-00000f10: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796e  //github.com/dyn
-00000f20: 6f62 6f2f 6e6f 726d 6361 702f 7265 6c65  obo/normcap/rele
-00000f30: 6173 6573 2f64 6f77 6e6c 6f61 642f 7630  ases/download/v0
-00000f40: 2e34 2e30 2f4e 6f72 6d43 6170 2d30 2e34  .4.0/NormCap-0.4
-00000f50: 2e30 2d61 726d 3634 2d6d 6163 4f53 2e64  .0-arm64-macOS.d
-00000f60: 6d67 290a 2020 5c0a 2020 3c73 7562 3e31  mg).  \.  <sub>1
-00000f70: 3a20 4f6e 206d 6163 4f53 2c20 616c 6c6f  : On macOS, allo
-00000f80: 7720 7468 6520 756e 7369 676e 6564 2061  w the unsigned a
-00000f90: 7070 6c69 6361 7469 6f6e 206f 6e20 6669  pplication on fi
-00000fa0: 7273 7420 7374 6172 743a 2022 5379 7374  rst start: "Syst
-00000fb0: 656d 0a20 2050 7265 6665 7265 6e63 6573  em.  Preferences
-00000fc0: 2220 e286 9220 2253 6563 7572 6974 7920  " ... "Security 
-00000fd0: 2620 5072 6976 6163 7922 20e2 8692 2022  & Privacy" ... "
-00000fe0: 4765 6e65 7261 6c22 20e2 8692 2022 4f70  General" ... "Op
-00000ff0: 656e 2061 6e79 7761 7922 2e20 596f 7520  en anyway". You 
-00001000: 6d69 6768 7420 616c 736f 206e 6565 640a  might also need.
-00001010: 2020 746f 2061 6c6c 6f77 204e 6f72 6d43    to allow NormC
-00001020: 6170 2074 6f20 7461 6b65 2073 6372 6565  ap to take scree
-00001030: 6e73 686f 7473 2e0a 2020 5b23 3133 355d  nshots..  [#135]
-00001040: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001050: 636f 6d2f 6479 6e6f 626f 2f6e 6f72 6d63  com/dynobo/normc
-00001060: 6170 2f69 7373 7565 732f 3133 3529 3c62  ap/issues/135)<b
-00001070: 723e 2032 3a20 4d69 6768 7420 6265 2061  r> 2: Might be a
-00001080: 7661 696c 6162 6c65 2061 2062 6974 0a20  vailable a bit. 
-00001090: 2064 656c 6179 6564 2c20 6173 2069 7420   delayed, as it 
-000010a0: 6973 2063 7572 7265 6e74 6c79 2062 7569  is currently bui
-000010b0: 6c64 206d 616e 7561 6c6c 792e 2028 5468  ld manually. (Th
-000010c0: 782c 0a20 205b 4054 616b 7269 6e5d 2868  x,.  [@Takrin](h
-000010d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000010e0: 6d2f 5461 6b72 696e 2921 293c 2f73 7562  m/Takrin)!)</sub
-000010f0: 3e0a 0a49 6e73 7461 6c6c 2066 726f 6d20  >..Install from 
-00001100: 7265 706f 7369 746f 7269 6573 3a0a 0a2d  repositories:..-
-00001110: 202a 2a41 7263 6820 2f20 4d61 6e6a 6172   **Arch / Manjar
-00001120: 6f2a 2a3a 2049 6e73 7461 6c6c 2074 6865  o**: Install the
-00001130: 0a20 205b 606e 6f72 6d63 6170 605d 2868  .  [`normcap`](h
-00001140: 7474 7073 3a2f 2f61 7572 2e61 7263 686c  ttps://aur.archl
-00001150: 696e 7578 2e6f 7267 2f70 6163 6b61 6765  inux.org/package
-00001160: 732f 6e6f 726d 6361 7029 2070 6163 6b61  s/normcap) packa
-00001170: 6765 2066 726f 6d20 4155 522e 0a2d 202a  ge from AUR..- *
-00001180: 2a46 6c61 7450 616b 2028 4c69 6e75 7829  *FlatPak (Linux)
-00001190: 2a2a 3a20 496e 7374 616c 6c0a 2020 5b63  **: Install.  [c
-000011a0: 6f6d 2e67 6974 6875 622e 6479 6e6f 626f  om.github.dynobo
-000011b0: 2e6e 6f72 6d63 6170 5d28 6874 7470 733a  .normcap](https:
-000011c0: 2f2f 666c 6174 6875 622e 6f72 672f 6170  //flathub.org/ap
-000011d0: 7073 2f64 6574 6169 6c73 2f63 6f6d 2e67  ps/details/com.g
-000011e0: 6974 6875 622e 6479 6e6f 626f 2e6e 6f72  ithub.dynobo.nor
-000011f0: 6d63 6170 290a 2020 6672 6f6d 2046 6c61  mcap).  from Fla
-00001200: 7448 7562 2e0a 0a49 6620 796f 7520 6578  tHub...If you ex
-00001210: 7065 7269 656e 6365 2069 7373 7565 7320  perience issues 
-00001220: 706c 6561 7365 206c 6f6f 6b20 6174 2074  please look at t
-00001230: 6865 0a5b 4641 5173 5d28 6874 7470 733a  he.[FAQs](https:
-00001240: 2f2f 6479 6e6f 626f 2e67 6974 6875 622e  //dynobo.github.
-00001250: 696f 2f6e 6f72 6d63 6170 2f23 6661 7173  io/normcap/#faqs
-00001260: 2920 6f72 0a5b 6f70 656e 2061 6e20 6973  ) or.[open an is
-00001270: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
-00001280: 6875 622e 636f 6d2f 6479 6e6f 626f 2f6e  hub.com/dynobo/n
-00001290: 6f72 6d63 6170 2f69 7373 7565 7329 2e0a  ormcap/issues)..
-000012a0: 0a23 2320 5079 7468 6f6e 2070 6163 6b61  .## Python packa
-000012b0: 6765 0a0a 4173 2061 6e20 5f61 6c74 6572  ge..As an _alter
-000012c0: 6e61 7469 7665 5f20 746f 2061 2070 7265  native_ to a pre
-000012d0: 6275 696c 7420 7061 636b 6167 6520 796f  built package yo
-000012e0: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
-000012f0: 650a 5b4e 6f72 6d43 6170 2050 7974 686f  e.[NormCap Pytho
-00001300: 6e20 7061 636b 6167 655d 2868 7474 7073  n package](https
-00001310: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00001320: 6563 742f 6e6f 726d 6361 702f 2920 666f  ect/normcap/) fo
-00001330: 7220 2a2a 5079 7468 6f6e 203e 3d33 2e39  r **Python >=3.9
-00001340: 2a2a 3a0a 0a23 2323 2320 4f6e 204c 696e  **:..#### On Lin
-00001350: 7578 0a0a 6060 6073 680a 2320 496e 7374  ux..```sh.# Inst
-00001360: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
-00001370: 2028 5562 756e 7475 2f44 6562 6961 6e29   (Ubuntu/Debian)
-00001380: 0a73 7564 6f20 6170 7420 696e 7374 616c  .sudo apt instal
-00001390: 6c20 6275 696c 642d 6573 7365 6e74 6961  l build-essentia
-000013a0: 6c20 7465 7373 6572 6163 742d 6f63 7220  l tesseract-ocr 
-000013b0: 7465 7373 6572 6163 742d 6f63 722d 656e  tesseract-ocr-en
-000013c0: 6720 6c69 6274 6573 7365 7261 6374 2d64  g libtesseract-d
-000013d0: 6576 206c 6962 6c65 7074 6f6e 6963 612d  ev libleptonica-
-000013e0: 6465 7620 776c 2d63 6c69 7062 6f61 7264  dev wl-clipboard
-000013f0: 0a0a 2323 2049 6e73 7461 6c6c 2064 6570  ..## Install dep
-00001400: 656e 6465 6e63 6965 7320 2841 7263 6829  endencies (Arch)
-00001410: 0a73 7564 6f20 7061 636d 616e 202d 5320  .sudo pacman -S 
-00001420: 7465 7373 6572 6163 7420 7465 7373 6572  tesseract tesser
-00001430: 6163 742d 6461 7461 2d65 6e67 2077 6c2d  act-data-eng wl-
-00001440: 636c 6970 626f 6172 640a 0a23 2320 496e  clipboard..## In
-00001450: 7374 616c 6c20 6465 7065 6e64 656e 6369  stall dependenci
-00001460: 6573 2028 4665 646f 7261 290a 7375 646f  es (Fedora).sudo
-00001470: 2064 6e66 2069 6e73 7461 6c6c 2074 6573   dnf install tes
-00001480: 7365 7261 6374 2077 6c2d 636c 6970 626f  seract wl-clipbo
-00001490: 6172 640a 0a23 2320 496e 7374 616c 6c20  ard..## Install 
-000014a0: 6465 7065 6e64 656e 6369 6573 2028 6f70  dependencies (op
-000014b0: 656e 5355 5345 290a 7375 646f 207a 7970  enSUSE).sudo zyp
-000014c0: 7065 7220 696e 7374 616c 6c20 7079 7468  per install pyth
-000014d0: 6f6e 332d 6465 7665 6c20 7465 7373 6572  on3-devel tesser
-000014e0: 6163 742d 6f63 7220 7465 7373 6572 6163  act-ocr tesserac
-000014f0: 742d 6f63 722d 6465 7665 6c20 776c 2d63  t-ocr-devel wl-c
-00001500: 6c69 7062 6f61 7264 0a0a 2320 496e 7374  lipboard..# Inst
-00001510: 616c 6c20 6e6f 726d 6361 700a 7069 7020  all normcap.pip 
-00001520: 696e 7374 616c 6c20 6e6f 726d 6361 700a  install normcap.
-00001530: 0a23 2052 756e 0a2e 2f6e 6f72 6d63 6170  .# Run../normcap
-00001540: 0a60 6060 0a0a 2323 2323 204f 6e20 6d61  .```..#### On ma
-00001550: 634f 530a 0a60 6060 7368 0a23 2049 6e73  cOS..```sh.# Ins
-00001560: 7461 6c6c 2064 6570 656e 6465 6e63 6965  tall dependencie
-00001570: 730a 6272 6577 2069 6e73 7461 6c6c 2074  s.brew install t
-00001580: 6573 7365 7261 6374 2074 6573 7365 7261  esseract tessera
-00001590: 6374 2d6c 616e 670a 0a23 2049 6e73 7461  ct-lang..# Insta
-000015a0: 6c6c 206e 6f72 6d63 6170 0a70 6970 2069  ll normcap.pip i
-000015b0: 6e73 7461 6c6c 206e 6f72 6d63 6170 0a0a  nstall normcap..
-000015c0: 2320 5275 6e0a 2e2f 6e6f 726d 6361 700a  # Run../normcap.
-000015d0: 6060 600a 0a23 2323 2320 4f6e 2057 696e  ```..#### On Win
-000015e0: 646f 7773 0a0a 315c 2e20 496e 7374 616c  dows..1\. Instal
-000015f0: 6c20 6054 6573 7365 7261 6374 2035 6020  l `Tesseract 5` 
-00001600: 6279 2075 7369 6e67 2074 6865 0a5b 696e  by using the.[in
-00001610: 7374 616c 6c65 7220 7072 6f76 6964 6564  staller provided
-00001620: 2062 7920 5542 204d 616e 6e68 6569 6d5d   by UB Mannheim]
-00001630: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001640: 636f 6d2f 5542 2d4d 616e 6e68 6569 6d2f  com/UB-Mannheim/
-00001650: 7465 7373 6572 6163 742f 7769 6b69 292e  tesseract/wiki).
-00001660: 0a0a 325c 2e20 4164 6a75 7374 2065 6e76  ..2\. Adjust env
-00001670: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00001680: 6573 3a0a 0a2d 2043 7265 6174 6520 616e  es:..- Create an
-00001690: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-000016a0: 6961 626c 6520 6054 4553 5344 4154 415f  iable `TESSDATA_
-000016b0: 5052 4546 4958 6020 616e 6420 7365 7420  PREFIX` and set 
-000016c0: 6974 2074 6f20 5465 7373 6572 6163 7427  it to Tesseract'
-000016d0: 7320 6461 7461 0a20 2066 6f6c 6465 722c  s data.  folder,
-000016e0: 2065 2e67 2e3a 0a0a 2020 6060 6063 6d64   e.g.:..  ```cmd
-000016f0: 0a20 2073 6574 7820 5445 5353 4441 5441  .  setx TESSDATA
-00001700: 5f50 5245 4649 5820 2243 3a5c 5072 6f67  _PREFIX "C:\Prog
-00001710: 7261 6d20 4669 6c65 735c 5465 7373 6572  ram Files\Tesser
-00001720: 6163 742d 4f43 525c 7465 7373 6461 7461  act-OCR\tessdata
-00001730: 220a 2020 6060 600a 0a2d 2041 7070 656e  ".  ```..- Appen
-00001740: 6420 5465 7373 6572 6163 7427 7320 6c6f  d Tesseract's lo
-00001750: 6361 7469 6f6e 2074 6f20 7468 6520 656e  cation to the en
-00001760: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00001770: 6c65 2060 5061 7468 602c 2065 2e67 2e3a  le `Path`, e.g.:
-00001780: 0a0a 2020 6060 6063 6d64 0a20 2073 6574  ..  ```cmd.  set
-00001790: 7820 5061 7468 2022 2550 6174 6825 3b43  x Path "%Path%;C
-000017a0: 3a5c 5072 6f67 7261 6d20 4669 6c65 735c  :\Program Files\
-000017b0: 5465 7373 6572 6163 742d 4f43 5222 0a20  Tesseract-OCR". 
-000017c0: 2060 6060 0a0a 2d20 4d61 6b65 2073 7572   ```..- Make sur
-000017d0: 6520 746f 2063 6c6f 7365 2061 6e64 2072  e to close and r
-000017e0: 656f 7065 6e20 796f 7572 2063 7572 7265  eopen your curre
-000017f0: 6e74 2074 6572 6d69 6e61 6c20 7769 6e64  nt terminal wind
-00001800: 6f77 2074 6f20 6170 706c 7920 7468 6520  ow to apply the 
-00001810: 6e65 7720 7661 7269 6162 6c65 732e 0a20  new variables.. 
-00001820: 2054 6573 7420 6974 2062 7920 7275 6e6e   Test it by runn
-00001830: 696e 673a 0a0a 2020 6060 6063 6d64 0a20  ing:..  ```cmd. 
-00001840: 2074 6573 7365 7261 6374 202d 2d6c 6973   tesseract --lis
-00001850: 742d 6c61 6e67 730a 2020 6060 600a 0a33  t-langs.  ```..3
-00001860: 5c2e 2049 6e73 7461 6c6c 2061 6e64 2072  \. Install and r
-00001870: 756e 204e 6f72 6d43 6170 3a0a 0a60 6060  un NormCap:..```
-00001880: 6261 7368 0a23 2049 6e73 7461 6c6c 206e  bash.# Install n
-00001890: 6f72 6d63 6170 0a70 6970 2069 6e73 7461  ormcap.pip insta
-000018a0: 6c6c 206e 6f72 6d63 6170 0a0a 2320 5275  ll normcap..# Ru
-000018b0: 6e0a 6e6f 726d 6361 700a 6060 600a 0a23  n.normcap.```..#
-000018c0: 2320 5768 7920 224e 6f72 6d43 6170 223f  # Why "NormCap"?
-000018d0: 0a0a 5365 6520 5b58 4b43 445d 2868 7474  ..See [XKCD](htt
-000018e0: 7073 3a2f 2f78 6b63 642e 636f 6d29 3a0a  ps://xkcd.com):.
-000018f0: 0a5b 215b 436f 6d69 635d 2868 7474 7073  .[![Comic](https
-00001900: 3a2f 2f69 6d67 732e 786b 6364 2e63 6f6d  ://imgs.xkcd.com
-00001910: 2f63 6f6d 6963 732f 6e6f 726d 5f6e 6f72  /comics/norm_nor
-00001920: 6d61 6c5f 6669 6c65 5f66 6f72 6d61 742e  mal_file_format.
-00001930: 706e 6729 5d28 6874 7470 733a 2f2f 786b  png)](https://xk
-00001940: 6364 2e63 6f6d 2f32 3131 362f 290a 0a23  cd.com/2116/)..#
-00001950: 2320 4465 7665 6c6f 706d 656e 740a 0a50  # Development..P
-00001960: 7265 7265 7175 6973 6974 6573 2066 6f72  rerequisites for
-00001970: 2073 6574 7469 6e67 2075 7020 6120 6465   setting up a de
-00001980: 7665 6c6f 706d 656e 7420 656e 7669 726f  velopment enviro
-00001990: 6e6d 656e 7420 6172 653a 202a 2a50 7974  nment are: **Pyt
-000019a0: 686f 6e20 3e3d 332e 392a 2a2c 0a2a 2a50  hon >=3.9**,.**P
-000019b0: 6f65 7472 793e 3d31 2e33 2e32 2a2a 2061  oetry>=1.3.2** a
-000019c0: 6e64 202a 2a54 6573 7365 7261 6374 2a2a  nd **Tesseract**
-000019d0: 2028 696e 636c 2e20 2a2a 6c61 6e67 7561   (incl. **langua
-000019e0: 6765 2064 6174 612a 2a29 2e0a 0a60 6060  ge data**)...```
-000019f0: 7368 0a23 2043 6c6f 6e65 2072 6570 6f73  sh.# Clone repos
-00001a00: 6974 6f72 790a 6769 7420 636c 6f6e 6520  itory.git clone 
-00001a10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001a20: 6f6d 2f64 796e 6f62 6f2f 6e6f 726d 6361  om/dynobo/normca
-00001a30: 702e 6769 740a 0a23 2043 6861 6e67 6520  p.git..# Change 
-00001a40: 696e 746f 2070 726f 6a65 6374 2064 6972  into project dir
-00001a50: 6563 746f 7279 0a63 6420 6e6f 726d 6361  ectory.cd normca
-00001a60: 700a 0a23 2043 7265 6174 6520 7669 7274  p..# Create virt
-00001a70: 7561 6c20 656e 7620 616e 6420 696e 7374  ual env and inst
-00001a80: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
-00001a90: 0a70 6f65 7472 7920 696e 7374 616c 6c0a  .poetry install.
-00001aa0: 0a23 2052 6567 6973 7465 7220 7072 652d  .# Register pre-
-00001ab0: 636f 6d6d 6974 2068 6f6f 6b0a 706f 6574  commit hook.poet
-00001ac0: 7279 2072 756e 2070 7265 2d63 6f6d 6d69  ry run pre-commi
-00001ad0: 7420 696e 7374 616c 6c0a 0a23 2052 756e  t install..# Run
-00001ae0: 204e 6f72 6d43 6170 2069 6e20 7669 7274   NormCap in virt
-00001af0: 7561 6c20 656e 760a 706f 6574 7279 2072  ual env.poetry r
-00001b00: 756e 2070 7974 686f 6e20 2d6d 206e 6f72  un python -m nor
-00001b10: 6d63 6170 0a60 6060 0a0a 2323 2043 7265  mcap.```..## Cre
-00001b20: 6469 7473 0a0a 5468 6973 2070 726f 6a65  dits..This proje
-00001b30: 6374 2075 7365 7320 7468 6520 666f 6c6c  ct uses the foll
-00001b40: 6f77 696e 6720 6e6f 6e2d 7374 616e 6461  owing non-standa
-00001b50: 7264 206c 6962 7261 7269 6573 3a0a 0a2d  rd libraries:..-
-00001b60: 205b 7079 7369 6465 365d 2868 7474 7073   [pyside6](https
-00001b70: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00001b80: 6563 742f 5079 5369 6465 362f 2920 5f2d  ect/PySide6/) _-
-00001b90: 2062 696e 6469 6e67 7320 666f 7220 5174   bindings for Qt
-00001ba0: 2055 4920 4672 616d 6577 6f72 6b5f 0a2d   UI Framework_.-
-00001bb0: 205b 7079 7465 7373 6572 6163 745d 2868   [pytesseract](h
-00001bc0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00001bd0: 7072 6f6a 6563 742f 7079 7465 7373 6572  project/pytesser
-00001be0: 6163 742f 2920 5f2d 2077 7261 7070 6572  act/) _- wrapper
-00001bf0: 2066 6f72 2074 6573 7365 7261 6374 2773   for tesseract's
-00001c00: 2041 5049 5f0a 2d20 5b6a 6565 706e 6579   API_.- [jeepney
-00001c10: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00001c20: 7267 2f70 726f 6a65 6374 2f6a 6565 706e  rg/project/jeepn
-00001c30: 6579 2f29 205f 2d20 4442 5553 2063 6c69  ey/) _- DBUS cli
-00001c40: 656e 745f 0a0a 416e 6420 6974 2064 6570  ent_..And it dep
-00001c50: 656e 6473 206f 6e20 6578 7465 726e 616c  ends on external
-00001c60: 2073 6f66 7477 6172 653a 0a0a 2d20 5b74   software:..- [t
-00001c70: 6573 7365 7261 6374 5d28 6874 7470 733a  esseract](https:
-00001c80: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6573  //github.com/tes
-00001c90: 7365 7261 6374 2d6f 6372 2f74 6573 7365  seract-ocr/tesse
-00001ca0: 7261 6374 2920 2d20 5f4f 4352 2065 6e67  ract) - _OCR eng
-00001cb0: 696e 655f 0a2d 205b 776c 2d63 6c69 7062  ine_.- [wl-clipb
-00001cc0: 6f61 7264 5d28 6874 7470 733a 2f2f 6769  oard](https://gi
-00001cd0: 7468 7562 2e63 6f6d 2f62 7567 6165 7663  thub.com/bugaevc
-00001ce0: 2f77 6c2d 636c 6970 626f 6172 6429 202d  /wl-clipboard) -
-00001cf0: 205f 5761 796c 616e 6420 636c 6970 626f   _Wayland clipbo
-00001d00: 6172 640a 2020 7574 696c 6974 6965 735f  ard.  utilities_
-00001d10: 0a0a 5061 636b 6167 696e 6720 6973 2064  ..Packaging is d
-00001d20: 6f6e 6520 7769 7468 3a0a 0a2d 205b 6272  one with:..- [br
-00001d30: 6965 6663 6173 655d 2868 7474 7073 3a2f  iefcase](https:/
-00001d40: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001d50: 742f 6272 6965 6663 6173 652f 2920 5f2d  t/briefcase/) _-
-00001d60: 2063 6f6e 7665 7274 696e 6720 5079 7468   converting Pyth
-00001d70: 6f6e 2070 726f 6a65 6374 7320 696e 746f  on projects into
-00001d80: 5f0a 2020 5f73 7461 6e64 616c 6f6e 6520  _.  _standalone 
-00001d90: 6170 7073 5f0a 0a54 6861 6e6b 7320 746f  apps_..Thanks to
-00001da0: 2074 6865 206d 6169 6e74 6169 6e65 7273   the maintainers
-00001db0: 206f 6620 7468 6f73 6520 6e69 6365 2074   of those nice t
-00001dc0: 6f6f 6c73 210a 0a23 2320 5369 6d69 6c61  ools!..## Simila
-00001dd0: 7220 6f70 656e 2073 6f75 7263 6520 746f  r open source to
-00001de0: 6f6c 730a 0a49 6620 4e6f 726d 4361 7020  ols..If NormCap 
-00001df0: 646f 6573 6e27 7420 6669 7420 796f 7572  doesn't fit your
-00001e00: 206e 6565 6473 2c20 7472 7920 7468 6f73   needs, try thos
-00001e10: 6520 616c 7465 726e 6174 6976 6573 2028  e alternatives (
-00001e20: 6e6f 2070 6172 7469 6375 6c61 7220 6f72  no particular or
-00001e30: 6465 7229 3a0a 0a2d 205b 5465 7874 536e  der):..- [TextSn
-00001e40: 6174 6368 6572 5d28 6874 7470 733a 2f2f  atcher](https://
-00001e50: 6769 7468 7562 2e63 6f6d 2f52 616a 536f  github.com/RajSo
-00001e60: 6c61 692f 5465 7874 536e 6174 6368 6572  lai/TextSnatcher
-00001e70: 2920 284c 696e 7578 290a 2d20 5b47 7265  ) (Linux).- [Gre
-00001e80: 656e 5368 6f74 5d28 6874 7470 733a 2f2f  enShot](https://
-00001e90: 6765 7467 7265 656e 7368 6f74 2e6f 7267  getgreenshot.org
-00001ea0: 2f29 2028 4c69 6e75 782c 206d 6163 4f53  /) (Linux, macOS
-00001eb0: 290a 2d20 5b54 6578 7453 686f 745d 2868  ).- [TextShot](h
-00001ec0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001ed0: 6d2f 6961 6e7a 6861 6f30 352f 7465 7874  m/ianzhao05/text
-00001ee0: 7368 6f74 2920 2857 696e 646f 7773 290a  shot) (Windows).
-00001ef0: 2d20 5b67 496d 6167 6552 6561 6465 725d  - [gImageReader]
-00001f00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001f10: 636f 6d2f 6d61 6e69 7361 6e64 726f 2f67  com/manisandro/g
-00001f20: 496d 6167 6552 6561 6465 7229 2028 4c69  ImageReader) (Li
-00001f30: 6e75 782c 2057 696e 646f 7773 290a 2d20  nux, Windows).- 
-00001f40: 5b43 6170 7475 7265 3254 6578 745d 2868  [Capture2Text](h
-00001f50: 7474 7073 3a2f 2f73 6f75 7263 6566 6f72  ttps://sourcefor
-00001f60: 6765 2e6e 6574 2f70 726f 6a65 6374 732f  ge.net/projects/
-00001f70: 6361 7074 7572 6532 7465 7874 2920 2857  capture2text) (W
-00001f80: 696e 646f 7773 290a 2d20 5b46 726f 675d  indows).- [Frog]
-00001f90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001fa0: 636f 6d2f 5465 6e64 6572 4f77 6c2f 4672  com/TenderOwl/Fr
-00001fb0: 6f67 2920 284c 696e 7578 290a 2d20 5b54  og) (Linux).- [T
-00001fc0: 6578 7469 6e61 746f 725d 2868 7474 7073  extinator](https
-00001fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5268  ://github.com/Rh
-00001fe0: 6574 5462 756c 6c2f 7465 7874 696e 6174  etTbull/textinat
-00001ff0: 6f72 2920 286d 6163 4f53 290a 0a23 2320  or) (macOS)..## 
-00002000: 4365 7274 6966 6963 6174 696f 6e0a 0a21  Certification..!
-00002010: 5b57 4f4d 4d5d 2868 7474 7073 3a2f 2f72  [WOMM](https://r
-00002020: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002030: 7465 6e74 2e63 6f6d 2f64 796e 6f62 6f2f  tent.com/dynobo/
-00002040: 6c6d 6469 6167 2f6d 6173 7465 722f 6261  lmdiag/master/ba
-00002050: 6467 652e 706e 6729 0a0a                 dge.png)..
+000004b0: 7373 656e 7469 616c 7320 283d 3d36 2e34  ssentials (==6.4
+000004c0: 2e32 290a 5265 7175 6972 6573 2d44 6973  .2).Requires-Dis
+000004d0: 743a 206a 6565 706e 6579 2028 3e3d 302e  t: jeepney (>=0.
+000004e0: 382e 302c 3c30 2e39 2e30 290a 5072 6f6a  8.0,<0.9.0).Proj
+000004f0: 6563 742d 5552 4c3a 2046 4151 732c 2068  ect-URL: FAQs, h
+00000500: 7474 7073 3a2f 2f64 796e 6f62 6f2e 6769  ttps://dynobo.gi
+00000510: 7468 7562 2e69 6f2f 6e6f 726d 6361 702f  thub.io/normcap/
+00000520: 2366 6171 730a 5072 6f6a 6563 742d 5552  #faqs.Project-UR
+00000530: 4c3a 2049 7373 7565 732c 2068 7474 7073  L: Issues, https
+00000540: 3a2f 2f67 6974 6875 622e 636f 6d2f 6479  ://github.com/dy
+00000550: 6e6f 626f 2f6e 6f72 6d63 6170 2f69 7373  nobo/normcap/iss
+00000560: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
+00000570: 2052 6570 6f73 6974 6f72 792c 2068 7474   Repository, htt
+00000580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000590: 6479 6e6f 626f 2f6e 6f72 6d63 6170 0a44  dynobo/normcap.D
+000005a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000005b0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000005c0: 726b 646f 776e 0a0a 3c21 2d2d 206d 6172  rkdown..<!-- mar
+000005d0: 6b64 6f77 6e6c 696e 742d 6469 7361 626c  kdownlint-disabl
+000005e0: 6520 4d44 3031 3320 4d44 3032 3620 4d44  e MD013 MD026 MD
+000005f0: 3033 3320 2d2d 3e0a 0a23 204e 6f72 6d43  033 -->..# NormC
+00000600: 6170 0a0a 2a2a 5f4f 4352 2070 6f77 6572  ap..**_OCR power
+00000610: 6564 2073 6372 6565 6e2d 6361 7074 7572  ed screen-captur
+00000620: 6520 746f 6f6c 2074 6f20 6361 7074 7572  e tool to captur
+00000630: 6520 696e 666f 726d 6174 696f 6e20 696e  e information in
+00000640: 7374 6561 6420 6f66 2069 6d61 6765 732e  stead of images.
+00000650: 2046 6f72 204c 696e 7578 2c0a 6d61 634f   For Linux,.macO
+00000660: 5320 616e 6420 5769 6e64 6f77 732e 5f2a  S and Windows._*
+00000670: 2a0a 0a5b 215b 4275 696c 645d 2868 7474  *..[![Build](htt
+00000680: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000690: 2e69 6f2f 6769 7468 7562 2f61 6374 696f  .io/github/actio
+000006a0: 6e73 2f77 6f72 6b66 6c6f 772f 7374 6174  ns/workflow/stat
+000006b0: 7573 2f64 796e 6f62 6f2f 6e6f 726d 6361  us/dynobo/normca
+000006c0: 702f 7079 7468 6f6e 2e79 616d 6c3f 6272  p/python.yaml?br
+000006d0: 616e 6368 3d6d 6169 6e29 5d28 6874 7470  anch=main)](http
+000006e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000006f0: 796e 6f62 6f2f 6e6f 726d 6361 702f 7265  ynobo/normcap/re
+00000700: 6c65 6173 6573 290a 5b21 5b43 6f76 6572  leases).[![Cover
+00000710: 6167 6520 5374 6174 7573 5d28 6874 7470  age Status](http
+00000720: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000730: 696f 2f63 6f76 6572 616c 6c73 436f 7665  io/coverallsCove
+00000740: 7261 6765 2f67 6974 6875 622f 6479 6e6f  rage/github/dyno
+00000750: 626f 2f6e 6f72 6d63 6170 3f6c 6162 656c  bo/normcap?label
+00000760: 3d54 6573 7425 3230 636f 7665 7261 6765  =Test%20coverage
+00000770: 2662 7261 6e63 683d 6d61 696e 295d 2868  &branch=main)](h
+00000780: 7474 7073 3a2f 2f63 6f76 6572 616c 6c73  ttps://coveralls
+00000790: 2e69 6f2f 6769 7468 7562 2f64 796e 6f62  .io/github/dynob
+000007a0: 6f2f 6e6f 726d 6361 7029 0a5b 215b 436f  o/normcap).[![Co
+000007b0: 6465 514c 5d28 6874 7470 733a 2f2f 696d  deQL](https://im
+000007c0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000007d0: 6875 622f 6163 7469 6f6e 732f 776f 726b  hub/actions/work
+000007e0: 666c 6f77 2f73 7461 7475 732f 6479 6e6f  flow/status/dyno
+000007f0: 626f 2f6e 6f72 6d63 6170 2f63 6f64 6571  bo/normcap/codeq
+00000800: 6c2d 616e 616c 7973 6973 2e79 6d6c 3f62  l-analysis.yml?b
+00000810: 7261 6e63 683d 6d61 696e 266c 6162 656c  ranch=main&label
+00000820: 3d43 6f64 6551 4c29 5d28 6874 7470 733a  =CodeQL)](https:
+00000830: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796e  //github.com/dyn
+00000840: 6f62 6f2f 6e6f 726d 6361 702f 6163 7469  obo/normcap/acti
+00000850: 6f6e 732f 776f 726b 666c 6f77 732f 636f  ons/workflows/co
+00000860: 6465 716c 2d61 6e61 6c79 7369 732e 796d  deql-analysis.ym
+00000870: 6c29 0a0a 5b21 5b47 6974 4875 625d 2868  l)..[![GitHub](h
+00000880: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000890: 6473 2e69 6f2f 6769 7468 7562 2f64 6f77  ds.io/github/dow
+000008a0: 6e6c 6f61 6473 2f64 796e 6f62 6f2f 6e6f  nloads/dynobo/no
+000008b0: 726d 6361 702f 746f 7461 6c3f 6c61 6265  rmcap/total?labe
+000008c0: 6c3d 4769 7468 7562 2532 3064 6f77 6e6c  l=Github%20downl
+000008d0: 6f61 6473 2663 6f6c 6f72 3d62 6c75 6529  oads&color=blue)
+000008e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008f0: 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f 726d  .com/dynobo/norm
+00000900: 6361 702f 7265 6c65 6173 6573 290a 5b21  cap/releases).[!
+00000910: 5b50 7950 695d 2868 7474 7073 3a2f 2f69  [PyPi](https://i
+00000920: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000930: 7069 2f64 6d2f 6e6f 726d 6361 703f 6c61  pi/dm/normcap?la
+00000940: 6265 6c3d 5079 5069 2532 3064 6f77 6e6c  bel=PyPi%20downl
+00000950: 6f61 6473 2663 6f6c 6f72 3d62 6c75 6529  oads&color=blue)
+00000960: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000970: 7267 2f70 726f 6a65 6374 2f6e 6f72 6d63  rg/project/normc
+00000980: 6170 290a 5b21 5b46 6c61 7468 7562 5d28  ap).[![Flathub](
+00000990: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000009a0: 6c64 732e 696f 2f66 6c61 7468 7562 2f64  lds.io/flathub/d
+000009b0: 6f77 6e6c 6f61 6473 2f63 6f6d 2e67 6974  ownloads/com.git
+000009c0: 6875 622e 6479 6e6f 626f 2e6e 6f72 6d63  hub.dynobo.normc
+000009d0: 6170 3f6c 6162 656c 3d46 6c61 7468 7562  ap?label=Flathub
+000009e0: 2532 3064 6f77 6e6c 6f61 6473 2663 6f6c  %20downloads&col
+000009f0: 6f72 3d62 6c75 6529 5d28 6874 7470 733a  or=blue)](https:
+00000a00: 2f2f 666c 6174 6875 622e 6f72 672f 6170  //flathub.org/ap
+00000a10: 7073 2f64 6574 6169 6c73 2f63 6f6d 2e67  ps/details/com.g
+00000a20: 6974 6875 622e 6479 6e6f 626f 2e6e 6f72  ithub.dynobo.nor
+00000a30: 6d63 6170 290a 5b21 5b41 5552 5d28 6874  mcap).[![AUR](ht
+00000a40: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000a50: 732e 696f 2f61 7572 2f76 6f74 6573 2f6e  s.io/aur/votes/n
+00000a60: 6f72 6d63 6170 3f6c 6162 656c 3d41 5552  ormcap?label=AUR
+00000a70: 2532 3076 6f74 6573 2663 6f6c 6f72 3d62  %20votes&color=b
+00000a80: 6c75 6529 5d28 6874 7470 733a 2f2f 6175  lue)](https://au
+00000a90: 722e 6172 6368 6c69 6e75 782e 6f72 672f  r.archlinux.org/
+00000aa0: 7061 636b 6167 6573 2f6e 6f72 6d63 6170  packages/normcap
+00000ab0: 290a 0a3c 6120 6872 6566 3d22 6874 7470  )..<a href="http
+00000ac0: 733a 2f2f 7777 772e 6275 796d 6561 636f  s://www.buymeaco
+00000ad0: 6666 6565 2e63 6f6d 2f64 796e 6f62 6f22  ffee.com/dynobo"
+00000ae0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000af0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000b00: 3a2f 2f63 646e 2e62 7579 6d65 6163 6f66  ://cdn.buymeacof
+00000b10: 6665 652e 636f 6d2f 6275 7474 6f6e 732f  fee.com/buttons/
+00000b20: 7632 2f64 6566 6175 6c74 2d79 656c 6c6f  v2/default-yello
+00000b30: 772e 706e 6722 2061 6c74 3d22 4275 7920  w.png" alt="Buy 
+00000b40: 4d65 2041 2043 6f66 6665 6522 2073 7479  Me A Coffee" sty
+00000b50: 6c65 3d22 6865 6967 6874 3a20 3430 7078  le="height: 40px
+00000b60: 2021 696d 706f 7274 616e 743b 2220 3e3c   !important;" ><
+00000b70: 2f61 3e0a 0a2a 2a4c 696e 6b73 3a2a 2a20  /a>..**Links:** 
+00000b80: 5b53 6f75 7263 6520 436f 6465 5d28 6874  [Source Code](ht
+00000b90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ba0: 2f64 796e 6f62 6f2f 6e6f 726d 6361 7029  /dynobo/normcap)
+00000bb0: 207c 0a5b 446f 6375 6d65 6e74 6174 696f   |.[Documentatio
+00000bc0: 6e5d 2868 7474 7073 3a2f 2f64 796e 6f62  n](https://dynob
+00000bd0: 6f2e 6769 7468 7562 2e69 6f2f 6e6f 726d  o.github.io/norm
+00000be0: 6361 702f 2920 7c0a 5b46 4151 735d 2868  cap/) |.[FAQs](h
+00000bf0: 7474 7073 3a2f 2f64 796e 6f62 6f2e 6769  ttps://dynobo.gi
+00000c00: 7468 7562 2e69 6f2f 6e6f 726d 6361 702f  thub.io/normcap/
+00000c10: 2366 6171 7329 207c 0a5b 5265 6c65 6173  #faqs) |.[Releas
+00000c20: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00000c30: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
+00000c40: 726d 6361 702f 7265 6c65 6173 6573 2920  rmcap/releases) 
+00000c50: 7c0a 5b43 6861 6e67 656c 6f67 5d28 6874  |.[Changelog](ht
+00000c60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000c70: 2f64 796e 6f62 6f2f 6e6f 726d 6361 702f  /dynobo/normcap/
+00000c80: 626c 6f62 2f6d 6169 6e2f 4348 414e 4745  blob/main/CHANGE
+00000c90: 4c4f 4729 0a0a 5b21 5b53 6372 6565 6e63  LOG)..[![Screenc
+00000ca0: 6173 745d 2868 7474 7073 3a2f 2f75 7365  ast](https://use
+00000cb0: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
+00000cc0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f31  sercontent.com/1
+00000cd0: 3130 3731 3837 362f 3138 3937 3637 3538  1071876/18976758
+00000ce0: 352d 3862 6334 3563 3138 2d38 3339 322d  5-8bc45c18-8392-
+00000cf0: 3431 3164 2d38 3464 632d 6365 6631 6362  411d-84dc-cef1cb
+00000d00: 3564 6263 3437 2e67 6966 295d 2868 7474  5dbc47.gif)](htt
+00000d10: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000d20: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000d30: 796e 6f62 6f2f 6e6f 726d 6361 702f 6d61  ynobo/normcap/ma
+00000d40: 696e 2f61 7373 6574 732f 6e6f 726d 6361  in/assets/normca
+00000d50: 702e 6769 6629 0a0a 2323 2051 7569 636b  p.gif)..## Quick
+00000d60: 7374 6172 740a 0a49 6e73 7461 6c6c 2061  start..Install a
+00000d70: 2070 7265 6275 696c 7420 7265 6c65 6173   prebuilt releas
+00000d80: 653a 0a0a 2d20 2a2a 5769 6e64 6f77 732a  e:..- **Windows*
+00000d90: 2a3a 0a20 205b 4e6f 726d 4361 702d 302e  *:.  [NormCap-0.
+00000da0: 342e 312d 7838 365f 3634 2d57 696e 646f  4.1-x86_64-Windo
+00000db0: 7773 2e6d 7369 5d28 6874 7470 733a 2f2f  ws.msi](https://
+00000dc0: 6769 7468 7562 2e63 6f6d 2f64 796e 6f62  github.com/dynob
+00000dd0: 6f2f 6e6f 726d 6361 702f 7265 6c65 6173  o/normcap/releas
+00000de0: 6573 2f64 6f77 6e6c 6f61 642f 7630 2e34  es/download/v0.4
+00000df0: 2e31 2f4e 6f72 6d43 6170 2d30 2e34 2e31  .1/NormCap-0.4.1
+00000e00: 2d78 3836 5f36 342d 5769 6e64 6f77 732e  -x86_64-Windows.
+00000e10: 6d73 6929 0a2d 202a 2a4c 696e 7578 2a2a  msi).- **Linux**
+00000e20: 3a0a 2020 5b4e 6f72 6d43 6170 2d30 2e34  :.  [NormCap-0.4
+00000e30: 2e31 2d78 3836 5f36 342e 4170 7049 6d61  .1-x86_64.AppIma
+00000e40: 6765 5d28 6874 7470 733a 2f2f 6769 7468  ge](https://gith
+00000e50: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
+00000e60: 726d 6361 702f 7265 6c65 6173 6573 2f64  rmcap/releases/d
+00000e70: 6f77 6e6c 6f61 642f 7630 2e34 2e31 2f4e  ownload/v0.4.1/N
+00000e80: 6f72 6d43 6170 2d30 2e34 2e31 2d78 3836  ormCap-0.4.1-x86
+00000e90: 5f36 342e 4170 7049 6d61 6765 290a 2d20  _64.AppImage).- 
+00000ea0: 2a2a 6d61 634f 532a 2a20 2878 3836 2920  **macOS** (x86) 
+00000eb0: c2b9 3a0a 2020 5b4e 6f72 6d43 6170 2d30  ..:.  [NormCap-0
+00000ec0: 2e34 2e31 2d78 3836 5f36 342d 6d61 634f  .4.1-x86_64-macO
+00000ed0: 532e 646d 675d 2868 7474 7073 3a2f 2f67  S.dmg](https://g
+00000ee0: 6974 6875 622e 636f 6d2f 6479 6e6f 626f  ithub.com/dynobo
+00000ef0: 2f6e 6f72 6d63 6170 2f72 656c 6561 7365  /normcap/release
+00000f00: 732f 646f 776e 6c6f 6164 2f76 302e 342e  s/download/v0.4.
+00000f10: 312f 4e6f 726d 4361 702d 302e 342e 312d  1/NormCap-0.4.1-
+00000f20: 7838 365f 3634 2d6d 6163 4f53 2e64 6d67  x86_64-macOS.dmg
+00000f30: 290a 2d20 2a2a 6d61 634f 532a 2a20 284d  ).- **macOS** (M
+00000f40: 3129 20c2 b9c2 b7c2 b23a 0a20 205b 4e6f  1) ......:.  [No
+00000f50: 726d 4361 702d 302e 342e 312d 6172 6d36  rmCap-0.4.1-arm6
+00000f60: 342d 6d61 634f 532e 646d 675d 2868 7474  4-macOS.dmg](htt
+00000f70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000f80: 6479 6e6f 626f 2f6e 6f72 6d63 6170 2f72  dynobo/normcap/r
+00000f90: 656c 6561 7365 732f 646f 776e 6c6f 6164  eleases/download
+00000fa0: 2f76 302e 342e 312f 4e6f 726d 4361 702d  /v0.4.1/NormCap-
+00000fb0: 302e 342e 312d 6172 6d36 342d 6d61 634f  0.4.1-arm64-macO
+00000fc0: 532e 646d 6729 0a20 205c 0a20 203c 7375  S.dmg).  \.  <su
+00000fd0: 623e 313a 204f 6e20 6d61 634f 532c 2061  b>1: On macOS, a
+00000fe0: 6c6c 6f77 2074 6865 2075 6e73 6967 6e65  llow the unsigne
+00000ff0: 6420 6170 706c 6963 6174 696f 6e20 6f6e  d application on
+00001000: 2066 6972 7374 2073 7461 7274 3a20 2253   first start: "S
+00001010: 7973 7465 6d0a 2020 5072 6566 6572 656e  ystem.  Preferen
+00001020: 6365 7322 20e2 8692 2022 5365 6375 7269  ces" ... "Securi
+00001030: 7479 2026 2050 7269 7661 6379 2220 e286  ty & Privacy" ..
+00001040: 9220 2247 656e 6572 616c 2220 e286 9220  . "General" ... 
+00001050: 224f 7065 6e20 616e 7977 6179 222e 2059  "Open anyway". Y
+00001060: 6f75 206d 6967 6874 2061 6c73 6f20 6e65  ou might also ne
+00001070: 6564 0a20 2074 6f20 616c 6c6f 7720 4e6f  ed.  to allow No
+00001080: 726d 4361 7020 746f 2074 616b 6520 7363  rmCap to take sc
+00001090: 7265 656e 7368 6f74 732e 0a20 205b 2331  reenshots..  [#1
+000010a0: 3335 5d28 6874 7470 733a 2f2f 6769 7468  35](https://gith
+000010b0: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
+000010c0: 726d 6361 702f 6973 7375 6573 2f31 3335  rmcap/issues/135
+000010d0: 293c 6272 3e20 323a 204d 6967 6874 2062  )<br> 2: Might b
+000010e0: 6520 6176 6169 6c61 626c 6520 6120 6269  e available a bi
+000010f0: 740a 2020 6465 6c61 7965 642c 2061 7320  t.  delayed, as 
+00001100: 6974 2069 7320 6375 7272 656e 746c 7920  it is currently 
+00001110: 6275 696c 6420 6d61 6e75 616c 6c79 2e20  build manually. 
+00001120: 2854 6878 2c0a 2020 5b40 5461 6b72 696e  (Thx,.  [@Takrin
+00001130: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001140: 2e63 6f6d 2f54 616b 7269 6e29 2129 3c2f  .com/Takrin)!)</
+00001150: 7375 623e 0a0a 496e 7374 616c 6c20 6672  sub>..Install fr
+00001160: 6f6d 2072 6570 6f73 6974 6f72 6965 733a  om repositories:
+00001170: 0a0a 2d20 2a2a 5769 6e64 6f77 732a 2a3a  ..- **Windows**:
+00001180: 2049 6e73 7461 6c6c 2066 726f 6d0a 2020   Install from.  
+00001190: 5b4d 6963 726f 736f 6674 2053 746f 7265  [Microsoft Store
+000011a0: 5d28 6874 7470 733a 2f2f 6170 7073 2e6d  ](https://apps.m
+000011b0: 6963 726f 736f 6674 2e63 6f6d 2f73 746f  icrosoft.com/sto
+000011c0: 7265 2f64 6574 6169 6c2f 6e6f 726d 6361  re/detail/normca
+000011d0: 702f 5850 444c 4a4e 4234 4236 4332 5a52  p/XPDLJNB4B6C2ZR
+000011e0: 292e 0a2d 202a 2a41 7263 6820 2f20 4d61  )..- **Arch / Ma
+000011f0: 6e6a 6172 6f2a 2a3a 2049 6e73 7461 6c6c  njaro**: Install
+00001200: 2074 6865 0a20 205b 606e 6f72 6d63 6170   the.  [`normcap
+00001210: 605d 2868 7474 7073 3a2f 2f61 7572 2e61  `](https://aur.a
+00001220: 7263 686c 696e 7578 2e6f 7267 2f70 6163  rchlinux.org/pac
+00001230: 6b61 6765 732f 6e6f 726d 6361 7029 2070  kages/normcap) p
+00001240: 6163 6b61 6765 2066 726f 6d20 4155 522e  ackage from AUR.
+00001250: 0a2d 202a 2a46 6c61 7450 616b 2028 4c69  .- **FlatPak (Li
+00001260: 6e75 7829 2a2a 3a20 496e 7374 616c 6c0a  nux)**: Install.
+00001270: 2020 5b63 6f6d 2e67 6974 6875 622e 6479    [com.github.dy
+00001280: 6e6f 626f 2e6e 6f72 6d63 6170 5d28 6874  nobo.normcap](ht
+00001290: 7470 733a 2f2f 666c 6174 6875 622e 6f72  tps://flathub.or
+000012a0: 672f 6170 7073 2f64 6574 6169 6c73 2f63  g/apps/details/c
+000012b0: 6f6d 2e67 6974 6875 622e 6479 6e6f 626f  om.github.dynobo
+000012c0: 2e6e 6f72 6d63 6170 290a 2020 6672 6f6d  .normcap).  from
+000012d0: 2046 6c61 7448 7562 2e0a 0a49 6620 796f   FlatHub...If yo
+000012e0: 7520 6578 7065 7269 656e 6365 2069 7373  u experience iss
+000012f0: 7565 7320 706c 6561 7365 206c 6f6f 6b20  ues please look 
+00001300: 6174 2074 6865 0a5b 4641 5173 5d28 6874  at the.[FAQs](ht
+00001310: 7470 733a 2f2f 6479 6e6f 626f 2e67 6974  tps://dynobo.git
+00001320: 6875 622e 696f 2f6e 6f72 6d63 6170 2f23  hub.io/normcap/#
+00001330: 6661 7173 2920 6f72 0a5b 6f70 656e 2061  faqs) or.[open a
+00001340: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
+00001350: 2f67 6974 6875 622e 636f 6d2f 6479 6e6f  /github.com/dyno
+00001360: 626f 2f6e 6f72 6d63 6170 2f69 7373 7565  bo/normcap/issue
+00001370: 7329 2e0a 0a23 2320 5079 7468 6f6e 2070  s)...## Python p
+00001380: 6163 6b61 6765 0a0a 4173 2061 6e20 5f61  ackage..As an _a
+00001390: 6c74 6572 6e61 7469 7665 5f20 746f 2061  lternative_ to a
+000013a0: 2070 7265 6275 696c 7420 7061 636b 6167   prebuilt packag
+000013b0: 6520 796f 7520 6361 6e20 696e 7374 616c  e you can instal
+000013c0: 6c20 7468 650a 5b4e 6f72 6d43 6170 2050  l the.[NormCap P
+000013d0: 7974 686f 6e20 7061 636b 6167 655d 2868  ython package](h
+000013e0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000013f0: 7072 6f6a 6563 742f 6e6f 726d 6361 702f  project/normcap/
+00001400: 2920 666f 7220 2a2a 5079 7468 6f6e 203e  ) for **Python >
+00001410: 3d33 2e39 2a2a 3a0a 0a23 2323 2320 4f6e  =3.9**:..#### On
+00001420: 204c 696e 7578 0a0a 6060 6073 680a 2320   Linux..```sh.# 
+00001430: 496e 7374 616c 6c20 6465 7065 6e64 656e  Install dependen
+00001440: 6369 6573 2028 5562 756e 7475 2f44 6562  cies (Ubuntu/Deb
+00001450: 6961 6e29 0a73 7564 6f20 6170 7420 696e  ian).sudo apt in
+00001460: 7374 616c 6c20 6275 696c 642d 6573 7365  stall build-esse
+00001470: 6e74 6961 6c20 7465 7373 6572 6163 742d  ntial tesseract-
+00001480: 6f63 7220 7465 7373 6572 6163 742d 6f63  ocr tesseract-oc
+00001490: 722d 656e 6720 6c69 6274 6573 7365 7261  r-eng libtessera
+000014a0: 6374 2d64 6576 206c 6962 6c65 7074 6f6e  ct-dev liblepton
+000014b0: 6963 612d 6465 7620 776c 2d63 6c69 7062  ica-dev wl-clipb
+000014c0: 6f61 7264 0a0a 2323 2049 6e73 7461 6c6c  oard..## Install
+000014d0: 2064 6570 656e 6465 6e63 6965 7320 2841   dependencies (A
+000014e0: 7263 6829 0a73 7564 6f20 7061 636d 616e  rch).sudo pacman
+000014f0: 202d 5320 7465 7373 6572 6163 7420 7465   -S tesseract te
+00001500: 7373 6572 6163 742d 6461 7461 2d65 6e67  sseract-data-eng
+00001510: 2077 6c2d 636c 6970 626f 6172 640a 0a23   wl-clipboard..#
+00001520: 2320 496e 7374 616c 6c20 6465 7065 6e64  # Install depend
+00001530: 656e 6369 6573 2028 4665 646f 7261 290a  encies (Fedora).
+00001540: 7375 646f 2064 6e66 2069 6e73 7461 6c6c  sudo dnf install
+00001550: 2074 6573 7365 7261 6374 2077 6c2d 636c   tesseract wl-cl
+00001560: 6970 626f 6172 640a 0a23 2320 496e 7374  ipboard..## Inst
+00001570: 616c 6c20 6465 7065 6e64 656e 6369 6573  all dependencies
+00001580: 2028 6f70 656e 5355 5345 290a 7375 646f   (openSUSE).sudo
+00001590: 207a 7970 7065 7220 696e 7374 616c 6c20   zypper install 
+000015a0: 7079 7468 6f6e 332d 6465 7665 6c20 7465  python3-devel te
+000015b0: 7373 6572 6163 742d 6f63 7220 7465 7373  sseract-ocr tess
+000015c0: 6572 6163 742d 6f63 722d 6465 7665 6c20  eract-ocr-devel 
+000015d0: 776c 2d63 6c69 7062 6f61 7264 0a0a 2320  wl-clipboard..# 
+000015e0: 496e 7374 616c 6c20 6e6f 726d 6361 700a  Install normcap.
+000015f0: 7069 7020 696e 7374 616c 6c20 6e6f 726d  pip install norm
+00001600: 6361 700a 0a23 2052 756e 0a2e 2f6e 6f72  cap..# Run../nor
+00001610: 6d63 6170 0a60 6060 0a0a 2323 2323 204f  mcap.```..#### O
+00001620: 6e20 6d61 634f 530a 0a60 6060 7368 0a23  n macOS..```sh.#
+00001630: 2049 6e73 7461 6c6c 2064 6570 656e 6465   Install depende
+00001640: 6e63 6965 730a 6272 6577 2069 6e73 7461  ncies.brew insta
+00001650: 6c6c 2074 6573 7365 7261 6374 2074 6573  ll tesseract tes
+00001660: 7365 7261 6374 2d6c 616e 670a 0a23 2049  seract-lang..# I
+00001670: 6e73 7461 6c6c 206e 6f72 6d63 6170 0a70  nstall normcap.p
+00001680: 6970 2069 6e73 7461 6c6c 206e 6f72 6d63  ip install normc
+00001690: 6170 0a0a 2320 5275 6e0a 2e2f 6e6f 726d  ap..# Run../norm
+000016a0: 6361 700a 6060 600a 0a23 2323 2320 4f6e  cap.```..#### On
+000016b0: 2057 696e 646f 7773 0a0a 315c 2e20 496e   Windows..1\. In
+000016c0: 7374 616c 6c20 6054 6573 7365 7261 6374  stall `Tesseract
+000016d0: 2035 6020 6279 2075 7369 6e67 2074 6865   5` by using the
+000016e0: 0a5b 696e 7374 616c 6c65 7220 7072 6f76  .[installer prov
+000016f0: 6964 6564 2062 7920 5542 204d 616e 6e68  ided by UB Mannh
+00001700: 6569 6d5d 2868 7474 7073 3a2f 2f67 6974  eim](https://git
+00001710: 6875 622e 636f 6d2f 5542 2d4d 616e 6e68  hub.com/UB-Mannh
+00001720: 6569 6d2f 7465 7373 6572 6163 742f 7769  eim/tesseract/wi
+00001730: 6b69 292e 0a0a 325c 2e20 4164 6a75 7374  ki)...2\. Adjust
+00001740: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00001750: 6961 626c 6573 3a0a 0a2d 2043 7265 6174  iables:..- Creat
+00001760: 6520 616e 2065 6e76 6972 6f6e 6d65 6e74  e an environment
+00001770: 2076 6172 6961 626c 6520 6054 4553 5344   variable `TESSD
+00001780: 4154 415f 5052 4546 4958 6020 616e 6420  ATA_PREFIX` and 
+00001790: 7365 7420 6974 2074 6f20 5465 7373 6572  set it to Tesser
+000017a0: 6163 7427 7320 6461 7461 0a20 2066 6f6c  act's data.  fol
+000017b0: 6465 722c 2065 2e67 2e3a 0a0a 2020 6060  der, e.g.:..  ``
+000017c0: 6063 6d64 0a20 2073 6574 7820 5445 5353  `cmd.  setx TESS
+000017d0: 4441 5441 5f50 5245 4649 5820 2243 3a5c  DATA_PREFIX "C:\
+000017e0: 5072 6f67 7261 6d20 4669 6c65 735c 5465  Program Files\Te
+000017f0: 7373 6572 6163 742d 4f43 525c 7465 7373  sseract-OCR\tess
+00001800: 6461 7461 220a 2020 6060 600a 0a2d 2041  data".  ```..- A
+00001810: 7070 656e 6420 5465 7373 6572 6163 7427  ppend Tesseract'
+00001820: 7320 6c6f 6361 7469 6f6e 2074 6f20 7468  s location to th
+00001830: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
+00001840: 7269 6162 6c65 2060 5061 7468 602c 2065  riable `Path`, e
+00001850: 2e67 2e3a 0a0a 2020 6060 6063 6d64 0a20  .g.:..  ```cmd. 
+00001860: 2073 6574 7820 5061 7468 2022 2550 6174   setx Path "%Pat
+00001870: 6825 3b43 3a5c 5072 6f67 7261 6d20 4669  h%;C:\Program Fi
+00001880: 6c65 735c 5465 7373 6572 6163 742d 4f43  les\Tesseract-OC
+00001890: 5222 0a20 2060 6060 0a0a 2d20 4d61 6b65  R".  ```..- Make
+000018a0: 2073 7572 6520 746f 2063 6c6f 7365 2061   sure to close a
+000018b0: 6e64 2072 656f 7065 6e20 796f 7572 2063  nd reopen your c
+000018c0: 7572 7265 6e74 2074 6572 6d69 6e61 6c20  urrent terminal 
+000018d0: 7769 6e64 6f77 2074 6f20 6170 706c 7920  window to apply 
+000018e0: 7468 6520 6e65 7720 7661 7269 6162 6c65  the new variable
+000018f0: 732e 0a20 2054 6573 7420 6974 2062 7920  s..  Test it by 
+00001900: 7275 6e6e 696e 673a 0a0a 2020 6060 6063  running:..  ```c
+00001910: 6d64 0a20 2074 6573 7365 7261 6374 202d  md.  tesseract -
+00001920: 2d6c 6973 742d 6c61 6e67 730a 2020 6060  -list-langs.  ``
+00001930: 600a 0a33 5c2e 2049 6e73 7461 6c6c 2061  `..3\. Install a
+00001940: 6e64 2072 756e 204e 6f72 6d43 6170 3a0a  nd run NormCap:.
+00001950: 0a60 6060 6261 7368 0a23 2049 6e73 7461  .```bash.# Insta
+00001960: 6c6c 206e 6f72 6d63 6170 0a70 6970 2069  ll normcap.pip i
+00001970: 6e73 7461 6c6c 206e 6f72 6d63 6170 0a0a  nstall normcap..
+00001980: 2320 5275 6e0a 6e6f 726d 6361 700a 6060  # Run.normcap.``
+00001990: 600a 0a23 2320 5768 7920 224e 6f72 6d43  `..## Why "NormC
+000019a0: 6170 223f 0a0a 5365 6520 5b58 4b43 445d  ap"?..See [XKCD]
+000019b0: 2868 7474 7073 3a2f 2f78 6b63 642e 636f  (https://xkcd.co
+000019c0: 6d29 3a0a 0a5b 215b 436f 6d69 635d 2868  m):..[![Comic](h
+000019d0: 7474 7073 3a2f 2f69 6d67 732e 786b 6364  ttps://imgs.xkcd
+000019e0: 2e63 6f6d 2f63 6f6d 6963 732f 6e6f 726d  .com/comics/norm
+000019f0: 5f6e 6f72 6d61 6c5f 6669 6c65 5f66 6f72  _normal_file_for
+00001a00: 6d61 742e 706e 6729 5d28 6874 7470 733a  mat.png)](https:
+00001a10: 2f2f 786b 6364 2e63 6f6d 2f32 3131 362f  //xkcd.com/2116/
+00001a20: 290a 0a23 2320 4465 7665 6c6f 706d 656e  )..## Developmen
+00001a30: 740a 0a50 7265 7265 7175 6973 6974 6573  t..Prerequisites
+00001a40: 2066 6f72 2073 6574 7469 6e67 2075 7020   for setting up 
+00001a50: 6120 6465 7665 6c6f 706d 656e 7420 656e  a development en
+00001a60: 7669 726f 6e6d 656e 7420 6172 653a 202a  vironment are: *
+00001a70: 2a50 7974 686f 6e20 3e3d 332e 392a 2a2c  *Python >=3.9**,
+00001a80: 0a2a 2a50 6f65 7472 793e 3d31 2e33 2e32  .**Poetry>=1.3.2
+00001a90: 2a2a 2061 6e64 202a 2a54 6573 7365 7261  ** and **Tessera
+00001aa0: 6374 2a2a 2028 696e 636c 2e20 2a2a 6c61  ct** (incl. **la
+00001ab0: 6e67 7561 6765 2064 6174 612a 2a29 2e0a  nguage data**)..
+00001ac0: 0a60 6060 7368 0a23 2043 6c6f 6e65 2072  .```sh.# Clone r
+00001ad0: 6570 6f73 6974 6f72 790a 6769 7420 636c  epository.git cl
+00001ae0: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+00001af0: 7562 2e63 6f6d 2f64 796e 6f62 6f2f 6e6f  ub.com/dynobo/no
+00001b00: 726d 6361 702e 6769 740a 0a23 2043 6861  rmcap.git..# Cha
+00001b10: 6e67 6520 696e 746f 2070 726f 6a65 6374  nge into project
+00001b20: 2064 6972 6563 746f 7279 0a63 6420 6e6f   directory.cd no
+00001b30: 726d 6361 700a 0a23 2043 7265 6174 6520  rmcap..# Create 
+00001b40: 7669 7274 7561 6c20 656e 7620 616e 6420  virtual env and 
+00001b50: 696e 7374 616c 6c20 6465 7065 6e64 656e  install dependen
+00001b60: 6369 6573 0a70 6f65 7472 7920 696e 7374  cies.poetry inst
+00001b70: 616c 6c0a 0a23 2052 6567 6973 7465 7220  all..# Register 
+00001b80: 7072 652d 636f 6d6d 6974 2068 6f6f 6b0a  pre-commit hook.
+00001b90: 706f 6574 7279 2072 756e 2070 7265 2d63  poetry run pre-c
+00001ba0: 6f6d 6d69 7420 696e 7374 616c 6c0a 0a23  ommit install..#
+00001bb0: 2052 756e 204e 6f72 6d43 6170 2069 6e20   Run NormCap in 
+00001bc0: 7669 7274 7561 6c20 656e 760a 706f 6574  virtual env.poet
+00001bd0: 7279 2072 756e 2070 7974 686f 6e20 2d6d  ry run python -m
+00001be0: 206e 6f72 6d63 6170 0a60 6060 0a0a 2323   normcap.```..##
+00001bf0: 2043 7265 6469 7473 0a0a 5468 6973 2070   Credits..This p
+00001c00: 726f 6a65 6374 2075 7365 7320 7468 6520  roject uses the 
+00001c10: 666f 6c6c 6f77 696e 6720 6e6f 6e2d 7374  following non-st
+00001c20: 616e 6461 7264 206c 6962 7261 7269 6573  andard libraries
+00001c30: 3a0a 0a2d 205b 7079 7369 6465 365d 2868  :..- [pyside6](h
+00001c40: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00001c50: 7072 6f6a 6563 742f 5079 5369 6465 362f  project/PySide6/
+00001c60: 2920 5f2d 2062 696e 6469 6e67 7320 666f  ) _- bindings fo
+00001c70: 7220 5174 2055 4920 4672 616d 6577 6f72  r Qt UI Framewor
+00001c80: 6b5f 0a2d 205b 6a65 6570 6e65 795d 2868  k_.- [jeepney](h
+00001c90: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00001ca0: 7072 6f6a 6563 742f 6a65 6570 6e65 792f  project/jeepney/
+00001cb0: 2920 5f2d 2044 4255 5320 636c 6965 6e74  ) _- DBUS client
+00001cc0: 5f0a 0a41 6e64 2069 7420 6465 7065 6e64  _..And it depend
+00001cd0: 7320 6f6e 2065 7874 6572 6e61 6c20 736f  s on external so
+00001ce0: 6674 7761 7265 3a0a 0a2d 205b 7465 7373  ftware:..- [tess
+00001cf0: 6572 6163 745d 2868 7474 7073 3a2f 2f67  eract](https://g
+00001d00: 6974 6875 622e 636f 6d2f 7465 7373 6572  ithub.com/tesser
+00001d10: 6163 742d 6f63 722f 7465 7373 6572 6163  act-ocr/tesserac
+00001d20: 7429 202d 205f 4f43 5220 656e 6769 6e65  t) - _OCR engine
+00001d30: 5f0a 2d20 5b77 6c2d 636c 6970 626f 6172  _.- [wl-clipboar
+00001d40: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
+00001d50: 622e 636f 6d2f 6275 6761 6576 632f 776c  b.com/bugaevc/wl
+00001d60: 2d63 6c69 7062 6f61 7264 2920 2d20 5f57  -clipboard) - _W
+00001d70: 6179 6c61 6e64 2063 6c69 7062 6f61 7264  ayland clipboard
+00001d80: 0a20 2075 7469 6c69 7469 6573 5f0a 0a50  .  utilities_..P
+00001d90: 6163 6b61 6769 6e67 2069 7320 646f 6e65  ackaging is done
+00001da0: 2077 6974 683a 0a0a 2d20 5b62 7269 6566   with:..- [brief
+00001db0: 6361 7365 5d28 6874 7470 733a 2f2f 7079  case](https://py
+00001dc0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f62  pi.org/project/b
+00001dd0: 7269 6566 6361 7365 2f29 205f 2d20 636f  riefcase/) _- co
+00001de0: 6e76 6572 7469 6e67 2050 7974 686f 6e20  nverting Python 
+00001df0: 7072 6f6a 6563 7473 2069 6e74 6f5f 0a20  projects into_. 
+00001e00: 205f 7374 616e 6461 6c6f 6e65 2061 7070   _standalone app
+00001e10: 735f 0a0a 5468 616e 6b73 2074 6f20 7468  s_..Thanks to th
+00001e20: 6520 6d61 696e 7461 696e 6572 7320 6f66  e maintainers of
+00001e30: 2074 686f 7365 206e 6963 6520 746f 6f6c   those nice tool
+00001e40: 7321 0a0a 2323 2053 696d 696c 6172 206f  s!..## Similar o
+00001e50: 7065 6e20 736f 7572 6365 2074 6f6f 6c73  pen source tools
+00001e60: 0a0a 4966 204e 6f72 6d43 6170 2064 6f65  ..If NormCap doe
+00001e70: 736e 2774 2066 6974 2079 6f75 7220 6e65  sn't fit your ne
+00001e80: 6564 732c 2074 7279 2074 686f 7365 2061  eds, try those a
+00001e90: 6c74 6572 6e61 7469 7665 7320 286e 6f20  lternatives (no 
+00001ea0: 7061 7274 6963 756c 6172 206f 7264 6572  particular order
+00001eb0: 293a 0a0a 2d20 5b54 6578 7453 6e61 7463  ):..- [TextSnatc
+00001ec0: 6865 725d 2868 7474 7073 3a2f 2f67 6974  her](https://git
+00001ed0: 6875 622e 636f 6d2f 5261 6a53 6f6c 6169  hub.com/RajSolai
+00001ee0: 2f54 6578 7453 6e61 7463 6865 7229 2028  /TextSnatcher) (
+00001ef0: 4c69 6e75 7829 0a2d 205b 4772 6565 6e53  Linux).- [GreenS
+00001f00: 686f 745d 2868 7474 7073 3a2f 2f67 6574  hot](https://get
+00001f10: 6772 6565 6e73 686f 742e 6f72 672f 2920  greenshot.org/) 
+00001f20: 284c 696e 7578 2c20 6d61 634f 5329 0a2d  (Linux, macOS).-
+00001f30: 205b 5465 7874 5368 6f74 5d28 6874 7470   [TextShot](http
+00001f40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00001f50: 616e 7a68 616f 3035 2f74 6578 7473 686f  anzhao05/textsho
+00001f60: 7429 2028 5769 6e64 6f77 7329 0a2d 205b  t) (Windows).- [
+00001f70: 6749 6d61 6765 5265 6164 6572 5d28 6874  gImageReader](ht
+00001f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001f90: 2f6d 616e 6973 616e 6472 6f2f 6749 6d61  /manisandro/gIma
+00001fa0: 6765 5265 6164 6572 2920 284c 696e 7578  geReader) (Linux
+00001fb0: 2c20 5769 6e64 6f77 7329 0a2d 205b 4361  , Windows).- [Ca
+00001fc0: 7074 7572 6532 5465 7874 5d28 6874 7470  pture2Text](http
+00001fd0: 733a 2f2f 736f 7572 6365 666f 7267 652e  s://sourceforge.
+00001fe0: 6e65 742f 7072 6f6a 6563 7473 2f63 6170  net/projects/cap
+00001ff0: 7475 7265 3274 6578 7429 2028 5769 6e64  ture2text) (Wind
+00002000: 6f77 7329 0a2d 205b 4672 6f67 5d28 6874  ows).- [Frog](ht
+00002010: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002020: 2f54 656e 6465 724f 776c 2f46 726f 6729  /TenderOwl/Frog)
+00002030: 2028 4c69 6e75 7829 0a2d 205b 5465 7874   (Linux).- [Text
+00002040: 696e 6174 6f72 5d28 6874 7470 733a 2f2f  inator](https://
+00002050: 6769 7468 7562 2e63 6f6d 2f52 6865 7454  github.com/RhetT
+00002060: 6275 6c6c 2f74 6578 7469 6e61 746f 7229  bull/textinator)
+00002070: 2028 6d61 634f 5329 0a2d 205b 5465 7874   (macOS).- [Text
+00002080: 2d47 7261 625d 2868 7474 7073 3a2f 2f67  -Grab](https://g
+00002090: 6974 6875 622e 636f 6d2f 5468 654a 6f65  ithub.com/TheJoe
+000020a0: 4669 6e2f 5465 7874 2d47 7261 6229 2028  Fin/Text-Grab) (
+000020b0: 5769 6e64 6f77 7329 0a2d 205b 6470 5363  Windows).- [dpSc
+000020c0: 7265 656e 4f43 525d 2868 7474 7073 3a2f  reenOCR](https:/
+000020d0: 2f64 616e 706c 612e 6769 7468 7562 2e69  /danpla.github.i
+000020e0: 6f2f 6470 7363 7265 656e 6f63 722f 2920  o/dpscreenocr/) 
+000020f0: 284c 696e 7578 2c20 5769 6e64 6f77 7329  (Linux, Windows)
+00002100: 0a0a 2323 2043 6572 7469 6669 6361 7469  ..## Certificati
+00002110: 6f6e 0a0a 215b 574f 4d4d 5d28 6874 7470  on..![WOMM](http
+00002120: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002130: 6572 636f 6e74 656e 742e 636f 6d2f 6479  ercontent.com/dy
+00002140: 6e6f 626f 2f6c 6d64 6961 672f 6d61 7374  nobo/lmdiag/mast
+00002150: 6572 2f62 6164 6765 2e70 6e67 290a 0a    er/badge.png)..
```

