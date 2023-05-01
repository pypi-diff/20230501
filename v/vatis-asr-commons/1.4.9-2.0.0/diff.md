# Comparing `tmp/vatis_asr_commons-1.4.9.tar.gz` & `tmp/vatis_asr_commons-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vatis_asr_commons-1.4.9.tar", last modified: Tue Feb 21 19:18:41 2023, max compression
+gzip compressed data, was "dist/vatis_asr_commons-2.0.0.tar", last modified: Mon May  1 06:48:09 2023, max compression
```

## Comparing `vatis_asr_commons-1.4.9.tar` & `vatis_asr_commons-2.0.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/
--rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-1.4.9/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.9/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/requirements/
--rw-r--r--   0 mac        (501) staff       (20)       25 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/requirements/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       79 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1906 2023-02-04 10:25:09.000000 vatis_asr_commons-1.4.9/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/
--rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/
--rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6120 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/audio.py
--rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/logging.py
--rw-r--r--   0 mac        (501) staff       (20)     6417 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/config/parse.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/
--rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/constants/custom_models.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/
--rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/en_GB.py
--rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/model.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/ro_RO.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/
--rw-r--r--   0 mac        (501) staff       (20)      922 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/exception.py
--rw-r--r--   0 mac        (501) staff       (20)     2245 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/expression.py
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/find_replace.py
--rw-r--r--   0 mac        (501) staff       (20)      131 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/speaker.py
--rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/spoken_commands.py
--rw-r--r--   0 mac        (501) staff       (20)    10416 2023-02-21 19:15:38.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/domain/transcriber.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/
--rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/i18n_keys.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
--rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/locale/speakers_service.pot
--rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/translate.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/deserialization.py
--rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/json/serialization.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/
--rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/event.py
--rw-r--r--   0 mac        (501) staff       (20)     1562 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/headers.py
--rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/response.py
--rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/sio_topics.py
--rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/live/utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/scaler/response.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/
--rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/security/jwt.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/exceptions.py
--rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-1.4.9/vatis/asr_commons/static/request.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2145 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       25 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-02-21 19:18:41.000000 vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/
+-rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-2.0.0/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.0/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/requirements/
+-rw-r--r--   0 mac        (501) staff       (20)       25 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/requirements/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       79 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1906 2023-05-01 06:47:39.000000 vatis_asr_commons-2.0.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/
+-rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6360 2023-04-09 20:40:42.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/audio.py
+-rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/logging.py
+-rw-r--r--   0 mac        (501) staff       (20)     7643 2023-03-10 11:08:30.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/config/parse.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/constants/
+-rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/constants/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/constants/custom_models.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/
+-rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/en_GB.py
+-rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/model.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/ro_RO.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/
+-rw-r--r--   0 mac        (501) staff       (20)     1702 2023-03-07 11:38:19.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/exception.py
+-rw-r--r--   0 mac        (501) staff       (20)     2146 2023-03-07 10:36:16.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/expression.py
+-rw-r--r--   0 mac        (501) staff       (20)     7410 2023-03-10 10:46:39.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/find_replace.py
+-rw-r--r--   0 mac        (501) staff       (20)      158 2023-04-28 08:59:22.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/speaker.py
+-rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/spoken_commands.py
+-rw-r--r--   0 mac        (501) staff       (20)     8330 2023-03-06 21:08:28.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/transcriber.py
+-rw-r--r--   0 mac        (501) staff       (20)     2599 2023-04-26 19:11:33.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/domain/word.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/
+-rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/i18n_keys.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/en/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/ro/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
+-rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/locale/speakers_service.pot
+-rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/translate.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/json/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/json/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/json/deserialization.py
+-rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/json/serialization.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/
+-rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/event.py
+-rw-r--r--   0 mac        (501) staff       (20)     1629 2023-03-03 19:52:10.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/response.py
+-rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/sio_topics.py
+-rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/live/utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/scaler/
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/scaler/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/scaler/response.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/security/
+-rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/security/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/security/jwt.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/static/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/static/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/static/exceptions.py
+-rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/static/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.0/vatis/asr_commons/static/request.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2178 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (501) staff       (20)       25 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-05-01 06:48:09.000000 vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/top_level.txt
```

### Comparing `vatis_asr_commons-1.4.9/LICENSE.txt` & `vatis_asr_commons-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/PKG-INFO` & `vatis_asr_commons-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis_asr_commons
-Version: 1.4.9
+Version: 2.0.0
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.9/asr_commons-1.4.9.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.0/asr_commons-2.0.0.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-1.4.9/README.md` & `vatis_asr_commons-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/setup.py` & `vatis_asr_commons-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_namespace_packages, setup
 
 __name__ = 'vatis_asr_commons'
-__tag__ = '1.4.9'
+__tag__ = '2.0.0'
 __short_description__ = 'Common objects for Vatis ASR clients'
 __download_url__ = 'https://gitlab.com/vatistech/asr-commons/-/archive/{__tag__}/asr_commons-{__tag__}.zip'\
     .format(__tag__=__tag__)
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/config/__init__.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/config/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/config/audio.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/config/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 
 from vatis.asr_commons.domain import AudioFormatError
 
 
 class Language(Enum):
     ro_RO = 'ro_RO'
     en_GB = 'en_GB'
+    de_DE = 'de_DE'
+    es_ES = 'es_ES'
+    fr_FR = 'fr_FR'
+    en_US = 'en_US'
+    it_IT = 'it_IT'
+    ca_ES = 'ca_ES'
+    pl_PL = 'pl_PL'
+    nl_NL = 'nl_NL'
+    pt_PT = 'pt_PT'
+    pt_BR = 'pt_BR'
+    ru_RU = 'ru_RU'
+    ua_UA = 'ua_UA'
 
 
 class SampleRate(Enum):
     RATE_16000 = 16000
 
 
 class Channel(Enum):
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/config/headers.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/config/headers.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/config/logging.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/config/logging.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/config/parse.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/config/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     FRAME_OVERLAP: ClassVar[str] = 'frame_overlap'
     BUFFER_OFFSET: ClassVar[str] = 'buffer_offset'
 
     HOTWORDS: ClassVar[str] = 'hotwords'
     HOTWORDS_WEIGHT: ClassVar[str] = 'hotwords_weight'
 
     COMMANDS_EXPRESSIONS: ClassVar[str] = 'commands_expression'
+    ENABLE_ON_COMMAND_FINAL_FRAME: ClassVar[str] = 'enable_on_command_final_frame'
     FIND_REPLACE_EXPRESSIONS: ClassVar[str] = 'find_replace_expressions'
 
 
 def parse_post_processing_options(headers) -> Dict[str, Any]:
     post_processing_config: Dict[str, Any] = {}
 
     if DISABLE_DISFLUENCIES_HEADER in headers:
@@ -130,22 +131,44 @@
     if HOTWORDS_WEIGHT_KEY in headers:
         hotwords_config[TranscriptionOptions.HOTWORDS_WEIGHT] = float(headers.get(HOTWORDS_WEIGHT_KEY))
 
     return hotwords_config
 
 
 def parse_formatting_config(headers) -> Dict[str, Any]:
+    from vatis.asr_commons.domain import SpokenCommandConfig
+    from vatis.asr_commons.domain import FindReplaceConfig
+
     config: Dict[str, Any] = {}
 
     if COMMANDS_EXPRESSIONS_HEADER in headers:
-        command_configs = json.loads(headers[COMMANDS_EXPRESSIONS_HEADER])
+        command_configs: list = json.loads(headers[COMMANDS_EXPRESSIONS_HEADER])
+
+        if isinstance(command_configs, dict):
+            command_configs = [SpokenCommandConfig.from_json(command_configs)]
+        elif isinstance(command_configs, list):
+            command_configs = [SpokenCommandConfig.from_json(config) for config in command_configs]
+        else:
+            logger.warning(f'Spoken commands not parsable: {str(headers[COMMANDS_EXPRESSIONS_HEADER])}')
+
         config[TranscriptionOptions.COMMANDS_EXPRESSIONS] = command_configs
 
+    if ENABLE_ON_COMMAND_FINAL_FRAME_HEADER in headers:
+        config[TranscriptionOptions.ENABLE_ON_COMMAND_FINAL_FRAME] = str(headers[ENABLE_ON_COMMAND_FINAL_FRAME_HEADER]).lower() == 'true'
+
     if FIND_REPLACE_EXPRESSIONS_HEADER in headers:
-        find_replace_configs = json.loads(headers[FIND_REPLACE_EXPRESSIONS_HEADER])
+        find_replace_configs: list = json.loads(headers[FIND_REPLACE_EXPRESSIONS_HEADER])
+
+        if isinstance(find_replace_configs, dict):
+            find_replace_configs = [FindReplaceConfig.from_json(find_replace_configs)]
+        elif isinstance(find_replace_configs, list):
+            find_replace_configs = [FindReplaceConfig.from_json(config) for config in find_replace_configs]
+        else:
+            logger.warning(f'find replace not parsable: {str(headers[FIND_REPLACE_EXPRESSIONS_HEADER])}')
+
         config[TranscriptionOptions.FIND_REPLACE_EXPRESSIONS] = find_replace_configs
 
     return config
 
 
 def parse_input_packet(json_packet: dict) -> Union[Base64InputPacket, ConfigPacket]:
     if json_packet.get('type') == PacketType.BASE64_INPUT:
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/__init__.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/custom_models/model.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/custom_models/model.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/exception.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/domain/exception.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/expression.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/domain/expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from os import PathLike
 from pathlib import Path
-from typing import List, Union, Dict, Optional
+from typing import List, Dict, Optional
 
 
 class Expressions:
+
     def __init__(self, expressions: Dict[str, List[str]] = None):
         self._expressions: Dict[str, List[str]] = expressions if expressions is not None else {}
 
     @staticmethod
     def _parse_tsv_string(tsv_str: str) -> Dict[str, List[str]]:
         expressions: Dict[str, List[str]] = {}
 
         for line in tsv_str.split('\n'):
+            line = line.strip()
+
+            if line.startswith('#') or not len(line):
+                continue
+
             tokens = line.split('\t')
             expressions[tokens[0]] = tokens[1:]
 
         return expressions
 
     def get(self, key: str) -> List[str]:
         expressions: Optional[List[str]] = self._expressions.get(key, [])
@@ -44,34 +50,29 @@
     def from_tsv_str(tsv: str) -> 'Expressions':
         expressions = Expressions._parse_tsv_string(tsv)
         return Expressions(expressions)
 
     @staticmethod
     def from_tsv_file(tsv_file: PathLike, raise_if_not_found: bool = False) -> 'Expressions':
         tsv_file = Path(tsv_file)
-        expressions: Dict[str, List[str]] = {}
 
         if tsv_file.exists():
             with open(tsv_file, 'r') as f:
-                for line in f:
-                    line: str = line.strip()
-
-                    if not len(line) or line.startswith('#'):
-                        continue
+                lines = f.readlines()
 
-                    tokens = line.split('\t')
+            tsv = ''.join(lines)
 
-                    expressions[tokens[0]] = tokens[1:]
+            return Expressions.from_tsv_str(tsv)
         else:
             message = f'Expressions path does not exist: {str(tsv_file)}'
 
             if raise_if_not_found:
                 raise FileNotFoundError(message)
 
-        return Expressions(expressions)
+        return Expressions.empty()
 
     @staticmethod
     def empty():
         return Expressions()
 
     @staticmethod
     def from_dict(expressions: Dict[str, List[str]]):
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/spoken_commands.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/domain/spoken_commands.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/domain/transcriber.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/domain/transcriber.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import binascii
 
 import numpy as np
 
-from typing import List, Tuple, Optional, Type, ClassVar, Union
+from typing import List, Tuple, Type, ClassVar
 
+from vatis.asr_commons.domain.word import Word
 from vatis.asr_commons.json.deserialization import JSONDeserializable
 from vatis.asr_commons.live.headers import FLUSH_HEADER, FINAL_FRAME_HEADER
 from vatis.asr_commons.domain.find_replace import FindReplaceConfig
 from vatis.asr_commons.domain.spoken_commands import SpokenCommandConfig
 
 
 class PacketType:
@@ -159,71 +160,14 @@
         super().__init__(headers, type, **kwargs)
         self.transcript = transcript
 
     def __str__(self):
         return f'{{"transcript": {hash(self.transcript)}, {super().__str__()}}}'
 
 
-class Word:
-    class Entity:
-        PERSON: ClassVar[str] = 'PERSON'
-        GPE: ClassVar[str] = 'GPE'
-        LOC: ClassVar[str] = 'LOC'
-        ORG: ClassVar[str] = 'ORG'
-        LANGUAGE: ClassVar[str] = 'LANGUAGE'
-        NAT_REL_POL: ClassVar[str] = 'NAT_REL_POL'
-        DATETIME: ClassVar[str] = 'DATETIME'
-        PERIOD: ClassVar[str] = 'PERIOD'
-        QUANTITY: ClassVar[str] = 'QUANTITY'
-        MONEY: ClassVar[str] = 'MONEY'
-        NUMERIC: ClassVar[str] = 'NUMERIC'
-        ORDINAL: ClassVar[str] = 'ORDINAL'
-        FACILITY: ClassVar[str] = 'FACILITY'
-        WORK_OF_ART: ClassVar[str] = 'WORK_OF_ART'
-        EVENT: ClassVar[str] = 'EVENT'
-        REPLACED: ClassVar[str] = 'REPLACED'
-
-    def __init__(self, word: str, start_time_millis: float, end_time_millis: float, speaker: Optional[Union[str, int]] = None,
-                 confidence: float = 0, entity: Optional[str] = None, entity_group_id: Optional[Union[int, str]] = None):
-        self.word: str = word
-        self.start_time: float = start_time_millis
-        self.end_time: float = end_time_millis
-        self.speaker: str = str(speaker) if speaker is not None else None
-        self.confidence: float = confidence
-        self.entity: Optional[str] = entity
-        self.entity_group_id: Optional[str] = str(entity_group_id) if entity_group_id is not None else None
-
-    def __str__(self):
-        return f'''
-        {{
-            "word": "{self.word}",
-            "start_time": {self.start_time},
-            "end_time": {self.end_time},
-            "speaker": "{self.speaker}",
-            "confidence": {self.confidence},
-            "entity": "{self.entity}",
-            "entity_group_id": {self.entity_group_id}
-        }}
-        '''
-
-    def __repr__(self):
-        return self.__str__()
-
-    def copy(self):
-        return Word(
-            word=self.word,
-            start_time_millis=self.start_time,
-            end_time_millis=self.end_time,
-            speaker=self.speaker,
-            confidence=self.confidence,
-            entity=self.entity,
-            entity_group_id=self.entity_group_id
-        )
-
-
 class TimestampedTranscriptionPacket(TranscriptionPacket):
     """
     Packet that contains the transcript with the timestamps associated to each word.
 
     Params:
      - words: list of transcribed words
      - headers: headers of the packet
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/i18n/translate.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/live/event.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/live/event.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/live/headers.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/live/headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 # request headers ####################################################################################################
 FRAME_LEN_HEADER = 'FrameLength'
 FRAME_OVERLAP_HEADER = 'FrameOverlap'
 BUFFER_OFFSET_HEADER = 'BufferOffset'
 RESERVATION_KEY_HEADER = 'ReservationKey'
 # spoken formatting
 COMMANDS_EXPRESSIONS_HEADER = 'CommandsExpressions'
+ENABLE_ON_COMMAND_FINAL_FRAME_HEADER = 'EnableOnCommandFinalFrame'
 FIND_REPLACE_EXPRESSIONS_HEADER = 'FindReplaceExpressions'
 
 # AMQP message headers ###############################################################################################
 USER_AMQP_HEADER: str = 'UserId'
 MODEL_AMQP_HEADER: str = 'ModelUid'
```

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/live/utils.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/live/utils.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis/asr_commons/static/request.py` & `vatis_asr_commons-2.0.0/vatis/asr_commons/static/request.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/PKG-INFO` & `vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis-asr-commons
-Version: 1.4.9
+Version: 2.0.0
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/1.4.9/asr_commons-1.4.9.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.0/asr_commons-2.0.0.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-1.4.9/vatis_asr_commons.egg-info/SOURCES.txt` & `vatis_asr_commons-2.0.0/vatis_asr_commons.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 vatis/asr_commons/domain/__init__.py
 vatis/asr_commons/domain/exception.py
 vatis/asr_commons/domain/expression.py
 vatis/asr_commons/domain/find_replace.py
 vatis/asr_commons/domain/speaker.py
 vatis/asr_commons/domain/spoken_commands.py
 vatis/asr_commons/domain/transcriber.py
+vatis/asr_commons/domain/word.py
 vatis/asr_commons/i18n/__init__.py
 vatis/asr_commons/i18n/i18n_keys.py
 vatis/asr_commons/i18n/translate.py
 vatis/asr_commons/i18n/locale/speakers_service.pot
 vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
 vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
 vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
```

