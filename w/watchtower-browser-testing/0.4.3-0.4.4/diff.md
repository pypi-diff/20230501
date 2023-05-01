# Comparing `tmp/watchtower_browser_testing-0.4.3.tar.gz` & `tmp/watchtower_browser_testing-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.3.tar", last modified: Tue Apr 25 13:34:14 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.4.tar", last modified: Mon May  1 13:43:38 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.3.tar` & `watchtower_browser_testing-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.328711 watchtower_browser_testing-0.4.3/
--rw-rw-rw-   0        0        0      310 2023-04-25 13:34:14.327710 watchtower_browser_testing-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 13:34:14.328711 watchtower_browser_testing-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.316519 watchtower_browser_testing-0.4.3/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.325666 watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6193 2023-04-18 07:25:52.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    17323 2023-04-25 13:13:32.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-25 13:33:49.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:34:14.323492 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-25 13:34:14.000000 watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 13:43:38.427689 watchtower_browser_testing-0.4.4/
+-rw-rw-rw-   0        0        0      310 2023-05-01 13:43:38.427689 watchtower_browser_testing-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 13:43:38.428746 watchtower_browser_testing-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:43:38.406491 watchtower_browser_testing-0.4.4/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:43:38.417081 watchtower_browser_testing-0.4.4/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    17575 2023-05-01 13:38:29.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-05-01 13:43:06.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-05-01 13:43:38.417081 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-01 13:43:38.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-01 13:43:38.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 13:43:38.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-01 13:43:38.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 13:43:38.000000 watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.3/setup.py` & `watchtower_browser_testing-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                             {{ scenario.description }}
                             {% if scenario.children %}
                                 {% for event in scenario.children %}
                                     <div class="{{ event.type }}" id="container_{{ event.id }}">
                                         {{ event.description }}
                                         {% if test_results %}
                                             {% for test_result in test_results.results %}
-                                                {% if test_result.css_id==event.id and not test_result.ok %}
+                                                {% if test_result.css_id == event.id and not test_result.ok %}
                                                 <div class="alert alert-danger" role="alert" style="margin-top:1rem;">
                                                     <svg xmlns="http://www.w3.org/2000/svg" width="1.2rem" height="1.2rem" fill="currentColor" class="bi bi-exclamation-triangle alert_exclamation" viewBox="0 0 16 16" style="float:left;">
                                                         <path d="M7.938 2.016A.13.13 0 0 1 8.002 2a.13.13 0 0 1 .063.016.146.146 0 0 1 .054.057l6.857 11.667c.036.06.035.124.002.183a.163.163 0 0 1-.054.06.116.116 0 0 1-.066.017H1.146a.115.115 0 0 1-.066-.017.163.163 0 0 1-.054-.06.176.176 0 0 1 .002-.183L7.884 2.073a.147.147 0 0 1 .054-.057zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/>
                                                         <path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/>
                                                     </svg>
                                                     <details>
                                                     <summary style="list-style: none">Test failed for browser <strong>{{ test_result.browser }}</strong></summary>
```

#### html2text {}

```diff
@@ -10,14 +10,14 @@
 content.children %}
 {{ test.description }}
 ** Tests **
 {% for scenario in test.children %}
 {{ scenario.description }} {% if scenario.children %} {% for event in
 scenario.children %}
 {{ event.description }} {% if test_results %} {% for test_result in
-test_results.results %} {% if test_result.css_id==event.id and not
+test_results.results %} {% if test_result.css_id == event.id and not
 test_result.ok %}
      Test failed for browser {{ test_result.browser }} {{ test_result.errors }}
 {% endif %} {% endfor %} {% endif %}
 {% endfor %} {% endif %}
 {% endfor %}
 {% endfor %}
```

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing/testsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,16 @@
         return structure
 
 
 class MeasurementPlan(object):
 
     test_modules = None
     test_directory = None
+    _display_name = None
+    _slug = None
 
     def __init__(self,
                  test_modules=None,
                  test_directory=None):
 
         self.test_modules = self.test_modules or test_modules
         self.test_directory = self.test_directory or test_directory
@@ -475,7 +477,15 @@
                     run_tests_token=None):
 
         jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
         template = jenv.get_template('measurement_plan.html')
 
         return template.render(title=title, content=content,
                                test_results=test_results, run_tests_token=run_tests_token)
+
+    @property
+    def display_name(self):
+        return self._display_name or self.__class__.__name__
+
+    @display_name.setter
+    def display_name(self, value):
+        self._display_name = value
```

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.3/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.4/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

