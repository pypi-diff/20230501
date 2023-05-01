# Comparing `tmp/mara-page-1.6.1.tar.gz` & `tmp/mara-page-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mara-page-1.6.1.tar", last modified: Fri Jan 27 08:31:44 2023, max compression
+gzip compressed data, was "mara-page-1.7.0.tar", last modified: Mon May  1 19:18:41 2023, max compression
```

## Comparing `mara-page-1.6.1.tar` & `mara-page-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-01-27 08:31:44.649655 mara-page-1.6.1/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1061 2022-03-25 12:57:32.000000 mara-page-1.6.1/LICENSE
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4266 2023-01-27 08:31:44.649655 mara-page-1.6.1/PKG-INFO
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)     3926 2022-12-02 09:48:39.000000 mara-page-1.6.1/README.md
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-01-27 08:31:44.639655 mara-page-1.6.1/mara_page/
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)       51 2023-01-27 08:13:11.000000 mara-page-1.6.1/mara_page/__init__.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3911 2022-12-02 09:48:39.000000 mara-page-1.6.1/mara_page/acl.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     3213 2022-12-02 09:48:39.000000 mara-page-1.6.1/mara_page/bootstrap.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     2715 2022-12-02 09:48:39.000000 mara-page-1.6.1/mara_page/html.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1951 2022-03-25 12:57:32.000000 mara-page-1.6.1/mara_page/navigation.py
--rw-r--r--   0 lschick   (1000) lschick   (1000)     1156 2022-12-02 09:48:39.000000 mara-page-1.6.1/mara_page/response.py
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)     3412 2022-03-25 12:57:32.000000 mara-page-1.6.1/mara_page/xml.py
-drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-01-27 08:31:44.649655 mara-page-1.6.1/mara_page.egg-info/
--rw-r--r--   0 lschick   (1000) lschick   (1000)     4266 2023-01-27 08:31:44.000000 mara-page-1.6.1/mara_page.egg-info/PKG-INFO
--rw-r--r--   0 lschick   (1000) lschick   (1000)      358 2023-01-27 08:31:44.000000 mara-page-1.6.1/mara_page.egg-info/SOURCES.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2023-01-27 08:31:44.000000 mara-page-1.6.1/mara_page.egg-info/dependency_links.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)       28 2023-01-27 08:31:44.000000 mara-page-1.6.1/mara_page.egg-info/requires.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)       10 2023-01-27 08:31:44.000000 mara-page-1.6.1/mara_page.egg-info/top_level.txt
--rw-r--r--   0 lschick   (1000) lschick   (1000)      100 2022-05-20 20:56:52.000000 mara-page-1.6.1/pyproject.toml
--rw-r--r--   0 lschick   (1000) lschick   (1000)      496 2023-01-27 08:31:44.649655 mara-page-1.6.1/setup.cfg
--rwxr-xr-x   0 lschick   (1000) lschick   (1000)       38 2022-12-02 09:48:39.000000 mara-page-1.6.1/setup.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:18:41.623239 mara-page-1.7.0/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1061 2022-03-25 12:57:32.000000 mara-page-1.7.0/LICENSE
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4258 2023-05-01 19:18:41.623239 mara-page-1.7.0/PKG-INFO
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)     3918 2023-05-01 19:09:25.000000 mara-page-1.7.0/README.md
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:18:41.613239 mara-page-1.7.0/mara_page/
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)       51 2023-05-01 19:15:45.000000 mara-page-1.7.0/mara_page/__init__.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3911 2023-01-27 09:00:13.000000 mara-page-1.7.0/mara_page/acl.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     3193 2023-05-01 19:11:31.000000 mara-page-1.7.0/mara_page/bootstrap.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     2703 2023-05-01 19:09:25.000000 mara-page-1.7.0/mara_page/html.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1950 2023-05-01 19:09:25.000000 mara-page-1.7.0/mara_page/navigation.py
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     1156 2023-01-27 09:00:13.000000 mara-page-1.7.0/mara_page/response.py
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)     3412 2022-03-25 12:57:32.000000 mara-page-1.7.0/mara_page/xml.py
+drwxr-xr-x   0 lschick   (1000) lschick   (1000)        0 2023-05-01 19:18:41.623239 mara-page-1.7.0/mara_page.egg-info/
+-rw-r--r--   0 lschick   (1000) lschick   (1000)     4258 2023-05-01 19:18:41.000000 mara-page-1.7.0/mara_page.egg-info/PKG-INFO
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      358 2023-05-01 19:18:41.000000 mara-page-1.7.0/mara_page.egg-info/SOURCES.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)        1 2023-05-01 19:18:41.000000 mara-page-1.7.0/mara_page.egg-info/dependency_links.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       28 2023-05-01 19:18:41.000000 mara-page-1.7.0/mara_page.egg-info/requires.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)       10 2023-05-01 19:18:41.000000 mara-page-1.7.0/mara_page.egg-info/top_level.txt
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      100 2023-01-27 09:00:13.000000 mara-page-1.7.0/pyproject.toml
+-rw-r--r--   0 lschick   (1000) lschick   (1000)      496 2023-05-01 19:18:41.623239 mara-page-1.7.0/setup.cfg
+-rwxr-xr-x   0 lschick   (1000) lschick   (1000)       38 2023-01-27 09:00:13.000000 mara-page-1.7.0/setup.py
```

### Comparing `mara-page-1.6.1/LICENSE` & `mara-page-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mara-page-1.6.1/PKG-INFO` & `mara-page-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mara-page
-Version: 1.6.1
+Version: 1.7.0
 Summary: Minimal API for defining pages of Flask-based backends independently from the actual backend infrastructure
 Home-page: https://github.com/mara/mara-page
 Author: Mara contributors
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,32 +13,32 @@
 
 [![mara-page](https://github.com/mara/mara-page/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-page/actions/workflows/build.yaml)
 [![PyPI - License](https://img.shields.io/pypi/l/mara-page.svg)](https://github.com/mara/mara-page/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-page.svg)](https://badge.fury.io/py/mara-page)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 Minimal API for defining pages of Flask-based backends independently from the actual backend infrastructure.
- 
+
 When a web app is spread across many independent Flask blueprints, then this library can be used to add
 
 - navigation entries
-- page titles 
+- page titles
 - resource-based ACL protection
 - page-specific CSS and JS files
 
-without having access to a global layout or the Flask app. 
+without having access to a global layout or the Flask app.
 
 
-The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a 
+The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a
 backend can use to render the final html page.
-  
+
 ## Example
 
 This is a simple web ui for displaying the current time:
- 
+
 ```python
 """Clock UI"""
 
 import flask
 from awesome_clock import clock
 from mara_page import acl, navigation, response, bootstrap, _
 
@@ -83,15 +83,15 @@
         action_buttons=[
             response.ActionButton('javascript:location.reload()', 'Refresh', 'Refresh clock', 'refresh'),
             response.ActionButton('javascript:location.reload()', 'Update', 'Refresh clock', 'clock-o')
         ]
     )
 ```
 
-It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries. 
+It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries.
 The [mara app](https://github.com/mara/mara-app) will render the response like this:
 
 ![Example backend](https://github.com/mara/mara-page/raw/main/docs/_static/awesome-clock.png)
 
 ## Links
 
 * Documentation: https://mara-page.readthedocs.io/
```

### Comparing `mara-page-1.6.1/README.md` & `mara-page-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 [![mara-page](https://github.com/mara/mara-page/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-page/actions/workflows/build.yaml)
 [![PyPI - License](https://img.shields.io/pypi/l/mara-page.svg)](https://github.com/mara/mara-page/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-page.svg)](https://badge.fury.io/py/mara-page)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 Minimal API for defining pages of Flask-based backends independently from the actual backend infrastructure.
- 
+
 When a web app is spread across many independent Flask blueprints, then this library can be used to add
 
 - navigation entries
-- page titles 
+- page titles
 - resource-based ACL protection
 - page-specific CSS and JS files
 
-without having access to a global layout or the Flask app. 
+without having access to a global layout or the Flask app.
 
 
-The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a 
+The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a
 backend can use to render the final html page.
-  
+
 ## Example
 
 This is a simple web ui for displaying the current time:
- 
+
 ```python
 """Clock UI"""
 
 import flask
 from awesome_clock import clock
 from mara_page import acl, navigation, response, bootstrap, _
 
@@ -72,15 +72,15 @@
         action_buttons=[
             response.ActionButton('javascript:location.reload()', 'Refresh', 'Refresh clock', 'refresh'),
             response.ActionButton('javascript:location.reload()', 'Update', 'Refresh clock', 'clock-o')
         ]
     )
 ```
 
-It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries. 
+It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries.
 The [mara app](https://github.com/mara/mara-app) will render the response like this:
 
 ![Example backend](https://github.com/mara/mara-page/raw/main/docs/_static/awesome-clock.png)
 
 ## Links
 
 * Documentation: https://mara-page.readthedocs.io/
```

### Comparing `mara-page-1.6.1/mara_page/acl.py` & `mara-page-1.7.0/mara_page/acl.py`

 * *Files identical despite different names*

### Comparing `mara-page-1.6.1/mara_page/bootstrap.py` & `mara-page-1.7.0/mara_page/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,46 +21,46 @@
         self.icon = icon
         self.label = label
 
 
 def card(header_left='', header_right='', fixed_header_height: bool = True,
          body=[], sections=[], id: str = None, action_buttons: [str] = None):
     """
-    Renders a bootstrap card `bootstrap_card`_ 
+    Renders a bootstrap card `bootstrap_card`_
 
     Args:
         header_left: A header that is displayed at the top left of the card
         header_right: A header that is displayed at the top right of the card
         fixed_header_height: When true, then the header is restricted to 1 line
         body: Elements to be shown on the card
         sections: Parts of the card that are separated by an horizontal line
         id: An optional id for the outer dom element of the card
     Returns:
         The rendered card
 
     .. _bootstrap_card:
-       https://v4-alpha.getbootstrap.com/components/card/     
+       https://getbootstrap.com/docs/4.6/components/card/
     """
     return _.div(id=id or uuid.uuid1(), class_="card mara-card")[
         (_.div(class_='card-header' + (' fixed-header-height' if fixed_header_height else ''))[
              (_.div(class_='card-header-left')[header_left] if header_left else ''),
              (_.div(class_='card-header-right')[header_right] if header_right else '')]
          if header_left != '' or header_right != ''
          else ''),
 
-        (_.div(class_='card-block')[_.div(class_='card-block-content')[body]] if body else ''),
-        [_.div(class_='card-block card-section')[_.div(class_='card-block-content')[section]]
+        (_.div(class_='card-body')[_.div(class_='card-text')[body]] if body else ''),
+        [_.div(class_='list-group list-group-flush')[_.div(class_='list-group-item')[section]]
          for section in sections] or ''
     ]
 
 
 def table(headers: [str], rows: [], id: str = None):
     """
     Renders a bootstrap table with some defaults applied
-     
+
     Args:
         headers: The column headers (list of strings)
         rows: All table rows (rendered trs)
         id: An optional id for the table
 
     Returns:
         The rendered table
```

### Comparing `mara-page-1.6.1/mara_page/html.py` & `mara-page-1.7.0/mara_page/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,24 @@
     Returns:
         Html markup of the container div
     """
     div_id = div_id or str(uuid.uuid1())
     return _.div(id=div_id)[
         spinner(),
         _.script["""
- 
+
 (function() {
-    // immediately (even before the DOM is completely loaded) set the height of the div 
-    // to the last content height (stored in local storage) to avoid height flickering  
+    // immediately (even before the DOM is completely loaded) set the height of the div
+    // to the last content height (stored in local storage) to avoid height flickering
     var divHeightKey = 'div-height--' + window.location.pathname + '--' + '""" + url + """';
     var divHeight = localStorage.getItem(divHeightKey);
     if (divHeight) {
-        document.getElementById('""" + div_id + """').style.height = divHeight + 'px';    
+        document.getElementById('""" + div_id + """').style.height = divHeight + 'px';
     }
-    
+
     document.addEventListener('DOMContentLoaded', function() {
         if (typeof loadContentAsynchronously == 'undefined') {
             console.error('Please implement function "loadContentAsynchronously"');
         } else {
             loadContentAsynchronously('""" + div_id + """', '""" + url + """', divHeightKey);
         }
     });
```

### Comparing `mara-page-1.6.1/mara_page/navigation.py` & `mara-page-1.7.0/mara_page/navigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,7 @@
         return '<NavigationEntry "' + self.label + '">'
 
     def __hash__(self) -> int:
         return hash((self.label, self.icon, self.description))
 
     def __eq__(self, o: 'NavigationEntry') -> bool:
         return self.label == o.label and self.icon == o.icon and self.description == o.description
-
```

### Comparing `mara-page-1.6.1/mara_page/response.py` & `mara-page-1.7.0/mara_page/response.py`

 * *Files identical despite different names*

### Comparing `mara-page-1.6.1/mara_page/xml.py` & `mara-page-1.7.0/mara_page/xml.py`

 * *Files identical despite different names*

### Comparing `mara-page-1.6.1/mara_page.egg-info/PKG-INFO` & `mara-page-1.7.0/mara_page.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mara-page
-Version: 1.6.1
+Version: 1.7.0
 Summary: Minimal API for defining pages of Flask-based backends independently from the actual backend infrastructure
 Home-page: https://github.com/mara/mara-page
 Author: Mara contributors
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,32 +13,32 @@
 
 [![mara-page](https://github.com/mara/mara-page/actions/workflows/build.yaml/badge.svg)](https://github.com/mara/mara-page/actions/workflows/build.yaml)
 [![PyPI - License](https://img.shields.io/pypi/l/mara-page.svg)](https://github.com/mara/mara-page/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/mara-page.svg)](https://badge.fury.io/py/mara-page)
 [![Slack Status](https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social)](https://communityinviter.com/apps/mara-users/public-invite)
 
 Minimal API for defining pages of Flask-based backends independently from the actual backend infrastructure.
- 
+
 When a web app is spread across many independent Flask blueprints, then this library can be used to add
 
 - navigation entries
-- page titles 
+- page titles
 - resource-based ACL protection
 - page-specific CSS and JS files
 
-without having access to a global layout or the Flask app. 
+without having access to a global layout or the Flask app.
 
 
-The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a 
+The library provides a drop-in werkzeug ``Response`` class that is enriched with additional information that a
 backend can use to render the final html page.
-  
+
 ## Example
 
 This is a simple web ui for displaying the current time:
- 
+
 ```python
 """Clock UI"""
 
 import flask
 from awesome_clock import clock
 from mara_page import acl, navigation, response, bootstrap, _
 
@@ -83,15 +83,15 @@
         action_buttons=[
             response.ActionButton('javascript:location.reload()', 'Refresh', 'Refresh clock', 'refresh'),
             response.ActionButton('javascript:location.reload()', 'Update', 'Refresh clock', 'clock-o')
         ]
     )
 ```
 
-It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries. 
+It is up to the actual Flask app to define how to render such a response and what to do with the ACL resources and navigation entries.
 The [mara app](https://github.com/mara/mara-app) will render the response like this:
 
 ![Example backend](https://github.com/mara/mara-page/raw/main/docs/_static/awesome-clock.png)
 
 ## Links
 
 * Documentation: https://mara-page.readthedocs.io/
```

