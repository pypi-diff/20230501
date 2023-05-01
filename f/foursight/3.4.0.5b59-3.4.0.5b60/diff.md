# Comparing `tmp/foursight-3.4.0.5b59.tar.gz` & `tmp/foursight-3.4.0.5b60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.4.0.5b59.tar", max compression
+gzip compressed data, was "foursight-3.4.0.5b60.tar", max compression
```

## Comparing `foursight-3.4.0.5b59.tar` & `foursight-3.4.0.5b60.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.0.5b59/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.0.5b59/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.0.5b59/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.0.5b59/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.0.5b59/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.0.5b59/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    59585 2023-01-19 14:12:17.959883 foursight-3.4.0.5b59/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.0.5b59/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.0.5b59/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.0.5b59/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.0.5b59/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.0.5b59/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.0.5b59/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.0.5b59/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.4.0.5b59/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.0.5b59/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.0.5b59/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.0.5b59/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.0.5b59/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.0.5b59/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1271 2023-04-28 12:54:21.017984 foursight-3.4.0.5b59/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 foursight-3.4.0.5b59/setup.py
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 foursight-3.4.0.5b59/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.0.5b60/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.0.5b60/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.0.5b60/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.0.5b60/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.0.5b60/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.0.5b60/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    60938 2023-05-01 15:36:32.611790 foursight-3.4.0.5b60/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.0.5b60/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.0.5b60/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.0.5b60/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.0.5b60/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.0.5b60/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.0.5b60/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.0.5b60/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.4.0.5b60/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.0.5b60/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.0.5b60/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.0.5b60/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.0.5b60/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.0.5b60/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1267 2023-05-01 15:36:59.995542 foursight-3.4.0.5b60/pyproject.toml
+-rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 foursight-3.4.0.5b60/setup.py
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 foursight-3.4.0.5b60/PKG-INFO
```

### Comparing `foursight-3.4.0.5b59/LICENSE.txt` & `foursight-3.4.0.5b60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/app_utils.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/check_schedules.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/check_setup.json` & `foursight-3.4.0.5b60/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/audit_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,40 +62,66 @@
         check.summary = 'Cell line biosources found missing cell_line metadata'
     else:
         check.status = 'PASS'
         check.summary = 'No cell line biosources are missing cell_line metadata'
     return check
 
 
-@check_function()
+@check_function(uuids_to_ignore=None, reset_ignore=False)
 def external_expsets_without_pub(connection, **kwargs):
     '''
     checks external experiment sets to see if they are attributed to a publication
     '''
     check = CheckResult(connection, 'external_expsets_without_pub')
+    # determine which uuids of expsets to ignore
+    expsets_to_ignore = []
+    # check for any new expsets to ignore in kwargs
+    new_ignores = kwargs.get('uuids_to_ignore')
+    if new_ignores:
+        expsets_to_ignore = [u.strip() for u in new_ignores.split(',')]
+
+    last_result = check.get_primary_result()
+    # if last one was fail, find an earlier check with non-FAIL status
+    it = 0
+    while last_result['status'] == 'ERROR' or not last_result['kwargs'].get('primary'):
+        it += 1
+        hours = it * 24  # this is a daily check, so look for checks with 7 days iteration
+        last_result = check.get_closest_result(diff_hours=hours)
+        if it > 7:
+            check.summary = 'Cannot find a non-fail primary check in the past week'
+            check.status = 'ERROR'
+            return check
+    # get any cases to ignore from previous runs and add to any provided uuids
+    if 'ignore' in last_result['full_output']:  # kludge to account for change in result full_output structure
+        expsets_to_ignore.extend(last_result['full_output'].get('ignore', []))
 
     ext = ff_utils.search_metadata('search/?award.project=External&type=ExperimentSet&frame=object',
                                    key=connection.ff_keys, page_limit=50)
     no_pub = []
     for expset in ext:
+        if expset.get('uuid') in expsets_to_ignore:
+            continue
         if not expset.get('publications_of_set') and not expset.get('produced_in_pub'):
             no_pub.append({'uuid': expset['uuid'],
                            '@id': expset['@id'],
                            'description': expset.get('description'),
                            'lab': expset.get('lab'),
                            'error': 'Missing attribution to a publication'})
     if no_pub:
         check.status = 'WARN'
         check.summary = 'External experiment sets found without associated publication. Searched %s' % len(ext)
         check.description = '{} external experiment sets are missing attribution to a publication.'.format(len(no_pub))
     else:
         check.status = 'PASS'
         check.summary = 'No external experiment sets are missing publication. Searched %s' % len(ext)
         check.description = '0 external experiment sets are missing attribution to a publication.'
-    check.full_output = no_pub
+    # see if want to reset ignored
+    if kwargs.get('reset_ignore') is True:
+        expsets_to_ignore = []
+    check.full_output = {'problems': no_pub, 'ignore': expsets_to_ignore}
     check.brief_output = [item['uuid'] for item in no_pub]
     return check
 
 
 @check_function()
 def expset_opfsets_unique_titles(connection, **kwargs):
     '''
```

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/chalicelib_fourfront/package.py` & `foursight-3.4.0.5b60/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.0.5b59/pyproject.toml` & `foursight-3.4.0.5b60/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "foursight"
-version = "3.4.0.5b59"
+version = "3.4.0.5b60"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-dcicutils = "7.3.2.1b2"
+dcicutils = "7.4.0"
 click = "^7.1.2"
 PyJWT = "^2.5.0"
 Jinja2 = "2.10.1"
 MarkupSafe = "1.1.1"
 google-api-python-client = "^1.7.4"
 geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "4.1.0.5b59"
+foursight-core = "4.1.0.5b60"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.4.0.5b59/setup.py` & `foursight-3.4.0.5b60/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils==7.3.2.1b2',
+ 'dcicutils==7.4.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.1.0.5b59',
+ 'foursight-core==4.1.0.5b60',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
  'oauth2client>=4.1.3',
  'pandas>=1.1.4',
  'pytest==5.1.2',
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.4.0.5b59',
+    'version': '3.4.0.5b60',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.4.0.5b59/PKG-INFO` & `foursight-3.4.0.5b60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.4.0.5b59
+Version: 3.4.0.5b60
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (==7.3.2.1b2)
+Requires-Dist: dcicutils (==7.4.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.1.0.5b59)
+Requires-Dist: foursight-core (==4.1.0.5b60)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
```

