# Comparing `tmp/tap-adql-sandbox-0.7.2.tar.gz` & `tmp/tap-adql-sandbox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-adql-sandbox-0.7.2.tar", last modified: Sun Nov 20 11:26:28 2022, max compression
+gzip compressed data, was "tap-adql-sandbox-0.8.0.tar", last modified: Mon May  1 14:19:12 2023, max compression
```

## Comparing `tap-adql-sandbox-0.7.2.tar` & `tap-adql-sandbox-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.953757 tap-adql-sandbox-0.7.2/
--rw-r--r--   0 artem      (501) staff       (20)    35096 2021-12-31 11:31:53.000000 tap-adql-sandbox-0.7.2/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       66 2022-01-05 21:03:15.000000 tap-adql-sandbox-0.7.2/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     5431 2022-11-20 11:26:28.953962 tap-adql-sandbox-0.7.2/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     4342 2022-11-09 20:41:47.000000 tap-adql-sandbox-0.7.2/README.md
--rw-r--r--   0 artem      (501) staff       (20)      104 2021-09-01 08:06:44.000000 tap-adql-sandbox-0.7.2/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)     1354 2022-11-20 11:26:28.955397 tap-adql-sandbox-0.7.2/setup.cfg
--rw-r--r--   0 artem      (501) staff       (20)       84 2022-01-05 21:01:37.000000 tap-adql-sandbox-0.7.2/setup.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.938449 tap-adql-sandbox-0.7.2/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.945721 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/
--rw-r--r--   0 artem      (501) staff       (20)      127 2022-01-06 22:08:04.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)    20600 2022-11-20 11:11:47.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/__main__.py
--rw-r--r--   0 artem      (501) staff       (20)     6702 2022-10-09 12:14:57.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/examples.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.949999 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/fonts/
--rwxr-xr-x   0 artem      (501) staff       (20)   169480 2021-01-27 11:23:40.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/fonts/JetBrainsMono-Thin.ttf
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.953282 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/icons/
--rw-r--r--   0 artem      (501) staff       (20)    67646 2022-01-05 20:17:33.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/icons/planet-128.ico
--rw-r--r--   0 artem      (501) staff       (20)    52287 2022-01-05 20:17:13.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/icons/planet-256.ico
--rw-r--r--   0 artem      (501) staff       (20)     6878 2022-11-06 11:16:49.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/theme.py
--rw-r--r--   0 artem      (501) staff       (20)      273 2022-11-20 11:18:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/version.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2022-11-20 11:26:28.949334 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     5431 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      624 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       68 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/entry_points.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       17 2022-11-20 11:26:28.000000 tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.316327 tap-adql-sandbox-0.8.0/
+-rw-r--r--   0 artem      (501) staff       (20)    35096 2021-12-31 11:31:53.000000 tap-adql-sandbox-0.8.0/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       66 2022-01-05 21:03:15.000000 tap-adql-sandbox-0.8.0/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     5504 2023-05-01 14:19:12.316543 tap-adql-sandbox-0.8.0/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     4415 2023-05-01 14:17:19.000000 tap-adql-sandbox-0.8.0/README.md
+-rw-r--r--   0 artem      (501) staff       (20)      104 2021-09-01 08:06:44.000000 tap-adql-sandbox-0.8.0/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)     1376 2023-05-01 14:19:12.317934 tap-adql-sandbox-0.8.0/setup.cfg
+-rw-r--r--   0 artem      (501) staff       (20)       84 2022-01-05 21:01:37.000000 tap-adql-sandbox-0.8.0/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.291061 tap-adql-sandbox-0.8.0/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.296992 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/
+-rw-r--r--   0 artem      (501) staff       (20)      127 2022-01-06 22:08:04.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)    26370 2023-05-01 14:13:10.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/__main__.py
+-rw-r--r--   0 artem      (501) staff       (20)     6687 2023-05-01 07:56:23.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/examples.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.313189 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/fonts/
+-rwxr-xr-x   0 artem      (501) staff       (20)   169480 2021-01-27 11:23:40.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/fonts/JetBrainsMono-Thin.ttf
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.315639 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/icons/
+-rw-r--r--   0 artem      (501) staff       (20)    67646 2022-01-05 20:17:33.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/icons/planet-128.ico
+-rw-r--r--   0 artem      (501) staff       (20)    52287 2022-01-05 20:17:13.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/icons/planet-256.ico
+-rw-r--r--   0 artem      (501) staff       (20)     6880 2023-05-01 13:30:06.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/theme.py
+-rw-r--r--   0 artem      (501) staff       (20)      273 2023-05-01 14:10:38.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/version.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-05-01 14:19:12.312326 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     5504 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      624 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       68 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/entry_points.txt
+-rw-r--r--   0 artem      (501) staff       (20)       49 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       17 2023-05-01 14:19:12.000000 tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/top_level.txt
```

### Comparing `tap-adql-sandbox-0.7.2/LICENSE` & `tap-adql-sandbox-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-adql-sandbox-0.7.2/PKG-INFO` & `tap-adql-sandbox-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-adql-sandbox
-Version: 0.7.2
+Version: 0.8.0
 Summary: A sandbox application for executing ADQL queries via TAP interface
 Home-page: https://github.com/retifrav/tap-adql-sandbox
 Author: retif
 Project-URL: Bug Tracker, https://github.com/retifrav/tap-adql-sandbox/issues
 Project-URL: Changelog, https://github.com/retifrav/tap-adql-sandbox/blob/master/changelog.md
 Keywords: tap,adql,gui,astronomy,astrophysics,cosmology,science
 Classifier: Programming Language :: Python :: 3.6
@@ -34,15 +34,15 @@
 - [Running](#running)
 - [Platforms](#platforms)
 - [Known problems](#known-problems)
     - [Application tries to connect to remote hosts on startup and sometimes crashes](#application-tries-to-connect-to-remote-hosts-on-startup-and-sometimes-crashes)
     - [Application crashes when query has too many columns](#application-crashes-when-query-has-too-many-columns)
     - [Queries might fail with UnicodeDecodeError](#queries-might-fail-with-unicodedecodeerror)
 - [3rd-party](#3rd-party)
-    - [Requirements](#requirements)
+    - [Dependencies](#dependencies)
     - [Resources](#resources)
 
 <!-- /MarkdownTOC -->
 
 ## About
 
 A sandbox application for executing ADQL queries via TAP interface of various data sources, such as astronomical databases. Essentially, it's just a GUI for [PyVO](https://pypi.org/project/pyvo/).
@@ -125,19 +125,20 @@
 
 ### Queries might fail with UnicodeDecodeError
 
 If query results from a TAP service contain non-ASCII symbols, then PyVO will raise [an exception](https://github.com/retifrav/tap-adql-sandbox/issues/19). The application won't crash, but you won't get query results either.
 
 ## 3rd-party
 
-### Requirements
+### Dependencies
 
-- Python 3.6 or later (*though the oldest tested version is 3.7*)
+- Python 3.6 or later (*the oldest tested is 3.7, though*)
 - [Dear PyGui](https://pypi.org/project/dearpygui/) - application window and UI controls
 - [PyVO](https://pypi.org/project/pyvo/) - handling TAP ADQL requests
+- [Astroquery](https://pypi.org/project/astroquery/) - looking up IDs in Simbad
 - [pandas](https://pypi.org/project/pandas/) - processing results and saving to pickle
 - [tabulate](https://pypi.org/project/tabulate/) - printing results to stdout (*with `--debug`*)
 
 ### Resources
 
 - [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font
 - [an icon](https://github.com/retifrav/tap-adql-sandbox/tree/master/src/tap_adql_sandbox/icons) of unknown origin
```

### Comparing `tap-adql-sandbox-0.7.2/README.md` & `tap-adql-sandbox-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - [Running](#running)
 - [Platforms](#platforms)
 - [Known problems](#known-problems)
     - [Application tries to connect to remote hosts on startup and sometimes crashes](#application-tries-to-connect-to-remote-hosts-on-startup-and-sometimes-crashes)
     - [Application crashes when query has too many columns](#application-crashes-when-query-has-too-many-columns)
     - [Queries might fail with UnicodeDecodeError](#queries-might-fail-with-unicodedecodeerror)
 - [3rd-party](#3rd-party)
-    - [Requirements](#requirements)
+    - [Dependencies](#dependencies)
     - [Resources](#resources)
 
 <!-- /MarkdownTOC -->
 
 ## About
 
 A sandbox application for executing ADQL queries via TAP interface of various data sources, such as astronomical databases. Essentially, it's just a GUI for [PyVO](https://pypi.org/project/pyvo/).
@@ -101,19 +101,20 @@
 
 ### Queries might fail with UnicodeDecodeError
 
 If query results from a TAP service contain non-ASCII symbols, then PyVO will raise [an exception](https://github.com/retifrav/tap-adql-sandbox/issues/19). The application won't crash, but you won't get query results either.
 
 ## 3rd-party
 
-### Requirements
+### Dependencies
 
-- Python 3.6 or later (*though the oldest tested version is 3.7*)
+- Python 3.6 or later (*the oldest tested is 3.7, though*)
 - [Dear PyGui](https://pypi.org/project/dearpygui/) - application window and UI controls
 - [PyVO](https://pypi.org/project/pyvo/) - handling TAP ADQL requests
+- [Astroquery](https://pypi.org/project/astroquery/) - looking up IDs in Simbad
 - [pandas](https://pypi.org/project/pandas/) - processing results and saving to pickle
 - [tabulate](https://pypi.org/project/tabulate/) - printing results to stdout (*with `--debug`*)
 
 ### Resources
 
 - [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font
 - [an icon](https://github.com/retifrav/tap-adql-sandbox/tree/master/src/tap_adql_sandbox/icons) of unknown origin
```

### Comparing `tap-adql-sandbox-0.7.2/setup.cfg` & `tap-adql-sandbox-0.8.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 	Intended Audience :: Science/Research
 	Intended Audience :: Education
 	Intended Audience :: Developers
 
 [options]
 package_dir = 
 	= src
-packages = find:
+packages = find_namespace:
 python_requires = >=3.6
 install_requires = 
 	dearpygui >= 1.5.0
 	pyvo
+	astroquery
 	pandas
 	tabulate
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/__main__.py` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # dependencies
 import dearpygui.dearpygui as dpg
 from dearpygui.demo import show_demo
+from astroquery.simbad import Simbad
 from tabulate import tabulate
 import pathlib
 import pandas
 import pyvo
 # standard libraries
 from time import sleep
 import argparse
@@ -71,14 +72,126 @@
     else:
         dpg.hide_item("loadingAnimation")
         dpg.show_item("btnExecuteQuery")
         dpg.configure_item("menuExecuteQuery", enabled=True)
         executingQuery = False
 
 
+def getSimbadIDs() -> None:
+    dpg.hide_item("resultsGroupSimbadIDs")
+    if dpg.does_item_exist("resultsTableSimbadIDs"):
+        dpg.delete_item("resultsTableSimbadIDs")
+    dpg.hide_item("errorMessageSimbadIDs")
+    dpg.set_value("errorMessageSimbadIDs", "")
+
+    dpg.hide_item("btn_getSimbadIDs")
+    dpg.show_item("loadingAnimationSimbadIDs")
+
+    idToLookUpInSimbad: str = dpg.get_value("idToLookUpInSimbad").strip()
+
+    if not idToLookUpInSimbad:
+        dpg.set_value("errorMessageSimbadIDs", "No ID provided")
+        dpg.show_item("errorMessageSimbadIDs")
+        dpg.hide_item("loadingAnimationSimbadIDs")
+        dpg.show_item("btn_getSimbadIDs")
+        return
+
+    oids = None
+    try:
+        oids = Simbad.query_objectids(idToLookUpInSimbad)
+    except Exception as ex:
+        dpg.set_value("errorMessageSimbadIDs", ex)
+        dpg.show_item("errorMessageSimbadIDs")
+        dpg.hide_item("loadingAnimationSimbadIDs")
+        dpg.show_item("btn_getSimbadIDs")
+        return
+
+    if oids:
+        oidsCnt: int = len(oids)
+        if debugMode:
+            print("\n[DEBUG] IDs found in Simbad:", oidsCnt)
+            try:
+                print(
+                    tabulate(
+                        oids,
+                        headers=oids.colnames,
+                        tablefmt="psql",
+                        floatfmt=tabulateFloatfmtPrecision
+                    )
+                )
+            except Exception as ex:
+                print(f"[WARNING] Couldn't print results. {ex}")
+        try:
+            with dpg.table(
+                parent="resultsGroupSimbadIDs",
+                tag="resultsTableSimbadIDs",
+                header_row=True,
+                resizable=True,
+                borders_outerH=True,
+                borders_innerV=True,
+                borders_innerH=True,
+                borders_outerV=True,
+                clipper=True,
+                # row_background=True,
+                # freeze_rows=0,
+                # freeze_columns=1,
+                # scrollY=True
+            ):
+                dpg.add_table_column(label="#", init_width_or_weight=0.05)
+                for header in oids.colnames:
+                    dpg.add_table_column(label=header)
+                index = 0
+                for o in oids:
+                    # reveal_type(index)
+                    with dpg.table_row():
+                        with dpg.table_cell():
+                            dpg.add_text(default_value=f"{index+1}")
+                        with dpg.table_cell():
+                            cellID = f"cellSimbadID-{index+1}"
+                            dpg.add_text(
+                                tag=cellID,
+                                default_value=o["ID"]
+                            )
+                            dpg.bind_item_handler_registry(
+                                cellID,
+                                "cell-handler"
+                            )
+                        index += 1
+        except Exception as ex:
+            errorMsg = "Couldn't generate the results table"
+            print(f"[ERROR] {errorMsg}. {ex}", file=sys.stderr)
+            if debugMode:
+                traceback.print_exc(file=sys.stderr)
+            dpg.set_value(
+                "errorMessageSimbadIDs",
+                f"{errorMsg}. There might be more details in console/stderr."
+            )
+            dpg.show_item("errorMessageSimbadIDs")
+            dpg.hide_item("loadingAnimationSimbadIDs")
+            dpg.show_item("btn_getSimbadIDs")
+            return
+        dpg.hide_item("loadingAnimationSimbadIDs")
+        dpg.show_item("btn_getSimbadIDs")
+        dpg.show_item("resultsGroupSimbadIDs")
+    else:
+        dpg.set_value(
+            "errorMessageSimbadIDs",
+            "Simbad doesn't have any IDs for this object"
+        )
+        dpg.show_item("errorMessageSimbadIDs")
+        dpg.hide_item("loadingAnimationSimbadIDs")
+        dpg.show_item("btn_getSimbadIDs")
+        return
+
+
+def showSimbadIDsWindow() -> None:
+    dpg.hide_item("menu_getSimbadIDs")
+    dpg.show_item("window_simbadIDs")
+
+
 def keyPressCallback(sender, app_data) -> None:
     global executingQuery
 
     # print(sender, app_data)
     # dpg.is_item_focused
     if not dpg.is_item_active(queryTextID) or executingQuery:
         return
@@ -293,15 +406,15 @@
     global noEnumerationColumn
 
     argParser = argparse.ArgumentParser(
         prog="tap-adql-sandbox",
         description=" ".join((
             f"%(prog)s\n{__copyright__}\nA",
             "sandbox application for executing ADQL queries",
-            "via TAP interface"
+            "via TAP interface of various data sources"
         )),
         formatter_class=argparse.RawDescriptionHelpFormatter,
         allow_abbrev=False
     )
     argParser.add_argument(
         "--version",
         action="version",
@@ -338,14 +451,59 @@
     dpg.configure_app(init_file=settingsFile)
 
     # dpg.set_frame_callback(2, callback=updateGeometry)
     # dpg.set_viewport_resize_callback(callback=updateGeometry)
     dpg.set_exit_callback(callback=lambda: dpg.save_init_file(settingsFile))
 
     #
+    # --- Simbad IDs window
+    #
+    with dpg.window(
+        tag="window_simbadIDs",
+        label="Simbad IDs",
+        min_size=(550, 650),
+        show=False,
+        on_close=lambda: dpg.show_item("menu_getSimbadIDs")
+    ):
+        dpg.add_input_text(
+            tag="idToLookUpInSimbad",
+            hint="ID to lookup in Simbad",
+            width=-1
+        )
+        dpg.add_button(
+            tag="btn_getSimbadIDs",
+            label="Lookup",
+            callback=getSimbadIDs
+        )
+        dpg.add_loading_indicator(
+            tag="loadingAnimationSimbadIDs",
+            style=1,
+            radius=1.5,
+            # speed=2,
+            indent=7,
+            color=stylePrimaryColorActive,
+            secondary_color=stylePrimaryColor,
+            show=False
+        )
+
+        dpg.add_spacer()
+
+        dpg.add_text(
+            tag="errorMessageSimbadIDs",
+            default_value="Error",
+            # https://github.com/hoffstadt/DearPyGui/issues/1275
+            wrap=500,  # window width - 50
+            show=False
+        )
+
+        with dpg.group(tag="resultsGroupSimbadIDs", show=False):
+            dpg.add_text(default_value="Found the following IDs:")
+            with dpg.table(tag="resultsTableSimbadIDs"):
+                dpg.add_table_column(label="ResultsSimbadIDs")
+    #
     # --- main window
     #
     with dpg.window(tag=mainWindowID):
         #
         # --- menu
         #
         with dpg.menu_bar():
@@ -380,14 +538,21 @@
             #         check=True
             #     )
             #     dpg.add_menu_item(
             #         label="Setting 2",
             #         callback=lambda: print("ololo")
             #     )
 
+            with dpg.menu(label="Tools"):
+                dpg.add_menu_item(
+                    tag="menu_getSimbadIDs",
+                    label="Lookup IDs in Simbad",
+                    callback=showSimbadIDsWindow
+                )
+
             if debugMode:
                 with dpg.menu(label="Dev"):
                     dpg.add_menu_item(
                         label="Performance metrics",
                         callback=lambda: dpg.show_metrics()
                     )
                     dpg.add_menu_item(
@@ -588,14 +753,15 @@
         )
         dpg.add_spacer(height=2)
 
     # themes/styles bindings
     dpg.bind_font(getGlobalFont())
     dpg.bind_theme(getGlobalTheme())
     dpg.bind_item_theme("errorMessage", getErrorTheme())
+    dpg.bind_item_theme("errorMessageSimbadIDs", getErrorTheme())
     dpg.bind_item_theme("aboutWindow", getWindowTheme())
     # dpg.bind_item_theme("errorDialog", getWindowTheme())
     # dpg.bind_item_theme("errorDialogText", getErrorTheme())
 
     # mouse clicks handler for results table cells
     with dpg.item_handler_registry(tag="cell-handler") as handler:
         dpg.add_item_clicked_handler(callback=cellClicked)
```

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/examples.py` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,13 +184,13 @@
         ))
     },
     "gaia-star-parameters":
     {
         "description": "Star parameters",
         "serviceURL": "https://gea.esac.esa.int/tap-server/tap",
         "queryText": "".join((
-            "SELECT source_id, solution_id, radius_flame_spec, mass_flame_spec\n",
-            "FROM gaiadr3.astrophysical_parameters_supp\n",
+            "SELECT source_id, solution_id, mass_flame, radius_flame\n",
+            "FROM gaiadr3.astrophysical_parameters\n",
             "WHERE source_id = 3145754895088191744"
         ))
     }
 }
```

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/fonts/JetBrainsMono-Thin.ttf` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/fonts/JetBrainsMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/icons/planet-128.ico` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/icons/planet-128.ico`

 * *Files identical despite different names*

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/icons/planet-256.ico` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/icons/planet-256.ico`

 * *Files identical despite different names*

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox/theme.py` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 
 def getErrorTheme():
     with dpg.theme() as errorTheme:
         with dpg.theme_component(dpg.mvAll):
             dpg.add_theme_color(
                 dpg.mvThemeCol_Text,
-                (255, 0, 0),
+                (255, 30, 30),
                 category=dpg.mvThemeCat_Core
             )
         return errorTheme
 
 
 def getCellHighlightedTheme():
     with dpg.theme() as cellHighlightedTheme:
```

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/PKG-INFO` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-adql-sandbox
-Version: 0.7.2
+Version: 0.8.0
 Summary: A sandbox application for executing ADQL queries via TAP interface
 Home-page: https://github.com/retifrav/tap-adql-sandbox
 Author: retif
 Project-URL: Bug Tracker, https://github.com/retifrav/tap-adql-sandbox/issues
 Project-URL: Changelog, https://github.com/retifrav/tap-adql-sandbox/blob/master/changelog.md
 Keywords: tap,adql,gui,astronomy,astrophysics,cosmology,science
 Classifier: Programming Language :: Python :: 3.6
@@ -34,15 +34,15 @@
 - [Running](#running)
 - [Platforms](#platforms)
 - [Known problems](#known-problems)
     - [Application tries to connect to remote hosts on startup and sometimes crashes](#application-tries-to-connect-to-remote-hosts-on-startup-and-sometimes-crashes)
     - [Application crashes when query has too many columns](#application-crashes-when-query-has-too-many-columns)
     - [Queries might fail with UnicodeDecodeError](#queries-might-fail-with-unicodedecodeerror)
 - [3rd-party](#3rd-party)
-    - [Requirements](#requirements)
+    - [Dependencies](#dependencies)
     - [Resources](#resources)
 
 <!-- /MarkdownTOC -->
 
 ## About
 
 A sandbox application for executing ADQL queries via TAP interface of various data sources, such as astronomical databases. Essentially, it's just a GUI for [PyVO](https://pypi.org/project/pyvo/).
@@ -125,19 +125,20 @@
 
 ### Queries might fail with UnicodeDecodeError
 
 If query results from a TAP service contain non-ASCII symbols, then PyVO will raise [an exception](https://github.com/retifrav/tap-adql-sandbox/issues/19). The application won't crash, but you won't get query results either.
 
 ## 3rd-party
 
-### Requirements
+### Dependencies
 
-- Python 3.6 or later (*though the oldest tested version is 3.7*)
+- Python 3.6 or later (*the oldest tested is 3.7, though*)
 - [Dear PyGui](https://pypi.org/project/dearpygui/) - application window and UI controls
 - [PyVO](https://pypi.org/project/pyvo/) - handling TAP ADQL requests
+- [Astroquery](https://pypi.org/project/astroquery/) - looking up IDs in Simbad
 - [pandas](https://pypi.org/project/pandas/) - processing results and saving to pickle
 - [tabulate](https://pypi.org/project/tabulate/) - printing results to stdout (*with `--debug`*)
 
 ### Resources
 
 - [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font
 - [an icon](https://github.com/retifrav/tap-adql-sandbox/tree/master/src/tap_adql_sandbox/icons) of unknown origin
```

### Comparing `tap-adql-sandbox-0.7.2/src/tap_adql_sandbox.egg-info/SOURCES.txt` & `tap-adql-sandbox-0.8.0/src/tap_adql_sandbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

