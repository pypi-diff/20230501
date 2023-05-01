# Comparing `tmp/harmony-py-0.4.6.tar.gz` & `tmp/harmony-py-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-py-0.4.6.tar", last modified: Mon Mar 20 16:39:04 2023, max compression
+gzip compressed data, was "harmony-py-0.4.7.tar", last modified: Mon May  1 15:02:22 2023, max compression
```

## Comparing `harmony-py-0.4.6.tar` & `harmony-py-0.4.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:39:04.330394 harmony-py-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-20 16:38:35.000000 harmony-py-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-03-20 16:38:35.000000 harmony-py-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-20 16:38:35.000000 harmony-py-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-20 16:39:04.330394 harmony-py-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-20 16:38:35.000000 harmony-py-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:39:04.330394 harmony-py-0.4.6/harmony/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-20 16:38:58.000000 harmony-py-0.4.6/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-20 16:38:35.000000 harmony-py-0.4.6/harmony/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-20 16:38:35.000000 harmony-py-0.4.6/harmony/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    49993 2023-03-20 16:38:35.000000 harmony-py-0.4.6/harmony/harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-20 16:38:35.000000 harmony-py-0.4.6/harmony/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:39:04.330394 harmony-py-0.4.6/harmony_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-20 16:39:04.000000 harmony-py-0.4.6/harmony_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-20 16:39:04.000000 harmony-py-0.4.6/harmony_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:39:04.000000 harmony-py-0.4.6/harmony_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-20 16:39:04.000000 harmony-py-0.4.6/harmony_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 16:39:04.000000 harmony-py-0.4.6/harmony_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 16:39:04.330394 harmony-py-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-20 16:38:35.000000 harmony-py-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:39:04.330394 harmony-py-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-03-20 16:38:35.000000 harmony-py-0.4.6/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    47105 2023-03-20 16:38:35.000000 harmony-py-0.4.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-20 16:38:35.000000 harmony-py-0.4.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-20 16:38:35.000000 harmony-py-0.4.6/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-20 16:38:35.000000 harmony-py-0.4.6/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-01 15:01:37.000000 harmony-py-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-01 15:01:37.000000 harmony-py-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 15:01:37.000000 harmony-py-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-01 15:02:22.720744 harmony-py-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-01 15:01:37.000000 harmony-py-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/harmony/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 15:02:16.000000 harmony-py-0.4.7/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50839 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 15:01:37.000000 harmony-py-0.4.7/harmony/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/harmony_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 15:02:22.000000 harmony-py-0.4.7/harmony_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 15:02:22.724745 harmony-py-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-01 15:01:37.000000 harmony-py-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:22.720744 harmony-py-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47105 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 15:01:37.000000 harmony-py-0.4.7/tests/test_util.py
```

### Comparing `harmony-py-0.4.6/CONTRIBUTING.md` & `harmony-py-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/LICENSE` & `harmony-py-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/PKG-INFO` & `harmony-py-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.6
+Version: 0.4.7
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `harmony-py-0.4.6/README.md` & `harmony-py-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/harmony/auth.py` & `harmony-py-0.4.7/harmony/auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/harmony/config.py` & `harmony-py-0.4.7/harmony/config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/harmony/harmony.py` & `harmony-py-0.4.7/harmony/harmony.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,17 @@
         max_results: limits the number of input granules processed in the request
 
         concatenate: Whether to invoke a service that supports concatenation
 
         skip_preview: Whether Harmony should skip auto-pausing and generating a preview for
           large jobs
 
+        ignore_errors: if "true", continue processing a request to completion
+          even if some items fail
+
         destination_url: Destination URL specified by the client
           (only S3 is supported, e.g. s3://my-bucket-name/mypath)
 
         grid: The name of the output grid to use for regridding requests. The name must
           match the UMM grid name in the CMR.
 
     Returns:
@@ -238,14 +241,15 @@
                  scale_extent: List[float] = None,
                  scale_size: List[float] = None,
                  shape: Optional[Tuple[IO, str]] = None,
                  variables: List[str] = ['all'],
                  width: int = None,
                  concatenate: bool = None,
                  skip_preview: bool = None,
+                 ignore_errors: bool = None,
                  grid: str = None):
         """Creates a new Request instance from all specified criteria.'
         """
         self.collection = collection
         self.spatial = spatial
         self.temporal = temporal
         self.dimensions = dimensions
@@ -260,14 +264,15 @@
         self.scale_extent = scale_extent
         self.scale_size = scale_size
         self.shape = shape
         self.variables = variables
         self.width = width
         self.concatenate = concatenate
         self.skip_preview = skip_preview
+        self.ignore_errors = ignore_errors
         self.grid = grid
 
         self.variable_name_to_query_param = {
             'crs': 'outputcrs',
             'destination_url': 'destinationUrl',
             'interpolation': 'interpolation',
             'scale_extent': 'scaleExtent',
@@ -277,14 +282,15 @@
             'granule_name': 'granuleName',
             'width': 'width',
             'height': 'height',
             'format': 'format',
             'max_results': 'maxResults',
             'concatenate': 'concatenate',
             'skip_preview': 'skipPreview',
+            'ignore_errors': 'ignoreErrors',
             'grid': 'grid',
         }
 
         self.spatial_validations = [
             (lambda bb: bb.s <= bb.n, ('Southern latitude must be less than '
                                        'or equal to Northern latitude')),
             (lambda bb: bb.s >= -90.0, 'Southern latitude must be greater than -90.0'),
@@ -386,14 +392,18 @@
     environment variables to authenticate with Earthdata Login, or will use the credentials
     in the user's ``.netrc`` file, if one is available.
 
     To explicitly include the user's credentials::
 
         >>> client = Client(auth=('rfeynman', 'quantumf1eld5'))
 
+    You can also create a Harmony client using user's EDL token::
+
+        >>> client = Client(token='myEDLTokenValue')
+
     By default, the Client will validate the provided credentials immediately. This can be
     disabled by passing ``should_validate_auth=False``.
     """
 
     def __init__(
         self,
         *,
@@ -834,14 +844,15 @@
 
         :raises
             Exception: This can happen if an invalid job_id is provided or Harmony services
             can't be reached.
         """
         # How often to refresh the screen for progress updates and animating spinners.
         ui_update_interval = 0.33  # in seconds
+        running_w_errors_logged = False
 
         intervals = round(self.check_interval / ui_update_interval)
         if show_progress:
             with progressbar.ProgressBar(max_value=100, widgets=progressbar_widgets) as bar:
                 progress = 0
                 while progress < 100:
                     progress, status, message = self.progress(job_id)
@@ -849,14 +860,18 @@
                         raise ProcessingFailedException(job_id, message)
                     if status == 'canceled':
                         print('Job has been canceled.')
                         break
                     if status == 'paused':
                         print('\nJob has been paused. Call `resume()` to resume.', file=sys.stderr)
                         break
+                    if (not running_w_errors_logged and status == 'running_with_errors'):
+                        print('\nJob is running with errors.', file=sys.stderr)
+                        running_w_errors_logged = True
+
                     # This gets around an issue with progressbar. If we update() with 0, the
                     # output shows up as "N/A". If we update with, e.g. 0.1, it rounds down or
                     # truncates to 0 but, importantly, actually displays that.
                     if progress == 0:
                         progress = 0.1
 
                     for _ in range(intervals):
@@ -873,14 +888,17 @@
                 if status == 'failed':
                     raise ProcessingFailedException(job_id, message)
                 if status == 'canceled':
                     break
                 if status == 'paused':
                     print('Job has been paused. Call `resume()` to resume.', file=sys.stderr)
                     break
+                if (not running_w_errors_logged and status == 'running_with_errors'):
+                    print('\nJob is running with errors.', file=sys.stderr)
+                    running_w_errors_logged = True
                 time.sleep(self.check_interval)
 
     def result_json(self,
                     job_id: str,
                     show_progress: bool = False,
                     link_type: LinkType = LinkType.https) -> str:
         """Retrieve a job's final json output.
```

### Comparing `harmony-py-0.4.6/harmony/util.py` & `harmony-py-0.4.7/harmony/util.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/harmony_py.egg-info/PKG-INFO` & `harmony-py-0.4.7/harmony_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-py
-Version: 0.4.6
+Version: 0.4.7
 Summary: The NASA Harmony Python library
 Home-page: https://github.com/nasa/harmony-py
 Keywords: nasa,harmony,remote-sensing,science,geoscience
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `harmony-py-0.4.6/setup.py` & `harmony-py-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/tests/test_auth.py` & `harmony-py-0.4.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/tests/test_client.py` & `harmony-py-0.4.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/tests/test_config.py` & `harmony-py-0.4.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `harmony-py-0.4.6/tests/test_request.py` & `harmony-py-0.4.7/tests/test_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,28 @@
     assert request.is_valid()
     assert request.skip_preview is not None and request.skip_preview == True
 
 def test_request_defaults_to_skip_preview_false():
     request = Request(collection=Collection('foobar'))
     assert not request.skip_preview
 
+def test_request_with_ignore_errors_false():
+    request = Request(collection=Collection('foobar'), ignore_errors=False)
+    assert request.is_valid()
+    assert request.ignore_errors is not None and request.ignore_errors == False
+
+def test_request_with_ignore_errors_true():
+    request = Request(collection=Collection('foobar'), ignore_errors=True)
+    assert request.is_valid()
+    assert request.ignore_errors is not None and request.ignore_errors == True
+
+def test_request_defaults_to_ignore_errors_false():
+    request = Request(collection=Collection('foobar'))
+    assert not request.ignore_errors
+
 @settings(max_examples=100)
 @given(west=st.floats(allow_infinity=True),
        south=st.floats(allow_infinity=True),
        east=st.floats(allow_infinity=True),
        north=st.floats(allow_infinity=True))
 def test_request_spatial_bounding_box(west, south, east, north):
     spatial = BBox(west, south, east, north)
```

