# Comparing `tmp/hdsr_fewspy-1.2.tar.gz` & `tmp/hdsr_fewspy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.2.tar", last modified: Wed Apr 26 16:28:17 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.3.tar", last modified: Mon May  1 14:59:36 2023, max compression
```

## Comparing `hdsr_fewspy-1.2.tar` & `hdsr_fewspy-1.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    22492 2023-04-26 16:28:19.000000 hdsr_fewspy-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    21631 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/
--rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    14174 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     8173 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     5719 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2636 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4258 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      956 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    11635 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     6652 2023-04-26 16:17:41.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    22492 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-26 16:28:17.000000 hdsr_fewspy-1.2/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-04-26 16:28:19.000000 hdsr_fewspy-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1672 2023-04-26 16:27:58.000000 hdsr_fewspy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    22740 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21864 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      331 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    13821 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     8329 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     5781 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2636 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6001 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      942 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     6599 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1811 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3051 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4570 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      384 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-01 14:10:38.000000 hdsr_fewspy-1.3/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1405 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4332 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      713 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    13380 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     6655 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3967 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    22740 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 14:59:36.000000 hdsr_fewspy-1.3/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-01 14:59:37.000000 hdsr_fewspy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-01 14:59:17.000000 hdsr_fewspy-1.3/setup.py
```

### Comparing `hdsr_fewspy-1.2/LICENSE.txt` & `hdsr_fewspy-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/PKG-INFO` & `hdsr_fewspy-1.3/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: hdsr_fewspy
-Version: 1.2
-Summary: A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
+Name: hdsr-fewspy
+Version: 1.3
+Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.2.tar.gz
-Keywords: hdsr,fews,api
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.3.tar.gz
+Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -146,14 +146,15 @@
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
+# ...etc...
 ```
 
 5. get_timezone_id
 ```
 response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
 
 # verify response
@@ -176,14 +177,15 @@
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
 )
 
+print(responses[0].text)
 # <?xml version="1.0" encoding="UTF-8"?>
 # <TimeSeries xmlns="http://www.wldelft.nl/fews/PI" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.wldelft.nl/fews/PI http://fews.wldelft.nl/schemas/version1.0/pi-schemas/pi_timeseries.xsd" version="1.25" xmlns:fs="http://www.wldelft.nl/fews/fs">
 #     <timeZone>0.0</timeZone>
 #     <series>
 #         <header>
 #             <type>instantaneous</type>
 #             <moduleInstanceId>WerkFilter</moduleInstanceId>
@@ -204,15 +206,15 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are aggregated into one dataframe. 
+# If your output_choice is dataframe, then all responses are collected in one dataframe. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
@@ -237,14 +239,15 @@
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
 )
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
+# <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
 # If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
@@ -322,31 +325,33 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (26 april 2023)
+### Test Coverage (May 1st 2023)
 ```
+-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
+
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   98     10    90%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           71      6    92%
+hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
@@ -359,15 +364,15 @@
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            12      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1495    183    88%
+TOTAL                                                              1497    183    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.2/README.md` & `hdsr_fewspy-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
+# ...etc...
 ```
 
 5. get_timezone_id
 ```
 response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
 
 # verify response
@@ -154,14 +155,15 @@
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
 )
 
+print(responses[0].text)
 # <?xml version="1.0" encoding="UTF-8"?>
 # <TimeSeries xmlns="http://www.wldelft.nl/fews/PI" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.wldelft.nl/fews/PI http://fews.wldelft.nl/schemas/version1.0/pi-schemas/pi_timeseries.xsd" version="1.25" xmlns:fs="http://www.wldelft.nl/fews/fs">
 #     <timeZone>0.0</timeZone>
 #     <series>
 #         <header>
 #             <type>instantaneous</type>
 #             <moduleInstanceId>WerkFilter</moduleInstanceId>
@@ -182,15 +184,15 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are aggregated into one dataframe. 
+# If your output_choice is dataframe, then all responses are collected in one dataframe. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
@@ -215,14 +217,15 @@
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
 )
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
+# <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
 # If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
@@ -300,31 +303,33 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (26 april 2023)
+### Test Coverage (May 1st 2023)
 ```
+-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
+
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   98     10    90%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           71      6    92%
+hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
@@ -337,15 +342,15 @@
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            12      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1495    183    88%
+TOTAL                                                              1497    183    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,42 +288,40 @@
 
 # TODO: don't use strings as urls...
 
 # Done: authenticate by GET request a hdsr-mid repo (yet to build) that holds email_token items per user
 
 # DONE: test other get requests than get_timeseries
 
-# TODO: improve documentation
+# DONE: improve documentation
 
 # DONE: enable users to override Api.pi_settings
 
 # DONE: conversion client - server timezone
 
 # DONE: fix moduleInstanceIds and filterId
 
 # DONE: wat als iemand alleen maar statistieken wil van tijdseries?
 
 # DONE: besides allowed_request_args use a required_request_args (get_locations zonder filter duurt tering lang!!)
 
-# TODO: create pypi package
-
+# DONE: create pypi package
 
 # TODO: Ciska wel interesse wel in:
 #  --------------------------------
 #  get_samples (grote request)
 #  - Deltares is hier begin 2024 klaar. Nu geeft FEWS EFICS piwebservice na 2 of 5 minuten een timeout
 #  get_timeseries (grote request)
 #  - altijd start + end
 #  - altijd omitEmptyTimeSeries op True anders geeft ie minimaal weken aan tijdseries terug
 #  - vaak filter_id
 #  - soms parameter_id, location_id, moduleinstance_id
 #  - heel soms qualifier_id
 #  get_parameters (middlegrote request = 400 parameters)
 #  get_locations (kleine request = 300 locaties)
-#
 
 # TODO: Ciska geen interesse in:
 #  --------------------------------
 #  get_qualifiers
 
 # TODO: check of properties goed meekomen in get_timeseries in PI_JSON (in PI_XML gaat het goed) -> Ciska:" bij
 #  EFICS werkt niet helemaal lekker. bij get_samples gaat het helemaal fout"
@@ -333,15 +331,7 @@
 
 # TODO: use onlyHeader=True kan voor get_timeseries en get_samples (beide hebben ook start + eind).
 #  Echter, get_qualifiers heeft dat niet. FEWS-WIS response is snel (<1sec). FEWS-EFICS duurt lang (8 sec)
 #  get_lcoations duurt 7 sec.
 #  Voorstel Ciska: alleen func get_timeseries + get_samples via PiWebService. De andere request disabelen:
 #  logger.info('Stuur ciska.overbeek@hdsr.nl een mailtje of dat lijstje mag, dan krijg je er ook nog meer info bij)
 #  die lijstjes worden 2 a 3 per jaar script + handmatig ge-update.
-
-# TODO: add usage examples to readme.md
-#  pip install hdsr_fewspy
-#  user + token
-#  request naar repo met bovenstaande csv (check)
-#  api = Api(user=rob, token=adsfads;flkj, output_folder=..., convert_output_to_csv=False)
-#  response = api.get_time_series(parameter_ids=['H.G.0'])
-#  # TODO: voor Ciska belangrijk dat er een xml uitkomt
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from hdsr_fewspy.constants.choices import PiRestDocumentFormatChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.converters.utils import datetime_to_fews_str
 from hdsr_fewspy.converters.xml_to_python_obj import parse
 from hdsr_fewspy.date_frequency import DateFrequencyBuilder
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import logging
 import pandas as pd
 
 
@@ -90,22 +91,23 @@
         ]
 
     def _download_timeseries(
         self,
         date_ranges: List[Tuple[pd.Timestamp, pd.Timestamp]],
         date_range_freq: pd.Timedelta,
         request_params: Dict,
+        responses: Optional[List[ResponseType]] = None,
     ) -> List[ResponseType]:
         """Download timeseries in little chunks by updating parameters 'startTime' and 'endTime' every loop.
 
         Before each download of actual timeseries we first check nr_timestamps_in_response (a small request with
         showHeaders=True, and showStatistics=True). If that number if outside a certain bandwith, then we update
         (smaller or larger windows) parameters 'startTime' and 'endTime' again.
         """
-        responses = []
+        responses = responses if responses else []
         for request_index, (data_range_start, data_range_end) in enumerate(date_ranges):
             # update start and end in request params
             request_params["startTime"] = datetime_to_fews_str(data_range_start)
             request_params["endTime"] = datetime_to_fews_str(data_range_end)
             nr_timestamps_in_response = self._get_nr_timestamps(request_params=request_params)
             logger.debug(f"nr_timestamps_in_response={nr_timestamps_in_response}")
             new_date_range_freq = DateFrequencyBuilder.optional_change_date_range_freq(
@@ -124,14 +126,15 @@
                 )
                 logger.info(f"Updated request time-window from {date_range_freq} to {new_date_range_freq}")
                 # continue with recursive call with updated (smaller or larger) time-window
                 return self._download_timeseries(
                     date_ranges=new_date_ranges,
                     date_range_freq=new_date_range_freq,
                     request_params=request_params,
+                    responses=responses,
                 )
             else:
                 DateFrequencyBuilder.log_progress_download_ts(
                     data_range_start=data_range_start,
                     data_range_end=data_range_end,
                     ts_end=pd.Timestamp(self.end_time),
                 )
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,25 +44,27 @@
             OutputChoices.xml_file_in_download_dir,
             OutputChoices.json_file_in_download_dir,
             OutputChoices.csv_file_in_download_dir,
         ]
 
     def run(self) -> List[Path]:
         all_file_paths = []
+        responses = []
         cartesian_parameters_list = self._get_cartesian_parameters_list(parameters=self.initial_fews_parameters)
         for index, request_params in enumerate(cartesian_parameters_list):
             date_ranges, date_range_freq = DateFrequencyBuilder.create_date_ranges_and_frequency_used(
                 startdate_obj=pd.Timestamp(self.start_time),
                 enddate_obj=pd.Timestamp(self.end_time),
                 frequency=self.request_settings.default_request_period,
             )
             responses = self._download_timeseries(
                 date_ranges=date_ranges,
                 date_range_freq=date_range_freq,
                 request_params=request_params,
+                responses=responses,
             )
             file_name_keys = ["locationIds", "parameterIds", "qualifierIds", "startTime", "endTime"]
             file_name_values = [request_params.get(param, None) for param in file_name_keys]
             file_paths_created = self.response_manager.run(
                 responses=responses,
                 file_name_values=file_name_values,
                 drop_missing_values=self.drop_missing_values,
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.3/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.3/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/constants/paths.py` & `hdsr_fewspy-1.3/hdsr_fewspy/constants/paths.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.3/hdsr_fewspy/constants/pi_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.3/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.3/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.3/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.3/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.3/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.3/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.3/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.3/hdsr_fewspy/permissions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.3/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/secrets.py` & `hdsr_fewspy-1.3/hdsr_fewspy/secrets.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 class RequestTimeSeriesSingle2(RequestTimeSeriesBase):
     """Single as we use 1 location_ids and 1 parameter_ids."""
 
     # OW433001 H.G.O loopt van 29 sep 2011 tm 17 jan 2023 (filters: WIS/Werkfilter, WIS/Metingenfilter, HDSR/CAW)
     location_ids = "OW433001"
     parameter_ids = "H.G.0"
     start_time = datetime(2012, 1, 1)
-    end_time = datetime(2012, 6, 1)  # get many timestamp
+    # end_time = datetime(2012, 6, 1)  # 11227 df rows?? get many timestamp
+    end_time = datetime(2016, 1, 1)  # 9157 df rows ??
 
     @classmethod
     def file_dir_expected_files(cls) -> Path:
         return Path("not used in test")
 
 
 class RequestTimeSeriesMulti1(RequestTimeSeriesBase):
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,14 @@
 
 import pytest
 
 
 # silence flake8
 fixture_api_sa_no_download_dir = fixture_api_sa_no_download_dir
 
-a = {
-    "version": "1.25",
-    "filters": [
-        {
-            "id": "INTERNAL-API",
-            "name": "INTERNAL-API",
-            "child": [{"id": "INTERNAL-API.RUWMET", "name": "Ruwe metingen (punt)"}],
-        }
-    ],
-}
-
 
 def test_sa_filters_json(fixture_api_sa_no_download_dir):
     response = fixture_api_sa_no_download_dir.get_filters(output_choice=OutputChoices.json_response_in_memory)
     assert response.status_code == 200
 
 
 def test_sa_filters_dataframe(fixture_api_sa_no_download_dir):
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,15 +56,19 @@
             location_ids=request_data.location_ids,
             parameter_ids=request_data.parameter_ids,
             start_time=request_data.start_time,
             end_time=request_data.end_time,
             output_choice=OutputChoices.json_response_in_memory,
         )
     except Exception as err:
-        msg = "invalid output_choice 'json_response_in_memory'. GetTimeSeriesMulti has valid_output_choices ['xml_file_in_download_dir', 'json_file_in_download_dir', 'csv_file_in_download_dir']. See earlier logging why we use GetTimeSeriesMulti."
+        msg = (
+            "invalid output_choice 'json_response_in_memory'. GetTimeSeriesMulti has valid_output_choices "
+            "['xml_file_in_download_dir', 'json_file_in_download_dir', 'csv_file_in_download_dir']. See earlier "
+            "logging why we use GetTimeSeriesMulti."
+        )
         assert err.args[0] == msg
 
 
 def test_sa_multi_timeseries_1_ok_json_download(fixture_api_sa_with_download_dir):
     """OutputChoices.json_file_in_download_dir"""
     api = fixture_api_sa_with_download_dir
     request_data = fixtures_requests.RequestTimeSeriesMulti1
@@ -72,17 +76,18 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_file_in_download_dir,
     )
-    assert len(all_file_paths) == 2
+    assert len(all_file_paths) == 3
     assert all_file_paths[0].name == "gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json"
     assert all_file_paths[1].name == "gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json"
+    assert all_file_paths[2].name == "gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json"
 
     mapper_expected_jsons = request_data.get_expected_jsons()
     for downloaded_file in all_file_paths:
         with open(downloaded_file.as_posix()) as src:
             found_json = json.load(src)
         expected_json = mapper_expected_jsons[downloaded_file.stem]
         assert found_json == expected_json
@@ -96,17 +101,18 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_file_in_download_dir,
     )
-    assert len(all_file_paths) == 2
+    assert len(all_file_paths) == 3
     assert all_file_paths[0].name == "gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.xml"
     assert all_file_paths[1].name == "gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.xml"
+    assert all_file_paths[2].name == "gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.xml"
 
     mapper_expected_xmls = request_data.get_expected_xmls()
     for downloaded_file in all_file_paths:
         found = parse(downloaded_file.as_posix())
         found_header = found.TimeSeries.series.header
         found_events = found.TimeSeries.series.event
 
@@ -151,19 +157,25 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_file_in_download_dir,
     )
-    assert len(all_file_paths) == 4
+    assert len(all_file_paths) == 10
     assert all_file_paths[0].name == "gettimeseriesmulti_kw215712_qby_20050101t000000z_20050102t000000z_0.json"
     assert all_file_paths[1].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_0.json"
-    assert all_file_paths[2].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_0.json"
-    assert all_file_paths[3].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.json"
+    assert all_file_paths[2].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_1.json"
+    assert all_file_paths[3].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_0.json"
+    assert all_file_paths[4].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_1.json"
+    assert all_file_paths[5].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_2.json"
+    assert all_file_paths[6].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.json"
+    assert all_file_paths[7].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_1.json"
+    assert all_file_paths[8].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_2.json"
+    assert all_file_paths[9].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_3.json"
 
     mapper_expected_jsons = request_data.get_expected_jsons()
     for downloaded_file in all_file_paths:
         with open(downloaded_file.as_posix()) as src:
             found_json = json.load(src)
         expected_json = mapper_expected_jsons[downloaded_file.stem]
         assert found_json == expected_json
@@ -177,19 +189,25 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_file_in_download_dir,
     )
-    assert len(all_file_paths) == 4
+    assert len(all_file_paths) == 10
     assert all_file_paths[0].name == "gettimeseriesmulti_kw215712_qby_20050101t000000z_20050102t000000z_0.xml"
     assert all_file_paths[1].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[2].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_0.xml"
-    assert all_file_paths[3].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.xml"
+    assert all_file_paths[2].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z_1.xml"
+    assert all_file_paths[3].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_0.xml"
+    assert all_file_paths[4].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_1.xml"
+    assert all_file_paths[5].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z_2.xml"
+    assert all_file_paths[6].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.xml"
+    assert all_file_paths[7].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_1.xml"
+    assert all_file_paths[8].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_2.xml"
+    assert all_file_paths[9].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_3.xml"
 
     mapper_expected_xmls = request_data.get_expected_xmls()
     for downloaded_file in all_file_paths:
         try:
             found = parse(downloaded_file.as_posix())
             found_header = found.TimeSeries.series.header
             found_events = found.TimeSeries.series.event
@@ -199,15 +217,15 @@
             expected_events = expected.TimeSeries.series.event
 
             assert found_header.timeStep._attributes["unit"] == expected_header.timeStep._attributes["unit"]
             assert len(found_events) == len(expected_events)
             assert found_events[0]._attributes["date"] == expected_events[0]._attributes["date"]
             assert found_events[-1]._attributes["date"] == expected_events[-1]._attributes["date"]
         except AttributeError:
-            assert downloaded_file.name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_0.xml"
+            assert downloaded_file.name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z_3.xml"
             found = parse(downloaded_file.as_posix())
             expected = mapper_expected_xmls[downloaded_file.stem]
             for x in (found, expected):
                 assert x.root.doc.response_http_status.cdata == "400"
                 assert x.root.doc.response_text.cdata == "No timeSeries found"
 
 
@@ -219,16 +237,17 @@
     all_file_paths = api.get_time_series_multi(
         location_ids=request_data.location_ids,
         parameter_ids=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.csv_file_in_download_dir,
     )
-    assert len(all_file_paths) == 2
+    assert len(all_file_paths) == 3
     assert all_file_paths[0].name == "gettimeseriesmulti_kw215712_ddy_20050101t000000z_20050102t000000z.csv"
     assert all_file_paths[1].name == "gettimeseriesmulti_kw322613_qby_20050101t000000z_20050102t000000z.csv"
+    assert all_file_paths[2].name == "gettimeseriesmulti_kw322613_ddy_20050101t000000z_20050102t000000z.csv"
 
     mapper_csv_expected = request_data.get_expected_dfs_from_csvs()
     for downloaded_file in all_file_paths:
         df_found = pd.read_csv(filepath_or_buffer=downloaded_file, sep=",")
         df_expected = mapper_csv_expected[downloaded_file.stem]
         pd.testing.assert_frame_equal(left=df_found, right=df_expected)
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,36 +122,36 @@
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.json_response_in_memory,
     )
-    assert len(responses) == 2
+    assert len(responses) == 11
 
 
 def test_sa_single_timeseries_2_ok_xml_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingle2
 
     responses = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.xml_response_in_memory,
     )
-    assert len(responses) == 2
+    assert len(responses) == 11
 
 
 def test_sa_single_timeseries_2_ok_df_memory(fixture_api_sa_no_download_dir):
     api = fixture_api_sa_no_download_dir
     request_data = fixtures_requests.RequestTimeSeriesSingle2
 
     df_found = api.get_time_series_single(
         location_id=request_data.location_ids,
         parameter_id=request_data.parameter_ids,
         start_time=request_data.start_time,
         end_time=request_data.end_time,
         output_choice=OutputChoices.pandas_dataframe_in_memory,
     )
-    assert len(df_found) == 11227
+    assert len(df_found) == 199251
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.3/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: hdsr-fewspy
-Version: 1.2
-Summary: A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
+Name: hdsr_fewspy
+Version: 1.3
+Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.2.tar.gz
-Keywords: hdsr,fews,api
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.3.tar.gz
+Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -146,14 +146,15 @@
     
 # id      name               group_id
 # -----------------------------------
 # ergkrap erg krap (max 10%) None
 # krap    krap (max 30%)     None
 # normaal normaal (max 50%)  None
 # ruim    ruim (max 70%)     None
+# ...etc...
 ```
 
 5. get_timezone_id
 ```
 response = api.get_timezone_id(output_choice=OutputChoices.json_response_in_memory)
 
 # verify response
@@ -176,14 +177,15 @@
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_response_in_memory,
 )
 
+print(responses[0].text)
 # <?xml version="1.0" encoding="UTF-8"?>
 # <TimeSeries xmlns="http://www.wldelft.nl/fews/PI" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.wldelft.nl/fews/PI http://fews.wldelft.nl/schemas/version1.0/pi-schemas/pi_timeseries.xsd" version="1.25" xmlns:fs="http://www.wldelft.nl/fews/fs">
 #     <timeZone>0.0</timeZone>
 #     <series>
 #         <header>
 #             <type>instantaneous</type>
 #             <moduleInstanceId>WerkFilter</moduleInstanceId>
@@ -204,15 +206,15 @@
 #         <event date="2012-01-01" time="00:15:00" value="-0.35" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="00:45:00" value="-0.36" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:30:00" value="-0.37" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="02:31:17" value="-0.38" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         <event date="2012-01-01" time="03:15:00" value="-0.39" flag="0" fs:PRIMAIR="OK" fs:VISUEEL="OK"/>
 #         ...etc..
 
-# If your output_choice is dataframe, then all responses are aggregated into one dataframe. 
+# If your output_choice is dataframe, then all responses are collected in one dataframe. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
 
 df = api.get_time_series_single(
     location_id = "OW433001",
     parameter_id = "H.G.0",
     start_time = datetime(year=2012, month=1, day=1),
     end_time = datetime(year=2012, month=1, day=2),
@@ -237,14 +239,15 @@
     end_time = datetime(year=2012, month=1, day=2),
     output_choice = OutputChoices.xml_file_in_download_dir,
 )
 
 print(list_with_donwloaded_csv_filepaths)
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433001_hg0_20120101t000000z_20120102t000000z_0.json
 # <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_0.json
+# <output_directory_root>/hdsr_fewspy_<datetime>/gettimeseriesmulti_ow433002_hg0_20120101t000000z_20120102t000000z_1.json
 
 
 # If output_choice is csv to file, then all responses per unique combi are grouped in one csv file. 
 # Arguments 'flag_threshold' and 'drop_missing_values' do have effect.
   
 list_with_donwloaded_csv_filepaths = api.get_time_series_multi(
     location_ids = ["OW433001", "OW433002"]
@@ -322,31 +325,33 @@
 
 ### Releases
 TODO
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (26 april 2023)
+### Test Coverage (May 1st 2023)
 ```
+-- Docs: https://docs.pytest.org/en/stable/how-to/capture-warnings.html
+
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                               8      0   100%
 hdsr_fewspy\api.py                                                   98     10    90%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
 hdsr_fewspy\api_calls\get_timezone_id.py                             26      1    96%
-hdsr_fewspy\api_calls\time_series\base.py                            91      6    93%
-hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           71      6    92%
+hdsr_fewspy\api_calls\time_series\base.py                            92      6    93%
+hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           72      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          34      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
 hdsr_fewspy\constants\paths.py                                       11      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 73      7    90%
@@ -359,15 +364,15 @@
 hdsr_fewspy\date_frequency.py                                        46      5    89%
 hdsr_fewspy\exceptions.py                                            12      0   100%
 hdsr_fewspy\permissions.py                                           67      5    93%
 hdsr_fewspy\retry_session.py                                         68     12    82%
 hdsr_fewspy\secrets.py                                               64     20    69%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1495    183    88%
+TOTAL                                                              1497    183    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.2/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.3/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/pyproject.toml` & `hdsr_fewspy-1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.2/setup.py` & `hdsr_fewspy-1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.2"
+version = "1.3"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
@@ -23,26 +23,22 @@
 tests_require = ["pytest", "pytest-cov"]
 
 setup(
     name="hdsr_fewspy",
     packages=find_packages(include=["hdsr_fewspy", "hdsr_fewspy.*"]),
     version=version,
     license="MIT",
-    description="A python project to get data (locations, timeseries, etc.) from a HDSR FEWS PiWebService",
+    description="A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Renier Kramer",
     author_email="renier.kramer@hdsr.nl",
     url="https://github.com/hdsr-mid/hdsr_fewspy",
     download_url=f"https://github.com/hdsr-mid/hdsr_fewspy/archive/v{version}.tar.gz",
-    keywords=[
-        "hdsr",
-        "fews",
-        "api",
-    ],
+    keywords=["hdsr", "fews", "api", "fewspy", "wis"],
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={"test": tests_require},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

