# Comparing `tmp/pymarc-4.2.2.tar.gz` & `tmp/pymarc-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymarc-4.2.2.tar", last modified: Mon Jan 30 16:06:16 2023, max compression
+gzip compressed data, was "pymarc-5.0.0.tar", last modified: Mon May  1 12:17:32 2023, max compression
```

## Comparing `pymarc-4.2.2.tar` & `pymarc-5.0.0.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.412038 pymarc-4.2.2/
--rw-r--r--   0 edsummers   (505) staff       (20)      650 2022-03-02 20:54:44.000000 pymarc-4.2.2/CONTRIBUTING.md
--rw-r--r--   0 edsummers   (505) staff       (20)     3061 2022-10-17 20:30:20.000000 pymarc-4.2.2/LICENSE
--rw-r--r--   0 edsummers   (505) staff       (20)      150 2022-03-02 20:54:44.000000 pymarc-4.2.2/MANIFEST.in
--rw-r--r--   0 edsummers   (505) staff       (20)    10745 2023-01-30 16:06:16.412503 pymarc-4.2.2/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)     9943 2022-10-17 20:15:40.000000 pymarc-4.2.2/README.md
--rw-r--r--   0 edsummers   (505) staff       (20)    10604 2022-03-02 20:54:44.000000 pymarc-4.2.2/README_pt_Br.md
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.366038 pymarc-4.2.2/docs/
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.372474 pymarc-4.2.2/docs/source/
--rw-r--r--   0 edsummers   (505) staff       (20)    10360 2022-03-02 20:54:44.000000 pymarc-4.2.2/docs/source/conf.py
--rw-r--r--   0 edsummers   (505) staff       (20)     7532 2022-03-02 20:54:44.000000 pymarc-4.2.2/docs/source/index.rst
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.379245 pymarc-4.2.2/pymarc/
--rw-r--r--   0 edsummers   (505) staff       (20)      552 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/__init__.py
--rw-r--r--   0 edsummers   (505) staff       (20)      467 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/constants.py
--rw-r--r--   0 edsummers   (505) staff       (20)     3283 2022-04-04 22:40:47.000000 pymarc-4.2.2/pymarc/exceptions.py
--rw-r--r--   0 edsummers   (505) staff       (20)    10732 2022-10-17 20:15:40.000000 pymarc-4.2.2/pymarc/field.py
--rw-r--r--   0 edsummers   (505) staff       (20)    10117 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/leader.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6647 2022-03-02 22:13:36.000000 pymarc-4.2.2/pymarc/marc8.py
--rw-r--r--   0 edsummers   (505) staff       (20)   835551 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/marc8_mapping.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2322 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/marcjson.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6483 2022-03-02 22:13:36.000000 pymarc-4.2.2/pymarc/marcxml.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8425 2022-03-02 21:47:58.000000 pymarc-4.2.2/pymarc/reader.py
--rw-r--r--   0 edsummers   (505) staff       (20)    22844 2022-04-04 22:40:47.000000 pymarc-4.2.2/pymarc/record.py
--rw-r--r--   0 edsummers   (505) staff       (20)     6316 2022-03-02 20:54:44.000000 pymarc-4.2.2/pymarc/writer.py
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.381648 pymarc-4.2.2/pymarc.egg-info/
--rw-r--r--   0 edsummers   (505) staff       (20)    10745 2023-01-30 16:06:16.000000 pymarc-4.2.2/pymarc.egg-info/PKG-INFO
--rw-r--r--   0 edsummers   (505) staff       (20)     1252 2023-01-30 16:06:16.000000 pymarc-4.2.2/pymarc.egg-info/SOURCES.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-01-30 16:06:16.000000 pymarc-4.2.2/pymarc.egg-info/dependency_links.txt
--rw-r--r--   0 edsummers   (505) staff       (20)        7 2023-01-30 16:06:16.000000 pymarc-4.2.2/pymarc.egg-info/top_level.txt
--rw-r--r--   0 edsummers   (505) staff       (20)       46 2022-03-02 20:54:44.000000 pymarc-4.2.2/requirements.dev.txt
--rw-r--r--   0 edsummers   (505) staff       (20)      177 2023-01-30 16:06:16.413575 pymarc-4.2.2/setup.cfg
--rw-r--r--   0 edsummers   (505) staff       (20)     1314 2023-01-30 16:05:18.000000 pymarc-4.2.2/setup.py
-drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-01-30 16:06:16.411370 pymarc-4.2.2/test/
--rw-r--r--   0 edsummers   (505) staff       (20)     5344 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/1251.dat
--rw-r--r--   0 edsummers   (505) staff       (20)        0 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/__init__.py
--rw-r--r--   0 edsummers   (505) staff       (20)     1339 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/alphatag.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1632 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_eacc_encoding.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1980 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_indicator.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1491 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_marc8_escape.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1017 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_records.mrc
--rw-r--r--   0 edsummers   (505) staff       (20)      756 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_subfield_code.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     2063 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/bad_tag.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     9063 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/batch.json
--rw-r--r--   0 edsummers   (505) staff       (20)     8247 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/batch.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     2710 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/diacritic.dat
--rw-r--r--   0 edsummers   (505) staff       (20)    20388 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/marc.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1117 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/marc8.dat
--rw-r--r--   0 edsummers   (505) staff       (20)      794 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/multi_isbn.dat
--rw-r--r--   0 edsummers   (505) staff       (20)      755 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/one.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     3260 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/one.json
--rw-r--r--   0 edsummers   (505) staff       (20)    49461 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/regression45.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     6591 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     9410 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test.json
--rw-r--r--   0 edsummers   (505) staff       (20)     1551 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_encode.py
--rw-r--r--   0 edsummers   (505) staff       (20)     7850 2022-10-17 20:15:40.000000 pymarc-4.2.2/test/test_field.py
--rw-r--r--   0 edsummers   (505) staff       (20)     4945 2022-03-02 22:13:36.000000 pymarc-4.2.2/test/test_json.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2869 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_leader.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8734 2022-03-02 22:13:36.000000 pymarc-4.2.2/test/test_marc8.py
--rw-r--r--   0 edsummers   (505) staff       (20)    55430 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_marc8.txt
--rw-r--r--   0 edsummers   (505) staff       (20)     1808 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_ordered_fields.py
--rw-r--r--   0 edsummers   (505) staff       (20)     8939 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_reader.py
--rw-r--r--   0 edsummers   (505) staff       (20)    19644 2022-04-04 22:40:47.000000 pymarc-4.2.2/test/test_record.py
--rw-r--r--   0 edsummers   (505) staff       (20)     1617 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_utf8.py
--rw-r--r--   0 edsummers   (505) staff       (20)    38127 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_utf8.txt
--rw-r--r--   0 edsummers   (505) staff       (20)    20342 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/test_writer.py
--rw-r--r--   0 edsummers   (505) staff       (20)     3907 2022-03-02 22:13:36.000000 pymarc-4.2.2/test/test_xml.py
--rw-r--r--   0 edsummers   (505) staff       (20)     2499 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/testunimarc.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1438 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/utf8.xml
--rw-r--r--   0 edsummers   (505) staff       (20)     1474 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/utf8_errors.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1004 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/utf8_invalid.mrc
--rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/utf8_with_leader_flag.dat
--rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-4.2.2/test/utf8_without_leader_flag.dat
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.842829 pymarc-5.0.0/
+-rw-r--r--   0 edsummers   (505) staff       (20)      650 2022-03-02 20:54:44.000000 pymarc-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0 edsummers   (505) staff       (20)     3061 2023-04-17 10:38:11.000000 pymarc-5.0.0/LICENSE
+-rw-r--r--   0 edsummers   (505) staff       (20)      150 2022-03-02 20:54:44.000000 pymarc-5.0.0/MANIFEST.in
+-rw-r--r--   0 edsummers   (505) staff       (20)    12174 2023-05-01 12:17:32.843049 pymarc-5.0.0/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)    11290 2023-05-01 11:24:10.000000 pymarc-5.0.0/README.md
+-rw-r--r--   0 edsummers   (505) staff       (20)    10604 2022-03-02 20:54:44.000000 pymarc-5.0.0/README_pt_Br.md
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.791262 pymarc-5.0.0/docs/
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.796232 pymarc-5.0.0/docs/source/
+-rw-r--r--   0 edsummers   (505) staff       (20)    10360 2022-03-02 20:54:44.000000 pymarc-5.0.0/docs/source/conf.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8403 2023-05-01 11:24:10.000000 pymarc-5.0.0/docs/source/index.rst
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.804486 pymarc-5.0.0/pymarc/
+-rw-r--r--   0 edsummers   (505) staff       (20)      552 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/__init__.py
+-rw-r--r--   0 edsummers   (505) staff       (20)      467 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/constants.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     3080 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/exceptions.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    13619 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/field.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     9989 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/leader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     6617 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marc8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)   835551 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/marc8_mapping.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2322 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marcjson.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     6443 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/marcxml.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8700 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/reader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    24455 2023-05-01 11:24:10.000000 pymarc-5.0.0/pymarc/record.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     6316 2022-03-02 20:54:44.000000 pymarc-5.0.0/pymarc/writer.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.806640 pymarc-5.0.0/pymarc.egg-info/
+-rw-r--r--   0 edsummers   (505) staff       (20)    12174 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/PKG-INFO
+-rw-r--r--   0 edsummers   (505) staff       (20)     1289 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/SOURCES.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        1 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/dependency_links.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)        7 2023-05-01 12:17:32.000000 pymarc-5.0.0/pymarc.egg-info/top_level.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)      282 2023-04-25 13:12:39.000000 pymarc-5.0.0/release.md
+-rw-r--r--   0 edsummers   (505) staff       (20)       46 2022-03-02 20:54:44.000000 pymarc-5.0.0/requirements.dev.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)      177 2023-05-01 12:17:32.843793 pymarc-5.0.0/setup.cfg
+-rw-r--r--   0 edsummers   (505) staff       (20)     1392 2023-05-01 11:24:10.000000 pymarc-5.0.0/setup.py
+drwxr-xr-x   0 edsummers   (505) staff       (20)        0 2023-05-01 12:17:32.842298 pymarc-5.0.0/test/
+-rw-r--r--   0 edsummers   (505) staff       (20)     5344 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/1251.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)        0 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/__init__.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     1339 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/alphatag.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1632 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_eacc_encoding.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1980 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_indicator.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1491 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_marc8_escape.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1017 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_records.mrc
+-rw-r--r--   0 edsummers   (505) staff       (20)      756 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_subfield_code.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     2063 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/bad_tag.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     9063 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/batch.json
+-rw-r--r--   0 edsummers   (505) staff       (20)     8247 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/batch.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     2710 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/diacritic.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)    20388 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/marc.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1117 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/marc8-to-unicode.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1117 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/marc8.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)      794 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/multi_isbn.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)      755 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/one.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     3260 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/one.json
+-rw-r--r--   0 edsummers   (505) staff       (20)    49461 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/regression45.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     6591 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     9410 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test.json
+-rw-r--r--   0 edsummers   (505) staff       (20)     1551 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_encode.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    11822 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_field.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     5666 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_json.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2869 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_leader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8822 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_marc8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    55430 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_marc8.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)     1923 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_ordered_fields.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     8939 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_reader.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    25406 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_record.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     1652 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_utf8.py
+-rw-r--r--   0 edsummers   (505) staff       (20)    38127 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/test_utf8.txt
+-rw-r--r--   0 edsummers   (505) staff       (20)    23386 2023-05-01 11:24:10.000000 pymarc-5.0.0/test/test_writer.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     3907 2022-03-02 22:13:36.000000 pymarc-5.0.0/test/test_xml.py
+-rw-r--r--   0 edsummers   (505) staff       (20)     2499 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/testunimarc.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1438 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8.xml
+-rw-r--r--   0 edsummers   (505) staff       (20)     1474 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_errors.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1004 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_invalid.mrc
+-rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_with_leader_flag.dat
+-rw-r--r--   0 edsummers   (505) staff       (20)     1123 2022-03-02 20:54:44.000000 pymarc-5.0.0/test/utf8_without_leader_flag.dat
```

### Comparing `pymarc-4.2.2/CONTRIBUTING.md` & `pymarc-5.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/LICENSE` & `pymarc-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/PKG-INFO` & `pymarc-5.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,672 +1,706 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6d61  : 2.1.Name: pyma
-00000020: 7263 0a56 6572 7369 6f6e 3a20 342e 322e  rc.Version: 4.2.
-00000030: 320a 5375 6d6d 6172 793a 2052 6561 642c  2.Summary: Read,
-00000040: 2077 7269 7465 2061 6e64 206d 6f64 6966   write and modif
-00000050: 7920 4d41 5243 2062 6962 6c69 6f67 7261  y MARC bibliogra
-00000060: 7068 6963 2064 6174 610a 486f 6d65 2d70  phic data.Home-p
-00000070: 6167 653a 2068 7474 703a 2f2f 6769 746c  age: http://gitl
-00000080: 6162 2e63 6f6d 2f70 796d 6172 632f 7079  ab.com/pymarc/py
-00000090: 6d61 7263 0a41 7574 686f 723a 2045 6420  marc.Author: Ed 
-000000a0: 5375 6d6d 6572 730a 4175 7468 6f72 2d65  Summers.Author-e
-000000b0: 6d61 696c 3a20 6568 7340 706f 626f 782e  mail: ehs@pobox.
-000000c0: 636f 6d0a 4c69 6365 6e73 653a 2068 7474  com.License: htt
-000000d0: 703a 2f2f 7777 772e 6f70 656e 736f 7572  p://www.opensour
-000000e0: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-000000f0: 6273 642d 6c69 6365 6e73 652e 7068 700a  bsd-license.php.
-00000100: 506c 6174 666f 726d 3a20 554e 4b4e 4f57  Platform: UNKNOW
-00000110: 4e0a 436c 6173 7369 6669 6572 3a20 496e  N.Classifier: In
-00000120: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000130: 3a3a 2045 6475 6361 7469 6f6e 0a43 6c61  :: Education.Cla
-00000140: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000150: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000160: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-00000170: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-00000180: 6469 656e 6365 203a 3a20 496e 666f 726d  dience :: Inform
-00000190: 6174 696f 6e20 5465 6368 6e6f 6c6f 6779  ation Technology
-000001a0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001c0: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
-000001d0: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
-000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000200: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000230: 3a20 332e 360a 436c 6173 7369 6669 6572  : 3.6.Classifier
-00000240: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000260: 203a 3a20 332e 370a 436c 6173 7369 6669   :: 3.7.Classifi
-00000270: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000290: 6f6e 203a 3a20 332e 380a 436c 6173 7369  on :: 3.8.Classi
-000002a0: 6669 6572 3a20 546f 7069 6320 3a3a 2054  fier: Topic :: T
-000002b0: 6578 7420 5072 6f63 6573 7369 6e67 203a  ext Processing :
-000002c0: 3a20 4765 6e65 7261 6c0a 5265 7175 6972  : General.Requir
-000002d0: 6573 2d50 7974 686f 6e3a 203e 3d33 2e36  es-Python: >=3.6
-000002e0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000002f0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000300: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-00000310: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000320: 6060 600a 5f7c 5f7c 5f7c 2020 2020 5f7c  ```._|_|_|    _|
-00000330: 2020 2020 5f7c 2020 5f7c 5f7c 5f7c 2020      _|  _|_|_|  
-00000340: 5f7c 5f7c 2020 2020 2020 5f7c 5f7c 5f7c  _|_|      _|_|_|
-00000350: 2020 5f7c 2020 5f7c 5f7c 2020 2020 5f7c    _|  _|_|    _|
-00000360: 5f7c 5f7c 0a5f 7c20 2020 205f 7c20 205f  _|_|._|    _|  _
-00000370: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
-00000380: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
-00000390: 7c20 205f 7c5f 7c20 2020 2020 205f 7c0a  |  _|_|      _|.
-000003a0: 5f7c 2020 2020 5f7c 2020 5f7c 2020 2020  _|    _|  _|    
-000003b0: 5f7c 2020 5f7c 2020 2020 5f7c 2020 2020  _|  _|    _|    
-000003c0: 5f7c 2020 5f7c 2020 2020 5f7c 2020 5f7c  _|  _|    _|  _|
-000003d0: 2020 2020 2020 2020 5f7c 0a5f 7c5f 7c5f          _|._|_|_
-000003e0: 7c20 2020 2020 205f 7c5f 7c5f 7c20 205f  |      _|_|_|  _
-000003f0: 7c20 2020 205f 7c20 2020 205f 7c20 2020  |    _|    _|   
-00000400: 205f 7c5f 7c5f 7c20 205f 7c20 2020 2020   _|_|_|  _|     
-00000410: 2020 2020 205f 7c5f 7c5f 7c0a 5f7c 2020       _|_|_|._|  
-00000420: 2020 2020 2020 2020 2020 2020 5f7c 0a5f              _|._
-00000430: 7c20 2020 2020 2020 2020 205f 7c5f 7c0a  |          _|_|.
-00000440: 6060 600a 0a5b 215b 4275 696c 6420 7374  ```..[![Build st
-00000450: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
-00000460: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
-00000470: 7079 6d61 7263 2f62 6164 6765 732f 6d61  pymarc/badges/ma
-00000480: 696e 2f70 6970 656c 696e 652e 7376 6729  in/pipeline.svg)
-00000490: 5d28 6874 7470 733a 2f2f 6769 746c 6162  ](https://gitlab
-000004a0: 2e63 6f6d 2f70 796d 6172 632f 7079 6d61  .com/pymarc/pyma
-000004b0: 7263 2f2d 2f63 6f6d 6d69 7473 2f6d 6169  rc/-/commits/mai
-000004c0: 6e29 0a0a 7079 6d61 7263 2069 7320 6120  n)..pymarc is a 
-000004d0: 7079 7468 6f6e 206c 6962 7261 7279 2066  python library f
-000004e0: 6f72 2077 6f72 6b69 6e67 2077 6974 6820  or working with 
-000004f0: 6269 626c 696f 6772 6170 6869 6320 6461  bibliographic da
-00000500: 7461 2065 6e63 6f64 6564 2069 6e0a 5b4d  ta encoded in.[M
-00000510: 4152 4332 315d 2868 7474 7073 3a2f 2f65  ARC21](https://e
-00000520: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00000530: 7769 6b69 2f4d 4152 435f 7374 616e 6461  wiki/MARC_standa
-00000540: 7264 7329 2e20 4974 2070 726f 7669 6465  rds). It provide
-00000550: 7320 616e 2041 5049 2066 6f72 0a72 6561  s an API for.rea
-00000560: 6469 6e67 2c20 7772 6974 696e 6720 616e  ding, writing an
-00000570: 6420 6d6f 6469 6679 696e 6720 4d41 5243  d modifying MARC
-00000580: 2072 6563 6f72 6473 2e20 4974 2077 6173   records. It was
-00000590: 206d 6f73 746c 7920 6465 7369 676e 6564   mostly designed
-000005a0: 2074 6f20 6265 2061 6e0a 656d 6572 6765   to be an.emerge
-000005b0: 6e63 7920 656a 6563 7420 7365 6174 2c20  ncy eject seat, 
-000005c0: 666f 7220 6765 7474 696e 6720 796f 7572  for getting your
-000005d0: 2064 6174 6120 6173 7365 7473 206f 7574   data assets out
-000005e0: 206f 6620 4d41 5243 2061 6e64 2069 6e74   of MARC and int
-000005f0: 6f20 736f 6d65 0a6b 696e 6420 6f66 2073  o some.kind of s
-00000600: 616e 6572 2072 6570 7265 7365 6e74 6174  aner representat
-00000610: 696f 6e2e 2048 6f77 6576 6572 206f 7665  ion. However ove
-00000620: 7220 7468 6520 7965 6172 7320 6974 2068  r the years it h
-00000630: 6173 2062 6565 6e20 7573 6564 2074 6f20  as been used to 
-00000640: 6372 6561 7465 0a61 6e64 206d 6f64 6966  create.and modif
-00000650: 7920 4d41 5243 2072 6563 6f72 6473 2c20  y MARC records, 
-00000660: 7369 6e63 6520 6465 7370 6974 6520 5b72  since despite [r
-00000670: 6570 6561 7465 640a 6361 6c6c 735d 2868  epeated.calls](h
-00000680: 7474 7073 3a2f 2f77 6562 2e61 7263 6869  ttps://web.archi
-00000690: 7665 2e6f 7267 2f77 6562 2f32 3031 3730  ve.org/web/20170
-000006a0: 3733 3131 3633 3031 392f 6874 7470 3a2f  731163019/http:/
-000006b0: 2f77 7777 2e6d 6172 632d 6d75 7374 2d64  /www.marc-must-d
-000006c0: 6965 2e69 6e66 6f2f 696e 6465 782e 7068  ie.info/index.ph
-000006d0: 702f 4d61 696e 5f50 6167 6529 0a66 6f72  p/Main_Page).for
-000006e0: 2069 7420 746f 2064 6965 2061 7320 6120   it to die as a 
-000006f0: 666f 726d 6174 2c20 4d41 5243 2073 6565  format, MARC see
-00000700: 6d73 2074 6f20 6265 206c 6976 696e 6720  ms to be living 
-00000710: 7175 6974 6520 6861 7070 696c 7920 6173  quite happily as
-00000720: 2061 207a 6f6d 6269 652e 0a0a 4265 6c6f   a zombie...Belo
-00000730: 7720 6172 6520 736f 6d65 2063 6f6d 6d6f  w are some commo
-00000740: 6e20 6578 616d 706c 6573 206f 6620 686f  n examples of ho
-00000750: 7720 796f 7520 6d69 6768 7420 7761 6e74  w you might want
-00000760: 2074 6f20 7573 6520 7079 6d61 7263 2e20   to use pymarc. 
-00000770: 4966 0a79 6f75 2072 756e 2061 6372 6f73  If.you run acros
-00000780: 7320 616e 2065 7861 6d70 6c65 2074 6861  s an example tha
-00000790: 7420 796f 7520 7468 696e 6b20 7368 6f75  t you think shou
-000007a0: 6c64 2062 6520 6865 7265 2070 6c65 6173  ld be here pleas
-000007b0: 6520 7365 6e64 2061 0a70 756c 6c20 7265  e send a.pull re
-000007c0: 7175 6573 742e 0a0a 596f 7520 6361 6e20  quest...You can 
-000007d0: 7265 6164 2070 796d 6172 6320 646f 6375  read pymarc docu
-000007e0: 6d65 6e74 6174 696f 6e20 5b68 6572 655d  mentation [here]
-000007f0: 2868 7474 7073 3a2f 2f70 796d 6172 632e  (https://pymarc.
-00000800: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000810: 6e2f 6c61 7465 7374 2f29 2e0a 0a23 2323  n/latest/)...###
-00000820: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a59   Installation..Y
-00000830: 6f75 276c 6c20 7072 6f62 6162 6c79 206a  ou'll probably j
-00000840: 7573 7420 7761 6e74 2074 6f20 7573 6520  ust want to use 
-00000850: 7069 7020 746f 2069 6e73 7461 6c6c 2070  pip to install p
-00000860: 796d 6172 633a 0a0a 2020 2020 7069 7020  ymarc:..    pip 
-00000870: 696e 7374 616c 6c20 7079 6d61 7263 0a0a  install pymarc..
-00000880: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
-00000890: 2064 6f77 6e6c 6f61 6420 616e 6420 696e   download and in
-000008a0: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
-000008b0: 2073 6f75 7263 6520 796f 7527 6c6c 206e   source you'll n
-000008c0: 6565 6420 6769 743a 0a0a 2020 2020 6769  eed git:..    gi
-000008d0: 7420 636c 6f6e 6520 6769 743a 2f2f 6769  t clone git://gi
-000008e0: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
-000008f0: 7079 6d61 7263 2e67 6974 0a0a 596f 7527  pymarc.git..You'
-00000900: 6c6c 2061 6c73 6f20 6e65 6564 205b 7365  ll also need [se
-00000910: 7475 7074 6f6f 6c73 5d28 6874 7470 733a  tuptools](https:
-00000920: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000930: 672f 7079 7069 2f73 6574 7570 746f 6f6c  g/pypi/setuptool
-00000940: 7323 696e 7374 616c 6c61 7469 6f6e 2d69  s#installation-i
-00000950: 6e73 7472 7563 7469 6f6e 7329 2e20 4f6e  nstructions). On
-00000960: 6365 2079 6f75 2068 6176 6520 7468 6520  ce you have the 
-00000970: 736f 7572 6365 2061 6e64 2073 6574 7570  source and setup
-00000980: 746f 6f6c 7320 7275 6e20 7468 6520 7079  tools run the py
-00000990: 6d61 7263 2074 6573 740a 7375 6974 6520  marc test.suite 
-000009a0: 746f 206d 616b 6520 7375 7265 2074 6869  to make sure thi
-000009b0: 6e67 7320 6172 6520 696e 206f 7264 6572  ngs are in order
-000009c0: 2077 6974 6820 7468 6520 6469 7374 7269   with the distri
-000009d0: 6275 7469 6f6e 3a0a 0a20 2020 2070 7974  bution:..    pyt
-000009e0: 686f 6e20 7365 7475 702e 7079 2074 6573  hon setup.py tes
-000009f0: 740a 0a41 6e64 2074 6865 6e20 696e 7374  t..And then inst
-00000a00: 616c 6c3a 0a0a 2020 2020 7079 7468 6f6e  all:..    python
-00000a10: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
-00000a20: 6c0a 0a23 2323 2052 6561 6469 6e67 0a0a  l..### Reading..
-00000a30: 4d6f 7374 206f 6674 656e 2079 6f75 2077  Most often you w
-00000a40: 696c 6c20 6861 7665 2073 6f6d 6520 4d41  ill have some MA
-00000a50: 5243 2064 6174 6120 616e 6420 7769 6c6c  RC data and will
-00000a60: 2077 616e 7420 746f 2065 7874 7261 6374   want to extract
-00000a70: 2064 6174 610a 6672 6f6d 2069 742e 2048   data.from it. H
-00000a80: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
-00000a90: 206f 6620 7265 6164 696e 6720 6120 6261   of reading a ba
-00000aa0: 7463 6820 6f66 2072 6563 6f72 6473 2061  tch of records a
-00000ab0: 6e64 2070 7269 6e74 696e 6720 6f75 740a  nd printing out.
-00000ac0: 7468 6520 7469 746c 652e 2049 6620 796f  the title. If yo
-00000ad0: 7520 6172 6520 6375 7269 6f75 7320 7468  u are curious th
-00000ae0: 6973 2065 7861 6d70 6c65 2075 7365 7320  is example uses 
-00000af0: 7468 6520 6261 7463 6820 6669 6c65 0a61  the batch file.a
-00000b00: 7661 696c 6162 6c65 2068 6572 6520 696e  vailable here in
-00000b10: 2070 796d 6172 6320 7265 706f 7369 746f   pymarc reposito
-00000b20: 7279 3a0a 0a60 6060 7079 7468 6f6e 0a66  ry:..```python.f
-00000b30: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
-00000b40: 7420 4d41 5243 5265 6164 6572 0a77 6974  t MARCReader.wit
-00000b50: 6820 6f70 656e 2827 7465 7374 2f6d 6172  h open('test/mar
-00000b60: 632e 6461 7427 2c20 2772 6227 2920 6173  c.dat', 'rb') as
-00000b70: 2066 683a 0a20 2020 2072 6561 6465 7220   fh:.    reader 
-00000b80: 3d20 4d41 5243 5265 6164 6572 2866 6829  = MARCReader(fh)
-00000b90: 0a20 2020 2066 6f72 2072 6563 6f72 6420  .    for record 
-00000ba0: 696e 2072 6561 6465 723a 0a20 2020 2020  in reader:.     
-00000bb0: 2020 2070 7269 6e74 2872 6563 6f72 642e     print(record.
-00000bc0: 7469 746c 6528 2929 0a60 6060 0a60 6060  title()).```.```
-00000bd0: 0a54 6865 2070 7261 676d 6174 6963 2070  .The pragmatic p
-00000be0: 726f 6772 616d 6d65 7220 3a20 6672 6f6d  rogrammer : from
-00000bf0: 206a 6f75 726e 6579 6d61 6e20 746f 206d   journeyman to m
-00000c00: 6173 7465 7220 2f0a 5072 6f67 7261 6d6d  aster /.Programm
-00000c10: 696e 6720 5079 7468 6f6e 202f 0a4c 6561  ing Python /.Lea
-00000c20: 726e 696e 6720 5079 7468 6f6e 202f 0a50  rning Python /.P
-00000c30: 7974 686f 6e20 636f 6f6b 626f 6f6b 202f  ython cookbook /
-00000c40: 0a50 7974 686f 6e20 7072 6f67 7261 6d6d  .Python programm
-00000c50: 696e 6720 666f 7220 7468 6520 6162 736f  ing for the abso
-00000c60: 6c75 7465 2062 6567 696e 6e65 7220 2f0a  lute beginner /.
-00000c70: 5765 6220 7072 6f67 7261 6d6d 696e 6720  Web programming 
-00000c80: 3a20 7465 6368 6e69 7175 6573 2066 6f72  : techniques for
-00000c90: 2069 6e74 6567 7261 7469 6e67 2050 7974   integrating Pyt
-00000ca0: 686f 6e2c 204c 696e 7578 2c20 4170 6163  hon, Linux, Apac
-00000cb0: 6865 2c20 616e 6420 4d79 5351 4c20 2f0a  he, and MySQL /.
-00000cc0: 5079 7468 6f6e 2070 726f 6772 616d 6d69  Python programmi
-00000cd0: 6e67 206f 6e20 5769 6e33 3220 2f0a 5079  ng on Win32 /.Py
-00000ce0: 7468 6f6e 2070 726f 6772 616d 6d69 6e67  thon programming
-00000cf0: 203a 2061 6e20 696e 7472 6f64 7563 7469   : an introducti
-00000d00: 6f6e 2074 6f20 636f 6d70 7574 6572 2073  on to computer s
-00000d10: 6369 656e 6365 202f 0a50 7974 686f 6e20  cience /.Python 
-00000d20: 5765 6220 7072 6f67 7261 6d6d 696e 6720  Web programming 
-00000d30: 2f0a 436f 7265 2070 7974 686f 6e20 7072  /.Core python pr
-00000d40: 6f67 7261 6d6d 696e 6720 2f0a 5079 7468  ogramming /.Pyth
-00000d50: 6f6e 2061 6e64 2054 6b69 6e74 6572 2070  on and Tkinter p
-00000d60: 726f 6772 616d 6d69 6e67 202f 0a47 616d  rogramming /.Gam
-00000d70: 6520 7072 6f67 7261 6d6d 696e 6720 7769  e programming wi
-00000d80: 7468 2050 7974 686f 6e2c 204c 7561 2c20  th Python, Lua, 
-00000d90: 616e 6420 5275 6279 202f 0a50 7974 686f  and Ruby /.Pytho
-00000da0: 6e20 7072 6f67 7261 6d6d 696e 6720 7061  n programming pa
-00000db0: 7474 6572 6e73 202f 0a50 7974 686f 6e20  tterns /.Python 
-00000dc0: 7072 6f67 7261 6d6d 696e 6720 7769 7468  programming with
-00000dd0: 2074 6865 204a 6176 6120 636c 6173 7320   the Java class 
-00000de0: 6c69 6272 6172 6965 7320 3a20 6120 7475  libraries : a tu
-00000df0: 746f 7269 616c 2066 6f72 2062 7569 6c64  torial for build
-00000e00: 696e 6720 5765 620a 616e 6420 456e 7465  ing Web.and Ente
-00000e10: 7270 7269 7365 2061 7070 6c69 6361 7469  rprise applicati
-00000e20: 6f6e 7320 2f0a 4c65 6172 6e20 746f 2070  ons /.Learn to p
-00000e30: 726f 6772 616d 2075 7369 6e67 2050 7974  rogram using Pyt
-00000e40: 686f 6e20 3a20 6120 7475 746f 7269 616c  hon : a tutorial
-00000e50: 2066 6f72 2068 6f62 6279 6973 7473 2c20   for hobbyists, 
-00000e60: 7365 6c66 2d73 7461 7274 6572 732c 2061  self-starters, a
-00000e70: 6e64 2061 6c6c 0a77 686f 2077 616e 7420  nd all.who want 
-00000e80: 746f 206c 6561 726e 2074 6865 2061 7274  to learn the art
-00000e90: 206f 6620 636f 6d70 7574 6572 2070 726f   of computer pro
-00000ea0: 6772 616d 6d69 6e67 202f 0a50 726f 6772  gramming /.Progr
-00000eb0: 616d 6d69 6e67 2077 6974 6820 5079 7468  amming with Pyth
-00000ec0: 6f6e 202f 0a42 5344 2053 6f63 6b65 7473  on /.BSD Sockets
-00000ed0: 2070 726f 6772 616d 6d69 6e67 2066 726f   programming fro
-00000ee0: 6d20 6120 6d75 6c74 692d 6c61 6e67 7561  m a multi-langua
-00000ef0: 6765 2070 6572 7370 6563 7469 7665 202f  ge perspective /
-00000f00: 0a44 6573 6967 6e20 7061 7474 6572 6e73  .Design patterns
-00000f10: 203a 2065 6c65 6d65 6e74 7320 6f66 2072   : elements of r
-00000f20: 6575 7361 626c 6520 6f62 6a65 6374 2d6f  eusable object-o
-00000f30: 7269 656e 7465 6420 736f 6674 7761 7265  riented software
-00000f40: 202f 0a49 6e74 726f 6475 6374 696f 6e20   /.Introduction 
-00000f50: 746f 2061 6c67 6f72 6974 686d 7320 2f0a  to algorithms /.
-00000f60: 414e 5349 2043 6f6d 6d6f 6e20 4c69 7370  ANSI Common Lisp
-00000f70: 202f 0a60 6060 0a0a 4120 6070 796d 6172   /.```..A `pymar
-00000f80: 632e 5265 636f 7264 6020 6f62 6a65 6374  c.Record` object
-00000f90: 2068 6173 2061 2066 6577 2068 616e 6479   has a few handy
-00000fa0: 206d 6574 686f 6473 206c 696b 6520 6074   methods like `t
-00000fb0: 6974 6c65 6020 666f 7220 6765 7474 696e  itle` for gettin
-00000fc0: 6720 6174 0a62 6974 7320 6f66 2061 2062  g at.bits of a b
-00000fd0: 6962 6c69 6f67 7261 7068 6963 2072 6563  ibliographic rec
-00000fe0: 6f72 642c 206f 7468 6572 7320 696e 636c  ord, others incl
-00000ff0: 7564 653a 2060 6175 7468 6f72 602c 2060  ude: `author`, `
-00001000: 6973 626e 602c 2060 7375 626a 6563 7473  isbn`, `subjects
-00001010: 602c 0a60 6c6f 6361 7469 6f6e 602c 2060  `,.`location`, `
-00001020: 6e6f 7465 7360 2c20 6070 6879 7369 6361  notes`, `physica
-00001030: 6c64 6573 6372 6970 7469 6f6e 602c 2060  ldescription`, `
-00001040: 7075 626c 6973 6865 7260 2c20 6070 7562  publisher`, `pub
-00001050: 7965 6172 602c 2060 6973 736e 602c 0a60  year`, `issn`,.`
-00001060: 6973 736e 5f74 6974 6c65 602e 2042 7574  issn_title`. But
-00001070: 2072 6561 6c6c 792c 2074 6f20 776f 726b   really, to work
-00001080: 2077 6974 6820 4d41 5243 2064 6174 6120   with MARC data 
-00001090: 796f 7520 6e65 6564 2074 6f20 756e 6465  you need to unde
-000010a0: 7273 7461 6e64 2074 6865 0a6e 756d 6572  rstand the.numer
-000010b0: 6963 2066 6965 6c64 2074 6167 7320 616e  ic field tags an
-000010c0: 6420 7375 6266 6965 6c64 2063 6f64 6573  d subfield codes
-000010d0: 2074 6861 7420 6172 6520 7573 6564 2074   that are used t
-000010e0: 6f20 6465 7369 676e 6174 6520 7661 7269  o designate vari
-000010f0: 6f75 7320 6269 7473 0a6f 6620 696e 666f  ous bits.of info
-00001100: 726d 6174 696f 6e2e 2054 6865 7265 2069  rmation. There i
-00001110: 7320 6120 6c6f 7420 6d6f 7265 2068 6964  s a lot more hid
-00001120: 696e 6720 696e 2061 204d 4152 4320 7265  ing in a MARC re
-00001130: 636f 7264 2074 6861 6e20 7468 6573 6520  cord than these 
-00001140: 6d65 7468 6f64 730a 7072 6f76 6964 6520  methods.provide 
-00001150: 6163 6365 7373 2074 6f2e 2046 6f72 2065  access to. For e
-00001160: 7861 6d70 6c65 2074 6865 2060 7469 746c  xample the `titl
-00001170: 6560 206d 6574 686f 6420 6578 7472 6163  e` method extrac
-00001180: 7473 2074 6865 2069 6e66 6f72 6d61 7469  ts the informati
-00001190: 6f6e 2066 726f 6d0a 2074 6865 2060 3234  on from. the `24
-000011a0: 3560 2066 6965 6c64 2c20 7375 6266 6965  5` field, subfie
-000011b0: 6c64 7320 6061 6020 616e 6420 6062 602e  lds `a` and `b`.
-000011c0: 2059 6f75 2063 616e 2061 6363 6573 7320   You can access 
-000011d0: 6032 3435 6160 206c 696b 6520 736f 3a0a  `245a` like so:.
-000011e0: 0a60 6060 7079 7468 6f6e 0a70 7269 6e74  .```python.print
-000011f0: 2872 6563 6f72 645b 2732 3435 275d 5b27  (record['245']['
-00001200: 6127 5d29 0a60 6060 0a0a 536f 6d65 2066  a']).```..Some f
-00001210: 6965 6c64 7320 6c69 6b65 2073 7562 6a65  ields like subje
-00001220: 6374 7320 6361 6e20 7265 7065 6174 2e20  cts can repeat. 
-00001230: 496e 2063 6173 6573 206c 696b 6520 7468  In cases like th
-00001240: 6174 2079 6f75 2077 696c 6c20 7761 6e74  at you will want
-00001250: 2074 6f20 7573 650a 6067 6574 5f66 6965   to use.`get_fie
-00001260: 6c64 7360 2074 6f20 6765 7420 616c 6c20  lds` to get all 
-00001270: 6f66 2074 6865 6d20 6173 2060 7079 6d61  of them as `pyma
-00001280: 7263 2e46 6965 6c64 6020 6f62 6a65 6374  rc.Field` object
-00001290: 732c 2077 6869 6368 2079 6f75 2063 616e  s, which you can
-000012a0: 2074 6865 6e0a 696e 7465 7261 6374 2077   then.interact w
-000012b0: 6974 6820 6675 7274 6865 723a 0a0a 6060  ith further:..``
-000012c0: 6070 7974 686f 6e0a 666f 7220 6620 696e  `python.for f in
-000012d0: 2072 6563 6f72 642e 6765 745f 6669 656c   record.get_fiel
-000012e0: 6473 2827 3635 3027 293a 0a20 2020 2070  ds('650'):.    p
-000012f0: 7269 6e74 2866 290a 6060 600a 0a49 6620  rint(f).```..If 
-00001300: 796f 7520 6172 6520 6e65 7720 746f 204d  you are new to M
-00001310: 4152 4320 6669 656c 6473 205b 556e 6465  ARC fields [Unde
-00001320: 7273 7461 6e64 696e 670a 4d41 5243 5d28  rstanding.MARC](
-00001330: 6874 7470 3a2f 2f77 7777 2e6c 6f63 2e67  http://www.loc.g
-00001340: 6f76 2f6d 6172 632f 756d 622f 2920 6973  ov/marc/umb/) is
-00001350: 2061 2070 7265 7474 7920 676f 6f64 2070   a pretty good p
-00001360: 7269 6d65 722c 2061 6e64 2074 6865 205b  rimer, and the [
-00001370: 4d41 5243 2032 310a 466f 726d 6174 735d  MARC 21.Formats]
-00001380: 2868 7474 703a 2f2f 7777 772e 6c6f 632e  (http://www.loc.
-00001390: 676f 762f 6d61 7263 2f6d 6172 6364 6f63  gov/marc/marcdoc
-000013a0: 7a2e 6874 6d6c 2920 7061 6765 2061 7420  z.html) page at 
-000013b0: 7468 6520 4c69 6272 6172 7920 6f66 2043  the Library of C
-000013c0: 6f6e 6772 6573 7320 6973 2061 2067 6f6f  ongress is a goo
-000013d0: 6420 7265 6665 7265 6e63 6520 6f6e 6365  d reference once
-000013e0: 2079 6f75 2075 6e64 6572 7374 616e 6420   you understand 
-000013f0: 7468 6520 6261 7369 6373 2e0a 0a23 2323  the basics...###
-00001400: 2057 7269 7469 6e67 0a0a 4865 7265 2773   Writing..Here's
-00001410: 2061 6e20 6578 616d 706c 6520 6f66 2063   an example of c
-00001420: 7265 6174 696e 6720 6120 7265 636f 7264  reating a record
-00001430: 2061 6e64 2077 7269 7469 6e67 2069 7420   and writing it 
-00001440: 6f75 7420 746f 2061 2066 696c 652e 0a0a  out to a file...
-00001450: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
-00001460: 796d 6172 6320 696d 706f 7274 2052 6563  ymarc import Rec
-00001470: 6f72 642c 2046 6965 6c64 0a72 6563 6f72  ord, Field.recor
-00001480: 6420 3d20 5265 636f 7264 2829 0a72 6563  d = Record().rec
-00001490: 6f72 642e 6164 645f 6669 656c 6428 0a20  ord.add_field(. 
-000014a0: 2020 2046 6965 6c64 280a 2020 2020 2020     Field(.      
-000014b0: 2020 7461 6720 3d20 2732 3435 272c 0a20    tag = '245',. 
-000014c0: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
-000014d0: 7320 3d20 5b27 3027 2c27 3127 5d2c 0a20  s = ['0','1'],. 
-000014e0: 2020 2020 2020 2073 7562 6669 656c 6473         subfields
-000014f0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00001500: 2027 6127 2c20 2754 6865 2070 7261 676d   'a', 'The pragm
-00001510: 6174 6963 2070 726f 6772 616d 6d65 7220  atic programmer 
-00001520: 3a20 272c 0a20 2020 2020 2020 2020 2020  : ',.           
-00001530: 2027 6227 2c20 2766 726f 6d20 6a6f 7572   'b', 'from jour
-00001540: 6e65 796d 616e 2074 6f20 6d61 7374 6572  neyman to master
-00001550: 202f 272c 0a20 2020 2020 2020 2020 2020   /',.           
-00001560: 2027 6327 2c20 2741 6e64 7265 7720 4875   'c', 'Andrew Hu
-00001570: 6e74 2c20 4461 7669 6420 5468 6f6d 6173  nt, David Thomas
-00001580: 2e27 0a20 2020 2020 2020 205d 2929 0a77  .'.        ])).w
-00001590: 6974 6820 6f70 656e 2827 6669 6c65 2e64  ith open('file.d
-000015a0: 6174 272c 2027 7762 2729 2061 7320 6f75  at', 'wb') as ou
-000015b0: 743a 0a20 2020 206f 7574 2e77 7269 7465  t:.    out.write
-000015c0: 2872 6563 6f72 642e 6173 5f6d 6172 6328  (record.as_marc(
-000015d0: 2929 0a60 6060 0a0a 2323 2320 5570 6461  )).```..### Upda
-000015e0: 7469 6e67 0a0a 5570 6461 7469 6e67 2077  ting..Updating w
-000015f0: 6f72 6b73 2074 6865 2073 616d 6520 7761  orks the same wa
-00001600: 792c 2079 6f75 2072 6561 6420 6974 2069  y, you read it i
-00001610: 6e2c 206d 6f64 6966 7920 6974 2c20 616e  n, modify it, an
-00001620: 6420 7468 656e 2077 7269 7465 2069 7420  d then write it 
-00001630: 6f75 740a 6167 6169 6e3a 0a0a 6060 6070  out.again:..```p
-00001640: 7974 686f 6e0a 6672 6f6d 2070 796d 6172  ython.from pymar
-00001650: 6320 696d 706f 7274 204d 4152 4352 6561  c import MARCRea
-00001660: 6465 720a 7769 7468 206f 7065 6e28 2774  der.with open('t
-00001670: 6573 742f 6d61 7263 2e64 6174 272c 2027  est/marc.dat', '
-00001680: 7262 2729 2061 7320 6668 3a0a 2020 2020  rb') as fh:.    
-00001690: 7265 6164 6572 203d 204d 4152 4352 6561  reader = MARCRea
-000016a0: 6465 7228 6668 290a 2020 2020 7265 636f  der(fh).    reco
-000016b0: 7264 203d 206e 6578 7428 7265 6164 6572  rd = next(reader
-000016c0: 290a 2020 2020 7265 636f 7264 5b27 3234  ).    record['24
-000016d0: 3527 5d5b 2761 275d 203d 2027 5468 6520  5']['a'] = 'The 
-000016e0: 5a6f 6d62 6965 2050 726f 6772 616d 6d65  Zombie Programme
-000016f0: 7227 0a77 6974 6820 6f70 656e 2827 6669  r'.with open('fi
-00001700: 6c65 2e64 6174 272c 2027 7762 2729 2061  le.dat', 'wb') a
-00001710: 7320 6f75 743a 0a20 2020 206f 7574 2e77  s out:.    out.w
-00001720: 7269 7465 2872 6563 6f72 642e 6173 5f6d  rite(record.as_m
-00001730: 6172 6328 2929 0a60 6060 0a0a 0a23 2323  arc()).```...###
-00001740: 204a 534f 4e20 616e 6420 584d 4c0a 0a49   JSON and XML..I
-00001750: 6620 796f 7520 6669 6e64 2079 6f75 7273  f you find yours
-00001760: 656c 6620 7573 696e 6720 4d41 5243 2064  elf using MARC d
-00001770: 6174 6120 6120 6661 6972 2062 6974 2c20  ata a fair bit, 
-00001780: 616e 6420 6469 7374 7269 6275 7469 6e67  and distributing
-00001790: 2069 742c 2079 6f75 206d 6179 0a6d 616b   it, you may.mak
-000017a0: 6520 6f74 6865 7220 6465 7665 6c6f 7065  e other develope
-000017b0: 7273 2061 2062 6974 2068 6170 7069 6572  rs a bit happier
-000017c0: 2062 7920 7573 696e 6720 7468 6520 4a53   by using the JS
-000017d0: 4f4e 206f 7220 584d 4c20 7365 7269 616c  ON or XML serial
-000017e0: 697a 6174 696f 6e73 2e20 5468 650a 6d61  izations. The.ma
-000017f0: 696e 2062 656e 6566 6974 2074 6f20 7573  in benefit to us
-00001800: 696e 6720 584d 4c20 6f72 204a 534f 4e20  ing XML or JSON 
-00001810: 6973 2074 6861 7420 7468 6520 5554 4638  is that the UTF8
-00001820: 2063 6861 7261 6374 6572 2065 6e63 6f64   character encod
-00001830: 696e 6720 6973 2075 7365 642c 0a72 6174  ing is used,.rat
-00001840: 6865 7220 7468 616e 2074 6865 2066 7275  her than the fru
-00001850: 7374 7261 7469 6e67 6c79 2061 7263 6861  stratingly archa
-00001860: 6963 204d 4152 4338 2065 6e63 6f64 696e  ic MARC8 encodin
-00001870: 672e 2041 6c73 6f20 7468 6579 2077 696c  g. Also they wil
-00001880: 6c20 6265 2061 626c 6520 746f 0a75 7365  l be able to.use
-00001890: 2073 7461 6e64 6172 6420 4a53 4f4e 2061   standard JSON a
-000018a0: 6e64 2058 4d4c 2072 6561 6469 6e67 2f77  nd XML reading/w
-000018b0: 7269 7469 6e67 2074 6f6f 6c73 2074 6f20  riting tools to 
-000018c0: 6765 7420 6174 2074 6865 2064 6174 6120  get at the data 
-000018d0: 7468 6579 2077 616e 740a 696e 7374 6561  they want.instea
-000018e0: 6420 6f66 2073 6f6d 6520 6372 617a 7920  d of some crazy 
-000018f0: 4d41 5243 2070 726f 6365 7373 696e 6720  MARC processing 
-00001900: 6c69 6272 6172 7920 6c69 6b65 2c20 6168  library like, ah
-00001910: 656d 2c20 7079 6d61 7263 2e0a 0a2a 2a58  em, pymarc...**X
-00001920: 4d4c 2a2a 0a0a 546f 2070 6172 7365 2061  ML**..To parse a
-00001930: 2066 696c 6520 6f66 204d 4152 4358 4d4c   file of MARCXML
-00001940: 2072 6563 6f72 6473 2079 6f75 2063 616e   records you can
-00001950: 3a0a 0a60 6060 7079 7468 6f6e 0a0a 6672  :..```python..fr
-00001960: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
-00001970: 2070 6172 7365 5f78 6d6c 5f74 6f5f 6172   parse_xml_to_ar
-00001980: 7261 790a 0a72 6563 6f72 6473 203d 2070  ray..records = p
-00001990: 6172 7365 5f78 6d6c 5f74 6f5f 6172 7261  arse_xml_to_arra
-000019a0: 7928 2774 6573 742f 6261 7463 682e 786d  y('test/batch.xm
-000019b0: 6c27 290a 6060 600a 0a49 6620 796f 7520  l').```..If you 
-000019c0: 6861 7665 2061 206c 6172 6765 2058 4d4c  have a large XML
-000019d0: 2066 696c 6520 616e 6420 776f 756c 6420   file and would 
-000019e0: 7261 7468 6572 206e 6f74 2072 6561 6420  rather not read 
-000019f0: 7468 656d 2061 6c6c 2069 6e74 6f20 6d65  them all into me
-00001a00: 6d6f 7279 2079 6f75 0a63 616e 3a0a 0a60  mory you.can:..`
-00001a10: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2070  ``python..from p
-00001a20: 796d 6172 6320 696d 706f 7274 206d 6170  ymarc import map
-00001a30: 5f78 6d6c 0a0a 6465 6620 7072 696e 745f  _xml..def print_
-00001a40: 7469 746c 6528 7229 3a0a 2020 2020 7072  title(r):.    pr
-00001a50: 696e 7428 722e 7469 746c 6528 2929 0a0a  int(r.title())..
-00001a60: 6d61 705f 786d 6c28 7072 696e 745f 7469  map_xml(print_ti
-00001a70: 746c 652c 2027 7465 7374 2f62 6174 6368  tle, 'test/batch
-00001a80: 2e78 6d6c 2729 0a60 6060 0a0a 416c 736f  .xml').```..Also
-00001a90: 2c20 6966 2079 6f75 2070 7265 6665 7220  , if you prefer 
-00001aa0: 796f 7520 6361 6e20 7061 7373 2069 6e20  you can pass in 
-00001ab0: 6120 6669 6c65 206c 696b 6520 6f62 6a65  a file like obje
-00001ac0: 6374 2069 6e20 6164 6469 7469 6f6e 2074  ct in addition t
-00001ad0: 6f20 7468 6520 7061 7468 0a74 6f20 626f  o the path.to bo
-00001ae0: 7468 202a 6d61 705f 786d 6c2a 2061 6e64  th *map_xml* and
-00001af0: 202a 7061 7273 655f 786d 6c5f 746f 5f61   *parse_xml_to_a
-00001b00: 7272 6179 2a3a 0a0a 6060 6070 7974 686f  rray*:..```pytho
-00001b10: 6e0a 7265 636f 7264 7320 3d20 7061 7273  n.records = pars
-00001b20: 655f 786d 6c5f 746f 5f61 7272 6179 286f  e_xml_to_array(o
-00001b30: 7065 6e28 2774 6573 742f 6261 7463 682e  pen('test/batch.
-00001b40: 786d 6c27 2929 0a60 6060 0a0a 2a2a 4a53  xml')).```..**JS
-00001b50: 4f4e 2a2a 0a0a 4a53 4f4e 2073 7570 706f  ON**..JSON suppo
-00001b60: 7274 2069 7320 6661 6972 6c79 206d 696e  rt is fairly min
-00001b70: 696d 616c 2069 6e20 7468 6174 2079 6f75  imal in that you
-00001b80: 2063 616e 2063 616c 6c20 6120 6070 796d   can call a `pym
-00001b90: 6172 632e 5265 636f 7264 6027 730a 6061  arc.Record`'s.`a
-00001ba0: 735f 6a73 6f6e 2829 6020 6d65 7468 6f64  s_json()` method
-00001bb0: 2074 6f20 7265 7475 726e 204a 534f 4e20   to return JSON 
-00001bc0: 666f 7220 6120 6769 7665 6e20 4d41 5243  for a given MARC
-00001bd0: 2052 6563 6f72 643a 0a0a 6060 6070 7974   Record:..```pyt
-00001be0: 686f 6e0a 6672 6f6d 2070 796d 6172 6320  hon.from pymarc 
-00001bf0: 696d 706f 7274 204d 4152 4352 6561 6465  import MARCReade
-00001c00: 720a 0a77 6974 6820 6f70 656e 2827 7465  r..with open('te
-00001c10: 7374 2f6f 6e65 2e64 6174 272c 2772 6227  st/one.dat','rb'
-00001c20: 2920 6173 2066 683a 0a20 2020 2072 6561  ) as fh:.    rea
-00001c30: 6465 7220 3d20 4d41 5243 5265 6164 6572  der = MARCReader
-00001c40: 2866 6829 0a20 2020 2066 6f72 2072 6563  (fh).    for rec
-00001c50: 6f72 6420 696e 2072 6561 6465 723a 0a20  ord in reader:. 
-00001c60: 2020 2020 2020 2070 7269 6e74 2872 6563         print(rec
-00001c70: 6f72 642e 6173 5f6a 736f 6e28 696e 6465  ord.as_json(inde
-00001c80: 6e74 3d32 2929 0a60 6060 0a0a 6060 606a  nt=2)).```..```j
-00001c90: 6176 6173 6372 6970 740a 7b0a 2020 226c  avascript.{.  "l
-00001ca0: 6561 6465 7222 3a20 2230 3130 3630 6361  eader": "01060ca
-00001cb0: 6d20 2032 3230 3032 3839 3461 2034 3530  m  22002894a 450
-00001cc0: 3022 2c0a 2020 2266 6965 6c64 7322 3a20  0",.  "fields": 
-00001cd0: 5b0a 2020 2020 7b0a 2020 2020 2020 2230  [.    {.      "0
-00001ce0: 3031 223a 2022 3131 3737 3835 3034 220a  01": "11778504".
-00001cf0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00001d00: 2020 2022 3031 3022 3a20 7b0a 2020 2020     "010": {.    
-00001d10: 2020 2020 2269 6e64 3122 3a20 2220 222c      "ind1": " ",
-00001d20: 0a20 2020 2020 2020 2022 7375 6266 6965  .        "subfie
-00001d30: 6c64 7322 3a20 5b0a 2020 2020 2020 2020  lds": [.        
-00001d40: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001d50: 2261 223a 2022 2020 2039 3930 3433 3538  "a": "   9904358
-00001d60: 3120 220a 2020 2020 2020 2020 2020 7d0a  1 ".          }.
-00001d70: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00001d80: 2020 2022 696e 6432 223a 2022 2022 0a20     "ind2": " ". 
-00001d90: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-00001da0: 2020 7b0a 2020 2020 2020 2231 3030 223a    {.      "100":
-00001db0: 207b 0a20 2020 2020 2020 2022 696e 6431   {.        "ind1
-00001dc0: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
-00001dd0: 2273 7562 6669 656c 6473 223a 205b 0a20  "subfields": [. 
-00001de0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00001df0: 2020 2020 2020 2022 6122 3a20 2248 756e         "a": "Hun
-00001e00: 742c 2041 6e64 7265 772c 220a 2020 2020  t, Andrew,".    
-00001e10: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001e20: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001e30: 2022 6422 3a20 2231 3936 342d 220a 2020   "d": "1964-".  
-00001e40: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001e50: 2020 5d2c 0a20 2020 2020 2020 2022 696e    ],.        "in
-00001e60: 6432 223a 2022 2022 0a20 2020 2020 207d  d2": " ".      }
-00001e70: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-00001e80: 2020 2020 2232 3435 223a 207b 0a20 2020      "245": {.   
-00001e90: 2020 2020 2022 696e 6431 223a 2022 3122       "ind1": "1"
-00001ea0: 2c0a 2020 2020 2020 2020 2273 7562 6669  ,.        "subfi
-00001eb0: 656c 6473 223a 205b 0a20 2020 2020 2020  elds": [.       
-00001ec0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001ed0: 2022 6122 3a20 2254 6865 2070 7261 676d   "a": "The pragm
-00001ee0: 6174 6963 2070 726f 6772 616d 6d65 7220  atic programmer 
-00001ef0: 3a22 0a20 2020 2020 2020 2020 207d 2c0a  :".          },.
-00001f00: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00001f10: 2020 2020 2020 2020 2262 223a 2022 6672          "b": "fr
-00001f20: 6f6d 206a 6f75 726e 6579 6d61 6e20 746f  om journeyman to
-00001f30: 206d 6173 7465 7220 2f22 0a20 2020 2020   master /".     
-00001f40: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001f50: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001f60: 2263 223a 2022 416e 6472 6577 2048 756e  "c": "Andrew Hun
-00001f70: 742c 2044 6176 6964 2054 686f 6d61 732e  t, David Thomas.
-00001f80: 220a 2020 2020 2020 2020 2020 7d0a 2020  ".          }.  
-00001f90: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00001fa0: 2022 696e 6432 223a 2022 3422 0a20 2020   "ind2": "4".   
-00001fb0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
-00001fc0: 7b0a 2020 2020 2020 2232 3630 223a 207b  {.      "260": {
-00001fd0: 0a20 2020 2020 2020 2022 696e 6431 223a  .        "ind1":
-00001fe0: 2022 2022 2c0a 2020 2020 2020 2020 2273   " ",.        "s
-00001ff0: 7562 6669 656c 6473 223a 205b 0a20 2020  ubfields": [.   
-00002000: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00002010: 2020 2020 2022 6122 3a20 2252 6561 6469       "a": "Readi
-00002020: 6e67 2c20 4d61 7373 203a 220a 2020 2020  ng, Mass :".    
-00002030: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002040: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00002050: 2022 6222 3a20 2241 6464 6973 6f6e 2d57   "b": "Addison-W
-00002060: 6573 6c65 792c 220a 2020 2020 2020 2020  esley,".        
-00002070: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
-00002080: 0a20 2020 2020 2020 2020 2020 2022 6322  .            "c"
-00002090: 3a20 2232 3030 302e 220a 2020 2020 2020  : "2000.".      
-000020a0: 2020 2020 7d0a 2020 2020 2020 2020 5d2c      }.        ],
-000020b0: 0a20 2020 2020 2020 2022 696e 6432 223a  .        "ind2":
-000020c0: 2022 2022 0a20 2020 2020 207d 0a20 2020   " ".      }.   
-000020d0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-000020e0: 2233 3030 223a 207b 0a20 2020 2020 2020  "300": {.       
-000020f0: 2022 696e 6431 223a 2022 2022 2c0a 2020   "ind1": " ",.  
-00002100: 2020 2020 2020 2273 7562 6669 656c 6473        "subfields
-00002110: 223a 205b 0a20 2020 2020 2020 2020 207b  ": [.          {
-00002120: 0a20 2020 2020 2020 2020 2020 2022 6122  .            "a"
-00002130: 3a20 2278 7869 762c 2033 3231 2070 2e20  : "xxiv, 321 p. 
-00002140: 3b22 0a20 2020 2020 2020 2020 207d 2c0a  ;".          },.
-00002150: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00002160: 2020 2020 2020 2020 2263 223a 2022 3234          "c": "24
-00002170: 2063 6d2e 220a 2020 2020 2020 2020 2020   cm.".          
-00002180: 7d0a 2020 2020 2020 2020 5d2c 0a20 2020  }.        ],.   
-00002190: 2020 2020 2022 696e 6432 223a 2022 2022       "ind2": " "
-000021a0: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
-000021b0: 2020 2020 7b0a 2020 2020 2020 2235 3034      {.      "504
-000021c0: 223a 207b 0a20 2020 2020 2020 2022 696e  ": {.        "in
-000021d0: 6431 223a 2022 2022 2c0a 2020 2020 2020  d1": " ",.      
-000021e0: 2020 2273 7562 6669 656c 6473 223a 205b    "subfields": [
-000021f0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
-00002200: 2020 2020 2020 2020 2022 6122 3a20 2249           "a": "I
-00002210: 6e63 6c75 6465 7320 6269 626c 696f 6772  ncludes bibliogr
-00002220: 6170 6869 6361 6c20 7265 6665 7265 6e63  aphical referenc
-00002230: 6573 2e22 0a20 2020 2020 2020 2020 207d  es.".          }
-00002240: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00002250: 2020 2020 2269 6e64 3222 3a20 2220 220a      "ind2": " ".
-00002260: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
-00002270: 2020 207b 0a20 2020 2020 2022 3635 3022     {.      "650"
-00002280: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
-00002290: 3122 3a20 2220 222c 0a20 2020 2020 2020  1": " ",.       
-000022a0: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
-000022b0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-000022c0: 2020 2020 2020 2020 2261 223a 2022 436f          "a": "Co
-000022d0: 6d70 7574 6572 2070 726f 6772 616d 6d69  mputer programmi
-000022e0: 6e67 2e22 0a20 2020 2020 2020 2020 207d  ng.".          }
-000022f0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00002300: 2020 2020 2269 6e64 3222 3a20 2230 220a      "ind2": "0".
-00002310: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
-00002320: 2020 207b 0a20 2020 2020 2022 3730 3022     {.      "700"
-00002330: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
-00002340: 3122 3a20 2231 222c 0a20 2020 2020 2020  1": "1",.       
-00002350: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
-00002360: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00002370: 2020 2020 2020 2020 2261 223a 2022 5468          "a": "Th
-00002380: 6f6d 6173 2c20 4461 7669 642c 220a 2020  omas, David,".  
-00002390: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000023a0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-000023b0: 2020 2022 6422 3a20 2231 3935 362d 220a     "d": "1956-".
-000023c0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000023d0: 2020 2020 5d2c 0a20 2020 2020 2020 2022      ],.        "
-000023e0: 696e 6432 223a 2022 2022 0a20 2020 2020  ind2": " ".     
-000023f0: 207d 0a20 2020 207d 0a20 205d 0a7d 0a60   }.    }.  ].}.`
-00002400: 6060 0a0a 4966 2079 6f75 2077 616e 7420  ``..If you want 
-00002410: 746f 2070 6172 7365 2061 2066 696c 6520  to parse a file 
-00002420: 6f66 204d 4152 434a 534f 4e20 7265 636f  of MARCJSON reco
-00002430: 7264 7320 796f 7520 6361 6e3a 0a0a 6060  rds you can:..``
-00002440: 6070 7974 686f 6e0a 6672 6f6d 2070 796d  `python.from pym
-00002450: 6172 6320 696d 706f 7274 2070 6172 7365  arc import parse
-00002460: 5f6a 736f 6e5f 746f 5f61 7272 6179 0a0a  _json_to_array..
-00002470: 7265 636f 7264 7320 3d20 7061 7273 655f  records = parse_
-00002480: 6a73 6f6e 5f74 6f5f 6172 7261 7928 6f70  json_to_array(op
-00002490: 656e 2827 7465 7374 2f62 6174 6368 2e6a  en('test/batch.j
-000024a0: 736f 6e27 2929 0a0a 7072 696e 7428 7265  son'))..print(re
-000024b0: 636f 7264 735b 305d 290a 6060 600a 0a60  cords[0]).```..`
-000024c0: 6060 0a3d 4c44 5220 2030 3039 3235 6e6a  ``.=LDR  00925nj
-000024d0: 6d20 2032 3230 3032 3737 3761 2034 3530  m  22002777a 450
-000024e0: 300a 3d30 3031 2020 3536 3337 3234 310a  0.=001  5637241.
-000024f0: 3d30 3033 2020 444c 430a 3d30 3035 2020  =003  DLC.=005  
-00002500: 3139 3932 3038 3236 3038 3430 3336 2e30  19920826084036.0
-00002510: 0a3d 3030 3720 2073 6475 6275 6d65 6e6e  .=007  sdubumenn
-00002520: 6d70 6c75 0a3d 3030 3820 2039 3130 3932  mplu.=008  91092
-00002530: 3673 3139 3537 5c5c 5c5c 6e79 7575 756e  6s1957\\\\nyuuun
-00002540: 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c 656e  \\\\\\\\\\\\\\en
-00002550: 675c 5c0a 3d30 3130 2020 5c5c 2461 2020  g\\.=010  \\$a  
-00002560: 2039 3137 3538 3333 350a 3d30 3238 2020   91758335.=028  
-00002570: 3030 2461 3132 3539 2462 4174 6c61 6e74  00$a1259$bAtlant
-00002580: 6963 0a3d 3034 3020 205c 5c24 6144 4c43  ic.=040  \\$aDLC
-00002590: 2463 444c 430a 3d30 3530 2020 3030 2461  $cDLC.=050  00$a
-000025a0: 4174 6c61 6e74 6963 2031 3235 390a 3d32  Atlantic 1259.=2
-000025b0: 3435 2020 3034 2461 5468 6520 4772 6561  45  04$aThe Grea
-000025c0: 7420 5261 7920 4368 6172 6c65 7324 685b  t Ray Charles$h[
-000025d0: 736f 756e 6420 7265 636f 7264 696e 675d  sound recording]
-000025e0: 2e0a 3d32 3630 2020 5c5c 2461 4e65 7720  ..=260  \\$aNew 
-000025f0: 596f 726b 2c20 4e2e 592e 203a 2462 4174  York, N.Y. :$bAt
-00002600: 6c61 6e74 6963 2c24 635b 3139 3537 3f5d  lantic,$c[1957?]
-00002610: 0a3d 3330 3020 205c 5c24 6131 2073 6f75  .=300  \\$a1 sou
-00002620: 6e64 2064 6973 6320 3a24 6261 6e61 6c6f  nd disc :$banalo
-00002630: 672c 2033 3320 312f 3320 7270 6d20 3b24  g, 33 1/3 rpm ;$
-00002640: 6331 3220 696e 2e0a 3d35 3131 2020 305c  c12 in..=511  0\
-00002650: 2461 5261 7920 4368 6172 6c65 732c 2070  $aRay Charles, p
-00002660: 6961 6e6f 2026 2063 656c 6573 7465 2e0a  iano & celeste..
-00002670: 3d35 3035 2020 305c 2461 5468 6520 5261  =505  0\$aThe Ra
-00002680: 7920 2d2d 204d 7920 6d65 6c61 6e63 686f  y -- My melancho
-00002690: 6c79 2062 6162 7920 2d2d 2042 6c61 636b  ly baby -- Black
-000026a0: 2063 6f66 6665 6520 2d2d 2054 6865 7265   coffee -- There
-000026b0: 2773 206e 6f20 796f 7520 2d2d 2044 6f6f  's no you -- Doo
-000026c0: 646c 696e 2720 2d2d 2053 7765 6574 2073  dlin' -- Sweet s
-000026d0: 6978 7465 656e 2062 6172 7320 2d2d 2049  ixteen bars -- I
-000026e0: 2073 7572 7265 6e64 6572 2064 6561 7220   surrender dear 
-000026f0: 2d2d 2055 6e64 6563 6964 6564 2e0a 3d35  -- Undecided..=5
-00002700: 3030 2020 5c5c 2461 4272 6965 6620 7265  00  \\$aBrief re
-00002710: 636f 7264 2e0a 3d36 3530 2020 5c30 2461  cord..=650  \0$a
-00002720: 4a61 7a7a 2479 3139 3531 2d31 3936 302e  Jazz$y1951-1960.
-00002730: 0a3d 3635 3020 205c 3024 6150 6961 6e6f  .=650  \0$aPiano
-00002740: 2077 6974 6820 6a61 7a7a 2065 6e73 656d   with jazz ensem
-00002750: 626c 652e 0a3d 3730 3020 2031 5c24 6143  ble..=700  1\$aC
-00002760: 6861 726c 6573 2c20 5261 792c 2464 3139  harles, Ray,$d19
-00002770: 3330 2d24 3470 7266 0a60 6060 0a0a 5375  30-$4prf.```..Su
-00002780: 7070 6f72 740a 2d2d 2d2d 2d2d 2d0a 0a54  pport.-------..T
-00002790: 6865 2070 796d 6172 6320 6465 7665 6c6f  he pymarc develo
-000027a0: 7065 7273 2065 6e63 6f75 7261 6765 2079  pers encourage y
-000027b0: 6f75 2074 6f20 6a6f 696e 2074 6865 205b  ou to join the [
-000027c0: 7079 6d61 7263 2047 6f6f 676c 650a 4772  pymarc Google.Gr
-000027d0: 6f75 705d 2868 7474 703a 2f2f 6772 6f75  oup](http://grou
-000027e0: 7073 2e67 6f6f 676c 652e 636f 6d2f 6772  ps.google.com/gr
-000027f0: 6f75 702f 7079 6d61 7263 2920 6966 2079  oup/pymarc) if y
-00002800: 6f75 206e 6565 6420 6865 6c70 2e20 2041  ou need help.  A
-00002810: 6c73 6f2c 2070 6c65 6173 650a 6665 656c  lso, please.feel
-00002820: 2066 7265 6520 746f 2075 7365 205b 6973   free to use [is
-00002830: 7375 6520 7472 6163 6b69 6e67 5d28 6874  sue tracking](ht
-00002840: 7470 733a 2f2f 6769 746c 6162 2e63 6f6d  tps://gitlab.com
-00002850: 2f70 796d 6172 632f 7079 6d61 7263 2f69  /pymarc/pymarc/i
-00002860: 7373 7565 7329 206f 6e0a 4769 744c 6162  ssues) on.GitLab
-00002870: 2074 6f20 7375 626d 6974 2066 6561 7475   to submit featu
-00002880: 7265 2072 6571 7565 7374 7320 6f72 2062  re requests or b
-00002890: 7567 2072 6570 6f72 7473 2e20 4966 2079  ug reports. If y
-000028a0: 6f75 2776 6520 676f 7420 616e 2069 7463  ou've got an itc
-000028b0: 6820 746f 0a73 6372 6174 6368 2c20 706c  h to.scratch, pl
-000028c0: 6561 7365 2073 6372 6174 6368 2069 742c  ease scratch it,
-000028d0: 2061 6e64 2073 656e 6420 6d65 7267 6520   and send merge 
-000028e0: 7265 7175 6573 7473 206f 6e0a 5b47 6974  requests on.[Git
-000028f0: 4c61 625d 2868 7474 703a 2f2f 6769 746c  Lab](http://gitl
-00002900: 6162 2e63 6f6d 2f70 796d 6172 632f 7079  ab.com/pymarc/py
-00002910: 6d61 7263 292e 0a0a 4966 2079 6f75 2073  marc)...If you s
-00002920: 7461 7274 2077 6f72 6b69 6e67 2077 6974  tart working wit
-00002930: 6820 4d41 5243 2079 6f75 206d 6179 2066  h MARC you may f
-00002940: 6565 6c20 6c69 6b65 2079 6f75 206e 6565  eel like you nee
-00002950: 6420 6d6f 7261 6c20 7375 7070 6f72 740a  d moral support.
-00002960: 696e 2061 6464 6974 696f 6e20 746f 2074  in addition to t
-00002970: 6563 686e 6963 616c 2073 7570 706f 7274  echnical support
-00002980: 2e20 5468 650a 5b23 636f 6465 346c 6962  . The.[#code4lib
-00002990: 5d28 6972 6373 3a2f 2f69 7263 2e6c 6962  ](ircs://irc.lib
-000029a0: 6572 612e 6368 6174 2f63 6f64 6534 6c69  era.chat/code4li
-000029b0: 6229 2063 6861 6e6e 656c 206f 6e20 5b4c  b) channel on [L
-000029c0: 6962 6572 615d 2868 7474 7073 3a2f 2f6c  ibera](https://l
-000029d0: 6962 6572 612e 6368 6174 2f29 2069 7320  ibera.chat/) is 
-000029e0: 6120 676f 6f64 2070 6c61 6365 2066 6f72  a good place for
-000029f0: 2062 6f74 682e 0a0a 0a                    both....
+00000000: 6060 600a 5f7c 5f7c 5f7c 2020 2020 5f7c  ```._|_|_|    _|
+00000010: 2020 2020 5f7c 2020 5f7c 5f7c 5f7c 2020      _|  _|_|_|  
+00000020: 5f7c 5f7c 2020 2020 2020 5f7c 5f7c 5f7c  _|_|      _|_|_|
+00000030: 2020 5f7c 2020 5f7c 5f7c 2020 2020 5f7c    _|  _|_|    _|
+00000040: 5f7c 5f7c 0a5f 7c20 2020 205f 7c20 205f  _|_|._|    _|  _
+00000050: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
+00000060: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
+00000070: 7c20 205f 7c5f 7c20 2020 2020 205f 7c0a  |  _|_|      _|.
+00000080: 5f7c 2020 2020 5f7c 2020 5f7c 2020 2020  _|    _|  _|    
+00000090: 5f7c 2020 5f7c 2020 2020 5f7c 2020 2020  _|  _|    _|    
+000000a0: 5f7c 2020 5f7c 2020 2020 5f7c 2020 5f7c  _|  _|    _|  _|
+000000b0: 2020 2020 2020 2020 5f7c 0a5f 7c5f 7c5f          _|._|_|_
+000000c0: 7c20 2020 2020 205f 7c5f 7c5f 7c20 205f  |      _|_|_|  _
+000000d0: 7c20 2020 205f 7c20 2020 205f 7c20 2020  |    _|    _|   
+000000e0: 205f 7c5f 7c5f 7c20 205f 7c20 2020 2020   _|_|_|  _|     
+000000f0: 2020 2020 205f 7c5f 7c5f 7c0a 5f7c 2020       _|_|_|._|  
+00000100: 2020 2020 2020 2020 2020 2020 5f7c 0a5f              _|._
+00000110: 7c20 2020 2020 2020 2020 205f 7c5f 7c0a  |          _|_|.
+00000120: 6060 600a 0a5b 215b 4275 696c 6420 7374  ```..[![Build st
+00000130: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
+00000140: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
+00000150: 7079 6d61 7263 2f62 6164 6765 732f 6d61  pymarc/badges/ma
+00000160: 696e 2f70 6970 656c 696e 652e 7376 6729  in/pipeline.svg)
+00000170: 5d28 6874 7470 733a 2f2f 6769 746c 6162  ](https://gitlab
+00000180: 2e63 6f6d 2f70 796d 6172 632f 7079 6d61  .com/pymarc/pyma
+00000190: 7263 2f2d 2f63 6f6d 6d69 7473 2f6d 6169  rc/-/commits/mai
+000001a0: 6e29 0a0a 7079 6d61 7263 2069 7320 6120  n)..pymarc is a 
+000001b0: 7079 7468 6f6e 206c 6962 7261 7279 2066  python library f
+000001c0: 6f72 2077 6f72 6b69 6e67 2077 6974 6820  or working with 
+000001d0: 6269 626c 696f 6772 6170 6869 6320 6461  bibliographic da
+000001e0: 7461 2065 6e63 6f64 6564 2069 6e0a 5b4d  ta encoded in.[M
+000001f0: 4152 4332 315d 2868 7474 7073 3a2f 2f65  ARC21](https://e
+00000200: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00000210: 7769 6b69 2f4d 4152 435f 7374 616e 6461  wiki/MARC_standa
+00000220: 7264 7329 2e20 4974 2070 726f 7669 6465  rds). It provide
+00000230: 7320 616e 2041 5049 2066 6f72 0a72 6561  s an API for.rea
+00000240: 6469 6e67 2c20 7772 6974 696e 6720 616e  ding, writing an
+00000250: 6420 6d6f 6469 6679 696e 6720 4d41 5243  d modifying MARC
+00000260: 2072 6563 6f72 6473 2e20 4974 2077 6173   records. It was
+00000270: 206d 6f73 746c 7920 6465 7369 676e 6564   mostly designed
+00000280: 2074 6f20 6265 2061 6e0a 656d 6572 6765   to be an.emerge
+00000290: 6e63 7920 656a 6563 7420 7365 6174 2c20  ncy eject seat, 
+000002a0: 666f 7220 6765 7474 696e 6720 796f 7572  for getting your
+000002b0: 2064 6174 6120 6173 7365 7473 206f 7574   data assets out
+000002c0: 206f 6620 4d41 5243 2061 6e64 2069 6e74   of MARC and int
+000002d0: 6f20 736f 6d65 0a6b 696e 6420 6f66 2073  o some.kind of s
+000002e0: 616e 6572 2072 6570 7265 7365 6e74 6174  aner representat
+000002f0: 696f 6e2e 2048 6f77 6576 6572 206f 7665  ion. However ove
+00000300: 7220 7468 6520 7965 6172 7320 6974 2068  r the years it h
+00000310: 6173 2062 6565 6e20 7573 6564 2074 6f20  as been used to 
+00000320: 6372 6561 7465 0a61 6e64 206d 6f64 6966  create.and modif
+00000330: 7920 4d41 5243 2072 6563 6f72 6473 2c20  y MARC records, 
+00000340: 7369 6e63 6520 6465 7370 6974 6520 5b72  since despite [r
+00000350: 6570 6561 7465 640a 6361 6c6c 735d 2868  epeated.calls](h
+00000360: 7474 7073 3a2f 2f77 6562 2e61 7263 6869  ttps://web.archi
+00000370: 7665 2e6f 7267 2f77 6562 2f32 3031 3730  ve.org/web/20170
+00000380: 3733 3131 3633 3031 392f 6874 7470 3a2f  731163019/http:/
+00000390: 2f77 7777 2e6d 6172 632d 6d75 7374 2d64  /www.marc-must-d
+000003a0: 6965 2e69 6e66 6f2f 696e 6465 782e 7068  ie.info/index.ph
+000003b0: 702f 4d61 696e 5f50 6167 6529 0a66 6f72  p/Main_Page).for
+000003c0: 2069 7420 746f 2064 6965 2061 7320 6120   it to die as a 
+000003d0: 666f 726d 6174 2c20 4d41 5243 2073 6565  format, MARC see
+000003e0: 6d73 2074 6f20 6265 206c 6976 696e 6720  ms to be living 
+000003f0: 7175 6974 6520 6861 7070 696c 7920 6173  quite happily as
+00000400: 2061 207a 6f6d 6269 652e 0a0a 4265 6c6f   a zombie...Belo
+00000410: 7720 6172 6520 736f 6d65 2063 6f6d 6d6f  w are some commo
+00000420: 6e20 6578 616d 706c 6573 206f 6620 686f  n examples of ho
+00000430: 7720 796f 7520 6d69 6768 7420 7761 6e74  w you might want
+00000440: 2074 6f20 7573 6520 7079 6d61 7263 2e20   to use pymarc. 
+00000450: 4966 0a79 6f75 2072 756e 2061 6372 6f73  If.you run acros
+00000460: 7320 616e 2065 7861 6d70 6c65 2074 6861  s an example tha
+00000470: 7420 796f 7520 7468 696e 6b20 7368 6f75  t you think shou
+00000480: 6c64 2062 6520 6865 7265 2070 6c65 6173  ld be here pleas
+00000490: 6520 7365 6e64 2061 0a70 756c 6c20 7265  e send a.pull re
+000004a0: 7175 6573 742e 0a0a 596f 7520 6361 6e20  quest...You can 
+000004b0: 7265 6164 2070 796d 6172 6320 646f 6375  read pymarc docu
+000004c0: 6d65 6e74 6174 696f 6e20 5b68 6572 655d  mentation [here]
+000004d0: 2868 7474 7073 3a2f 2f70 796d 6172 632e  (https://pymarc.
+000004e0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000004f0: 6e2f 6c61 7465 7374 2f29 2e0a 0a23 2323  n/latest/)...###
+00000500: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a59   Installation..Y
+00000510: 6f75 276c 6c20 7072 6f62 6162 6c79 206a  ou'll probably j
+00000520: 7573 7420 7761 6e74 2074 6f20 7573 6520  ust want to use 
+00000530: 7069 7020 746f 2069 6e73 7461 6c6c 2070  pip to install p
+00000540: 796d 6172 633a 0a0a 2020 2020 7069 7020  ymarc:..    pip 
+00000550: 696e 7374 616c 6c20 7079 6d61 7263 0a0a  install pymarc..
+00000560: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
+00000570: 2064 6f77 6e6c 6f61 6420 616e 6420 696e   download and in
+00000580: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
+00000590: 2073 6f75 7263 6520 796f 7527 6c6c 206e   source you'll n
+000005a0: 6565 6420 6769 743a 0a0a 2020 2020 6769  eed git:..    gi
+000005b0: 7420 636c 6f6e 6520 6769 743a 2f2f 6769  t clone git://gi
+000005c0: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
+000005d0: 7079 6d61 7263 2e67 6974 0a0a 596f 7527  pymarc.git..You'
+000005e0: 6c6c 2061 6c73 6f20 6e65 6564 205b 7365  ll also need [se
+000005f0: 7475 7074 6f6f 6c73 5d28 6874 7470 733a  tuptools](https:
+00000600: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000610: 672f 7079 7069 2f73 6574 7570 746f 6f6c  g/pypi/setuptool
+00000620: 7323 696e 7374 616c 6c61 7469 6f6e 2d69  s#installation-i
+00000630: 6e73 7472 7563 7469 6f6e 7329 2e20 4f6e  nstructions). On
+00000640: 6365 2079 6f75 2068 6176 6520 7468 6520  ce you have the 
+00000650: 736f 7572 6365 2061 6e64 2073 6574 7570  source and setup
+00000660: 746f 6f6c 7320 7275 6e20 7468 6520 7079  tools run the py
+00000670: 6d61 7263 2074 6573 740a 7375 6974 6520  marc test.suite 
+00000680: 746f 206d 616b 6520 7375 7265 2074 6869  to make sure thi
+00000690: 6e67 7320 6172 6520 696e 206f 7264 6572  ngs are in order
+000006a0: 2077 6974 6820 7468 6520 6469 7374 7269   with the distri
+000006b0: 6275 7469 6f6e 3a0a 0a20 2020 2070 7974  bution:..    pyt
+000006c0: 686f 6e20 7365 7475 702e 7079 2074 6573  hon setup.py tes
+000006d0: 740a 0a41 6e64 2074 6865 6e20 696e 7374  t..And then inst
+000006e0: 616c 6c3a 0a0a 2020 2020 7079 7468 6f6e  all:..    python
+000006f0: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
+00000700: 6c0a 0a23 2323 2052 6561 6469 6e67 0a0a  l..### Reading..
+00000710: 4d6f 7374 206f 6674 656e 2079 6f75 2077  Most often you w
+00000720: 696c 6c20 6861 7665 2073 6f6d 6520 4d41  ill have some MA
+00000730: 5243 2064 6174 6120 616e 6420 7769 6c6c  RC data and will
+00000740: 2077 616e 7420 746f 2065 7874 7261 6374   want to extract
+00000750: 2064 6174 610a 6672 6f6d 2069 742e 2048   data.from it. H
+00000760: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
+00000770: 206f 6620 7265 6164 696e 6720 6120 6261   of reading a ba
+00000780: 7463 6820 6f66 2072 6563 6f72 6473 2061  tch of records a
+00000790: 6e64 2070 7269 6e74 696e 6720 6f75 740a  nd printing out.
+000007a0: 7468 6520 7469 746c 652e 2049 6620 796f  the title. If yo
+000007b0: 7520 6172 6520 6375 7269 6f75 7320 7468  u are curious th
+000007c0: 6973 2065 7861 6d70 6c65 2075 7365 7320  is example uses 
+000007d0: 7468 6520 6261 7463 6820 6669 6c65 0a61  the batch file.a
+000007e0: 7661 696c 6162 6c65 2068 6572 6520 696e  vailable here in
+000007f0: 2070 796d 6172 6320 7265 706f 7369 746f   pymarc reposito
+00000800: 7279 3a0a 0a60 6060 7079 7468 6f6e 0a66  ry:..```python.f
+00000810: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
+00000820: 7420 4d41 5243 5265 6164 6572 0a77 6974  t MARCReader.wit
+00000830: 6820 6f70 656e 2827 7465 7374 2f6d 6172  h open('test/mar
+00000840: 632e 6461 7427 2c20 2772 6227 2920 6173  c.dat', 'rb') as
+00000850: 2066 683a 0a20 2020 2072 6561 6465 7220   fh:.    reader 
+00000860: 3d20 4d41 5243 5265 6164 6572 2866 6829  = MARCReader(fh)
+00000870: 0a20 2020 2066 6f72 2072 6563 6f72 6420  .    for record 
+00000880: 696e 2072 6561 6465 723a 0a20 2020 2020  in reader:.     
+00000890: 2020 2070 7269 6e74 2872 6563 6f72 642e     print(record.
+000008a0: 7469 746c 6529 0a60 6060 0a60 6060 0a54  title).```.```.T
+000008b0: 6865 2070 7261 676d 6174 6963 2070 726f  he pragmatic pro
+000008c0: 6772 616d 6d65 7220 3a20 6672 6f6d 206a  grammer : from j
+000008d0: 6f75 726e 6579 6d61 6e20 746f 206d 6173  ourneyman to mas
+000008e0: 7465 7220 2f0a 5072 6f67 7261 6d6d 696e  ter /.Programmin
+000008f0: 6720 5079 7468 6f6e 202f 0a4c 6561 726e  g Python /.Learn
+00000900: 696e 6720 5079 7468 6f6e 202f 0a50 7974  ing Python /.Pyt
+00000910: 686f 6e20 636f 6f6b 626f 6f6b 202f 0a50  hon cookbook /.P
+00000920: 7974 686f 6e20 7072 6f67 7261 6d6d 696e  ython programmin
+00000930: 6720 666f 7220 7468 6520 6162 736f 6c75  g for the absolu
+00000940: 7465 2062 6567 696e 6e65 7220 2f0a 5765  te beginner /.We
+00000950: 6220 7072 6f67 7261 6d6d 696e 6720 3a20  b programming : 
+00000960: 7465 6368 6e69 7175 6573 2066 6f72 2069  techniques for i
+00000970: 6e74 6567 7261 7469 6e67 2050 7974 686f  ntegrating Pytho
+00000980: 6e2c 204c 696e 7578 2c20 4170 6163 6865  n, Linux, Apache
+00000990: 2c20 616e 6420 4d79 5351 4c20 2f0a 5079  , and MySQL /.Py
+000009a0: 7468 6f6e 2070 726f 6772 616d 6d69 6e67  thon programming
+000009b0: 206f 6e20 5769 6e33 3220 2f0a 5079 7468   on Win32 /.Pyth
+000009c0: 6f6e 2070 726f 6772 616d 6d69 6e67 203a  on programming :
+000009d0: 2061 6e20 696e 7472 6f64 7563 7469 6f6e   an introduction
+000009e0: 2074 6f20 636f 6d70 7574 6572 2073 6369   to computer sci
+000009f0: 656e 6365 202f 0a50 7974 686f 6e20 5765  ence /.Python We
+00000a00: 6220 7072 6f67 7261 6d6d 696e 6720 2f0a  b programming /.
+00000a10: 436f 7265 2070 7974 686f 6e20 7072 6f67  Core python prog
+00000a20: 7261 6d6d 696e 6720 2f0a 5079 7468 6f6e  ramming /.Python
+00000a30: 2061 6e64 2054 6b69 6e74 6572 2070 726f   and Tkinter pro
+00000a40: 6772 616d 6d69 6e67 202f 0a47 616d 6520  gramming /.Game 
+00000a50: 7072 6f67 7261 6d6d 696e 6720 7769 7468  programming with
+00000a60: 2050 7974 686f 6e2c 204c 7561 2c20 616e   Python, Lua, an
+00000a70: 6420 5275 6279 202f 0a50 7974 686f 6e20  d Ruby /.Python 
+00000a80: 7072 6f67 7261 6d6d 696e 6720 7061 7474  programming patt
+00000a90: 6572 6e73 202f 0a50 7974 686f 6e20 7072  erns /.Python pr
+00000aa0: 6f67 7261 6d6d 696e 6720 7769 7468 2074  ogramming with t
+00000ab0: 6865 204a 6176 6120 636c 6173 7320 6c69  he Java class li
+00000ac0: 6272 6172 6965 7320 3a20 6120 7475 746f  braries : a tuto
+00000ad0: 7269 616c 2066 6f72 2062 7569 6c64 696e  rial for buildin
+00000ae0: 6720 5765 620a 616e 6420 456e 7465 7270  g Web.and Enterp
+00000af0: 7269 7365 2061 7070 6c69 6361 7469 6f6e  rise application
+00000b00: 7320 2f0a 4c65 6172 6e20 746f 2070 726f  s /.Learn to pro
+00000b10: 6772 616d 2075 7369 6e67 2050 7974 686f  gram using Pytho
+00000b20: 6e20 3a20 6120 7475 746f 7269 616c 2066  n : a tutorial f
+00000b30: 6f72 2068 6f62 6279 6973 7473 2c20 7365  or hobbyists, se
+00000b40: 6c66 2d73 7461 7274 6572 732c 2061 6e64  lf-starters, and
+00000b50: 2061 6c6c 0a77 686f 2077 616e 7420 746f   all.who want to
+00000b60: 206c 6561 726e 2074 6865 2061 7274 206f   learn the art o
+00000b70: 6620 636f 6d70 7574 6572 2070 726f 6772  f computer progr
+00000b80: 616d 6d69 6e67 202f 0a50 726f 6772 616d  amming /.Program
+00000b90: 6d69 6e67 2077 6974 6820 5079 7468 6f6e  ming with Python
+00000ba0: 202f 0a42 5344 2053 6f63 6b65 7473 2070   /.BSD Sockets p
+00000bb0: 726f 6772 616d 6d69 6e67 2066 726f 6d20  rogramming from 
+00000bc0: 6120 6d75 6c74 692d 6c61 6e67 7561 6765  a multi-language
+00000bd0: 2070 6572 7370 6563 7469 7665 202f 0a44   perspective /.D
+00000be0: 6573 6967 6e20 7061 7474 6572 6e73 203a  esign patterns :
+00000bf0: 2065 6c65 6d65 6e74 7320 6f66 2072 6575   elements of reu
+00000c00: 7361 626c 6520 6f62 6a65 6374 2d6f 7269  sable object-ori
+00000c10: 656e 7465 6420 736f 6674 7761 7265 202f  ented software /
+00000c20: 0a49 6e74 726f 6475 6374 696f 6e20 746f  .Introduction to
+00000c30: 2061 6c67 6f72 6974 686d 7320 2f0a 414e   algorithms /.AN
+00000c40: 5349 2043 6f6d 6d6f 6e20 4c69 7370 202f  SI Common Lisp /
+00000c50: 0a60 6060 0a0a 4120 6070 796d 6172 632e  .```..A `pymarc.
+00000c60: 5265 636f 7264 6020 6f62 6a65 6374 2068  Record` object h
+00000c70: 6173 2061 2066 6577 2068 616e 6479 2070  as a few handy p
+00000c80: 726f 7065 7274 6965 7320 6c69 6b65 2060  roperties like `
+00000c90: 7469 746c 6560 2066 6f72 2067 6574 7469  title` for getti
+00000ca0: 6e67 2061 740a 6269 7473 206f 6620 6120  ng at.bits of a 
+00000cb0: 6269 626c 696f 6772 6170 6869 6320 7265  bibliographic re
+00000cc0: 636f 7264 2c20 6f74 6865 7273 2069 6e63  cord, others inc
+00000cd0: 6c75 6465 3a20 6061 7574 686f 7260 2c20  lude: `author`, 
+00000ce0: 6069 7362 6e60 2c20 6073 7562 6a65 6374  `isbn`, `subject
+00000cf0: 7360 2c0a 606c 6f63 6174 696f 6e60 2c20  s`,.`location`, 
+00000d00: 606e 6f74 6573 602c 2060 7068 7973 6963  `notes`, `physic
+00000d10: 616c 6465 7363 7269 7074 696f 6e60 2c20  aldescription`, 
+00000d20: 6070 7562 6c69 7368 6572 602c 2060 7075  `publisher`, `pu
+00000d30: 6279 6561 7260 2c20 6069 7373 6e60 2c0a  byear`, `issn`,.
+00000d40: 6069 7373 6e5f 7469 746c 6560 2e20 4275  `issn_title`. Bu
+00000d50: 7420 7265 616c 6c79 2c20 746f 2077 6f72  t really, to wor
+00000d60: 6b20 7769 7468 204d 4152 4320 6461 7461  k with MARC data
+00000d70: 2079 6f75 206e 6565 6420 746f 2075 6e64   you need to und
+00000d80: 6572 7374 616e 6420 7468 650a 6e75 6d65  erstand the.nume
+00000d90: 7269 6320 6669 656c 6420 7461 6773 2061  ric field tags a
+00000da0: 6e64 2073 7562 6669 656c 6420 636f 6465  nd subfield code
+00000db0: 7320 7468 6174 2061 7265 2075 7365 6420  s that are used 
+00000dc0: 746f 2064 6573 6967 6e61 7465 2076 6172  to designate var
+00000dd0: 696f 7573 2062 6974 730a 6f66 2069 6e66  ious bits.of inf
+00000de0: 6f72 6d61 7469 6f6e 2e20 5468 6572 6520  ormation. There 
+00000df0: 6973 2061 206c 6f74 206d 6f72 6520 6461  is a lot more da
+00000e00: 7461 2068 6964 6465 6e20 696e 2061 204d  ta hidden in a M
+00000e10: 4152 4320 7265 636f 7264 2074 6861 6e20  ARC record than 
+00000e20: 7468 6573 650a 6865 6c70 6572 2070 726f  these.helper pro
+00000e30: 7065 7274 6965 7320 7072 6f76 6964 6520  perties provide 
+00000e40: 6163 6365 7373 2074 6f2e 2046 6f72 2065  access to. For e
+00000e50: 7861 6d70 6c65 2074 6865 2060 7469 746c  xample the `titl
+00000e60: 6560 2070 726f 7065 7274 7920 776f 726b  e` property work
+00000e70: 7320 6279 0a65 7874 7261 6374 696e 6720  s by.extracting 
+00000e80: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
+00000e90: 6672 6f6d 2074 6865 2060 3234 3560 2066  from the `245` f
+00000ea0: 6965 6c64 2c20 7375 6266 6965 6c64 7320  ield, subfields 
+00000eb0: 6061 6020 616e 6420 6062 6020 6265 6869  `a` and `b` behi
+00000ec0: 6e64 0a74 6865 2073 6365 6e65 732e 2059  nd.the scenes. Y
+00000ed0: 6f75 2063 616e 2061 6363 6573 7320 6032  ou can access `2
+00000ee0: 3435 6160 206c 696b 6520 736f 3a0a 0a60  45a` like so:..`
+00000ef0: 6060 7079 7468 6f6e 0a70 7269 6e74 2872  ``python.print(r
+00000f00: 6563 6f72 645b 2732 3435 275d 5b27 6127  ecord['245']['a'
+00000f10: 5d29 0a60 6060 0a0a 536f 6d65 2066 6965  ]).```..Some fie
+00000f20: 6c64 7320 6c69 6b65 2073 7562 6a65 6374  lds like subject
+00000f30: 7320 6361 6e20 7265 7065 6174 2e20 496e  s can repeat. In
+00000f40: 2063 6173 6573 206c 696b 6520 7468 6174   cases like that
+00000f50: 2079 6f75 2077 696c 6c20 7761 6e74 2074   you will want t
+00000f60: 6f20 7573 650a 6067 6574 5f66 6965 6c64  o use.`get_field
+00000f70: 7360 2074 6f20 6765 7420 616c 6c20 6f66  s` to get all of
+00000f80: 2074 6865 6d20 6173 2060 7079 6d61 7263   them as `pymarc
+00000f90: 2e46 6965 6c64 6020 6f62 6a65 6374 732c  .Field` objects,
+00000fa0: 2077 6869 6368 2079 6f75 2063 616e 2074   which you can t
+00000fb0: 6865 6e0a 696e 7465 7261 6374 2077 6974  hen.interact wit
+00000fc0: 6820 6675 7274 6865 723a 0a0a 6060 6070  h further:..```p
+00000fd0: 7974 686f 6e0a 666f 7220 6620 696e 2072  ython.for f in r
+00000fe0: 6563 6f72 642e 6765 745f 6669 656c 6473  ecord.get_fields
+00000ff0: 2827 3635 3027 293a 0a20 2020 2070 7269  ('650'):.    pri
+00001000: 6e74 2866 290a 6060 600a 0a49 6620 796f  nt(f).```..If yo
+00001010: 7520 6172 6520 6e65 7720 746f 204d 4152  u are new to MAR
+00001020: 4320 6669 656c 6473 205b 556e 6465 7273  C fields [Unders
+00001030: 7461 6e64 696e 670a 4d41 5243 5d28 6874  tanding.MARC](ht
+00001040: 7470 3a2f 2f77 7777 2e6c 6f63 2e67 6f76  tp://www.loc.gov
+00001050: 2f6d 6172 632f 756d 622f 2920 6973 2061  /marc/umb/) is a
+00001060: 2070 7265 7474 7920 676f 6f64 2070 7269   pretty good pri
+00001070: 6d65 722c 2061 6e64 2074 6865 205b 4d41  mer, and the [MA
+00001080: 5243 2032 310a 466f 726d 6174 735d 2868  RC 21.Formats](h
+00001090: 7474 703a 2f2f 7777 772e 6c6f 632e 676f  ttp://www.loc.go
+000010a0: 762f 6d61 7263 2f6d 6172 6364 6f63 7a2e  v/marc/marcdocz.
+000010b0: 6874 6d6c 2920 7061 6765 2061 7420 7468  html) page at th
+000010c0: 6520 4c69 6272 6172 7920 6f66 2043 6f6e  e Library of Con
+000010d0: 6772 6573 7320 6973 2061 2067 6f6f 6420  gress is a good 
+000010e0: 7265 6665 7265 6e63 6520 6f6e 6365 2079  reference once y
+000010f0: 6f75 2075 6e64 6572 7374 616e 6420 7468  ou understand th
+00001100: 6520 6261 7369 6373 2e0a 0a23 2323 2057  e basics...### W
+00001110: 7269 7469 6e67 0a0a 2a4e 6f74 653a 2041  riting..*Note: A
+00001120: 7320 6f66 2076 352e 302e 3020 6053 7562  s of v5.0.0 `Sub
+00001130: 6669 656c 6460 2069 7320 7573 6564 2074  field` is used t
+00001140: 6f20 6372 6561 7465 2073 7562 6669 656c  o create subfiel
+00001150: 6473 2e20 5072 696f 7220 746f 2076 352c  ds. Prior to v5,
+00001160: 0a73 7562 6669 656c 6473 2077 6572 6520  .subfields were 
+00001170: 636f 6e73 7472 7563 7465 6420 616e 6420  constructed and 
+00001180: 6163 6365 7373 6564 2061 7320 6120 6c69  accessed as a li
+00001190: 7374 206f 6620 7374 7269 6e67 732c 2065  st of strings, e
+000011a0: 2e67 2e2c 2060 5b63 6f64 652c 0a76 616c  .g., `[code,.val
+000011b0: 7565 2c20 636f 6465 2c20 7661 6c75 655d  ue, code, value]
+000011c0: 602e 2049 6e20 7635 2e30 2e30 2074 6869  `. In v5.0.0 thi
+000011d0: 7320 6861 7320 6265 656e 2063 6861 6e67  s has been chang
+000011e0: 6564 2074 6f20 6f72 6761 6e69 7a65 2074  ed to organize t
+000011f0: 6865 2073 7562 6669 656c 6473 0a69 6e74  he subfields.int
+00001200: 6f20 6120 6c69 7374 206f 6620 7475 706c  o a list of tupl
+00001210: 6573 2c20 652e 672e 2c20 605b 2863 6f64  es, e.g., `[(cod
+00001220: 652c 2076 616c 7565 292c 2028 636f 6465  e, value), (code
+00001230: 2c20 7661 6c75 6529 5d60 2e20 5468 6520  , value)]`. The 
+00001240: 6053 7562 6669 656c 6460 0a69 7320 696d  `Subfield`.is im
+00001250: 706c 656d 656e 7465 6420 6173 2061 2060  plemented as a `
+00001260: 4e61 6d65 6454 7570 6c65 6020 736f 2074  NamedTuple` so t
+00001270: 6861 7420 7468 6520 7475 706c 6573 2063  hat the tuples c
+00001280: 616e 2062 6520 636f 6e73 7472 7563 7465  an be constructe
+00001290: 6420 6173 0a60 5375 6266 6965 6c64 2863  d as.`Subfield(c
+000012a0: 6f64 653d 636f 6465 2c20 7661 6c75 653d  ode=code, value=
+000012b0: 7661 6c75 6529 602e 2054 6865 206f 6c64  value)`. The old
+000012c0: 2073 7479 6c65 206f 6620 6372 6561 7469   style of creati
+000012d0: 6e67 2073 7562 6669 656c 6473 2069 7320  ng subfields is 
+000012e0: 6e6f 0a6c 6f6e 6765 7220 7375 7070 6f72  no.longer suppor
+000012f0: 7465 642e 2041 7474 656d 7074 696e 6720  ted. Attempting 
+00001300: 746f 2070 6173 7320 6120 6c69 7374 206f  to pass a list o
+00001310: 6620 7374 7269 6e67 7320 746f 2074 6865  f strings to the
+00001320: 2060 7375 6266 6965 6c64 7360 0a70 6172   `subfields`.par
+00001330: 616d 6574 6572 2066 6f72 2074 6865 2060  ameter for the `
+00001340: 4669 656c 6460 2063 6f6e 7374 7275 6374  Field` construct
+00001350: 6f72 2077 696c 6c20 7261 6973 6520 6120  or will raise a 
+00001360: 6056 616c 7565 4572 726f 7260 2e20 466f  `ValueError`. Fo
+00001370: 720a 636f 6e76 656e 6965 6e63 6520 7468  r.convenience th
+00001380: 6520 6046 6965 6c64 2e63 6f6e 7665 7274  e `Field.convert
+00001390: 5f6c 6567 6163 795f 7375 6266 6965 6c64  _legacy_subfield
+000013a0: 7360 2063 616e 2062 6520 7573 6564 2074  s` can be used t
+000013b0: 6f20 636f 6e76 6572 7420 610a 6c65 6761  o convert a.lega
+000013c0: 6379 206c 6973 7420 6f66 2073 7472 696e  cy list of strin
+000013d0: 6773 2069 6e74 6f20 6120 6c69 7374 206f  gs into a list o
+000013e0: 6620 6053 7562 6669 656c 6460 732e 2a0a  f `Subfield`s.*.
+000013f0: 0a48 6572 6527 7320 616e 2065 7861 6d70  .Here's an examp
+00001400: 6c65 206f 6620 6372 6561 7469 6e67 2061  le of creating a
+00001410: 2072 6563 6f72 6420 616e 6420 7772 6974   record and writ
+00001420: 696e 6720 6974 206f 7574 2074 6f20 6120  ing it out to a 
+00001430: 6669 6c65 2e0a 0a60 6060 7079 7468 6f6e  file...```python
+00001440: 0a66 726f 6d20 7079 6d61 7263 2069 6d70  .from pymarc imp
+00001450: 6f72 7420 5265 636f 7264 2c20 4669 656c  ort Record, Fiel
+00001460: 642c 2053 7562 6669 656c 640a 0a72 6563  d, Subfield..rec
+00001470: 6f72 6420 3d20 5265 636f 7264 2829 0a72  ord = Record().r
+00001480: 6563 6f72 642e 6164 645f 6669 656c 6428  ecord.add_field(
+00001490: 0a20 2020 2046 6965 6c64 280a 2020 2020  .    Field(.    
+000014a0: 2020 2020 7461 673d 2732 3435 272c 0a20      tag='245',. 
+000014b0: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
+000014c0: 733d 5b27 3027 2c20 2731 275d 2c0a 2020  s=['0', '1'],.  
+000014d0: 2020 2020 2020 7375 6266 6965 6c64 733d        subfields=
+000014e0: 5b0a 2020 2020 2020 2020 2020 2020 5375  [.            Su
+000014f0: 6266 6965 6c64 2863 6f64 653d 2761 272c  bfield(code='a',
+00001500: 2076 616c 7565 3d27 5468 6520 7072 6167   value='The prag
+00001510: 6d61 7469 6320 7072 6f67 7261 6d6d 6572  matic programmer
+00001520: 203a 2027 292c 0a20 2020 2020 2020 2020   : '),.         
+00001530: 2020 2053 7562 6669 656c 6428 636f 6465     Subfield(code
+00001540: 3d27 6227 2c20 7661 6c75 653d 2766 726f  ='b', value='fro
+00001550: 6d20 6a6f 7572 6e65 796d 616e 2074 6f20  m journeyman to 
+00001560: 6d61 7374 6572 202f 2729 2c0a 2020 2020  master /'),.    
+00001570: 2020 2020 2020 2020 5375 6266 6965 6c64          Subfield
+00001580: 2863 6f64 653d 2763 272c 2076 616c 7565  (code='c', value
+00001590: 3d27 416e 6472 6577 2048 756e 742c 2044  ='Andrew Hunt, D
+000015a0: 6176 6964 2054 686f 6d61 732e 2729 0a20  avid Thomas.'). 
+000015b0: 2020 2020 2020 205d 2929 0a77 6974 6820         ])).with 
+000015c0: 6f70 656e 2827 6669 6c65 2e64 6174 272c  open('file.dat',
+000015d0: 2027 7762 2729 2061 7320 6f75 743a 0a20   'wb') as out:. 
+000015e0: 2020 206f 7574 2e77 7269 7465 2872 6563     out.write(rec
+000015f0: 6f72 642e 6173 5f6d 6172 6328 2929 0a60  ord.as_marc()).`
+00001600: 6060 0a0a 546f 2063 6f6e 7665 7274 2066  ``..To convert f
+00001610: 726f 6d20 7468 6520 6f6c 6420 7374 7269  rom the old stri
+00001620: 6e67 206c 6973 7420 746f 2061 206c 6973  ng list to a lis
+00001630: 7420 6f66 2060 5375 6266 6965 6c64 6073  t of `Subfield`s
+00001640: 2c20 7468 6520 602e 636f 6e76 6572 745f  , the `.convert_
+00001650: 6c65 6761 6379 5f73 7562 6669 656c 6473  legacy_subfields
+00001660: 6020 636c 6173 7320 6d65 7468 6f64 0a69  ` class method.i
+00001670: 7320 7072 6f76 6964 6564 206f 6e20 7468  s provided on th
+00001680: 6520 6046 6965 6c64 6020 636c 6173 732e  e `Field` class.
+00001690: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000016a0: 2070 796d 6172 6320 696d 706f 7274 2046   pymarc import F
+000016b0: 6965 6c64 2c20 5375 6266 6965 6c64 0a0a  ield, Subfield..
+000016c0: 6c65 6761 6379 5f66 6965 6c64 733a 206c  legacy_fields: l
+000016d0: 6973 745b 7374 725d 203d 205b 2761 272c  ist[str] = ['a',
+000016e0: 2027 5468 6520 7072 6167 6d61 7469 6320   'The pragmatic 
+000016f0: 7072 6f67 7261 6d6d 6572 203a 2027 2c0a  programmer : ',.
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 2020 2020 2020 2020 2762 272c              'b',
+00001720: 2027 6672 6f6d 206a 6f75 726e 6579 6d61   'from journeyma
+00001730: 6e20 746f 206d 6173 7465 7220 2f27 2c0a  n to master /',.
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 2020 2020 2020 2020 2763 272c              'c',
+00001760: 2027 416e 6472 6577 2048 756e 742c 2044   'Andrew Hunt, D
+00001770: 6176 6964 2054 686f 6d61 7327 5d0a 0a63  avid Thomas']..c
+00001780: 6f64 6564 5f66 6965 6c64 733a 206c 6973  oded_fields: lis
+00001790: 745b 5375 6266 6965 6c64 5d20 3d20 4669  t[Subfield] = Fi
+000017a0: 656c 642e 636f 6e76 6572 745f 6c65 6761  eld.convert_lega
+000017b0: 6379 5f73 7562 6669 656c 6473 286c 6567  cy_subfields(leg
+000017c0: 6163 795f 6669 656c 6473 290a 6060 600a  acy_fields).```.
+000017d0: 0a23 2323 2055 7064 6174 696e 670a 0a55  .### Updating..U
+000017e0: 7064 6174 696e 6720 776f 726b 7320 7468  pdating works th
+000017f0: 6520 7361 6d65 2077 6179 2c20 796f 7520  e same way, you 
+00001800: 7265 6164 2069 7420 696e 2c20 6d6f 6469  read it in, modi
+00001810: 6679 2069 742c 2061 6e64 2074 6865 6e20  fy it, and then 
+00001820: 7772 6974 6520 6974 206f 7574 0a61 6761  write it out.aga
+00001830: 696e 3a0a 0a60 6060 7079 7468 6f6e 0a66  in:..```python.f
+00001840: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
+00001850: 7420 4d41 5243 5265 6164 6572 0a77 6974  t MARCReader.wit
+00001860: 6820 6f70 656e 2827 7465 7374 2f6d 6172  h open('test/mar
+00001870: 632e 6461 7427 2c20 2772 6227 2920 6173  c.dat', 'rb') as
+00001880: 2066 683a 0a20 2020 2072 6561 6465 7220   fh:.    reader 
+00001890: 3d20 4d41 5243 5265 6164 6572 2866 6829  = MARCReader(fh)
+000018a0: 0a20 2020 2072 6563 6f72 6420 3d20 6e65  .    record = ne
+000018b0: 7874 2872 6561 6465 7229 0a20 2020 2072  xt(reader).    r
+000018c0: 6563 6f72 645b 2732 3435 275d 5b27 6127  ecord['245']['a'
+000018d0: 5d20 3d20 2754 6865 205a 6f6d 6269 6520  ] = 'The Zombie 
+000018e0: 5072 6f67 7261 6d6d 6572 203a 2027 0a77  Programmer : '.w
+000018f0: 6974 6820 6f70 656e 2827 6669 6c65 2e64  ith open('file.d
+00001900: 6174 272c 2027 7762 2729 2061 7320 6f75  at', 'wb') as ou
+00001910: 743a 0a20 2020 206f 7574 2e77 7269 7465  t:.    out.write
+00001920: 2872 6563 6f72 642e 6173 5f6d 6172 6328  (record.as_marc(
+00001930: 2929 0a60 6060 0a0a 0a23 2323 204a 534f  )).```...### JSO
+00001940: 4e20 616e 6420 584d 4c0a 0a49 6620 796f  N and XML..If yo
+00001950: 7520 6669 6e64 2079 6f75 7273 656c 6620  u find yourself 
+00001960: 7573 696e 6720 4d41 5243 2064 6174 6120  using MARC data 
+00001970: 6120 6661 6972 2062 6974 2c20 616e 6420  a fair bit, and 
+00001980: 6469 7374 7269 6275 7469 6e67 2069 742c  distributing it,
+00001990: 2079 6f75 206d 6179 0a6d 616b 6520 6f74   you may.make ot
+000019a0: 6865 7220 6465 7665 6c6f 7065 7273 2061  her developers a
+000019b0: 2062 6974 2068 6170 7069 6572 2062 7920   bit happier by 
+000019c0: 7573 696e 6720 7468 6520 4a53 4f4e 206f  using the JSON o
+000019d0: 7220 584d 4c20 7365 7269 616c 697a 6174  r XML serializat
+000019e0: 696f 6e73 2e20 5468 650a 6d61 696e 2062  ions. The.main b
+000019f0: 656e 6566 6974 2074 6f20 7573 696e 6720  enefit to using 
+00001a00: 584d 4c20 6f72 204a 534f 4e20 6973 2074  XML or JSON is t
+00001a10: 6861 7420 7468 6520 5554 4638 2063 6861  hat the UTF8 cha
+00001a20: 7261 6374 6572 2065 6e63 6f64 696e 6720  racter encoding 
+00001a30: 6973 2075 7365 642c 0a72 6174 6865 7220  is used,.rather 
+00001a40: 7468 616e 2074 6865 2066 7275 7374 7261  than the frustra
+00001a50: 7469 6e67 6c79 2061 7263 6861 6963 204d  tingly archaic M
+00001a60: 4152 4338 2065 6e63 6f64 696e 672e 2041  ARC8 encoding. A
+00001a70: 6c73 6f20 7468 6579 2077 696c 6c20 6265  lso they will be
+00001a80: 2061 626c 6520 746f 0a75 7365 2073 7461   able to.use sta
+00001a90: 6e64 6172 6420 4a53 4f4e 2061 6e64 2058  ndard JSON and X
+00001aa0: 4d4c 2072 6561 6469 6e67 2f77 7269 7469  ML reading/writi
+00001ab0: 6e67 2074 6f6f 6c73 2074 6f20 6765 7420  ng tools to get 
+00001ac0: 6174 2074 6865 2064 6174 6120 7468 6579  at the data they
+00001ad0: 2077 616e 740a 696e 7374 6561 6420 6f66   want.instead of
+00001ae0: 2073 6f6d 6520 6372 617a 7920 4d41 5243   some crazy MARC
+00001af0: 2070 726f 6365 7373 696e 6720 6c69 6272   processing libr
+00001b00: 6172 7920 6c69 6b65 2c20 6168 656d 2c20  ary like, ahem, 
+00001b10: 7079 6d61 7263 2e0a 0a2a 2a58 4d4c 2a2a  pymarc...**XML**
+00001b20: 0a0a 546f 2070 6172 7365 2061 2066 696c  ..To parse a fil
+00001b30: 6520 6f66 204d 4152 4358 4d4c 2072 6563  e of MARCXML rec
+00001b40: 6f72 6473 2079 6f75 2063 616e 3a0a 0a60  ords you can:..`
+00001b50: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2070  ``python..from p
+00001b60: 796d 6172 6320 696d 706f 7274 2070 6172  ymarc import par
+00001b70: 7365 5f78 6d6c 5f74 6f5f 6172 7261 790a  se_xml_to_array.
+00001b80: 0a72 6563 6f72 6473 203d 2070 6172 7365  .records = parse
+00001b90: 5f78 6d6c 5f74 6f5f 6172 7261 7928 2774  _xml_to_array('t
+00001ba0: 6573 742f 6261 7463 682e 786d 6c27 290a  est/batch.xml').
+00001bb0: 6060 600a 0a49 6620 796f 7520 6861 7665  ```..If you have
+00001bc0: 2061 206c 6172 6765 2058 4d4c 2066 696c   a large XML fil
+00001bd0: 6520 616e 6420 776f 756c 6420 7261 7468  e and would rath
+00001be0: 6572 206e 6f74 2072 6561 6420 7468 656d  er not read them
+00001bf0: 2061 6c6c 2069 6e74 6f20 6d65 6d6f 7279   all into memory
+00001c00: 2079 6f75 0a63 616e 3a0a 0a60 6060 7079   you.can:..```py
+00001c10: 7468 6f6e 0a0a 6672 6f6d 2070 796d 6172  thon..from pymar
+00001c20: 6320 696d 706f 7274 206d 6170 5f78 6d6c  c import map_xml
+00001c30: 0a0a 6465 6620 7072 696e 745f 7469 746c  ..def print_titl
+00001c40: 6528 7229 3a0a 2020 2020 7072 696e 7428  e(r):.    print(
+00001c50: 722e 7469 746c 6528 2929 0a0a 6d61 705f  r.title())..map_
+00001c60: 786d 6c28 7072 696e 745f 7469 746c 652c  xml(print_title,
+00001c70: 2027 7465 7374 2f62 6174 6368 2e78 6d6c   'test/batch.xml
+00001c80: 2729 0a60 6060 0a0a 416c 736f 2c20 6966  ').```..Also, if
+00001c90: 2079 6f75 2070 7265 6665 7220 796f 7520   you prefer you 
+00001ca0: 6361 6e20 7061 7373 2069 6e20 6120 6669  can pass in a fi
+00001cb0: 6c65 206c 696b 6520 6f62 6a65 6374 2069  le like object i
+00001cc0: 6e20 6164 6469 7469 6f6e 2074 6f20 7468  n addition to th
+00001cd0: 6520 7061 7468 0a74 6f20 626f 7468 202a  e path.to both *
+00001ce0: 6d61 705f 786d 6c2a 2061 6e64 202a 7061  map_xml* and *pa
+00001cf0: 7273 655f 786d 6c5f 746f 5f61 7272 6179  rse_xml_to_array
+00001d00: 2a3a 0a0a 6060 6070 7974 686f 6e0a 6672  *:..```python.fr
+00001d10: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
+00001d20: 2070 6172 7365 5f78 6d6c 5f74 6f5f 6172   parse_xml_to_ar
+00001d30: 7261 790a 0a72 6563 6f72 6473 203d 2070  ray..records = p
+00001d40: 6172 7365 5f78 6d6c 5f74 6f5f 6172 7261  arse_xml_to_arra
+00001d50: 7928 6f70 656e 2827 7465 7374 2f62 6174  y(open('test/bat
+00001d60: 6368 2e78 6d6c 2729 290a 6060 600a 0a2a  ch.xml')).```..*
+00001d70: 2a4a 534f 4e2a 2a0a 0a4a 534f 4e20 7375  *JSON**..JSON su
+00001d80: 7070 6f72 7420 6973 2066 6169 726c 7920  pport is fairly 
+00001d90: 6d69 6e69 6d61 6c20 696e 2074 6861 7420  minimal in that 
+00001da0: 796f 7520 6361 6e20 6361 6c6c 2061 2060  you can call a `
+00001db0: 7079 6d61 7263 2e52 6563 6f72 6460 2773  pymarc.Record`'s
+00001dc0: 0a60 6173 5f6a 736f 6e28 2960 206d 6574  .`as_json()` met
+00001dd0: 686f 6420 746f 2072 6574 7572 6e20 4a53  hod to return JS
+00001de0: 4f4e 2066 6f72 2061 2067 6976 656e 204d  ON for a given M
+00001df0: 4152 4320 5265 636f 7264 3a0a 0a60 6060  ARC Record:..```
+00001e00: 7079 7468 6f6e 0a66 726f 6d20 7079 6d61  python.from pyma
+00001e10: 7263 2069 6d70 6f72 7420 4d41 5243 5265  rc import MARCRe
+00001e20: 6164 6572 0a0a 7769 7468 206f 7065 6e28  ader..with open(
+00001e30: 2774 6573 742f 6f6e 652e 6461 7427 2c27  'test/one.dat','
+00001e40: 7262 2729 2061 7320 6668 3a0a 2020 2020  rb') as fh:.    
+00001e50: 7265 6164 6572 203d 204d 4152 4352 6561  reader = MARCRea
+00001e60: 6465 7228 6668 290a 2020 2020 666f 7220  der(fh).    for 
+00001e70: 7265 636f 7264 2069 6e20 7265 6164 6572  record in reader
+00001e80: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00001e90: 7265 636f 7264 2e61 735f 6a73 6f6e 2869  record.as_json(i
+00001ea0: 6e64 656e 743d 3229 290a 6060 600a 0a60  ndent=2)).```..`
+00001eb0: 6060 6a61 7661 7363 7269 7074 0a7b 0a20  ``javascript.{. 
+00001ec0: 2022 6c65 6164 6572 223a 2022 3031 3036   "leader": "0106
+00001ed0: 3063 616d 2020 3232 3030 3238 3934 6120  0cam  22002894a 
+00001ee0: 3435 3030 222c 0a20 2022 6669 656c 6473  4500",.  "fields
+00001ef0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
+00001f00: 2022 3030 3122 3a20 2231 3137 3738 3530   "001": "1177850
+00001f10: 3422 0a20 2020 207d 2c0a 2020 2020 7b0a  4".    },.    {.
+00001f20: 2020 2020 2020 2230 3130 223a 207b 0a20        "010": {. 
+00001f30: 2020 2020 2020 2022 696e 6431 223a 2022         "ind1": "
+00001f40: 2022 2c0a 2020 2020 2020 2020 2273 7562   ",.        "sub
+00001f50: 6669 656c 6473 223a 205b 0a20 2020 2020  fields": [.     
+00001f60: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001f70: 2020 2022 6122 3a20 2220 2020 3939 3034     "a": "   9904
+00001f80: 3335 3831 2022 0a20 2020 2020 2020 2020  3581 ".         
+00001f90: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
+00001fa0: 2020 2020 2020 2269 6e64 3222 3a20 2220        "ind2": " 
+00001fb0: 220a 2020 2020 2020 7d0a 2020 2020 7d2c  ".      }.    },
+00001fc0: 0a20 2020 207b 0a20 2020 2020 2022 3130  .    {.      "10
+00001fd0: 3022 3a20 7b0a 2020 2020 2020 2020 2269  0": {.        "i
+00001fe0: 6e64 3122 3a20 2231 222c 0a20 2020 2020  nd1": "1",.     
+00001ff0: 2020 2022 7375 6266 6965 6c64 7322 3a20     "subfields": 
+00002000: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
+00002010: 2020 2020 2020 2020 2020 2261 223a 2022            "a": "
+00002020: 4875 6e74 2c20 416e 6472 6577 2c22 0a20  Hunt, Andrew,". 
+00002030: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002040: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002050: 2020 2020 2264 223a 2022 3139 3634 2d22      "d": "1964-"
+00002060: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
+00002070: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00002080: 2269 6e64 3222 3a20 2220 220a 2020 2020  "ind2": " ".    
+00002090: 2020 7d0a 2020 2020 7d2c 0a20 2020 207b    }.    },.    {
+000020a0: 0a20 2020 2020 2022 3234 3522 3a20 7b0a  .      "245": {.
+000020b0: 2020 2020 2020 2020 2269 6e64 3122 3a20          "ind1": 
+000020c0: 2231 222c 0a20 2020 2020 2020 2022 7375  "1",.        "su
+000020d0: 6266 6965 6c64 7322 3a20 5b0a 2020 2020  bfields": [.    
+000020e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000020f0: 2020 2020 2261 223a 2022 5468 6520 7072      "a": "The pr
+00002100: 6167 6d61 7469 6320 7072 6f67 7261 6d6d  agmatic programm
+00002110: 6572 203a 220a 2020 2020 2020 2020 2020  er :".          
+00002120: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
+00002130: 2020 2020 2020 2020 2020 2022 6222 3a20             "b": 
+00002140: 2266 726f 6d20 6a6f 7572 6e65 796d 616e  "from journeyman
+00002150: 2074 6f20 6d61 7374 6572 202f 220a 2020   to master /".  
+00002160: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002170: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002180: 2020 2022 6322 3a20 2241 6e64 7265 7720     "c": "Andrew 
+00002190: 4875 6e74 2c20 4461 7669 6420 5468 6f6d  Hunt, David Thom
+000021a0: 6173 2e22 0a20 2020 2020 2020 2020 207d  as.".          }
+000021b0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+000021c0: 2020 2020 2269 6e64 3222 3a20 2234 220a      "ind2": "4".
+000021d0: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+000021e0: 2020 207b 0a20 2020 2020 2022 3236 3022     {.      "260"
+000021f0: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
+00002200: 3122 3a20 2220 222c 0a20 2020 2020 2020  1": " ",.       
+00002210: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
+00002220: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00002230: 2020 2020 2020 2020 2261 223a 2022 5265          "a": "Re
+00002240: 6164 696e 672c 204d 6173 7320 3a22 0a20  ading, Mass :". 
+00002250: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002260: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002270: 2020 2020 2262 223a 2022 4164 6469 736f      "b": "Addiso
+00002280: 6e2d 5765 736c 6579 2c22 0a20 2020 2020  n-Wesley,".     
+00002290: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000022a0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000022b0: 2263 223a 2022 3230 3030 2e22 0a20 2020  "c": "2000.".   
+000022c0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000022d0: 205d 2c0a 2020 2020 2020 2020 2269 6e64   ],.        "ind
+000022e0: 3222 3a20 2220 220a 2020 2020 2020 7d0a  2": " ".      }.
+000022f0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00002300: 2020 2022 3330 3022 3a20 7b0a 2020 2020     "300": {.    
+00002310: 2020 2020 2269 6e64 3122 3a20 2220 222c      "ind1": " ",
+00002320: 0a20 2020 2020 2020 2022 7375 6266 6965  .        "subfie
+00002330: 6c64 7322 3a20 5b0a 2020 2020 2020 2020  lds": [.        
+00002340: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00002350: 2261 223a 2022 7878 6976 2c20 3332 3120  "a": "xxiv, 321 
+00002360: 702e 203b 220a 2020 2020 2020 2020 2020  p. ;".          
+00002370: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
+00002380: 2020 2020 2020 2020 2020 2022 6322 3a20             "c": 
+00002390: 2232 3420 636d 2e22 0a20 2020 2020 2020  "24 cm.".       
+000023a0: 2020 207d 0a20 2020 2020 2020 205d 2c0a     }.        ],.
+000023b0: 2020 2020 2020 2020 2269 6e64 3222 3a20          "ind2": 
+000023c0: 2220 220a 2020 2020 2020 7d0a 2020 2020  " ".      }.    
+000023d0: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+000023e0: 3530 3422 3a20 7b0a 2020 2020 2020 2020  504": {.        
+000023f0: 2269 6e64 3122 3a20 2220 222c 0a20 2020  "ind1": " ",.   
+00002400: 2020 2020 2022 7375 6266 6965 6c64 7322       "subfields"
+00002410: 3a20 5b0a 2020 2020 2020 2020 2020 7b0a  : [.          {.
+00002420: 2020 2020 2020 2020 2020 2020 2261 223a              "a":
+00002430: 2022 496e 636c 7564 6573 2062 6962 6c69   "Includes bibli
+00002440: 6f67 7261 7068 6963 616c 2072 6566 6572  ographical refer
+00002450: 656e 6365 732e 220a 2020 2020 2020 2020  ences.".        
+00002460: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
+00002470: 2020 2020 2020 2022 696e 6432 223a 2022         "ind2": "
+00002480: 2022 0a20 2020 2020 207d 0a20 2020 207d   ".      }.    }
+00002490: 2c0a 2020 2020 7b0a 2020 2020 2020 2236  ,.    {.      "6
+000024a0: 3530 223a 207b 0a20 2020 2020 2020 2022  50": {.        "
+000024b0: 696e 6431 223a 2022 2022 2c0a 2020 2020  ind1": " ",.    
+000024c0: 2020 2020 2273 7562 6669 656c 6473 223a      "subfields":
+000024d0: 205b 0a20 2020 2020 2020 2020 207b 0a20   [.          {. 
+000024e0: 2020 2020 2020 2020 2020 2022 6122 3a20             "a": 
+000024f0: 2243 6f6d 7075 7465 7220 7072 6f67 7261  "Computer progra
+00002500: 6d6d 696e 672e 220a 2020 2020 2020 2020  mming.".        
+00002510: 2020 7d0a 2020 2020 2020 2020 5d2c 0a20    }.        ],. 
+00002520: 2020 2020 2020 2022 696e 6432 223a 2022         "ind2": "
+00002530: 3022 0a20 2020 2020 207d 0a20 2020 207d  0".      }.    }
+00002540: 2c0a 2020 2020 7b0a 2020 2020 2020 2237  ,.    {.      "7
+00002550: 3030 223a 207b 0a20 2020 2020 2020 2022  00": {.        "
+00002560: 696e 6431 223a 2022 3122 2c0a 2020 2020  ind1": "1",.    
+00002570: 2020 2020 2273 7562 6669 656c 6473 223a      "subfields":
+00002580: 205b 0a20 2020 2020 2020 2020 207b 0a20   [.          {. 
+00002590: 2020 2020 2020 2020 2020 2022 6122 3a20             "a": 
+000025a0: 2254 686f 6d61 732c 2044 6176 6964 2c22  "Thomas, David,"
+000025b0: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
+000025c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000025d0: 2020 2020 2020 2264 223a 2022 3139 3536        "d": "1956
+000025e0: 2d22 0a20 2020 2020 2020 2020 207d 0a20  -".          }. 
+000025f0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00002600: 2020 2269 6e64 3222 3a20 2220 220a 2020    "ind2": " ".  
+00002610: 2020 2020 7d0a 2020 2020 7d0a 2020 5d0a      }.    }.  ].
+00002620: 7d0a 6060 600a 0a49 6620 796f 7520 7761  }.```..If you wa
+00002630: 6e74 2074 6f20 7061 7273 6520 6120 6669  nt to parse a fi
+00002640: 6c65 206f 6620 4d41 5243 4a53 4f4e 2072  le of MARCJSON r
+00002650: 6563 6f72 6473 2079 6f75 2063 616e 3a0a  ecords you can:.
+00002660: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00002670: 7079 6d61 7263 2069 6d70 6f72 7420 7061  pymarc import pa
+00002680: 7273 655f 6a73 6f6e 5f74 6f5f 6172 7261  rse_json_to_arra
+00002690: 790a 0a72 6563 6f72 6473 203d 2070 6172  y..records = par
+000026a0: 7365 5f6a 736f 6e5f 746f 5f61 7272 6179  se_json_to_array
+000026b0: 286f 7065 6e28 2774 6573 742f 6261 7463  (open('test/batc
+000026c0: 682e 6a73 6f6e 2729 290a 0a70 7269 6e74  h.json'))..print
+000026d0: 2872 6563 6f72 6473 5b30 5d29 0a60 6060  (records[0]).```
+000026e0: 0a0a 6060 600a 3d4c 4452 2020 3030 3932  ..```.=LDR  0092
+000026f0: 356e 6a6d 2020 3232 3030 3237 3737 6120  5njm  22002777a 
+00002700: 3435 3030 0a3d 3030 3120 2035 3633 3732  4500.=001  56372
+00002710: 3431 0a3d 3030 3320 2044 4c43 0a3d 3030  41.=003  DLC.=00
+00002720: 3520 2031 3939 3230 3832 3630 3834 3033  5  1992082608403
+00002730: 362e 300a 3d30 3037 2020 7364 7562 756d  6.0.=007  sdubum
+00002740: 656e 6e6d 706c 750a 3d30 3038 2020 3931  ennmplu.=008  91
+00002750: 3039 3236 7331 3935 375c 5c5c 5c6e 7975  0926s1957\\\\nyu
+00002760: 7575 6e5c 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c  uun\\\\\\\\\\\\\
+00002770: 5c65 6e67 5c5c 0a3d 3031 3020 205c 5c24  \eng\\.=010  \\$
+00002780: 6120 2020 3931 3735 3833 3335 0a3d 3032  a   91758335.=02
+00002790: 3820 2030 3024 6131 3235 3924 6241 746c  8  00$a1259$bAtl
+000027a0: 616e 7469 630a 3d30 3430 2020 5c5c 2461  antic.=040  \\$a
+000027b0: 444c 4324 6344 4c43 0a3d 3035 3020 2030  DLC$cDLC.=050  0
+000027c0: 3024 6141 746c 616e 7469 6320 3132 3539  0$aAtlantic 1259
+000027d0: 0a3d 3234 3520 2030 3424 6154 6865 2047  .=245  04$aThe G
+000027e0: 7265 6174 2052 6179 2043 6861 726c 6573  reat Ray Charles
+000027f0: 2468 5b73 6f75 6e64 2072 6563 6f72 6469  $h[sound recordi
+00002800: 6e67 5d2e 0a3d 3236 3020 205c 5c24 614e  ng]..=260  \\$aN
+00002810: 6577 2059 6f72 6b2c 204e 2e59 2e20 3a24  ew York, N.Y. :$
+00002820: 6241 746c 616e 7469 632c 2463 5b31 3935  bAtlantic,$c[195
+00002830: 373f 5d0a 3d33 3030 2020 5c5c 2461 3120  7?].=300  \\$a1 
+00002840: 736f 756e 6420 6469 7363 203a 2462 616e  sound disc :$ban
+00002850: 616c 6f67 2c20 3333 2031 2f33 2072 706d  alog, 33 1/3 rpm
+00002860: 203b 2463 3132 2069 6e2e 0a3d 3531 3120   ;$c12 in..=511 
+00002870: 2030 5c24 6152 6179 2043 6861 726c 6573   0\$aRay Charles
+00002880: 2c20 7069 616e 6f20 2620 6365 6c65 7374  , piano & celest
+00002890: 652e 0a3d 3530 3520 2030 5c24 6154 6865  e..=505  0\$aThe
+000028a0: 2052 6179 202d 2d20 4d79 206d 656c 616e   Ray -- My melan
+000028b0: 6368 6f6c 7920 6261 6279 202d 2d20 426c  choly baby -- Bl
+000028c0: 6163 6b20 636f 6666 6565 202d 2d20 5468  ack coffee -- Th
+000028d0: 6572 6527 7320 6e6f 2079 6f75 202d 2d20  ere's no you -- 
+000028e0: 446f 6f64 6c69 6e27 202d 2d20 5377 6565  Doodlin' -- Swee
+000028f0: 7420 7369 7874 6565 6e20 6261 7273 202d  t sixteen bars -
+00002900: 2d20 4920 7375 7272 656e 6465 7220 6465  - I surrender de
+00002910: 6172 202d 2d20 556e 6465 6369 6465 642e  ar -- Undecided.
+00002920: 0a3d 3530 3020 205c 5c24 6142 7269 6566  .=500  \\$aBrief
+00002930: 2072 6563 6f72 642e 0a3d 3635 3020 205c   record..=650  \
+00002940: 3024 614a 617a 7a24 7931 3935 312d 3139  0$aJazz$y1951-19
+00002950: 3630 2e0a 3d36 3530 2020 5c30 2461 5069  60..=650  \0$aPi
+00002960: 616e 6f20 7769 7468 206a 617a 7a20 656e  ano with jazz en
+00002970: 7365 6d62 6c65 2e0a 3d37 3030 2020 315c  semble..=700  1\
+00002980: 2461 4368 6172 6c65 732c 2052 6179 2c24  $aCharles, Ray,$
+00002990: 6431 3933 302d 2434 7072 660a 6060 600a  d1930-$4prf.```.
+000029a0: 0a53 7570 706f 7274 0a2d 2d2d 2d2d 2d2d  .Support.-------
+000029b0: 0a0a 5468 6520 7079 6d61 7263 2064 6576  ..The pymarc dev
+000029c0: 656c 6f70 6572 7320 656e 636f 7572 6167  elopers encourag
+000029d0: 6520 796f 7520 746f 206a 6f69 6e20 7468  e you to join th
+000029e0: 6520 5b70 796d 6172 6320 476f 6f67 6c65  e [pymarc Google
+000029f0: 0a47 726f 7570 5d28 6874 7470 3a2f 2f67  .Group](http://g
+00002a00: 726f 7570 732e 676f 6f67 6c65 2e63 6f6d  roups.google.com
+00002a10: 2f67 726f 7570 2f70 796d 6172 6329 2069  /group/pymarc) i
+00002a20: 6620 796f 7520 6e65 6564 2068 656c 702e  f you need help.
+00002a30: 2020 416c 736f 2c20 706c 6561 7365 0a66    Also, please.f
+00002a40: 6565 6c20 6672 6565 2074 6f20 7573 6520  eel free to use 
+00002a50: 5b69 7373 7565 2074 7261 636b 696e 675d  [issue tracking]
+00002a60: 2868 7474 7073 3a2f 2f67 6974 6c61 622e  (https://gitlab.
+00002a70: 636f 6d2f 7079 6d61 7263 2f70 796d 6172  com/pymarc/pymar
+00002a80: 632f 6973 7375 6573 2920 6f6e 0a47 6974  c/issues) on.Git
+00002a90: 4c61 6220 746f 2073 7562 6d69 7420 6665  Lab to submit fe
+00002aa0: 6174 7572 6520 7265 7175 6573 7473 206f  ature requests o
+00002ab0: 7220 6275 6720 7265 706f 7274 732e 2049  r bug reports. I
+00002ac0: 6620 796f 7527 7665 2067 6f74 2061 6e20  f you've got an 
+00002ad0: 6974 6368 2074 6f0a 7363 7261 7463 682c  itch to.scratch,
+00002ae0: 2070 6c65 6173 6520 7363 7261 7463 6820   please scratch 
+00002af0: 6974 2c20 616e 6420 7365 6e64 206d 6572  it, and send mer
+00002b00: 6765 2072 6571 7565 7374 7320 6f6e 0a5b  ge requests on.[
+00002b10: 4769 744c 6162 5d28 6874 7470 3a2f 2f67  GitLab](http://g
+00002b20: 6974 6c61 622e 636f 6d2f 7079 6d61 7263  itlab.com/pymarc
+00002b30: 2f70 796d 6172 6329 2e0a 0a49 6620 796f  /pymarc)...If yo
+00002b40: 7520 7374 6172 7420 776f 726b 696e 6720  u start working 
+00002b50: 7769 7468 204d 4152 4320 796f 7520 6d61  with MARC you ma
+00002b60: 7920 6665 656c 206c 696b 6520 796f 7520  y feel like you 
+00002b70: 6e65 6564 206d 6f72 616c 2073 7570 706f  need moral suppo
+00002b80: 7274 0a69 6e20 6164 6469 7469 6f6e 2074  rt.in addition t
+00002b90: 6f20 7465 6368 6e69 6361 6c20 7375 7070  o technical supp
+00002ba0: 6f72 742e 2054 6865 0a5b 2363 6f64 6534  ort. The.[#code4
+00002bb0: 6c69 625d 2869 7263 733a 2f2f 6972 632e  lib](ircs://irc.
+00002bc0: 6c69 6265 7261 2e63 6861 742f 636f 6465  libera.chat/code
+00002bd0: 346c 6962 2920 6368 616e 6e65 6c20 6f6e  4lib) channel on
+00002be0: 205b 4c69 6265 7261 5d28 6874 7470 733a   [Libera](https:
+00002bf0: 2f2f 6c69 6265 7261 2e63 6861 742f 2920  //libera.chat/) 
+00002c00: 6973 2061 2067 6f6f 6420 706c 6163 6520  is a good place 
+00002c10: 666f 7220 626f 7468 2e0a                 for both..
```

### Comparing `pymarc-4.2.2/README.md` & `pymarc-5.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,622 +1,761 @@
-00000000: 6060 600a 5f7c 5f7c 5f7c 2020 2020 5f7c  ```._|_|_|    _|
-00000010: 2020 2020 5f7c 2020 5f7c 5f7c 5f7c 2020      _|  _|_|_|  
-00000020: 5f7c 5f7c 2020 2020 2020 5f7c 5f7c 5f7c  _|_|      _|_|_|
-00000030: 2020 5f7c 2020 5f7c 5f7c 2020 2020 5f7c    _|  _|_|    _|
-00000040: 5f7c 5f7c 0a5f 7c20 2020 205f 7c20 205f  _|_|._|    _|  _
-00000050: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
-00000060: 7c20 2020 205f 7c20 205f 7c20 2020 205f  |    _|  _|    _
-00000070: 7c20 205f 7c5f 7c20 2020 2020 205f 7c0a  |  _|_|      _|.
-00000080: 5f7c 2020 2020 5f7c 2020 5f7c 2020 2020  _|    _|  _|    
-00000090: 5f7c 2020 5f7c 2020 2020 5f7c 2020 2020  _|  _|    _|    
-000000a0: 5f7c 2020 5f7c 2020 2020 5f7c 2020 5f7c  _|  _|    _|  _|
-000000b0: 2020 2020 2020 2020 5f7c 0a5f 7c5f 7c5f          _|._|_|_
-000000c0: 7c20 2020 2020 205f 7c5f 7c5f 7c20 205f  |      _|_|_|  _
-000000d0: 7c20 2020 205f 7c20 2020 205f 7c20 2020  |    _|    _|   
-000000e0: 205f 7c5f 7c5f 7c20 205f 7c20 2020 2020   _|_|_|  _|     
-000000f0: 2020 2020 205f 7c5f 7c5f 7c0a 5f7c 2020       _|_|_|._|  
-00000100: 2020 2020 2020 2020 2020 2020 5f7c 0a5f              _|._
-00000110: 7c20 2020 2020 2020 2020 205f 7c5f 7c0a  |          _|_|.
-00000120: 6060 600a 0a5b 215b 4275 696c 6420 7374  ```..[![Build st
-00000130: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
-00000140: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
-00000150: 7079 6d61 7263 2f62 6164 6765 732f 6d61  pymarc/badges/ma
-00000160: 696e 2f70 6970 656c 696e 652e 7376 6729  in/pipeline.svg)
-00000170: 5d28 6874 7470 733a 2f2f 6769 746c 6162  ](https://gitlab
-00000180: 2e63 6f6d 2f70 796d 6172 632f 7079 6d61  .com/pymarc/pyma
-00000190: 7263 2f2d 2f63 6f6d 6d69 7473 2f6d 6169  rc/-/commits/mai
-000001a0: 6e29 0a0a 7079 6d61 7263 2069 7320 6120  n)..pymarc is a 
-000001b0: 7079 7468 6f6e 206c 6962 7261 7279 2066  python library f
-000001c0: 6f72 2077 6f72 6b69 6e67 2077 6974 6820  or working with 
-000001d0: 6269 626c 696f 6772 6170 6869 6320 6461  bibliographic da
-000001e0: 7461 2065 6e63 6f64 6564 2069 6e0a 5b4d  ta encoded in.[M
-000001f0: 4152 4332 315d 2868 7474 7073 3a2f 2f65  ARC21](https://e
-00000200: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00000210: 7769 6b69 2f4d 4152 435f 7374 616e 6461  wiki/MARC_standa
-00000220: 7264 7329 2e20 4974 2070 726f 7669 6465  rds). It provide
-00000230: 7320 616e 2041 5049 2066 6f72 0a72 6561  s an API for.rea
-00000240: 6469 6e67 2c20 7772 6974 696e 6720 616e  ding, writing an
-00000250: 6420 6d6f 6469 6679 696e 6720 4d41 5243  d modifying MARC
-00000260: 2072 6563 6f72 6473 2e20 4974 2077 6173   records. It was
-00000270: 206d 6f73 746c 7920 6465 7369 676e 6564   mostly designed
-00000280: 2074 6f20 6265 2061 6e0a 656d 6572 6765   to be an.emerge
-00000290: 6e63 7920 656a 6563 7420 7365 6174 2c20  ncy eject seat, 
-000002a0: 666f 7220 6765 7474 696e 6720 796f 7572  for getting your
-000002b0: 2064 6174 6120 6173 7365 7473 206f 7574   data assets out
-000002c0: 206f 6620 4d41 5243 2061 6e64 2069 6e74   of MARC and int
-000002d0: 6f20 736f 6d65 0a6b 696e 6420 6f66 2073  o some.kind of s
-000002e0: 616e 6572 2072 6570 7265 7365 6e74 6174  aner representat
-000002f0: 696f 6e2e 2048 6f77 6576 6572 206f 7665  ion. However ove
-00000300: 7220 7468 6520 7965 6172 7320 6974 2068  r the years it h
-00000310: 6173 2062 6565 6e20 7573 6564 2074 6f20  as been used to 
-00000320: 6372 6561 7465 0a61 6e64 206d 6f64 6966  create.and modif
-00000330: 7920 4d41 5243 2072 6563 6f72 6473 2c20  y MARC records, 
-00000340: 7369 6e63 6520 6465 7370 6974 6520 5b72  since despite [r
-00000350: 6570 6561 7465 640a 6361 6c6c 735d 2868  epeated.calls](h
-00000360: 7474 7073 3a2f 2f77 6562 2e61 7263 6869  ttps://web.archi
-00000370: 7665 2e6f 7267 2f77 6562 2f32 3031 3730  ve.org/web/20170
-00000380: 3733 3131 3633 3031 392f 6874 7470 3a2f  731163019/http:/
-00000390: 2f77 7777 2e6d 6172 632d 6d75 7374 2d64  /www.marc-must-d
-000003a0: 6965 2e69 6e66 6f2f 696e 6465 782e 7068  ie.info/index.ph
-000003b0: 702f 4d61 696e 5f50 6167 6529 0a66 6f72  p/Main_Page).for
-000003c0: 2069 7420 746f 2064 6965 2061 7320 6120   it to die as a 
-000003d0: 666f 726d 6174 2c20 4d41 5243 2073 6565  format, MARC see
-000003e0: 6d73 2074 6f20 6265 206c 6976 696e 6720  ms to be living 
-000003f0: 7175 6974 6520 6861 7070 696c 7920 6173  quite happily as
-00000400: 2061 207a 6f6d 6269 652e 0a0a 4265 6c6f   a zombie...Belo
-00000410: 7720 6172 6520 736f 6d65 2063 6f6d 6d6f  w are some commo
-00000420: 6e20 6578 616d 706c 6573 206f 6620 686f  n examples of ho
-00000430: 7720 796f 7520 6d69 6768 7420 7761 6e74  w you might want
-00000440: 2074 6f20 7573 6520 7079 6d61 7263 2e20   to use pymarc. 
-00000450: 4966 0a79 6f75 2072 756e 2061 6372 6f73  If.you run acros
-00000460: 7320 616e 2065 7861 6d70 6c65 2074 6861  s an example tha
-00000470: 7420 796f 7520 7468 696e 6b20 7368 6f75  t you think shou
-00000480: 6c64 2062 6520 6865 7265 2070 6c65 6173  ld be here pleas
-00000490: 6520 7365 6e64 2061 0a70 756c 6c20 7265  e send a.pull re
-000004a0: 7175 6573 742e 0a0a 596f 7520 6361 6e20  quest...You can 
-000004b0: 7265 6164 2070 796d 6172 6320 646f 6375  read pymarc docu
-000004c0: 6d65 6e74 6174 696f 6e20 5b68 6572 655d  mentation [here]
-000004d0: 2868 7474 7073 3a2f 2f70 796d 6172 632e  (https://pymarc.
-000004e0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000004f0: 6e2f 6c61 7465 7374 2f29 2e0a 0a23 2323  n/latest/)...###
-00000500: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a59   Installation..Y
-00000510: 6f75 276c 6c20 7072 6f62 6162 6c79 206a  ou'll probably j
-00000520: 7573 7420 7761 6e74 2074 6f20 7573 6520  ust want to use 
-00000530: 7069 7020 746f 2069 6e73 7461 6c6c 2070  pip to install p
-00000540: 796d 6172 633a 0a0a 2020 2020 7069 7020  ymarc:..    pip 
-00000550: 696e 7374 616c 6c20 7079 6d61 7263 0a0a  install pymarc..
-00000560: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
-00000570: 2064 6f77 6e6c 6f61 6420 616e 6420 696e   download and in
-00000580: 7374 616c 6c20 7468 6520 6c61 7465 7374  stall the latest
-00000590: 2073 6f75 7263 6520 796f 7527 6c6c 206e   source you'll n
-000005a0: 6565 6420 6769 743a 0a0a 2020 2020 6769  eed git:..    gi
-000005b0: 7420 636c 6f6e 6520 6769 743a 2f2f 6769  t clone git://gi
-000005c0: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
-000005d0: 7079 6d61 7263 2e67 6974 0a0a 596f 7527  pymarc.git..You'
-000005e0: 6c6c 2061 6c73 6f20 6e65 6564 205b 7365  ll also need [se
-000005f0: 7475 7074 6f6f 6c73 5d28 6874 7470 733a  tuptools](https:
-00000600: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000610: 672f 7079 7069 2f73 6574 7570 746f 6f6c  g/pypi/setuptool
-00000620: 7323 696e 7374 616c 6c61 7469 6f6e 2d69  s#installation-i
-00000630: 6e73 7472 7563 7469 6f6e 7329 2e20 4f6e  nstructions). On
-00000640: 6365 2079 6f75 2068 6176 6520 7468 6520  ce you have the 
-00000650: 736f 7572 6365 2061 6e64 2073 6574 7570  source and setup
-00000660: 746f 6f6c 7320 7275 6e20 7468 6520 7079  tools run the py
-00000670: 6d61 7263 2074 6573 740a 7375 6974 6520  marc test.suite 
-00000680: 746f 206d 616b 6520 7375 7265 2074 6869  to make sure thi
-00000690: 6e67 7320 6172 6520 696e 206f 7264 6572  ngs are in order
-000006a0: 2077 6974 6820 7468 6520 6469 7374 7269   with the distri
-000006b0: 6275 7469 6f6e 3a0a 0a20 2020 2070 7974  bution:..    pyt
-000006c0: 686f 6e20 7365 7475 702e 7079 2074 6573  hon setup.py tes
-000006d0: 740a 0a41 6e64 2074 6865 6e20 696e 7374  t..And then inst
-000006e0: 616c 6c3a 0a0a 2020 2020 7079 7468 6f6e  all:..    python
-000006f0: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
-00000700: 6c0a 0a23 2323 2052 6561 6469 6e67 0a0a  l..### Reading..
-00000710: 4d6f 7374 206f 6674 656e 2079 6f75 2077  Most often you w
-00000720: 696c 6c20 6861 7665 2073 6f6d 6520 4d41  ill have some MA
-00000730: 5243 2064 6174 6120 616e 6420 7769 6c6c  RC data and will
-00000740: 2077 616e 7420 746f 2065 7874 7261 6374   want to extract
-00000750: 2064 6174 610a 6672 6f6d 2069 742e 2048   data.from it. H
-00000760: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
-00000770: 206f 6620 7265 6164 696e 6720 6120 6261   of reading a ba
-00000780: 7463 6820 6f66 2072 6563 6f72 6473 2061  tch of records a
-00000790: 6e64 2070 7269 6e74 696e 6720 6f75 740a  nd printing out.
-000007a0: 7468 6520 7469 746c 652e 2049 6620 796f  the title. If yo
-000007b0: 7520 6172 6520 6375 7269 6f75 7320 7468  u are curious th
-000007c0: 6973 2065 7861 6d70 6c65 2075 7365 7320  is example uses 
-000007d0: 7468 6520 6261 7463 6820 6669 6c65 0a61  the batch file.a
-000007e0: 7661 696c 6162 6c65 2068 6572 6520 696e  vailable here in
-000007f0: 2070 796d 6172 6320 7265 706f 7369 746f   pymarc reposito
-00000800: 7279 3a0a 0a60 6060 7079 7468 6f6e 0a66  ry:..```python.f
-00000810: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
-00000820: 7420 4d41 5243 5265 6164 6572 0a77 6974  t MARCReader.wit
-00000830: 6820 6f70 656e 2827 7465 7374 2f6d 6172  h open('test/mar
-00000840: 632e 6461 7427 2c20 2772 6227 2920 6173  c.dat', 'rb') as
-00000850: 2066 683a 0a20 2020 2072 6561 6465 7220   fh:.    reader 
-00000860: 3d20 4d41 5243 5265 6164 6572 2866 6829  = MARCReader(fh)
-00000870: 0a20 2020 2066 6f72 2072 6563 6f72 6420  .    for record 
-00000880: 696e 2072 6561 6465 723a 0a20 2020 2020  in reader:.     
-00000890: 2020 2070 7269 6e74 2872 6563 6f72 642e     print(record.
-000008a0: 7469 746c 6528 2929 0a60 6060 0a60 6060  title()).```.```
-000008b0: 0a54 6865 2070 7261 676d 6174 6963 2070  .The pragmatic p
-000008c0: 726f 6772 616d 6d65 7220 3a20 6672 6f6d  rogrammer : from
-000008d0: 206a 6f75 726e 6579 6d61 6e20 746f 206d   journeyman to m
-000008e0: 6173 7465 7220 2f0a 5072 6f67 7261 6d6d  aster /.Programm
-000008f0: 696e 6720 5079 7468 6f6e 202f 0a4c 6561  ing Python /.Lea
-00000900: 726e 696e 6720 5079 7468 6f6e 202f 0a50  rning Python /.P
-00000910: 7974 686f 6e20 636f 6f6b 626f 6f6b 202f  ython cookbook /
-00000920: 0a50 7974 686f 6e20 7072 6f67 7261 6d6d  .Python programm
-00000930: 696e 6720 666f 7220 7468 6520 6162 736f  ing for the abso
-00000940: 6c75 7465 2062 6567 696e 6e65 7220 2f0a  lute beginner /.
-00000950: 5765 6220 7072 6f67 7261 6d6d 696e 6720  Web programming 
-00000960: 3a20 7465 6368 6e69 7175 6573 2066 6f72  : techniques for
-00000970: 2069 6e74 6567 7261 7469 6e67 2050 7974   integrating Pyt
-00000980: 686f 6e2c 204c 696e 7578 2c20 4170 6163  hon, Linux, Apac
-00000990: 6865 2c20 616e 6420 4d79 5351 4c20 2f0a  he, and MySQL /.
-000009a0: 5079 7468 6f6e 2070 726f 6772 616d 6d69  Python programmi
-000009b0: 6e67 206f 6e20 5769 6e33 3220 2f0a 5079  ng on Win32 /.Py
-000009c0: 7468 6f6e 2070 726f 6772 616d 6d69 6e67  thon programming
-000009d0: 203a 2061 6e20 696e 7472 6f64 7563 7469   : an introducti
-000009e0: 6f6e 2074 6f20 636f 6d70 7574 6572 2073  on to computer s
-000009f0: 6369 656e 6365 202f 0a50 7974 686f 6e20  cience /.Python 
-00000a00: 5765 6220 7072 6f67 7261 6d6d 696e 6720  Web programming 
-00000a10: 2f0a 436f 7265 2070 7974 686f 6e20 7072  /.Core python pr
-00000a20: 6f67 7261 6d6d 696e 6720 2f0a 5079 7468  ogramming /.Pyth
-00000a30: 6f6e 2061 6e64 2054 6b69 6e74 6572 2070  on and Tkinter p
-00000a40: 726f 6772 616d 6d69 6e67 202f 0a47 616d  rogramming /.Gam
-00000a50: 6520 7072 6f67 7261 6d6d 696e 6720 7769  e programming wi
-00000a60: 7468 2050 7974 686f 6e2c 204c 7561 2c20  th Python, Lua, 
-00000a70: 616e 6420 5275 6279 202f 0a50 7974 686f  and Ruby /.Pytho
-00000a80: 6e20 7072 6f67 7261 6d6d 696e 6720 7061  n programming pa
-00000a90: 7474 6572 6e73 202f 0a50 7974 686f 6e20  tterns /.Python 
-00000aa0: 7072 6f67 7261 6d6d 696e 6720 7769 7468  programming with
-00000ab0: 2074 6865 204a 6176 6120 636c 6173 7320   the Java class 
-00000ac0: 6c69 6272 6172 6965 7320 3a20 6120 7475  libraries : a tu
-00000ad0: 746f 7269 616c 2066 6f72 2062 7569 6c64  torial for build
-00000ae0: 696e 6720 5765 620a 616e 6420 456e 7465  ing Web.and Ente
-00000af0: 7270 7269 7365 2061 7070 6c69 6361 7469  rprise applicati
-00000b00: 6f6e 7320 2f0a 4c65 6172 6e20 746f 2070  ons /.Learn to p
-00000b10: 726f 6772 616d 2075 7369 6e67 2050 7974  rogram using Pyt
-00000b20: 686f 6e20 3a20 6120 7475 746f 7269 616c  hon : a tutorial
-00000b30: 2066 6f72 2068 6f62 6279 6973 7473 2c20   for hobbyists, 
-00000b40: 7365 6c66 2d73 7461 7274 6572 732c 2061  self-starters, a
-00000b50: 6e64 2061 6c6c 0a77 686f 2077 616e 7420  nd all.who want 
-00000b60: 746f 206c 6561 726e 2074 6865 2061 7274  to learn the art
-00000b70: 206f 6620 636f 6d70 7574 6572 2070 726f   of computer pro
-00000b80: 6772 616d 6d69 6e67 202f 0a50 726f 6772  gramming /.Progr
-00000b90: 616d 6d69 6e67 2077 6974 6820 5079 7468  amming with Pyth
-00000ba0: 6f6e 202f 0a42 5344 2053 6f63 6b65 7473  on /.BSD Sockets
-00000bb0: 2070 726f 6772 616d 6d69 6e67 2066 726f   programming fro
-00000bc0: 6d20 6120 6d75 6c74 692d 6c61 6e67 7561  m a multi-langua
-00000bd0: 6765 2070 6572 7370 6563 7469 7665 202f  ge perspective /
-00000be0: 0a44 6573 6967 6e20 7061 7474 6572 6e73  .Design patterns
-00000bf0: 203a 2065 6c65 6d65 6e74 7320 6f66 2072   : elements of r
-00000c00: 6575 7361 626c 6520 6f62 6a65 6374 2d6f  eusable object-o
-00000c10: 7269 656e 7465 6420 736f 6674 7761 7265  riented software
-00000c20: 202f 0a49 6e74 726f 6475 6374 696f 6e20   /.Introduction 
-00000c30: 746f 2061 6c67 6f72 6974 686d 7320 2f0a  to algorithms /.
-00000c40: 414e 5349 2043 6f6d 6d6f 6e20 4c69 7370  ANSI Common Lisp
-00000c50: 202f 0a60 6060 0a0a 4120 6070 796d 6172   /.```..A `pymar
-00000c60: 632e 5265 636f 7264 6020 6f62 6a65 6374  c.Record` object
-00000c70: 2068 6173 2061 2066 6577 2068 616e 6479   has a few handy
-00000c80: 206d 6574 686f 6473 206c 696b 6520 6074   methods like `t
-00000c90: 6974 6c65 6020 666f 7220 6765 7474 696e  itle` for gettin
-00000ca0: 6720 6174 0a62 6974 7320 6f66 2061 2062  g at.bits of a b
-00000cb0: 6962 6c69 6f67 7261 7068 6963 2072 6563  ibliographic rec
-00000cc0: 6f72 642c 206f 7468 6572 7320 696e 636c  ord, others incl
-00000cd0: 7564 653a 2060 6175 7468 6f72 602c 2060  ude: `author`, `
-00000ce0: 6973 626e 602c 2060 7375 626a 6563 7473  isbn`, `subjects
-00000cf0: 602c 0a60 6c6f 6361 7469 6f6e 602c 2060  `,.`location`, `
-00000d00: 6e6f 7465 7360 2c20 6070 6879 7369 6361  notes`, `physica
-00000d10: 6c64 6573 6372 6970 7469 6f6e 602c 2060  ldescription`, `
-00000d20: 7075 626c 6973 6865 7260 2c20 6070 7562  publisher`, `pub
-00000d30: 7965 6172 602c 2060 6973 736e 602c 0a60  year`, `issn`,.`
-00000d40: 6973 736e 5f74 6974 6c65 602e 2042 7574  issn_title`. But
-00000d50: 2072 6561 6c6c 792c 2074 6f20 776f 726b   really, to work
-00000d60: 2077 6974 6820 4d41 5243 2064 6174 6120   with MARC data 
-00000d70: 796f 7520 6e65 6564 2074 6f20 756e 6465  you need to unde
-00000d80: 7273 7461 6e64 2074 6865 0a6e 756d 6572  rstand the.numer
-00000d90: 6963 2066 6965 6c64 2074 6167 7320 616e  ic field tags an
-00000da0: 6420 7375 6266 6965 6c64 2063 6f64 6573  d subfield codes
-00000db0: 2074 6861 7420 6172 6520 7573 6564 2074   that are used t
-00000dc0: 6f20 6465 7369 676e 6174 6520 7661 7269  o designate vari
-00000dd0: 6f75 7320 6269 7473 0a6f 6620 696e 666f  ous bits.of info
-00000de0: 726d 6174 696f 6e2e 2054 6865 7265 2069  rmation. There i
-00000df0: 7320 6120 6c6f 7420 6d6f 7265 2068 6964  s a lot more hid
-00000e00: 696e 6720 696e 2061 204d 4152 4320 7265  ing in a MARC re
-00000e10: 636f 7264 2074 6861 6e20 7468 6573 6520  cord than these 
-00000e20: 6d65 7468 6f64 730a 7072 6f76 6964 6520  methods.provide 
-00000e30: 6163 6365 7373 2074 6f2e 2046 6f72 2065  access to. For e
-00000e40: 7861 6d70 6c65 2074 6865 2060 7469 746c  xample the `titl
-00000e50: 6560 206d 6574 686f 6420 6578 7472 6163  e` method extrac
-00000e60: 7473 2074 6865 2069 6e66 6f72 6d61 7469  ts the informati
-00000e70: 6f6e 2066 726f 6d0a 2074 6865 2060 3234  on from. the `24
-00000e80: 3560 2066 6965 6c64 2c20 7375 6266 6965  5` field, subfie
-00000e90: 6c64 7320 6061 6020 616e 6420 6062 602e  lds `a` and `b`.
-00000ea0: 2059 6f75 2063 616e 2061 6363 6573 7320   You can access 
-00000eb0: 6032 3435 6160 206c 696b 6520 736f 3a0a  `245a` like so:.
-00000ec0: 0a60 6060 7079 7468 6f6e 0a70 7269 6e74  .```python.print
-00000ed0: 2872 6563 6f72 645b 2732 3435 275d 5b27  (record['245']['
-00000ee0: 6127 5d29 0a60 6060 0a0a 536f 6d65 2066  a']).```..Some f
-00000ef0: 6965 6c64 7320 6c69 6b65 2073 7562 6a65  ields like subje
-00000f00: 6374 7320 6361 6e20 7265 7065 6174 2e20  cts can repeat. 
-00000f10: 496e 2063 6173 6573 206c 696b 6520 7468  In cases like th
-00000f20: 6174 2079 6f75 2077 696c 6c20 7761 6e74  at you will want
-00000f30: 2074 6f20 7573 650a 6067 6574 5f66 6965   to use.`get_fie
-00000f40: 6c64 7360 2074 6f20 6765 7420 616c 6c20  lds` to get all 
-00000f50: 6f66 2074 6865 6d20 6173 2060 7079 6d61  of them as `pyma
-00000f60: 7263 2e46 6965 6c64 6020 6f62 6a65 6374  rc.Field` object
-00000f70: 732c 2077 6869 6368 2079 6f75 2063 616e  s, which you can
-00000f80: 2074 6865 6e0a 696e 7465 7261 6374 2077   then.interact w
-00000f90: 6974 6820 6675 7274 6865 723a 0a0a 6060  ith further:..``
-00000fa0: 6070 7974 686f 6e0a 666f 7220 6620 696e  `python.for f in
-00000fb0: 2072 6563 6f72 642e 6765 745f 6669 656c   record.get_fiel
-00000fc0: 6473 2827 3635 3027 293a 0a20 2020 2070  ds('650'):.    p
-00000fd0: 7269 6e74 2866 290a 6060 600a 0a49 6620  rint(f).```..If 
-00000fe0: 796f 7520 6172 6520 6e65 7720 746f 204d  you are new to M
-00000ff0: 4152 4320 6669 656c 6473 205b 556e 6465  ARC fields [Unde
-00001000: 7273 7461 6e64 696e 670a 4d41 5243 5d28  rstanding.MARC](
-00001010: 6874 7470 3a2f 2f77 7777 2e6c 6f63 2e67  http://www.loc.g
-00001020: 6f76 2f6d 6172 632f 756d 622f 2920 6973  ov/marc/umb/) is
-00001030: 2061 2070 7265 7474 7920 676f 6f64 2070   a pretty good p
-00001040: 7269 6d65 722c 2061 6e64 2074 6865 205b  rimer, and the [
-00001050: 4d41 5243 2032 310a 466f 726d 6174 735d  MARC 21.Formats]
-00001060: 2868 7474 703a 2f2f 7777 772e 6c6f 632e  (http://www.loc.
-00001070: 676f 762f 6d61 7263 2f6d 6172 6364 6f63  gov/marc/marcdoc
-00001080: 7a2e 6874 6d6c 2920 7061 6765 2061 7420  z.html) page at 
-00001090: 7468 6520 4c69 6272 6172 7920 6f66 2043  the Library of C
-000010a0: 6f6e 6772 6573 7320 6973 2061 2067 6f6f  ongress is a goo
-000010b0: 6420 7265 6665 7265 6e63 6520 6f6e 6365  d reference once
-000010c0: 2079 6f75 2075 6e64 6572 7374 616e 6420   you understand 
-000010d0: 7468 6520 6261 7369 6373 2e0a 0a23 2323  the basics...###
-000010e0: 2057 7269 7469 6e67 0a0a 4865 7265 2773   Writing..Here's
-000010f0: 2061 6e20 6578 616d 706c 6520 6f66 2063   an example of c
-00001100: 7265 6174 696e 6720 6120 7265 636f 7264  reating a record
-00001110: 2061 6e64 2077 7269 7469 6e67 2069 7420   and writing it 
-00001120: 6f75 7420 746f 2061 2066 696c 652e 0a0a  out to a file...
-00001130: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
-00001140: 796d 6172 6320 696d 706f 7274 2052 6563  ymarc import Rec
-00001150: 6f72 642c 2046 6965 6c64 0a72 6563 6f72  ord, Field.recor
-00001160: 6420 3d20 5265 636f 7264 2829 0a72 6563  d = Record().rec
-00001170: 6f72 642e 6164 645f 6669 656c 6428 0a20  ord.add_field(. 
-00001180: 2020 2046 6965 6c64 280a 2020 2020 2020     Field(.      
-00001190: 2020 7461 6720 3d20 2732 3435 272c 0a20    tag = '245',. 
-000011a0: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
-000011b0: 7320 3d20 5b27 3027 2c27 3127 5d2c 0a20  s = ['0','1'],. 
-000011c0: 2020 2020 2020 2073 7562 6669 656c 6473         subfields
-000011d0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-000011e0: 2027 6127 2c20 2754 6865 2070 7261 676d   'a', 'The pragm
-000011f0: 6174 6963 2070 726f 6772 616d 6d65 7220  atic programmer 
-00001200: 3a20 272c 0a20 2020 2020 2020 2020 2020  : ',.           
-00001210: 2027 6227 2c20 2766 726f 6d20 6a6f 7572   'b', 'from jour
-00001220: 6e65 796d 616e 2074 6f20 6d61 7374 6572  neyman to master
-00001230: 202f 272c 0a20 2020 2020 2020 2020 2020   /',.           
-00001240: 2027 6327 2c20 2741 6e64 7265 7720 4875   'c', 'Andrew Hu
-00001250: 6e74 2c20 4461 7669 6420 5468 6f6d 6173  nt, David Thomas
-00001260: 2e27 0a20 2020 2020 2020 205d 2929 0a77  .'.        ])).w
-00001270: 6974 6820 6f70 656e 2827 6669 6c65 2e64  ith open('file.d
-00001280: 6174 272c 2027 7762 2729 2061 7320 6f75  at', 'wb') as ou
-00001290: 743a 0a20 2020 206f 7574 2e77 7269 7465  t:.    out.write
-000012a0: 2872 6563 6f72 642e 6173 5f6d 6172 6328  (record.as_marc(
-000012b0: 2929 0a60 6060 0a0a 2323 2320 5570 6461  )).```..### Upda
-000012c0: 7469 6e67 0a0a 5570 6461 7469 6e67 2077  ting..Updating w
-000012d0: 6f72 6b73 2074 6865 2073 616d 6520 7761  orks the same wa
-000012e0: 792c 2079 6f75 2072 6561 6420 6974 2069  y, you read it i
-000012f0: 6e2c 206d 6f64 6966 7920 6974 2c20 616e  n, modify it, an
-00001300: 6420 7468 656e 2077 7269 7465 2069 7420  d then write it 
-00001310: 6f75 740a 6167 6169 6e3a 0a0a 6060 6070  out.again:..```p
-00001320: 7974 686f 6e0a 6672 6f6d 2070 796d 6172  ython.from pymar
-00001330: 6320 696d 706f 7274 204d 4152 4352 6561  c import MARCRea
-00001340: 6465 720a 7769 7468 206f 7065 6e28 2774  der.with open('t
-00001350: 6573 742f 6d61 7263 2e64 6174 272c 2027  est/marc.dat', '
-00001360: 7262 2729 2061 7320 6668 3a0a 2020 2020  rb') as fh:.    
-00001370: 7265 6164 6572 203d 204d 4152 4352 6561  reader = MARCRea
-00001380: 6465 7228 6668 290a 2020 2020 7265 636f  der(fh).    reco
-00001390: 7264 203d 206e 6578 7428 7265 6164 6572  rd = next(reader
-000013a0: 290a 2020 2020 7265 636f 7264 5b27 3234  ).    record['24
-000013b0: 3527 5d5b 2761 275d 203d 2027 5468 6520  5']['a'] = 'The 
-000013c0: 5a6f 6d62 6965 2050 726f 6772 616d 6d65  Zombie Programme
-000013d0: 7227 0a77 6974 6820 6f70 656e 2827 6669  r'.with open('fi
-000013e0: 6c65 2e64 6174 272c 2027 7762 2729 2061  le.dat', 'wb') a
-000013f0: 7320 6f75 743a 0a20 2020 206f 7574 2e77  s out:.    out.w
-00001400: 7269 7465 2872 6563 6f72 642e 6173 5f6d  rite(record.as_m
-00001410: 6172 6328 2929 0a60 6060 0a0a 0a23 2323  arc()).```...###
-00001420: 204a 534f 4e20 616e 6420 584d 4c0a 0a49   JSON and XML..I
-00001430: 6620 796f 7520 6669 6e64 2079 6f75 7273  f you find yours
-00001440: 656c 6620 7573 696e 6720 4d41 5243 2064  elf using MARC d
-00001450: 6174 6120 6120 6661 6972 2062 6974 2c20  ata a fair bit, 
-00001460: 616e 6420 6469 7374 7269 6275 7469 6e67  and distributing
-00001470: 2069 742c 2079 6f75 206d 6179 0a6d 616b   it, you may.mak
-00001480: 6520 6f74 6865 7220 6465 7665 6c6f 7065  e other develope
-00001490: 7273 2061 2062 6974 2068 6170 7069 6572  rs a bit happier
-000014a0: 2062 7920 7573 696e 6720 7468 6520 4a53   by using the JS
-000014b0: 4f4e 206f 7220 584d 4c20 7365 7269 616c  ON or XML serial
-000014c0: 697a 6174 696f 6e73 2e20 5468 650a 6d61  izations. The.ma
-000014d0: 696e 2062 656e 6566 6974 2074 6f20 7573  in benefit to us
-000014e0: 696e 6720 584d 4c20 6f72 204a 534f 4e20  ing XML or JSON 
-000014f0: 6973 2074 6861 7420 7468 6520 5554 4638  is that the UTF8
-00001500: 2063 6861 7261 6374 6572 2065 6e63 6f64   character encod
-00001510: 696e 6720 6973 2075 7365 642c 0a72 6174  ing is used,.rat
-00001520: 6865 7220 7468 616e 2074 6865 2066 7275  her than the fru
-00001530: 7374 7261 7469 6e67 6c79 2061 7263 6861  stratingly archa
-00001540: 6963 204d 4152 4338 2065 6e63 6f64 696e  ic MARC8 encodin
-00001550: 672e 2041 6c73 6f20 7468 6579 2077 696c  g. Also they wil
-00001560: 6c20 6265 2061 626c 6520 746f 0a75 7365  l be able to.use
-00001570: 2073 7461 6e64 6172 6420 4a53 4f4e 2061   standard JSON a
-00001580: 6e64 2058 4d4c 2072 6561 6469 6e67 2f77  nd XML reading/w
-00001590: 7269 7469 6e67 2074 6f6f 6c73 2074 6f20  riting tools to 
-000015a0: 6765 7420 6174 2074 6865 2064 6174 6120  get at the data 
-000015b0: 7468 6579 2077 616e 740a 696e 7374 6561  they want.instea
-000015c0: 6420 6f66 2073 6f6d 6520 6372 617a 7920  d of some crazy 
-000015d0: 4d41 5243 2070 726f 6365 7373 696e 6720  MARC processing 
-000015e0: 6c69 6272 6172 7920 6c69 6b65 2c20 6168  library like, ah
-000015f0: 656d 2c20 7079 6d61 7263 2e0a 0a2a 2a58  em, pymarc...**X
-00001600: 4d4c 2a2a 0a0a 546f 2070 6172 7365 2061  ML**..To parse a
-00001610: 2066 696c 6520 6f66 204d 4152 4358 4d4c   file of MARCXML
-00001620: 2072 6563 6f72 6473 2079 6f75 2063 616e   records you can
-00001630: 3a0a 0a60 6060 7079 7468 6f6e 0a0a 6672  :..```python..fr
-00001640: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
-00001650: 2070 6172 7365 5f78 6d6c 5f74 6f5f 6172   parse_xml_to_ar
-00001660: 7261 790a 0a72 6563 6f72 6473 203d 2070  ray..records = p
-00001670: 6172 7365 5f78 6d6c 5f74 6f5f 6172 7261  arse_xml_to_arra
-00001680: 7928 2774 6573 742f 6261 7463 682e 786d  y('test/batch.xm
-00001690: 6c27 290a 6060 600a 0a49 6620 796f 7520  l').```..If you 
-000016a0: 6861 7665 2061 206c 6172 6765 2058 4d4c  have a large XML
-000016b0: 2066 696c 6520 616e 6420 776f 756c 6420   file and would 
-000016c0: 7261 7468 6572 206e 6f74 2072 6561 6420  rather not read 
-000016d0: 7468 656d 2061 6c6c 2069 6e74 6f20 6d65  them all into me
-000016e0: 6d6f 7279 2079 6f75 0a63 616e 3a0a 0a60  mory you.can:..`
-000016f0: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2070  ``python..from p
-00001700: 796d 6172 6320 696d 706f 7274 206d 6170  ymarc import map
-00001710: 5f78 6d6c 0a0a 6465 6620 7072 696e 745f  _xml..def print_
-00001720: 7469 746c 6528 7229 3a0a 2020 2020 7072  title(r):.    pr
-00001730: 696e 7428 722e 7469 746c 6528 2929 0a0a  int(r.title())..
-00001740: 6d61 705f 786d 6c28 7072 696e 745f 7469  map_xml(print_ti
-00001750: 746c 652c 2027 7465 7374 2f62 6174 6368  tle, 'test/batch
-00001760: 2e78 6d6c 2729 0a60 6060 0a0a 416c 736f  .xml').```..Also
-00001770: 2c20 6966 2079 6f75 2070 7265 6665 7220  , if you prefer 
-00001780: 796f 7520 6361 6e20 7061 7373 2069 6e20  you can pass in 
-00001790: 6120 6669 6c65 206c 696b 6520 6f62 6a65  a file like obje
-000017a0: 6374 2069 6e20 6164 6469 7469 6f6e 2074  ct in addition t
-000017b0: 6f20 7468 6520 7061 7468 0a74 6f20 626f  o the path.to bo
-000017c0: 7468 202a 6d61 705f 786d 6c2a 2061 6e64  th *map_xml* and
-000017d0: 202a 7061 7273 655f 786d 6c5f 746f 5f61   *parse_xml_to_a
-000017e0: 7272 6179 2a3a 0a0a 6060 6070 7974 686f  rray*:..```pytho
-000017f0: 6e0a 7265 636f 7264 7320 3d20 7061 7273  n.records = pars
-00001800: 655f 786d 6c5f 746f 5f61 7272 6179 286f  e_xml_to_array(o
-00001810: 7065 6e28 2774 6573 742f 6261 7463 682e  pen('test/batch.
-00001820: 786d 6c27 2929 0a60 6060 0a0a 2a2a 4a53  xml')).```..**JS
-00001830: 4f4e 2a2a 0a0a 4a53 4f4e 2073 7570 706f  ON**..JSON suppo
-00001840: 7274 2069 7320 6661 6972 6c79 206d 696e  rt is fairly min
-00001850: 696d 616c 2069 6e20 7468 6174 2079 6f75  imal in that you
-00001860: 2063 616e 2063 616c 6c20 6120 6070 796d   can call a `pym
-00001870: 6172 632e 5265 636f 7264 6027 730a 6061  arc.Record`'s.`a
-00001880: 735f 6a73 6f6e 2829 6020 6d65 7468 6f64  s_json()` method
-00001890: 2074 6f20 7265 7475 726e 204a 534f 4e20   to return JSON 
-000018a0: 666f 7220 6120 6769 7665 6e20 4d41 5243  for a given MARC
-000018b0: 2052 6563 6f72 643a 0a0a 6060 6070 7974   Record:..```pyt
-000018c0: 686f 6e0a 6672 6f6d 2070 796d 6172 6320  hon.from pymarc 
-000018d0: 696d 706f 7274 204d 4152 4352 6561 6465  import MARCReade
-000018e0: 720a 0a77 6974 6820 6f70 656e 2827 7465  r..with open('te
-000018f0: 7374 2f6f 6e65 2e64 6174 272c 2772 6227  st/one.dat','rb'
-00001900: 2920 6173 2066 683a 0a20 2020 2072 6561  ) as fh:.    rea
-00001910: 6465 7220 3d20 4d41 5243 5265 6164 6572  der = MARCReader
-00001920: 2866 6829 0a20 2020 2066 6f72 2072 6563  (fh).    for rec
-00001930: 6f72 6420 696e 2072 6561 6465 723a 0a20  ord in reader:. 
-00001940: 2020 2020 2020 2070 7269 6e74 2872 6563         print(rec
-00001950: 6f72 642e 6173 5f6a 736f 6e28 696e 6465  ord.as_json(inde
-00001960: 6e74 3d32 2929 0a60 6060 0a0a 6060 606a  nt=2)).```..```j
-00001970: 6176 6173 6372 6970 740a 7b0a 2020 226c  avascript.{.  "l
-00001980: 6561 6465 7222 3a20 2230 3130 3630 6361  eader": "01060ca
-00001990: 6d20 2032 3230 3032 3839 3461 2034 3530  m  22002894a 450
-000019a0: 3022 2c0a 2020 2266 6965 6c64 7322 3a20  0",.  "fields": 
-000019b0: 5b0a 2020 2020 7b0a 2020 2020 2020 2230  [.    {.      "0
-000019c0: 3031 223a 2022 3131 3737 3835 3034 220a  01": "11778504".
-000019d0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-000019e0: 2020 2022 3031 3022 3a20 7b0a 2020 2020     "010": {.    
-000019f0: 2020 2020 2269 6e64 3122 3a20 2220 222c      "ind1": " ",
-00001a00: 0a20 2020 2020 2020 2022 7375 6266 6965  .        "subfie
-00001a10: 6c64 7322 3a20 5b0a 2020 2020 2020 2020  lds": [.        
-00001a20: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001a30: 2261 223a 2022 2020 2039 3930 3433 3538  "a": "   9904358
-00001a40: 3120 220a 2020 2020 2020 2020 2020 7d0a  1 ".          }.
-00001a50: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00001a60: 2020 2022 696e 6432 223a 2022 2022 0a20     "ind2": " ". 
-00001a70: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-00001a80: 2020 7b0a 2020 2020 2020 2231 3030 223a    {.      "100":
-00001a90: 207b 0a20 2020 2020 2020 2022 696e 6431   {.        "ind1
-00001aa0: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
-00001ab0: 2273 7562 6669 656c 6473 223a 205b 0a20  "subfields": [. 
-00001ac0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00001ad0: 2020 2020 2020 2022 6122 3a20 2248 756e         "a": "Hun
-00001ae0: 742c 2041 6e64 7265 772c 220a 2020 2020  t, Andrew,".    
-00001af0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001b00: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001b10: 2022 6422 3a20 2231 3936 342d 220a 2020   "d": "1964-".  
-00001b20: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001b30: 2020 5d2c 0a20 2020 2020 2020 2022 696e    ],.        "in
-00001b40: 6432 223a 2022 2022 0a20 2020 2020 207d  d2": " ".      }
-00001b50: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-00001b60: 2020 2020 2232 3435 223a 207b 0a20 2020      "245": {.   
-00001b70: 2020 2020 2022 696e 6431 223a 2022 3122       "ind1": "1"
-00001b80: 2c0a 2020 2020 2020 2020 2273 7562 6669  ,.        "subfi
-00001b90: 656c 6473 223a 205b 0a20 2020 2020 2020  elds": [.       
-00001ba0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001bb0: 2022 6122 3a20 2254 6865 2070 7261 676d   "a": "The pragm
-00001bc0: 6174 6963 2070 726f 6772 616d 6d65 7220  atic programmer 
-00001bd0: 3a22 0a20 2020 2020 2020 2020 207d 2c0a  :".          },.
-00001be0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00001bf0: 2020 2020 2020 2020 2262 223a 2022 6672          "b": "fr
-00001c00: 6f6d 206a 6f75 726e 6579 6d61 6e20 746f  om journeyman to
-00001c10: 206d 6173 7465 7220 2f22 0a20 2020 2020   master /".     
-00001c20: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001c30: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001c40: 2263 223a 2022 416e 6472 6577 2048 756e  "c": "Andrew Hun
-00001c50: 742c 2044 6176 6964 2054 686f 6d61 732e  t, David Thomas.
-00001c60: 220a 2020 2020 2020 2020 2020 7d0a 2020  ".          }.  
-00001c70: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00001c80: 2022 696e 6432 223a 2022 3422 0a20 2020   "ind2": "4".   
-00001c90: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
-00001ca0: 7b0a 2020 2020 2020 2232 3630 223a 207b  {.      "260": {
-00001cb0: 0a20 2020 2020 2020 2022 696e 6431 223a  .        "ind1":
-00001cc0: 2022 2022 2c0a 2020 2020 2020 2020 2273   " ",.        "s
-00001cd0: 7562 6669 656c 6473 223a 205b 0a20 2020  ubfields": [.   
-00001ce0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00001cf0: 2020 2020 2022 6122 3a20 2252 6561 6469       "a": "Readi
-00001d00: 6e67 2c20 4d61 7373 203a 220a 2020 2020  ng, Mass :".    
-00001d10: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001d20: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00001d30: 2022 6222 3a20 2241 6464 6973 6f6e 2d57   "b": "Addison-W
-00001d40: 6573 6c65 792c 220a 2020 2020 2020 2020  esley,".        
-00001d50: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
-00001d60: 0a20 2020 2020 2020 2020 2020 2022 6322  .            "c"
-00001d70: 3a20 2232 3030 302e 220a 2020 2020 2020  : "2000.".      
-00001d80: 2020 2020 7d0a 2020 2020 2020 2020 5d2c      }.        ],
-00001d90: 0a20 2020 2020 2020 2022 696e 6432 223a  .        "ind2":
-00001da0: 2022 2022 0a20 2020 2020 207d 0a20 2020   " ".      }.   
-00001db0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00001dc0: 2233 3030 223a 207b 0a20 2020 2020 2020  "300": {.       
-00001dd0: 2022 696e 6431 223a 2022 2022 2c0a 2020   "ind1": " ",.  
-00001de0: 2020 2020 2020 2273 7562 6669 656c 6473        "subfields
-00001df0: 223a 205b 0a20 2020 2020 2020 2020 207b  ": [.          {
-00001e00: 0a20 2020 2020 2020 2020 2020 2022 6122  .            "a"
-00001e10: 3a20 2278 7869 762c 2033 3231 2070 2e20  : "xxiv, 321 p. 
-00001e20: 3b22 0a20 2020 2020 2020 2020 207d 2c0a  ;".          },.
-00001e30: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00001e40: 2020 2020 2020 2020 2263 223a 2022 3234          "c": "24
-00001e50: 2063 6d2e 220a 2020 2020 2020 2020 2020   cm.".          
-00001e60: 7d0a 2020 2020 2020 2020 5d2c 0a20 2020  }.        ],.   
-00001e70: 2020 2020 2022 696e 6432 223a 2022 2022       "ind2": " "
-00001e80: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
-00001e90: 2020 2020 7b0a 2020 2020 2020 2235 3034      {.      "504
-00001ea0: 223a 207b 0a20 2020 2020 2020 2022 696e  ": {.        "in
-00001eb0: 6431 223a 2022 2022 2c0a 2020 2020 2020  d1": " ",.      
-00001ec0: 2020 2273 7562 6669 656c 6473 223a 205b    "subfields": [
-00001ed0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
-00001ee0: 2020 2020 2020 2020 2022 6122 3a20 2249           "a": "I
-00001ef0: 6e63 6c75 6465 7320 6269 626c 696f 6772  ncludes bibliogr
-00001f00: 6170 6869 6361 6c20 7265 6665 7265 6e63  aphical referenc
-00001f10: 6573 2e22 0a20 2020 2020 2020 2020 207d  es.".          }
-00001f20: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00001f30: 2020 2020 2269 6e64 3222 3a20 2220 220a      "ind2": " ".
-00001f40: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
-00001f50: 2020 207b 0a20 2020 2020 2022 3635 3022     {.      "650"
-00001f60: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
-00001f70: 3122 3a20 2220 222c 0a20 2020 2020 2020  1": " ",.       
-00001f80: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
-00001f90: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00001fa0: 2020 2020 2020 2020 2261 223a 2022 436f          "a": "Co
-00001fb0: 6d70 7574 6572 2070 726f 6772 616d 6d69  mputer programmi
-00001fc0: 6e67 2e22 0a20 2020 2020 2020 2020 207d  ng.".          }
-00001fd0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00001fe0: 2020 2020 2269 6e64 3222 3a20 2230 220a      "ind2": "0".
-00001ff0: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
-00002000: 2020 207b 0a20 2020 2020 2022 3730 3022     {.      "700"
-00002010: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
-00002020: 3122 3a20 2231 222c 0a20 2020 2020 2020  1": "1",.       
-00002030: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
-00002040: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00002050: 2020 2020 2020 2020 2261 223a 2022 5468          "a": "Th
-00002060: 6f6d 6173 2c20 4461 7669 642c 220a 2020  omas, David,".  
-00002070: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002080: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002090: 2020 2022 6422 3a20 2231 3935 362d 220a     "d": "1956-".
-000020a0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000020b0: 2020 2020 5d2c 0a20 2020 2020 2020 2022      ],.        "
-000020c0: 696e 6432 223a 2022 2022 0a20 2020 2020  ind2": " ".     
-000020d0: 207d 0a20 2020 207d 0a20 205d 0a7d 0a60   }.    }.  ].}.`
-000020e0: 6060 0a0a 4966 2079 6f75 2077 616e 7420  ``..If you want 
-000020f0: 746f 2070 6172 7365 2061 2066 696c 6520  to parse a file 
-00002100: 6f66 204d 4152 434a 534f 4e20 7265 636f  of MARCJSON reco
-00002110: 7264 7320 796f 7520 6361 6e3a 0a0a 6060  rds you can:..``
-00002120: 6070 7974 686f 6e0a 6672 6f6d 2070 796d  `python.from pym
-00002130: 6172 6320 696d 706f 7274 2070 6172 7365  arc import parse
-00002140: 5f6a 736f 6e5f 746f 5f61 7272 6179 0a0a  _json_to_array..
-00002150: 7265 636f 7264 7320 3d20 7061 7273 655f  records = parse_
-00002160: 6a73 6f6e 5f74 6f5f 6172 7261 7928 6f70  json_to_array(op
-00002170: 656e 2827 7465 7374 2f62 6174 6368 2e6a  en('test/batch.j
-00002180: 736f 6e27 2929 0a0a 7072 696e 7428 7265  son'))..print(re
-00002190: 636f 7264 735b 305d 290a 6060 600a 0a60  cords[0]).```..`
-000021a0: 6060 0a3d 4c44 5220 2030 3039 3235 6e6a  ``.=LDR  00925nj
-000021b0: 6d20 2032 3230 3032 3737 3761 2034 3530  m  22002777a 450
-000021c0: 300a 3d30 3031 2020 3536 3337 3234 310a  0.=001  5637241.
-000021d0: 3d30 3033 2020 444c 430a 3d30 3035 2020  =003  DLC.=005  
-000021e0: 3139 3932 3038 3236 3038 3430 3336 2e30  19920826084036.0
-000021f0: 0a3d 3030 3720 2073 6475 6275 6d65 6e6e  .=007  sdubumenn
-00002200: 6d70 6c75 0a3d 3030 3820 2039 3130 3932  mplu.=008  91092
-00002210: 3673 3139 3537 5c5c 5c5c 6e79 7575 756e  6s1957\\\\nyuuun
-00002220: 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c 5c5c 656e  \\\\\\\\\\\\\\en
-00002230: 675c 5c0a 3d30 3130 2020 5c5c 2461 2020  g\\.=010  \\$a  
-00002240: 2039 3137 3538 3333 350a 3d30 3238 2020   91758335.=028  
-00002250: 3030 2461 3132 3539 2462 4174 6c61 6e74  00$a1259$bAtlant
-00002260: 6963 0a3d 3034 3020 205c 5c24 6144 4c43  ic.=040  \\$aDLC
-00002270: 2463 444c 430a 3d30 3530 2020 3030 2461  $cDLC.=050  00$a
-00002280: 4174 6c61 6e74 6963 2031 3235 390a 3d32  Atlantic 1259.=2
-00002290: 3435 2020 3034 2461 5468 6520 4772 6561  45  04$aThe Grea
-000022a0: 7420 5261 7920 4368 6172 6c65 7324 685b  t Ray Charles$h[
-000022b0: 736f 756e 6420 7265 636f 7264 696e 675d  sound recording]
-000022c0: 2e0a 3d32 3630 2020 5c5c 2461 4e65 7720  ..=260  \\$aNew 
-000022d0: 596f 726b 2c20 4e2e 592e 203a 2462 4174  York, N.Y. :$bAt
-000022e0: 6c61 6e74 6963 2c24 635b 3139 3537 3f5d  lantic,$c[1957?]
-000022f0: 0a3d 3330 3020 205c 5c24 6131 2073 6f75  .=300  \\$a1 sou
-00002300: 6e64 2064 6973 6320 3a24 6261 6e61 6c6f  nd disc :$banalo
-00002310: 672c 2033 3320 312f 3320 7270 6d20 3b24  g, 33 1/3 rpm ;$
-00002320: 6331 3220 696e 2e0a 3d35 3131 2020 305c  c12 in..=511  0\
-00002330: 2461 5261 7920 4368 6172 6c65 732c 2070  $aRay Charles, p
-00002340: 6961 6e6f 2026 2063 656c 6573 7465 2e0a  iano & celeste..
-00002350: 3d35 3035 2020 305c 2461 5468 6520 5261  =505  0\$aThe Ra
-00002360: 7920 2d2d 204d 7920 6d65 6c61 6e63 686f  y -- My melancho
-00002370: 6c79 2062 6162 7920 2d2d 2042 6c61 636b  ly baby -- Black
-00002380: 2063 6f66 6665 6520 2d2d 2054 6865 7265   coffee -- There
-00002390: 2773 206e 6f20 796f 7520 2d2d 2044 6f6f  's no you -- Doo
-000023a0: 646c 696e 2720 2d2d 2053 7765 6574 2073  dlin' -- Sweet s
-000023b0: 6978 7465 656e 2062 6172 7320 2d2d 2049  ixteen bars -- I
-000023c0: 2073 7572 7265 6e64 6572 2064 6561 7220   surrender dear 
-000023d0: 2d2d 2055 6e64 6563 6964 6564 2e0a 3d35  -- Undecided..=5
-000023e0: 3030 2020 5c5c 2461 4272 6965 6620 7265  00  \\$aBrief re
-000023f0: 636f 7264 2e0a 3d36 3530 2020 5c30 2461  cord..=650  \0$a
-00002400: 4a61 7a7a 2479 3139 3531 2d31 3936 302e  Jazz$y1951-1960.
-00002410: 0a3d 3635 3020 205c 3024 6150 6961 6e6f  .=650  \0$aPiano
-00002420: 2077 6974 6820 6a61 7a7a 2065 6e73 656d   with jazz ensem
-00002430: 626c 652e 0a3d 3730 3020 2031 5c24 6143  ble..=700  1\$aC
-00002440: 6861 726c 6573 2c20 5261 792c 2464 3139  harles, Ray,$d19
-00002450: 3330 2d24 3470 7266 0a60 6060 0a0a 5375  30-$4prf.```..Su
-00002460: 7070 6f72 740a 2d2d 2d2d 2d2d 2d0a 0a54  pport.-------..T
-00002470: 6865 2070 796d 6172 6320 6465 7665 6c6f  he pymarc develo
-00002480: 7065 7273 2065 6e63 6f75 7261 6765 2079  pers encourage y
-00002490: 6f75 2074 6f20 6a6f 696e 2074 6865 205b  ou to join the [
-000024a0: 7079 6d61 7263 2047 6f6f 676c 650a 4772  pymarc Google.Gr
-000024b0: 6f75 705d 2868 7474 703a 2f2f 6772 6f75  oup](http://grou
-000024c0: 7073 2e67 6f6f 676c 652e 636f 6d2f 6772  ps.google.com/gr
-000024d0: 6f75 702f 7079 6d61 7263 2920 6966 2079  oup/pymarc) if y
-000024e0: 6f75 206e 6565 6420 6865 6c70 2e20 2041  ou need help.  A
-000024f0: 6c73 6f2c 2070 6c65 6173 650a 6665 656c  lso, please.feel
-00002500: 2066 7265 6520 746f 2075 7365 205b 6973   free to use [is
-00002510: 7375 6520 7472 6163 6b69 6e67 5d28 6874  sue tracking](ht
-00002520: 7470 733a 2f2f 6769 746c 6162 2e63 6f6d  tps://gitlab.com
-00002530: 2f70 796d 6172 632f 7079 6d61 7263 2f69  /pymarc/pymarc/i
-00002540: 7373 7565 7329 206f 6e0a 4769 744c 6162  ssues) on.GitLab
-00002550: 2074 6f20 7375 626d 6974 2066 6561 7475   to submit featu
-00002560: 7265 2072 6571 7565 7374 7320 6f72 2062  re requests or b
-00002570: 7567 2072 6570 6f72 7473 2e20 4966 2079  ug reports. If y
-00002580: 6f75 2776 6520 676f 7420 616e 2069 7463  ou've got an itc
-00002590: 6820 746f 0a73 6372 6174 6368 2c20 706c  h to.scratch, pl
-000025a0: 6561 7365 2073 6372 6174 6368 2069 742c  ease scratch it,
-000025b0: 2061 6e64 2073 656e 6420 6d65 7267 6520   and send merge 
-000025c0: 7265 7175 6573 7473 206f 6e0a 5b47 6974  requests on.[Git
-000025d0: 4c61 625d 2868 7474 703a 2f2f 6769 746c  Lab](http://gitl
-000025e0: 6162 2e63 6f6d 2f70 796d 6172 632f 7079  ab.com/pymarc/py
-000025f0: 6d61 7263 292e 0a0a 4966 2079 6f75 2073  marc)...If you s
-00002600: 7461 7274 2077 6f72 6b69 6e67 2077 6974  tart working wit
-00002610: 6820 4d41 5243 2079 6f75 206d 6179 2066  h MARC you may f
-00002620: 6565 6c20 6c69 6b65 2079 6f75 206e 6565  eel like you nee
-00002630: 6420 6d6f 7261 6c20 7375 7070 6f72 740a  d moral support.
-00002640: 696e 2061 6464 6974 696f 6e20 746f 2074  in addition to t
-00002650: 6563 686e 6963 616c 2073 7570 706f 7274  echnical support
-00002660: 2e20 5468 650a 5b23 636f 6465 346c 6962  . The.[#code4lib
-00002670: 5d28 6972 6373 3a2f 2f69 7263 2e6c 6962  ](ircs://irc.lib
-00002680: 6572 612e 6368 6174 2f63 6f64 6534 6c69  era.chat/code4li
-00002690: 6229 2063 6861 6e6e 656c 206f 6e20 5b4c  b) channel on [L
-000026a0: 6962 6572 615d 2868 7474 7073 3a2f 2f6c  ibera](https://l
-000026b0: 6962 6572 612e 6368 6174 2f29 2069 7320  ibera.chat/) is 
-000026c0: 6120 676f 6f64 2070 6c61 6365 2066 6f72  a good place for
-000026d0: 2062 6f74 682e 0a                         both..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6d61  : 2.1.Name: pyma
+00000020: 7263 0a56 6572 7369 6f6e 3a20 352e 302e  rc.Version: 5.0.
+00000030: 300a 5375 6d6d 6172 793a 2052 6561 642c  0.Summary: Read,
+00000040: 2077 7269 7465 2061 6e64 206d 6f64 6966   write and modif
+00000050: 7920 4d41 5243 2062 6962 6c69 6f67 7261  y MARC bibliogra
+00000060: 7068 6963 2064 6174 610a 486f 6d65 2d70  phic data.Home-p
+00000070: 6167 653a 2068 7474 703a 2f2f 6769 746c  age: http://gitl
+00000080: 6162 2e63 6f6d 2f70 796d 6172 632f 7079  ab.com/pymarc/py
+00000090: 6d61 7263 0a41 7574 686f 723a 2045 6420  marc.Author: Ed 
+000000a0: 5375 6d6d 6572 730a 4175 7468 6f72 2d65  Summers.Author-e
+000000b0: 6d61 696c 3a20 6568 7340 706f 626f 782e  mail: ehs@pobox.
+000000c0: 636f 6d0a 4c69 6365 6e73 653a 2068 7474  com.License: htt
+000000d0: 703a 2f2f 7777 772e 6f70 656e 736f 7572  p://www.opensour
+000000e0: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+000000f0: 6273 642d 6c69 6365 6e73 652e 7068 700a  bsd-license.php.
+00000100: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000110: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000120: 2045 6475 6361 7469 6f6e 0a43 6c61 7373   Education.Class
+00000130: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000140: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000150: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
+00000160: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000170: 656e 6365 203a 3a20 496e 666f 726d 6174  ence :: Informat
+00000180: 696f 6e20 5465 6368 6e6f 6c6f 6779 0a43  ion Technology.C
+00000190: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000001a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001b0: 6564 203a 3a20 4253 4420 4c69 6365 6e73  ed :: BSD Licens
+000001c0: 650a 436c 6173 7369 6669 6572 3a20 5072  e.Classifier: Pr
+000001d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001f0: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
+00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000220: 332e 370a 436c 6173 7369 6669 6572 3a20  3.7.Classifier: 
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000250: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000260: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000280: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000290: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002b0: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+000002c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002e0: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+000002f0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000300: 3a3a 2054 6578 7420 5072 6f63 6573 7369  :: Text Processi
+00000310: 6e67 203a 3a20 4765 6e65 7261 6c0a 5265  ng :: General.Re
+00000320: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000330: 3d33 2e37 0a44 6573 6372 6970 7469 6f6e  =3.7.Description
+00000340: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000350: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+00000360: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000370: 5345 0a0a 6060 600a 5f7c 5f7c 5f7c 2020  SE..```._|_|_|  
+00000380: 2020 5f7c 2020 2020 5f7c 2020 5f7c 5f7c    _|    _|  _|_|
+00000390: 5f7c 2020 5f7c 5f7c 2020 2020 2020 5f7c  _|  _|_|      _|
+000003a0: 5f7c 5f7c 2020 5f7c 2020 5f7c 5f7c 2020  _|_|  _|  _|_|  
+000003b0: 2020 5f7c 5f7c 5f7c 0a5f 7c20 2020 205f    _|_|_|._|    _
+000003c0: 7c20 205f 7c20 2020 205f 7c20 205f 7c20  |  _|    _|  _| 
+000003d0: 2020 205f 7c20 2020 205f 7c20 205f 7c20     _|    _|  _| 
+000003e0: 2020 205f 7c20 205f 7c5f 7c20 2020 2020     _|  _|_|     
+000003f0: 205f 7c0a 5f7c 2020 2020 5f7c 2020 5f7c   _|._|    _|  _|
+00000400: 2020 2020 5f7c 2020 5f7c 2020 2020 5f7c      _|  _|    _|
+00000410: 2020 2020 5f7c 2020 5f7c 2020 2020 5f7c      _|  _|    _|
+00000420: 2020 5f7c 2020 2020 2020 2020 5f7c 0a5f    _|        _|._
+00000430: 7c5f 7c5f 7c20 2020 2020 205f 7c5f 7c5f  |_|_|      _|_|_
+00000440: 7c20 205f 7c20 2020 205f 7c20 2020 205f  |  _|    _|    _
+00000450: 7c20 2020 205f 7c5f 7c5f 7c20 205f 7c20  |    _|_|_|  _| 
+00000460: 2020 2020 2020 2020 205f 7c5f 7c5f 7c0a           _|_|_|.
+00000470: 5f7c 2020 2020 2020 2020 2020 2020 2020  _|              
+00000480: 5f7c 0a5f 7c20 2020 2020 2020 2020 205f  _|._|          _
+00000490: 7c5f 7c0a 6060 600a 0a5b 215b 4275 696c  |_|.```..[![Buil
+000004a0: 6420 7374 6174 7573 5d28 6874 7470 733a  d status](https:
+000004b0: 2f2f 6769 746c 6162 2e63 6f6d 2f70 796d  //gitlab.com/pym
+000004c0: 6172 632f 7079 6d61 7263 2f62 6164 6765  arc/pymarc/badge
+000004d0: 732f 6d61 696e 2f70 6970 656c 696e 652e  s/main/pipeline.
+000004e0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+000004f0: 746c 6162 2e63 6f6d 2f70 796d 6172 632f  tlab.com/pymarc/
+00000500: 7079 6d61 7263 2f2d 2f63 6f6d 6d69 7473  pymarc/-/commits
+00000510: 2f6d 6169 6e29 0a0a 7079 6d61 7263 2069  /main)..pymarc i
+00000520: 7320 6120 7079 7468 6f6e 206c 6962 7261  s a python libra
+00000530: 7279 2066 6f72 2077 6f72 6b69 6e67 2077  ry for working w
+00000540: 6974 6820 6269 626c 696f 6772 6170 6869  ith bibliographi
+00000550: 6320 6461 7461 2065 6e63 6f64 6564 2069  c data encoded i
+00000560: 6e0a 5b4d 4152 4332 315d 2868 7474 7073  n.[MARC21](https
+00000570: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00000580: 6f72 672f 7769 6b69 2f4d 4152 435f 7374  org/wiki/MARC_st
+00000590: 616e 6461 7264 7329 2e20 4974 2070 726f  andards). It pro
+000005a0: 7669 6465 7320 616e 2041 5049 2066 6f72  vides an API for
+000005b0: 0a72 6561 6469 6e67 2c20 7772 6974 696e  .reading, writin
+000005c0: 6720 616e 6420 6d6f 6469 6679 696e 6720  g and modifying 
+000005d0: 4d41 5243 2072 6563 6f72 6473 2e20 4974  MARC records. It
+000005e0: 2077 6173 206d 6f73 746c 7920 6465 7369   was mostly desi
+000005f0: 676e 6564 2074 6f20 6265 2061 6e0a 656d  gned to be an.em
+00000600: 6572 6765 6e63 7920 656a 6563 7420 7365  ergency eject se
+00000610: 6174 2c20 666f 7220 6765 7474 696e 6720  at, for getting 
+00000620: 796f 7572 2064 6174 6120 6173 7365 7473  your data assets
+00000630: 206f 7574 206f 6620 4d41 5243 2061 6e64   out of MARC and
+00000640: 2069 6e74 6f20 736f 6d65 0a6b 696e 6420   into some.kind 
+00000650: 6f66 2073 616e 6572 2072 6570 7265 7365  of saner represe
+00000660: 6e74 6174 696f 6e2e 2048 6f77 6576 6572  ntation. However
+00000670: 206f 7665 7220 7468 6520 7965 6172 7320   over the years 
+00000680: 6974 2068 6173 2062 6565 6e20 7573 6564  it has been used
+00000690: 2074 6f20 6372 6561 7465 0a61 6e64 206d   to create.and m
+000006a0: 6f64 6966 7920 4d41 5243 2072 6563 6f72  odify MARC recor
+000006b0: 6473 2c20 7369 6e63 6520 6465 7370 6974  ds, since despit
+000006c0: 6520 5b72 6570 6561 7465 640a 6361 6c6c  e [repeated.call
+000006d0: 735d 2868 7474 7073 3a2f 2f77 6562 2e61  s](https://web.a
+000006e0: 7263 6869 7665 2e6f 7267 2f77 6562 2f32  rchive.org/web/2
+000006f0: 3031 3730 3733 3131 3633 3031 392f 6874  0170731163019/ht
+00000700: 7470 3a2f 2f77 7777 2e6d 6172 632d 6d75  tp://www.marc-mu
+00000710: 7374 2d64 6965 2e69 6e66 6f2f 696e 6465  st-die.info/inde
+00000720: 782e 7068 702f 4d61 696e 5f50 6167 6529  x.php/Main_Page)
+00000730: 0a66 6f72 2069 7420 746f 2064 6965 2061  .for it to die a
+00000740: 7320 6120 666f 726d 6174 2c20 4d41 5243  s a format, MARC
+00000750: 2073 6565 6d73 2074 6f20 6265 206c 6976   seems to be liv
+00000760: 696e 6720 7175 6974 6520 6861 7070 696c  ing quite happil
+00000770: 7920 6173 2061 207a 6f6d 6269 652e 0a0a  y as a zombie...
+00000780: 4265 6c6f 7720 6172 6520 736f 6d65 2063  Below are some c
+00000790: 6f6d 6d6f 6e20 6578 616d 706c 6573 206f  ommon examples o
+000007a0: 6620 686f 7720 796f 7520 6d69 6768 7420  f how you might 
+000007b0: 7761 6e74 2074 6f20 7573 6520 7079 6d61  want to use pyma
+000007c0: 7263 2e20 4966 0a79 6f75 2072 756e 2061  rc. If.you run a
+000007d0: 6372 6f73 7320 616e 2065 7861 6d70 6c65  cross an example
+000007e0: 2074 6861 7420 796f 7520 7468 696e 6b20   that you think 
+000007f0: 7368 6f75 6c64 2062 6520 6865 7265 2070  should be here p
+00000800: 6c65 6173 6520 7365 6e64 2061 0a70 756c  lease send a.pul
+00000810: 6c20 7265 7175 6573 742e 0a0a 596f 7520  l request...You 
+00000820: 6361 6e20 7265 6164 2070 796d 6172 6320  can read pymarc 
+00000830: 646f 6375 6d65 6e74 6174 696f 6e20 5b68  documentation [h
+00000840: 6572 655d 2868 7474 7073 3a2f 2f70 796d  ere](https://pym
+00000850: 6172 632e 7265 6164 7468 6564 6f63 732e  arc.readthedocs.
+00000860: 696f 2f65 6e2f 6c61 7465 7374 2f29 2e0a  io/en/latest/)..
+00000870: 0a23 2323 2049 6e73 7461 6c6c 6174 696f  .### Installatio
+00000880: 6e0a 0a59 6f75 276c 6c20 7072 6f62 6162  n..You'll probab
+00000890: 6c79 206a 7573 7420 7761 6e74 2074 6f20  ly just want to 
+000008a0: 7573 6520 7069 7020 746f 2069 6e73 7461  use pip to insta
+000008b0: 6c6c 2070 796d 6172 633a 0a0a 2020 2020  ll pymarc:..    
+000008c0: 7069 7020 696e 7374 616c 6c20 7079 6d61  pip install pyma
+000008d0: 7263 0a0a 4966 2079 6f75 2764 206c 696b  rc..If you'd lik
+000008e0: 6520 746f 2064 6f77 6e6c 6f61 6420 616e  e to download an
+000008f0: 6420 696e 7374 616c 6c20 7468 6520 6c61  d install the la
+00000900: 7465 7374 2073 6f75 7263 6520 796f 7527  test source you'
+00000910: 6c6c 206e 6565 6420 6769 743a 0a0a 2020  ll need git:..  
+00000920: 2020 6769 7420 636c 6f6e 6520 6769 743a    git clone git:
+00000930: 2f2f 6769 746c 6162 2e63 6f6d 2f70 796d  //gitlab.com/pym
+00000940: 6172 632f 7079 6d61 7263 2e67 6974 0a0a  arc/pymarc.git..
+00000950: 596f 7527 6c6c 2061 6c73 6f20 6e65 6564  You'll also need
+00000960: 205b 7365 7475 7074 6f6f 6c73 5d28 6874   [setuptools](ht
+00000970: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+00000980: 6e2e 6f72 672f 7079 7069 2f73 6574 7570  n.org/pypi/setup
+00000990: 746f 6f6c 7323 696e 7374 616c 6c61 7469  tools#installati
+000009a0: 6f6e 2d69 6e73 7472 7563 7469 6f6e 7329  on-instructions)
+000009b0: 2e20 4f6e 6365 2079 6f75 2068 6176 6520  . Once you have 
+000009c0: 7468 6520 736f 7572 6365 2061 6e64 2073  the source and s
+000009d0: 6574 7570 746f 6f6c 7320 7275 6e20 7468  etuptools run th
+000009e0: 6520 7079 6d61 7263 2074 6573 740a 7375  e pymarc test.su
+000009f0: 6974 6520 746f 206d 616b 6520 7375 7265  ite to make sure
+00000a00: 2074 6869 6e67 7320 6172 6520 696e 206f   things are in o
+00000a10: 7264 6572 2077 6974 6820 7468 6520 6469  rder with the di
+00000a20: 7374 7269 6275 7469 6f6e 3a0a 0a20 2020  stribution:..   
+00000a30: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000a40: 2074 6573 740a 0a41 6e64 2074 6865 6e20   test..And then 
+00000a50: 696e 7374 616c 6c3a 0a0a 2020 2020 7079  install:..    py
+00000a60: 7468 6f6e 2073 6574 7570 2e70 7920 696e  thon setup.py in
+00000a70: 7374 616c 6c0a 0a23 2323 2052 6561 6469  stall..### Readi
+00000a80: 6e67 0a0a 4d6f 7374 206f 6674 656e 2079  ng..Most often y
+00000a90: 6f75 2077 696c 6c20 6861 7665 2073 6f6d  ou will have som
+00000aa0: 6520 4d41 5243 2064 6174 6120 616e 6420  e MARC data and 
+00000ab0: 7769 6c6c 2077 616e 7420 746f 2065 7874  will want to ext
+00000ac0: 7261 6374 2064 6174 610a 6672 6f6d 2069  ract data.from i
+00000ad0: 742e 2048 6572 6527 7320 616e 2065 7861  t. Here's an exa
+00000ae0: 6d70 6c65 206f 6620 7265 6164 696e 6720  mple of reading 
+00000af0: 6120 6261 7463 6820 6f66 2072 6563 6f72  a batch of recor
+00000b00: 6473 2061 6e64 2070 7269 6e74 696e 6720  ds and printing 
+00000b10: 6f75 740a 7468 6520 7469 746c 652e 2049  out.the title. I
+00000b20: 6620 796f 7520 6172 6520 6375 7269 6f75  f you are curiou
+00000b30: 7320 7468 6973 2065 7861 6d70 6c65 2075  s this example u
+00000b40: 7365 7320 7468 6520 6261 7463 6820 6669  ses the batch fi
+00000b50: 6c65 0a61 7661 696c 6162 6c65 2068 6572  le.available her
+00000b60: 6520 696e 2070 796d 6172 6320 7265 706f  e in pymarc repo
+00000b70: 7369 746f 7279 3a0a 0a60 6060 7079 7468  sitory:..```pyth
+00000b80: 6f6e 0a66 726f 6d20 7079 6d61 7263 2069  on.from pymarc i
+00000b90: 6d70 6f72 7420 4d41 5243 5265 6164 6572  mport MARCReader
+00000ba0: 0a77 6974 6820 6f70 656e 2827 7465 7374  .with open('test
+00000bb0: 2f6d 6172 632e 6461 7427 2c20 2772 6227  /marc.dat', 'rb'
+00000bc0: 2920 6173 2066 683a 0a20 2020 2072 6561  ) as fh:.    rea
+00000bd0: 6465 7220 3d20 4d41 5243 5265 6164 6572  der = MARCReader
+00000be0: 2866 6829 0a20 2020 2066 6f72 2072 6563  (fh).    for rec
+00000bf0: 6f72 6420 696e 2072 6561 6465 723a 0a20  ord in reader:. 
+00000c00: 2020 2020 2020 2070 7269 6e74 2872 6563         print(rec
+00000c10: 6f72 642e 7469 746c 6529 0a60 6060 0a60  ord.title).```.`
+00000c20: 6060 0a54 6865 2070 7261 676d 6174 6963  ``.The pragmatic
+00000c30: 2070 726f 6772 616d 6d65 7220 3a20 6672   programmer : fr
+00000c40: 6f6d 206a 6f75 726e 6579 6d61 6e20 746f  om journeyman to
+00000c50: 206d 6173 7465 7220 2f0a 5072 6f67 7261   master /.Progra
+00000c60: 6d6d 696e 6720 5079 7468 6f6e 202f 0a4c  mming Python /.L
+00000c70: 6561 726e 696e 6720 5079 7468 6f6e 202f  earning Python /
+00000c80: 0a50 7974 686f 6e20 636f 6f6b 626f 6f6b  .Python cookbook
+00000c90: 202f 0a50 7974 686f 6e20 7072 6f67 7261   /.Python progra
+00000ca0: 6d6d 696e 6720 666f 7220 7468 6520 6162  mming for the ab
+00000cb0: 736f 6c75 7465 2062 6567 696e 6e65 7220  solute beginner 
+00000cc0: 2f0a 5765 6220 7072 6f67 7261 6d6d 696e  /.Web programmin
+00000cd0: 6720 3a20 7465 6368 6e69 7175 6573 2066  g : techniques f
+00000ce0: 6f72 2069 6e74 6567 7261 7469 6e67 2050  or integrating P
+00000cf0: 7974 686f 6e2c 204c 696e 7578 2c20 4170  ython, Linux, Ap
+00000d00: 6163 6865 2c20 616e 6420 4d79 5351 4c20  ache, and MySQL 
+00000d10: 2f0a 5079 7468 6f6e 2070 726f 6772 616d  /.Python program
+00000d20: 6d69 6e67 206f 6e20 5769 6e33 3220 2f0a  ming on Win32 /.
+00000d30: 5079 7468 6f6e 2070 726f 6772 616d 6d69  Python programmi
+00000d40: 6e67 203a 2061 6e20 696e 7472 6f64 7563  ng : an introduc
+00000d50: 7469 6f6e 2074 6f20 636f 6d70 7574 6572  tion to computer
+00000d60: 2073 6369 656e 6365 202f 0a50 7974 686f   science /.Pytho
+00000d70: 6e20 5765 6220 7072 6f67 7261 6d6d 696e  n Web programmin
+00000d80: 6720 2f0a 436f 7265 2070 7974 686f 6e20  g /.Core python 
+00000d90: 7072 6f67 7261 6d6d 696e 6720 2f0a 5079  programming /.Py
+00000da0: 7468 6f6e 2061 6e64 2054 6b69 6e74 6572  thon and Tkinter
+00000db0: 2070 726f 6772 616d 6d69 6e67 202f 0a47   programming /.G
+00000dc0: 616d 6520 7072 6f67 7261 6d6d 696e 6720  ame programming 
+00000dd0: 7769 7468 2050 7974 686f 6e2c 204c 7561  with Python, Lua
+00000de0: 2c20 616e 6420 5275 6279 202f 0a50 7974  , and Ruby /.Pyt
+00000df0: 686f 6e20 7072 6f67 7261 6d6d 696e 6720  hon programming 
+00000e00: 7061 7474 6572 6e73 202f 0a50 7974 686f  patterns /.Pytho
+00000e10: 6e20 7072 6f67 7261 6d6d 696e 6720 7769  n programming wi
+00000e20: 7468 2074 6865 204a 6176 6120 636c 6173  th the Java clas
+00000e30: 7320 6c69 6272 6172 6965 7320 3a20 6120  s libraries : a 
+00000e40: 7475 746f 7269 616c 2066 6f72 2062 7569  tutorial for bui
+00000e50: 6c64 696e 6720 5765 620a 616e 6420 456e  lding Web.and En
+00000e60: 7465 7270 7269 7365 2061 7070 6c69 6361  terprise applica
+00000e70: 7469 6f6e 7320 2f0a 4c65 6172 6e20 746f  tions /.Learn to
+00000e80: 2070 726f 6772 616d 2075 7369 6e67 2050   program using P
+00000e90: 7974 686f 6e20 3a20 6120 7475 746f 7269  ython : a tutori
+00000ea0: 616c 2066 6f72 2068 6f62 6279 6973 7473  al for hobbyists
+00000eb0: 2c20 7365 6c66 2d73 7461 7274 6572 732c  , self-starters,
+00000ec0: 2061 6e64 2061 6c6c 0a77 686f 2077 616e   and all.who wan
+00000ed0: 7420 746f 206c 6561 726e 2074 6865 2061  t to learn the a
+00000ee0: 7274 206f 6620 636f 6d70 7574 6572 2070  rt of computer p
+00000ef0: 726f 6772 616d 6d69 6e67 202f 0a50 726f  rogramming /.Pro
+00000f00: 6772 616d 6d69 6e67 2077 6974 6820 5079  gramming with Py
+00000f10: 7468 6f6e 202f 0a42 5344 2053 6f63 6b65  thon /.BSD Socke
+00000f20: 7473 2070 726f 6772 616d 6d69 6e67 2066  ts programming f
+00000f30: 726f 6d20 6120 6d75 6c74 692d 6c61 6e67  rom a multi-lang
+00000f40: 7561 6765 2070 6572 7370 6563 7469 7665  uage perspective
+00000f50: 202f 0a44 6573 6967 6e20 7061 7474 6572   /.Design patter
+00000f60: 6e73 203a 2065 6c65 6d65 6e74 7320 6f66  ns : elements of
+00000f70: 2072 6575 7361 626c 6520 6f62 6a65 6374   reusable object
+00000f80: 2d6f 7269 656e 7465 6420 736f 6674 7761  -oriented softwa
+00000f90: 7265 202f 0a49 6e74 726f 6475 6374 696f  re /.Introductio
+00000fa0: 6e20 746f 2061 6c67 6f72 6974 686d 7320  n to algorithms 
+00000fb0: 2f0a 414e 5349 2043 6f6d 6d6f 6e20 4c69  /.ANSI Common Li
+00000fc0: 7370 202f 0a60 6060 0a0a 4120 6070 796d  sp /.```..A `pym
+00000fd0: 6172 632e 5265 636f 7264 6020 6f62 6a65  arc.Record` obje
+00000fe0: 6374 2068 6173 2061 2066 6577 2068 616e  ct has a few han
+00000ff0: 6479 2070 726f 7065 7274 6965 7320 6c69  dy properties li
+00001000: 6b65 2060 7469 746c 6560 2066 6f72 2067  ke `title` for g
+00001010: 6574 7469 6e67 2061 740a 6269 7473 206f  etting at.bits o
+00001020: 6620 6120 6269 626c 696f 6772 6170 6869  f a bibliographi
+00001030: 6320 7265 636f 7264 2c20 6f74 6865 7273  c record, others
+00001040: 2069 6e63 6c75 6465 3a20 6061 7574 686f   include: `autho
+00001050: 7260 2c20 6069 7362 6e60 2c20 6073 7562  r`, `isbn`, `sub
+00001060: 6a65 6374 7360 2c0a 606c 6f63 6174 696f  jects`,.`locatio
+00001070: 6e60 2c20 606e 6f74 6573 602c 2060 7068  n`, `notes`, `ph
+00001080: 7973 6963 616c 6465 7363 7269 7074 696f  ysicaldescriptio
+00001090: 6e60 2c20 6070 7562 6c69 7368 6572 602c  n`, `publisher`,
+000010a0: 2060 7075 6279 6561 7260 2c20 6069 7373   `pubyear`, `iss
+000010b0: 6e60 2c0a 6069 7373 6e5f 7469 746c 6560  n`,.`issn_title`
+000010c0: 2e20 4275 7420 7265 616c 6c79 2c20 746f  . But really, to
+000010d0: 2077 6f72 6b20 7769 7468 204d 4152 4320   work with MARC 
+000010e0: 6461 7461 2079 6f75 206e 6565 6420 746f  data you need to
+000010f0: 2075 6e64 6572 7374 616e 6420 7468 650a   understand the.
+00001100: 6e75 6d65 7269 6320 6669 656c 6420 7461  numeric field ta
+00001110: 6773 2061 6e64 2073 7562 6669 656c 6420  gs and subfield 
+00001120: 636f 6465 7320 7468 6174 2061 7265 2075  codes that are u
+00001130: 7365 6420 746f 2064 6573 6967 6e61 7465  sed to designate
+00001140: 2076 6172 696f 7573 2062 6974 730a 6f66   various bits.of
+00001150: 2069 6e66 6f72 6d61 7469 6f6e 2e20 5468   information. Th
+00001160: 6572 6520 6973 2061 206c 6f74 206d 6f72  ere is a lot mor
+00001170: 6520 6461 7461 2068 6964 6465 6e20 696e  e data hidden in
+00001180: 2061 204d 4152 4320 7265 636f 7264 2074   a MARC record t
+00001190: 6861 6e20 7468 6573 650a 6865 6c70 6572  han these.helper
+000011a0: 2070 726f 7065 7274 6965 7320 7072 6f76   properties prov
+000011b0: 6964 6520 6163 6365 7373 2074 6f2e 2046  ide access to. F
+000011c0: 6f72 2065 7861 6d70 6c65 2074 6865 2060  or example the `
+000011d0: 7469 746c 6560 2070 726f 7065 7274 7920  title` property 
+000011e0: 776f 726b 7320 6279 0a65 7874 7261 6374  works by.extract
+000011f0: 696e 6720 7468 6520 696e 666f 726d 6174  ing the informat
+00001200: 696f 6e20 6672 6f6d 2074 6865 2060 3234  ion from the `24
+00001210: 3560 2066 6965 6c64 2c20 7375 6266 6965  5` field, subfie
+00001220: 6c64 7320 6061 6020 616e 6420 6062 6020  lds `a` and `b` 
+00001230: 6265 6869 6e64 0a74 6865 2073 6365 6e65  behind.the scene
+00001240: 732e 2059 6f75 2063 616e 2061 6363 6573  s. You can acces
+00001250: 7320 6032 3435 6160 206c 696b 6520 736f  s `245a` like so
+00001260: 3a0a 0a60 6060 7079 7468 6f6e 0a70 7269  :..```python.pri
+00001270: 6e74 2872 6563 6f72 645b 2732 3435 275d  nt(record['245']
+00001280: 5b27 6127 5d29 0a60 6060 0a0a 536f 6d65  ['a']).```..Some
+00001290: 2066 6965 6c64 7320 6c69 6b65 2073 7562   fields like sub
+000012a0: 6a65 6374 7320 6361 6e20 7265 7065 6174  jects can repeat
+000012b0: 2e20 496e 2063 6173 6573 206c 696b 6520  . In cases like 
+000012c0: 7468 6174 2079 6f75 2077 696c 6c20 7761  that you will wa
+000012d0: 6e74 2074 6f20 7573 650a 6067 6574 5f66  nt to use.`get_f
+000012e0: 6965 6c64 7360 2074 6f20 6765 7420 616c  ields` to get al
+000012f0: 6c20 6f66 2074 6865 6d20 6173 2060 7079  l of them as `py
+00001300: 6d61 7263 2e46 6965 6c64 6020 6f62 6a65  marc.Field` obje
+00001310: 6374 732c 2077 6869 6368 2079 6f75 2063  cts, which you c
+00001320: 616e 2074 6865 6e0a 696e 7465 7261 6374  an then.interact
+00001330: 2077 6974 6820 6675 7274 6865 723a 0a0a   with further:..
+00001340: 6060 6070 7974 686f 6e0a 666f 7220 6620  ```python.for f 
+00001350: 696e 2072 6563 6f72 642e 6765 745f 6669  in record.get_fi
+00001360: 656c 6473 2827 3635 3027 293a 0a20 2020  elds('650'):.   
+00001370: 2070 7269 6e74 2866 290a 6060 600a 0a49   print(f).```..I
+00001380: 6620 796f 7520 6172 6520 6e65 7720 746f  f you are new to
+00001390: 204d 4152 4320 6669 656c 6473 205b 556e   MARC fields [Un
+000013a0: 6465 7273 7461 6e64 696e 670a 4d41 5243  derstanding.MARC
+000013b0: 5d28 6874 7470 3a2f 2f77 7777 2e6c 6f63  ](http://www.loc
+000013c0: 2e67 6f76 2f6d 6172 632f 756d 622f 2920  .gov/marc/umb/) 
+000013d0: 6973 2061 2070 7265 7474 7920 676f 6f64  is a pretty good
+000013e0: 2070 7269 6d65 722c 2061 6e64 2074 6865   primer, and the
+000013f0: 205b 4d41 5243 2032 310a 466f 726d 6174   [MARC 21.Format
+00001400: 735d 2868 7474 703a 2f2f 7777 772e 6c6f  s](http://www.lo
+00001410: 632e 676f 762f 6d61 7263 2f6d 6172 6364  c.gov/marc/marcd
+00001420: 6f63 7a2e 6874 6d6c 2920 7061 6765 2061  ocz.html) page a
+00001430: 7420 7468 6520 4c69 6272 6172 7920 6f66  t the Library of
+00001440: 2043 6f6e 6772 6573 7320 6973 2061 2067   Congress is a g
+00001450: 6f6f 6420 7265 6665 7265 6e63 6520 6f6e  ood reference on
+00001460: 6365 2079 6f75 2075 6e64 6572 7374 616e  ce you understan
+00001470: 6420 7468 6520 6261 7369 6373 2e0a 0a23  d the basics...#
+00001480: 2323 2057 7269 7469 6e67 0a0a 2a4e 6f74  ## Writing..*Not
+00001490: 653a 2041 7320 6f66 2076 352e 302e 3020  e: As of v5.0.0 
+000014a0: 6053 7562 6669 656c 6460 2069 7320 7573  `Subfield` is us
+000014b0: 6564 2074 6f20 6372 6561 7465 2073 7562  ed to create sub
+000014c0: 6669 656c 6473 2e20 5072 696f 7220 746f  fields. Prior to
+000014d0: 2076 352c 0a73 7562 6669 656c 6473 2077   v5,.subfields w
+000014e0: 6572 6520 636f 6e73 7472 7563 7465 6420  ere constructed 
+000014f0: 616e 6420 6163 6365 7373 6564 2061 7320  and accessed as 
+00001500: 6120 6c69 7374 206f 6620 7374 7269 6e67  a list of string
+00001510: 732c 2065 2e67 2e2c 2060 5b63 6f64 652c  s, e.g., `[code,
+00001520: 0a76 616c 7565 2c20 636f 6465 2c20 7661  .value, code, va
+00001530: 6c75 655d 602e 2049 6e20 7635 2e30 2e30  lue]`. In v5.0.0
+00001540: 2074 6869 7320 6861 7320 6265 656e 2063   this has been c
+00001550: 6861 6e67 6564 2074 6f20 6f72 6761 6e69  hanged to organi
+00001560: 7a65 2074 6865 2073 7562 6669 656c 6473  ze the subfields
+00001570: 0a69 6e74 6f20 6120 6c69 7374 206f 6620  .into a list of 
+00001580: 7475 706c 6573 2c20 652e 672e 2c20 605b  tuples, e.g., `[
+00001590: 2863 6f64 652c 2076 616c 7565 292c 2028  (code, value), (
+000015a0: 636f 6465 2c20 7661 6c75 6529 5d60 2e20  code, value)]`. 
+000015b0: 5468 6520 6053 7562 6669 656c 6460 0a69  The `Subfield`.i
+000015c0: 7320 696d 706c 656d 656e 7465 6420 6173  s implemented as
+000015d0: 2061 2060 4e61 6d65 6454 7570 6c65 6020   a `NamedTuple` 
+000015e0: 736f 2074 6861 7420 7468 6520 7475 706c  so that the tupl
+000015f0: 6573 2063 616e 2062 6520 636f 6e73 7472  es can be constr
+00001600: 7563 7465 6420 6173 0a60 5375 6266 6965  ucted as.`Subfie
+00001610: 6c64 2863 6f64 653d 636f 6465 2c20 7661  ld(code=code, va
+00001620: 6c75 653d 7661 6c75 6529 602e 2054 6865  lue=value)`. The
+00001630: 206f 6c64 2073 7479 6c65 206f 6620 6372   old style of cr
+00001640: 6561 7469 6e67 2073 7562 6669 656c 6473  eating subfields
+00001650: 2069 7320 6e6f 0a6c 6f6e 6765 7220 7375   is no.longer su
+00001660: 7070 6f72 7465 642e 2041 7474 656d 7074  pported. Attempt
+00001670: 696e 6720 746f 2070 6173 7320 6120 6c69  ing to pass a li
+00001680: 7374 206f 6620 7374 7269 6e67 7320 746f  st of strings to
+00001690: 2074 6865 2060 7375 6266 6965 6c64 7360   the `subfields`
+000016a0: 0a70 6172 616d 6574 6572 2066 6f72 2074  .parameter for t
+000016b0: 6865 2060 4669 656c 6460 2063 6f6e 7374  he `Field` const
+000016c0: 7275 6374 6f72 2077 696c 6c20 7261 6973  ructor will rais
+000016d0: 6520 6120 6056 616c 7565 4572 726f 7260  e a `ValueError`
+000016e0: 2e20 466f 720a 636f 6e76 656e 6965 6e63  . For.convenienc
+000016f0: 6520 7468 6520 6046 6965 6c64 2e63 6f6e  e the `Field.con
+00001700: 7665 7274 5f6c 6567 6163 795f 7375 6266  vert_legacy_subf
+00001710: 6965 6c64 7360 2063 616e 2062 6520 7573  ields` can be us
+00001720: 6564 2074 6f20 636f 6e76 6572 7420 610a  ed to convert a.
+00001730: 6c65 6761 6379 206c 6973 7420 6f66 2073  legacy list of s
+00001740: 7472 696e 6773 2069 6e74 6f20 6120 6c69  trings into a li
+00001750: 7374 206f 6620 6053 7562 6669 656c 6460  st of `Subfield`
+00001760: 732e 2a0a 0a48 6572 6527 7320 616e 2065  s.*..Here's an e
+00001770: 7861 6d70 6c65 206f 6620 6372 6561 7469  xample of creati
+00001780: 6e67 2061 2072 6563 6f72 6420 616e 6420  ng a record and 
+00001790: 7772 6974 696e 6720 6974 206f 7574 2074  writing it out t
+000017a0: 6f20 6120 6669 6c65 2e0a 0a60 6060 7079  o a file...```py
+000017b0: 7468 6f6e 0a66 726f 6d20 7079 6d61 7263  thon.from pymarc
+000017c0: 2069 6d70 6f72 7420 5265 636f 7264 2c20   import Record, 
+000017d0: 4669 656c 642c 2053 7562 6669 656c 640a  Field, Subfield.
+000017e0: 0a72 6563 6f72 6420 3d20 5265 636f 7264  .record = Record
+000017f0: 2829 0a72 6563 6f72 642e 6164 645f 6669  ().record.add_fi
+00001800: 656c 6428 0a20 2020 2046 6965 6c64 280a  eld(.    Field(.
+00001810: 2020 2020 2020 2020 7461 673d 2732 3435          tag='245
+00001820: 272c 0a20 2020 2020 2020 2069 6e64 6963  ',.        indic
+00001830: 6174 6f72 733d 5b27 3027 2c20 2731 275d  ators=['0', '1']
+00001840: 2c0a 2020 2020 2020 2020 7375 6266 6965  ,.        subfie
+00001850: 6c64 733d 5b0a 2020 2020 2020 2020 2020  lds=[.          
+00001860: 2020 5375 6266 6965 6c64 2863 6f64 653d    Subfield(code=
+00001870: 2761 272c 2076 616c 7565 3d27 5468 6520  'a', value='The 
+00001880: 7072 6167 6d61 7469 6320 7072 6f67 7261  pragmatic progra
+00001890: 6d6d 6572 203a 2027 292c 0a20 2020 2020  mmer : '),.     
+000018a0: 2020 2020 2020 2053 7562 6669 656c 6428         Subfield(
+000018b0: 636f 6465 3d27 6227 2c20 7661 6c75 653d  code='b', value=
+000018c0: 2766 726f 6d20 6a6f 7572 6e65 796d 616e  'from journeyman
+000018d0: 2074 6f20 6d61 7374 6572 202f 2729 2c0a   to master /'),.
+000018e0: 2020 2020 2020 2020 2020 2020 5375 6266              Subf
+000018f0: 6965 6c64 2863 6f64 653d 2763 272c 2076  ield(code='c', v
+00001900: 616c 7565 3d27 416e 6472 6577 2048 756e  alue='Andrew Hun
+00001910: 742c 2044 6176 6964 2054 686f 6d61 732e  t, David Thomas.
+00001920: 2729 0a20 2020 2020 2020 205d 2929 0a77  ').        ])).w
+00001930: 6974 6820 6f70 656e 2827 6669 6c65 2e64  ith open('file.d
+00001940: 6174 272c 2027 7762 2729 2061 7320 6f75  at', 'wb') as ou
+00001950: 743a 0a20 2020 206f 7574 2e77 7269 7465  t:.    out.write
+00001960: 2872 6563 6f72 642e 6173 5f6d 6172 6328  (record.as_marc(
+00001970: 2929 0a60 6060 0a0a 546f 2063 6f6e 7665  )).```..To conve
+00001980: 7274 2066 726f 6d20 7468 6520 6f6c 6420  rt from the old 
+00001990: 7374 7269 6e67 206c 6973 7420 746f 2061  string list to a
+000019a0: 206c 6973 7420 6f66 2060 5375 6266 6965   list of `Subfie
+000019b0: 6c64 6073 2c20 7468 6520 602e 636f 6e76  ld`s, the `.conv
+000019c0: 6572 745f 6c65 6761 6379 5f73 7562 6669  ert_legacy_subfi
+000019d0: 656c 6473 6020 636c 6173 7320 6d65 7468  elds` class meth
+000019e0: 6f64 0a69 7320 7072 6f76 6964 6564 206f  od.is provided o
+000019f0: 6e20 7468 6520 6046 6965 6c64 6020 636c  n the `Field` cl
+00001a00: 6173 732e 0a0a 6060 6070 7974 686f 6e0a  ass...```python.
+00001a10: 6672 6f6d 2070 796d 6172 6320 696d 706f  from pymarc impo
+00001a20: 7274 2046 6965 6c64 2c20 5375 6266 6965  rt Field, Subfie
+00001a30: 6c64 0a0a 6c65 6761 6379 5f66 6965 6c64  ld..legacy_field
+00001a40: 733a 206c 6973 745b 7374 725d 203d 205b  s: list[str] = [
+00001a50: 2761 272c 2027 5468 6520 7072 6167 6d61  'a', 'The pragma
+00001a60: 7469 6320 7072 6f67 7261 6d6d 6572 203a  tic programmer :
+00001a70: 2027 2c0a 2020 2020 2020 2020 2020 2020   ',.            
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2762 272c 2027 6672 6f6d 206a 6f75 726e  'b', 'from journ
+00001aa0: 6579 6d61 6e20 746f 206d 6173 7465 7220  eyman to master 
+00001ab0: 2f27 2c0a 2020 2020 2020 2020 2020 2020  /',.            
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2763 272c 2027 416e 6472 6577 2048 756e  'c', 'Andrew Hun
+00001ae0: 742c 2044 6176 6964 2054 686f 6d61 7327  t, David Thomas'
+00001af0: 5d0a 0a63 6f64 6564 5f66 6965 6c64 733a  ]..coded_fields:
+00001b00: 206c 6973 745b 5375 6266 6965 6c64 5d20   list[Subfield] 
+00001b10: 3d20 4669 656c 642e 636f 6e76 6572 745f  = Field.convert_
+00001b20: 6c65 6761 6379 5f73 7562 6669 656c 6473  legacy_subfields
+00001b30: 286c 6567 6163 795f 6669 656c 6473 290a  (legacy_fields).
+00001b40: 6060 600a 0a23 2323 2055 7064 6174 696e  ```..### Updatin
+00001b50: 670a 0a55 7064 6174 696e 6720 776f 726b  g..Updating work
+00001b60: 7320 7468 6520 7361 6d65 2077 6179 2c20  s the same way, 
+00001b70: 796f 7520 7265 6164 2069 7420 696e 2c20  you read it in, 
+00001b80: 6d6f 6469 6679 2069 742c 2061 6e64 2074  modify it, and t
+00001b90: 6865 6e20 7772 6974 6520 6974 206f 7574  hen write it out
+00001ba0: 0a61 6761 696e 3a0a 0a60 6060 7079 7468  .again:..```pyth
+00001bb0: 6f6e 0a66 726f 6d20 7079 6d61 7263 2069  on.from pymarc i
+00001bc0: 6d70 6f72 7420 4d41 5243 5265 6164 6572  mport MARCReader
+00001bd0: 0a77 6974 6820 6f70 656e 2827 7465 7374  .with open('test
+00001be0: 2f6d 6172 632e 6461 7427 2c20 2772 6227  /marc.dat', 'rb'
+00001bf0: 2920 6173 2066 683a 0a20 2020 2072 6561  ) as fh:.    rea
+00001c00: 6465 7220 3d20 4d41 5243 5265 6164 6572  der = MARCReader
+00001c10: 2866 6829 0a20 2020 2072 6563 6f72 6420  (fh).    record 
+00001c20: 3d20 6e65 7874 2872 6561 6465 7229 0a20  = next(reader). 
+00001c30: 2020 2072 6563 6f72 645b 2732 3435 275d     record['245']
+00001c40: 5b27 6127 5d20 3d20 2754 6865 205a 6f6d  ['a'] = 'The Zom
+00001c50: 6269 6520 5072 6f67 7261 6d6d 6572 203a  bie Programmer :
+00001c60: 2027 0a77 6974 6820 6f70 656e 2827 6669   '.with open('fi
+00001c70: 6c65 2e64 6174 272c 2027 7762 2729 2061  le.dat', 'wb') a
+00001c80: 7320 6f75 743a 0a20 2020 206f 7574 2e77  s out:.    out.w
+00001c90: 7269 7465 2872 6563 6f72 642e 6173 5f6d  rite(record.as_m
+00001ca0: 6172 6328 2929 0a60 6060 0a0a 0a23 2323  arc()).```...###
+00001cb0: 204a 534f 4e20 616e 6420 584d 4c0a 0a49   JSON and XML..I
+00001cc0: 6620 796f 7520 6669 6e64 2079 6f75 7273  f you find yours
+00001cd0: 656c 6620 7573 696e 6720 4d41 5243 2064  elf using MARC d
+00001ce0: 6174 6120 6120 6661 6972 2062 6974 2c20  ata a fair bit, 
+00001cf0: 616e 6420 6469 7374 7269 6275 7469 6e67  and distributing
+00001d00: 2069 742c 2079 6f75 206d 6179 0a6d 616b   it, you may.mak
+00001d10: 6520 6f74 6865 7220 6465 7665 6c6f 7065  e other develope
+00001d20: 7273 2061 2062 6974 2068 6170 7069 6572  rs a bit happier
+00001d30: 2062 7920 7573 696e 6720 7468 6520 4a53   by using the JS
+00001d40: 4f4e 206f 7220 584d 4c20 7365 7269 616c  ON or XML serial
+00001d50: 697a 6174 696f 6e73 2e20 5468 650a 6d61  izations. The.ma
+00001d60: 696e 2062 656e 6566 6974 2074 6f20 7573  in benefit to us
+00001d70: 696e 6720 584d 4c20 6f72 204a 534f 4e20  ing XML or JSON 
+00001d80: 6973 2074 6861 7420 7468 6520 5554 4638  is that the UTF8
+00001d90: 2063 6861 7261 6374 6572 2065 6e63 6f64   character encod
+00001da0: 696e 6720 6973 2075 7365 642c 0a72 6174  ing is used,.rat
+00001db0: 6865 7220 7468 616e 2074 6865 2066 7275  her than the fru
+00001dc0: 7374 7261 7469 6e67 6c79 2061 7263 6861  stratingly archa
+00001dd0: 6963 204d 4152 4338 2065 6e63 6f64 696e  ic MARC8 encodin
+00001de0: 672e 2041 6c73 6f20 7468 6579 2077 696c  g. Also they wil
+00001df0: 6c20 6265 2061 626c 6520 746f 0a75 7365  l be able to.use
+00001e00: 2073 7461 6e64 6172 6420 4a53 4f4e 2061   standard JSON a
+00001e10: 6e64 2058 4d4c 2072 6561 6469 6e67 2f77  nd XML reading/w
+00001e20: 7269 7469 6e67 2074 6f6f 6c73 2074 6f20  riting tools to 
+00001e30: 6765 7420 6174 2074 6865 2064 6174 6120  get at the data 
+00001e40: 7468 6579 2077 616e 740a 696e 7374 6561  they want.instea
+00001e50: 6420 6f66 2073 6f6d 6520 6372 617a 7920  d of some crazy 
+00001e60: 4d41 5243 2070 726f 6365 7373 696e 6720  MARC processing 
+00001e70: 6c69 6272 6172 7920 6c69 6b65 2c20 6168  library like, ah
+00001e80: 656d 2c20 7079 6d61 7263 2e0a 0a2a 2a58  em, pymarc...**X
+00001e90: 4d4c 2a2a 0a0a 546f 2070 6172 7365 2061  ML**..To parse a
+00001ea0: 2066 696c 6520 6f66 204d 4152 4358 4d4c   file of MARCXML
+00001eb0: 2072 6563 6f72 6473 2079 6f75 2063 616e   records you can
+00001ec0: 3a0a 0a60 6060 7079 7468 6f6e 0a0a 6672  :..```python..fr
+00001ed0: 6f6d 2070 796d 6172 6320 696d 706f 7274  om pymarc import
+00001ee0: 2070 6172 7365 5f78 6d6c 5f74 6f5f 6172   parse_xml_to_ar
+00001ef0: 7261 790a 0a72 6563 6f72 6473 203d 2070  ray..records = p
+00001f00: 6172 7365 5f78 6d6c 5f74 6f5f 6172 7261  arse_xml_to_arra
+00001f10: 7928 2774 6573 742f 6261 7463 682e 786d  y('test/batch.xm
+00001f20: 6c27 290a 6060 600a 0a49 6620 796f 7520  l').```..If you 
+00001f30: 6861 7665 2061 206c 6172 6765 2058 4d4c  have a large XML
+00001f40: 2066 696c 6520 616e 6420 776f 756c 6420   file and would 
+00001f50: 7261 7468 6572 206e 6f74 2072 6561 6420  rather not read 
+00001f60: 7468 656d 2061 6c6c 2069 6e74 6f20 6d65  them all into me
+00001f70: 6d6f 7279 2079 6f75 0a63 616e 3a0a 0a60  mory you.can:..`
+00001f80: 6060 7079 7468 6f6e 0a0a 6672 6f6d 2070  ``python..from p
+00001f90: 796d 6172 6320 696d 706f 7274 206d 6170  ymarc import map
+00001fa0: 5f78 6d6c 0a0a 6465 6620 7072 696e 745f  _xml..def print_
+00001fb0: 7469 746c 6528 7229 3a0a 2020 2020 7072  title(r):.    pr
+00001fc0: 696e 7428 722e 7469 746c 6528 2929 0a0a  int(r.title())..
+00001fd0: 6d61 705f 786d 6c28 7072 696e 745f 7469  map_xml(print_ti
+00001fe0: 746c 652c 2027 7465 7374 2f62 6174 6368  tle, 'test/batch
+00001ff0: 2e78 6d6c 2729 0a60 6060 0a0a 416c 736f  .xml').```..Also
+00002000: 2c20 6966 2079 6f75 2070 7265 6665 7220  , if you prefer 
+00002010: 796f 7520 6361 6e20 7061 7373 2069 6e20  you can pass in 
+00002020: 6120 6669 6c65 206c 696b 6520 6f62 6a65  a file like obje
+00002030: 6374 2069 6e20 6164 6469 7469 6f6e 2074  ct in addition t
+00002040: 6f20 7468 6520 7061 7468 0a74 6f20 626f  o the path.to bo
+00002050: 7468 202a 6d61 705f 786d 6c2a 2061 6e64  th *map_xml* and
+00002060: 202a 7061 7273 655f 786d 6c5f 746f 5f61   *parse_xml_to_a
+00002070: 7272 6179 2a3a 0a0a 6060 6070 7974 686f  rray*:..```pytho
+00002080: 6e0a 6672 6f6d 2070 796d 6172 6320 696d  n.from pymarc im
+00002090: 706f 7274 2070 6172 7365 5f78 6d6c 5f74  port parse_xml_t
+000020a0: 6f5f 6172 7261 790a 0a72 6563 6f72 6473  o_array..records
+000020b0: 203d 2070 6172 7365 5f78 6d6c 5f74 6f5f   = parse_xml_to_
+000020c0: 6172 7261 7928 6f70 656e 2827 7465 7374  array(open('test
+000020d0: 2f62 6174 6368 2e78 6d6c 2729 290a 6060  /batch.xml')).``
+000020e0: 600a 0a2a 2a4a 534f 4e2a 2a0a 0a4a 534f  `..**JSON**..JSO
+000020f0: 4e20 7375 7070 6f72 7420 6973 2066 6169  N support is fai
+00002100: 726c 7920 6d69 6e69 6d61 6c20 696e 2074  rly minimal in t
+00002110: 6861 7420 796f 7520 6361 6e20 6361 6c6c  hat you can call
+00002120: 2061 2060 7079 6d61 7263 2e52 6563 6f72   a `pymarc.Recor
+00002130: 6460 2773 0a60 6173 5f6a 736f 6e28 2960  d`'s.`as_json()`
+00002140: 206d 6574 686f 6420 746f 2072 6574 7572   method to retur
+00002150: 6e20 4a53 4f4e 2066 6f72 2061 2067 6976  n JSON for a giv
+00002160: 656e 204d 4152 4320 5265 636f 7264 3a0a  en MARC Record:.
+00002170: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00002180: 7079 6d61 7263 2069 6d70 6f72 7420 4d41  pymarc import MA
+00002190: 5243 5265 6164 6572 0a0a 7769 7468 206f  RCReader..with o
+000021a0: 7065 6e28 2774 6573 742f 6f6e 652e 6461  pen('test/one.da
+000021b0: 7427 2c27 7262 2729 2061 7320 6668 3a0a  t','rb') as fh:.
+000021c0: 2020 2020 7265 6164 6572 203d 204d 4152      reader = MAR
+000021d0: 4352 6561 6465 7228 6668 290a 2020 2020  CReader(fh).    
+000021e0: 666f 7220 7265 636f 7264 2069 6e20 7265  for record in re
+000021f0: 6164 6572 3a0a 2020 2020 2020 2020 7072  ader:.        pr
+00002200: 696e 7428 7265 636f 7264 2e61 735f 6a73  int(record.as_js
+00002210: 6f6e 2869 6e64 656e 743d 3229 290a 6060  on(indent=2)).``
+00002220: 600a 0a60 6060 6a61 7661 7363 7269 7074  `..```javascript
+00002230: 0a7b 0a20 2022 6c65 6164 6572 223a 2022  .{.  "leader": "
+00002240: 3031 3036 3063 616d 2020 3232 3030 3238  01060cam  220028
+00002250: 3934 6120 3435 3030 222c 0a20 2022 6669  94a 4500",.  "fi
+00002260: 656c 6473 223a 205b 0a20 2020 207b 0a20  elds": [.    {. 
+00002270: 2020 2020 2022 3030 3122 3a20 2231 3137       "001": "117
+00002280: 3738 3530 3422 0a20 2020 207d 2c0a 2020  78504".    },.  
+00002290: 2020 7b0a 2020 2020 2020 2230 3130 223a    {.      "010":
+000022a0: 207b 0a20 2020 2020 2020 2022 696e 6431   {.        "ind1
+000022b0: 223a 2022 2022 2c0a 2020 2020 2020 2020  ": " ",.        
+000022c0: 2273 7562 6669 656c 6473 223a 205b 0a20  "subfields": [. 
+000022d0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000022e0: 2020 2020 2020 2022 6122 3a20 2220 2020         "a": "   
+000022f0: 3939 3034 3335 3831 2022 0a20 2020 2020  99043581 ".     
+00002300: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
+00002310: 2c0a 2020 2020 2020 2020 2269 6e64 3222  ,.        "ind2"
+00002320: 3a20 2220 220a 2020 2020 2020 7d0a 2020  : " ".      }.  
+00002330: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
+00002340: 2022 3130 3022 3a20 7b0a 2020 2020 2020   "100": {.      
+00002350: 2020 2269 6e64 3122 3a20 2231 222c 0a20    "ind1": "1",. 
+00002360: 2020 2020 2020 2022 7375 6266 6965 6c64         "subfield
+00002370: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+00002380: 7b0a 2020 2020 2020 2020 2020 2020 2261  {.            "a
+00002390: 223a 2022 4875 6e74 2c20 416e 6472 6577  ": "Hunt, Andrew
+000023a0: 2c22 0a20 2020 2020 2020 2020 207d 2c0a  ,".          },.
+000023b0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000023c0: 2020 2020 2020 2020 2264 223a 2022 3139          "d": "19
+000023d0: 3634 2d22 0a20 2020 2020 2020 2020 207d  64-".          }
+000023e0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+000023f0: 2020 2020 2269 6e64 3222 3a20 2220 220a      "ind2": " ".
+00002400: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00002410: 2020 207b 0a20 2020 2020 2022 3234 3522     {.      "245"
+00002420: 3a20 7b0a 2020 2020 2020 2020 2269 6e64  : {.        "ind
+00002430: 3122 3a20 2231 222c 0a20 2020 2020 2020  1": "1",.       
+00002440: 2022 7375 6266 6965 6c64 7322 3a20 5b0a   "subfields": [.
+00002450: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00002460: 2020 2020 2020 2020 2261 223a 2022 5468          "a": "Th
+00002470: 6520 7072 6167 6d61 7469 6320 7072 6f67  e pragmatic prog
+00002480: 7261 6d6d 6572 203a 220a 2020 2020 2020  rammer :".      
+00002490: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000024a0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000024b0: 6222 3a20 2266 726f 6d20 6a6f 7572 6e65  b": "from journe
+000024c0: 796d 616e 2074 6f20 6d61 7374 6572 202f  yman to master /
+000024d0: 220a 2020 2020 2020 2020 2020 7d2c 0a20  ".          },. 
+000024e0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000024f0: 2020 2020 2020 2022 6322 3a20 2241 6e64         "c": "And
+00002500: 7265 7720 4875 6e74 2c20 4461 7669 6420  rew Hunt, David 
+00002510: 5468 6f6d 6173 2e22 0a20 2020 2020 2020  Thomas.".       
+00002520: 2020 207d 0a20 2020 2020 2020 205d 2c0a     }.        ],.
+00002530: 2020 2020 2020 2020 2269 6e64 3222 3a20          "ind2": 
+00002540: 2234 220a 2020 2020 2020 7d0a 2020 2020  "4".      }.    
+00002550: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00002560: 3236 3022 3a20 7b0a 2020 2020 2020 2020  260": {.        
+00002570: 2269 6e64 3122 3a20 2220 222c 0a20 2020  "ind1": " ",.   
+00002580: 2020 2020 2022 7375 6266 6965 6c64 7322       "subfields"
+00002590: 3a20 5b0a 2020 2020 2020 2020 2020 7b0a  : [.          {.
+000025a0: 2020 2020 2020 2020 2020 2020 2261 223a              "a":
+000025b0: 2022 5265 6164 696e 672c 204d 6173 7320   "Reading, Mass 
+000025c0: 3a22 0a20 2020 2020 2020 2020 207d 2c0a  :".          },.
+000025d0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000025e0: 2020 2020 2020 2020 2262 223a 2022 4164          "b": "Ad
+000025f0: 6469 736f 6e2d 5765 736c 6579 2c22 0a20  dison-Wesley,". 
+00002600: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002610: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002620: 2020 2020 2263 223a 2022 3230 3030 2e22      "c": "2000."
+00002630: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
+00002640: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00002650: 2269 6e64 3222 3a20 2220 220a 2020 2020  "ind2": " ".    
+00002660: 2020 7d0a 2020 2020 7d2c 0a20 2020 207b    }.    },.    {
+00002670: 0a20 2020 2020 2022 3330 3022 3a20 7b0a  .      "300": {.
+00002680: 2020 2020 2020 2020 2269 6e64 3122 3a20          "ind1": 
+00002690: 2220 222c 0a20 2020 2020 2020 2022 7375  " ",.        "su
+000026a0: 6266 6965 6c64 7322 3a20 5b0a 2020 2020  bfields": [.    
+000026b0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000026c0: 2020 2020 2261 223a 2022 7878 6976 2c20      "a": "xxiv, 
+000026d0: 3332 3120 702e 203b 220a 2020 2020 2020  321 p. ;".      
+000026e0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000026f0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002700: 6322 3a20 2232 3420 636d 2e22 0a20 2020  c": "24 cm.".   
+00002710: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002720: 205d 2c0a 2020 2020 2020 2020 2269 6e64   ],.        "ind
+00002730: 3222 3a20 2220 220a 2020 2020 2020 7d0a  2": " ".      }.
+00002740: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00002750: 2020 2022 3530 3422 3a20 7b0a 2020 2020     "504": {.    
+00002760: 2020 2020 2269 6e64 3122 3a20 2220 222c      "ind1": " ",
+00002770: 0a20 2020 2020 2020 2022 7375 6266 6965  .        "subfie
+00002780: 6c64 7322 3a20 5b0a 2020 2020 2020 2020  lds": [.        
+00002790: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000027a0: 2261 223a 2022 496e 636c 7564 6573 2062  "a": "Includes b
+000027b0: 6962 6c69 6f67 7261 7068 6963 616c 2072  ibliographical r
+000027c0: 6566 6572 656e 6365 732e 220a 2020 2020  eferences.".    
+000027d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000027e0: 5d2c 0a20 2020 2020 2020 2022 696e 6432  ],.        "ind2
+000027f0: 223a 2022 2022 0a20 2020 2020 207d 0a20  ": " ".      }. 
+00002800: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+00002810: 2020 2236 3530 223a 207b 0a20 2020 2020    "650": {.     
+00002820: 2020 2022 696e 6431 223a 2022 2022 2c0a     "ind1": " ",.
+00002830: 2020 2020 2020 2020 2273 7562 6669 656c          "subfiel
+00002840: 6473 223a 205b 0a20 2020 2020 2020 2020  ds": [.         
+00002850: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002860: 6122 3a20 2243 6f6d 7075 7465 7220 7072  a": "Computer pr
+00002870: 6f67 7261 6d6d 696e 672e 220a 2020 2020  ogramming.".    
+00002880: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00002890: 5d2c 0a20 2020 2020 2020 2022 696e 6432  ],.        "ind2
+000028a0: 223a 2022 3022 0a20 2020 2020 207d 0a20  ": "0".      }. 
+000028b0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000028c0: 2020 2237 3030 223a 207b 0a20 2020 2020    "700": {.     
+000028d0: 2020 2022 696e 6431 223a 2022 3122 2c0a     "ind1": "1",.
+000028e0: 2020 2020 2020 2020 2273 7562 6669 656c          "subfiel
+000028f0: 6473 223a 205b 0a20 2020 2020 2020 2020  ds": [.         
+00002900: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002910: 6122 3a20 2254 686f 6d61 732c 2044 6176  a": "Thomas, Dav
+00002920: 6964 2c22 0a20 2020 2020 2020 2020 207d  id,".          }
+00002930: 2c0a 2020 2020 2020 2020 2020 7b0a 2020  ,.          {.  
+00002940: 2020 2020 2020 2020 2020 2264 223a 2022            "d": "
+00002950: 3139 3536 2d22 0a20 2020 2020 2020 2020  1956-".         
+00002960: 207d 0a20 2020 2020 2020 205d 2c0a 2020   }.        ],.  
+00002970: 2020 2020 2020 2269 6e64 3222 3a20 2220        "ind2": " 
+00002980: 220a 2020 2020 2020 7d0a 2020 2020 7d0a  ".      }.    }.
+00002990: 2020 5d0a 7d0a 6060 600a 0a49 6620 796f    ].}.```..If yo
+000029a0: 7520 7761 6e74 2074 6f20 7061 7273 6520  u want to parse 
+000029b0: 6120 6669 6c65 206f 6620 4d41 5243 4a53  a file of MARCJS
+000029c0: 4f4e 2072 6563 6f72 6473 2079 6f75 2063  ON records you c
+000029d0: 616e 3a0a 0a60 6060 7079 7468 6f6e 0a66  an:..```python.f
+000029e0: 726f 6d20 7079 6d61 7263 2069 6d70 6f72  rom pymarc impor
+000029f0: 7420 7061 7273 655f 6a73 6f6e 5f74 6f5f  t parse_json_to_
+00002a00: 6172 7261 790a 0a72 6563 6f72 6473 203d  array..records =
+00002a10: 2070 6172 7365 5f6a 736f 6e5f 746f 5f61   parse_json_to_a
+00002a20: 7272 6179 286f 7065 6e28 2774 6573 742f  rray(open('test/
+00002a30: 6261 7463 682e 6a73 6f6e 2729 290a 0a70  batch.json'))..p
+00002a40: 7269 6e74 2872 6563 6f72 6473 5b30 5d29  rint(records[0])
+00002a50: 0a60 6060 0a0a 6060 600a 3d4c 4452 2020  .```..```.=LDR  
+00002a60: 3030 3932 356e 6a6d 2020 3232 3030 3237  00925njm  220027
+00002a70: 3737 6120 3435 3030 0a3d 3030 3120 2035  77a 4500.=001  5
+00002a80: 3633 3732 3431 0a3d 3030 3320 2044 4c43  637241.=003  DLC
+00002a90: 0a3d 3030 3520 2031 3939 3230 3832 3630  .=005  199208260
+00002aa0: 3834 3033 362e 300a 3d30 3037 2020 7364  84036.0.=007  sd
+00002ab0: 7562 756d 656e 6e6d 706c 750a 3d30 3038  ubumennmplu.=008
+00002ac0: 2020 3931 3039 3236 7331 3935 375c 5c5c    910926s1957\\\
+00002ad0: 5c6e 7975 7575 6e5c 5c5c 5c5c 5c5c 5c5c  \nyuuun\\\\\\\\\
+00002ae0: 5c5c 5c5c 5c65 6e67 5c5c 0a3d 3031 3020  \\\\\eng\\.=010 
+00002af0: 205c 5c24 6120 2020 3931 3735 3833 3335   \\$a   91758335
+00002b00: 0a3d 3032 3820 2030 3024 6131 3235 3924  .=028  00$a1259$
+00002b10: 6241 746c 616e 7469 630a 3d30 3430 2020  bAtlantic.=040  
+00002b20: 5c5c 2461 444c 4324 6344 4c43 0a3d 3035  \\$aDLC$cDLC.=05
+00002b30: 3020 2030 3024 6141 746c 616e 7469 6320  0  00$aAtlantic 
+00002b40: 3132 3539 0a3d 3234 3520 2030 3424 6154  1259.=245  04$aT
+00002b50: 6865 2047 7265 6174 2052 6179 2043 6861  he Great Ray Cha
+00002b60: 726c 6573 2468 5b73 6f75 6e64 2072 6563  rles$h[sound rec
+00002b70: 6f72 6469 6e67 5d2e 0a3d 3236 3020 205c  ording]..=260  \
+00002b80: 5c24 614e 6577 2059 6f72 6b2c 204e 2e59  \$aNew York, N.Y
+00002b90: 2e20 3a24 6241 746c 616e 7469 632c 2463  . :$bAtlantic,$c
+00002ba0: 5b31 3935 373f 5d0a 3d33 3030 2020 5c5c  [1957?].=300  \\
+00002bb0: 2461 3120 736f 756e 6420 6469 7363 203a  $a1 sound disc :
+00002bc0: 2462 616e 616c 6f67 2c20 3333 2031 2f33  $banalog, 33 1/3
+00002bd0: 2072 706d 203b 2463 3132 2069 6e2e 0a3d   rpm ;$c12 in..=
+00002be0: 3531 3120 2030 5c24 6152 6179 2043 6861  511  0\$aRay Cha
+00002bf0: 726c 6573 2c20 7069 616e 6f20 2620 6365  rles, piano & ce
+00002c00: 6c65 7374 652e 0a3d 3530 3520 2030 5c24  leste..=505  0\$
+00002c10: 6154 6865 2052 6179 202d 2d20 4d79 206d  aThe Ray -- My m
+00002c20: 656c 616e 6368 6f6c 7920 6261 6279 202d  elancholy baby -
+00002c30: 2d20 426c 6163 6b20 636f 6666 6565 202d  - Black coffee -
+00002c40: 2d20 5468 6572 6527 7320 6e6f 2079 6f75  - There's no you
+00002c50: 202d 2d20 446f 6f64 6c69 6e27 202d 2d20   -- Doodlin' -- 
+00002c60: 5377 6565 7420 7369 7874 6565 6e20 6261  Sweet sixteen ba
+00002c70: 7273 202d 2d20 4920 7375 7272 656e 6465  rs -- I surrende
+00002c80: 7220 6465 6172 202d 2d20 556e 6465 6369  r dear -- Undeci
+00002c90: 6465 642e 0a3d 3530 3020 205c 5c24 6142  ded..=500  \\$aB
+00002ca0: 7269 6566 2072 6563 6f72 642e 0a3d 3635  rief record..=65
+00002cb0: 3020 205c 3024 614a 617a 7a24 7931 3935  0  \0$aJazz$y195
+00002cc0: 312d 3139 3630 2e0a 3d36 3530 2020 5c30  1-1960..=650  \0
+00002cd0: 2461 5069 616e 6f20 7769 7468 206a 617a  $aPiano with jaz
+00002ce0: 7a20 656e 7365 6d62 6c65 2e0a 3d37 3030  z ensemble..=700
+00002cf0: 2020 315c 2461 4368 6172 6c65 732c 2052    1\$aCharles, R
+00002d00: 6179 2c24 6431 3933 302d 2434 7072 660a  ay,$d1930-$4prf.
+00002d10: 6060 600a 0a53 7570 706f 7274 0a2d 2d2d  ```..Support.---
+00002d20: 2d2d 2d2d 0a0a 5468 6520 7079 6d61 7263  ----..The pymarc
+00002d30: 2064 6576 656c 6f70 6572 7320 656e 636f   developers enco
+00002d40: 7572 6167 6520 796f 7520 746f 206a 6f69  urage you to joi
+00002d50: 6e20 7468 6520 5b70 796d 6172 6320 476f  n the [pymarc Go
+00002d60: 6f67 6c65 0a47 726f 7570 5d28 6874 7470  ogle.Group](http
+00002d70: 3a2f 2f67 726f 7570 732e 676f 6f67 6c65  ://groups.google
+00002d80: 2e63 6f6d 2f67 726f 7570 2f70 796d 6172  .com/group/pymar
+00002d90: 6329 2069 6620 796f 7520 6e65 6564 2068  c) if you need h
+00002da0: 656c 702e 2020 416c 736f 2c20 706c 6561  elp.  Also, plea
+00002db0: 7365 0a66 6565 6c20 6672 6565 2074 6f20  se.feel free to 
+00002dc0: 7573 6520 5b69 7373 7565 2074 7261 636b  use [issue track
+00002dd0: 696e 675d 2868 7474 7073 3a2f 2f67 6974  ing](https://git
+00002de0: 6c61 622e 636f 6d2f 7079 6d61 7263 2f70  lab.com/pymarc/p
+00002df0: 796d 6172 632f 6973 7375 6573 2920 6f6e  ymarc/issues) on
+00002e00: 0a47 6974 4c61 6220 746f 2073 7562 6d69  .GitLab to submi
+00002e10: 7420 6665 6174 7572 6520 7265 7175 6573  t feature reques
+00002e20: 7473 206f 7220 6275 6720 7265 706f 7274  ts or bug report
+00002e30: 732e 2049 6620 796f 7527 7665 2067 6f74  s. If you've got
+00002e40: 2061 6e20 6974 6368 2074 6f0a 7363 7261   an itch to.scra
+00002e50: 7463 682c 2070 6c65 6173 6520 7363 7261  tch, please scra
+00002e60: 7463 6820 6974 2c20 616e 6420 7365 6e64  tch it, and send
+00002e70: 206d 6572 6765 2072 6571 7565 7374 7320   merge requests 
+00002e80: 6f6e 0a5b 4769 744c 6162 5d28 6874 7470  on.[GitLab](http
+00002e90: 3a2f 2f67 6974 6c61 622e 636f 6d2f 7079  ://gitlab.com/py
+00002ea0: 6d61 7263 2f70 796d 6172 6329 2e0a 0a49  marc/pymarc)...I
+00002eb0: 6620 796f 7520 7374 6172 7420 776f 726b  f you start work
+00002ec0: 696e 6720 7769 7468 204d 4152 4320 796f  ing with MARC yo
+00002ed0: 7520 6d61 7920 6665 656c 206c 696b 6520  u may feel like 
+00002ee0: 796f 7520 6e65 6564 206d 6f72 616c 2073  you need moral s
+00002ef0: 7570 706f 7274 0a69 6e20 6164 6469 7469  upport.in additi
+00002f00: 6f6e 2074 6f20 7465 6368 6e69 6361 6c20  on to technical 
+00002f10: 7375 7070 6f72 742e 2054 6865 0a5b 2363  support. The.[#c
+00002f20: 6f64 6534 6c69 625d 2869 7263 733a 2f2f  ode4lib](ircs://
+00002f30: 6972 632e 6c69 6265 7261 2e63 6861 742f  irc.libera.chat/
+00002f40: 636f 6465 346c 6962 2920 6368 616e 6e65  code4lib) channe
+00002f50: 6c20 6f6e 205b 4c69 6265 7261 5d28 6874  l on [Libera](ht
+00002f60: 7470 733a 2f2f 6c69 6265 7261 2e63 6861  tps://libera.cha
+00002f70: 742f 2920 6973 2061 2067 6f6f 6420 706c  t/) is a good pl
+00002f80: 6163 6520 666f 7220 626f 7468 2e0a       ace for both..
```

### Comparing `pymarc-4.2.2/README_pt_Br.md` & `pymarc-5.0.0/README_pt_Br.md`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/docs/source/conf.py` & `pymarc-5.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/docs/source/index.rst` & `pymarc-5.0.0/docs/source/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
 
 
 Release v\ |version|
 
 Pymarc is a Python 3 library for working with bibliographic data encoded in MARC21.
 
-Starting with version 4.0.0 it requires python 3.6 and up. It provides an API
+Starting with version 5.0.0 it requires python 3.7 and up. It provides an API
 for reading, writing and modifying MARC records. It was mostly designed to be
 an emergency eject seat, for getting your data assets out of MARC and into some
 kind of saner representation. However over the years it has been used to create
 and modify MARC records, since despite `repeated calls`_ for it to die as a
 format, MARC seems to be living quite happily as a zombie.
 
 Below are some common examples of how you might want to use pymarc. If
@@ -94,59 +94,74 @@
 `FatalReaderError` happens when reader can't determine record's boundaries in
 the data stream. To avoid data misinterpretation it stops.
 In case of other errors (wrong encodind etc.) reader continues to
 the next record.
 
 A pymarc.Record object has a few handy methods like title for
 getting at bits of a bibliographic record, others include: author,
-isbn, subjects, location, notes,
-physicaldescription, publisher, pubyear. But really, to work
-with MARC data you need to understand the numeric field tags and
-subfield codes that are used to designate various bits of information.
-There is a lot more hiding in a MARC record than these methods provide
-access to. For example the title method extracts the information
-from the 245 field, subfields a and b. You can access
-245a like so:
+isbn, subjects, location, notes, physical description, publisher,
+pubyear. But really, to work with MARC data you need to understand the
+numeric field tags and subfield codes that are used to designate
+various bits of information. There is a lot more hiding in a MARC
+record than these methods provide access to. For example the title
+method extracts the information from the 245 field, subfields a and b.
+You can access `245a` like so:
 
 .. code-block:: python
 
     print(record['245']['a'])
 
 Some fields like subjects can repeat. In cases like that you will want
-to use get_fields to get all of them as pymarc.Field objects,
+to use `get_fields` to get all of them as `pymarc.Field` objects,
 which you can then interact with further:
 
 .. code-block:: python
 
     for f in record.get_fields('650'):
         print(f)
 
-If you are new to MARC fields Understanding
-MARC (http://www.loc.gov/marc/umb/) is a pretty good primer, and the
-MARC 21 Formats (http://www.loc.gov/marc/marcdocz.html) page at the
+If you are new to MARC fields, "Understanding MARC"
+(http://www.loc.gov/marc/umb/) is a pretty good primer, and the
+"MARC 21 Formats" (http://www.loc.gov/marc/marcdocz.html) page at the
 Library of Congress is a good reference once you understand the basics.
 
+**Note:** New in v5.0.0, `Subfield` is used to create subfields.
+Prior to v5, subfields were constructed as a list of strings, e.g.,
+`[code, value, code, value]`. This has been changed to organize the
+subfields into a list of tuples, e.g., `[(code, value), (code, value)]`.
+The `Subfield` is implemented as a `NamedTuple` so that the tuples
+can be constructed as `Subfield(code=code, value=value)`. See the
+ code below for an example of how this is used.
+
+The old style of creating subfields is no longer supported. Passing
+a list of strings to the `subfields` parameter for the `Field` constructor
+will raise a `ValueError`.
+
+For convenience, a class method is provided to convert the legacy list of
+strings into a list of `Subfield`s. An example of how to do this is
+given below.
+
 Writing
 ~~~~~~~
 
 Here's an example of creating a record and writing it out to a file.
 
 .. code-block:: python
 
-    from pymarc import Record, Field
+    from pymarc import Record, Field, Subfield
 
     record = Record()
     record.add_field(
         Field(
             tag = '245',
             indicators = ['0','1'],
             subfields = [
-                'a', 'The pragmatic programmer : ',
-                'b', 'from journeyman to master /',
-                'c', 'Andrew Hunt, David Thomas.'
+                Subfield(code='a', value='The pragmatic programmer : '),
+                Subfield(code='b', value='from journeyman to master /'),
+                Subfield(code='c', value='Andrew Hunt, David Thomas.')
             ]))
     with open('file.dat', 'wb') as out:
         out.write(record.as_marc())
 
 Updating
 ~~~~~~~~
 
@@ -156,15 +171,15 @@
 .. code-block:: python
 
     from pymarc import MARCReader
 
     with open('test/marc.dat', 'rb') as fh:
        reader = MARCReader(fh)
        record = next(reader)
-       record['245']['a'] = 'The Zombie Programmer'
+       record['245']['a'] = 'The Zombie Programmer : '
     with open('file.dat', 'wb') as out:
        out.write(record.as_marc())
 
 JSON and XML
 ~~~~~~~~~~~~
 
 If you find yourself using MARC data a fair bit, and distributing it,
```

### Comparing `pymarc-4.2.2/pymarc/__init__.py` & `pymarc-5.0.0/pymarc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/pymarc/exceptions.py` & `pymarc-5.0.0/pymarc/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,17 +113,8 @@
 
     def __init__(self, field):
         """Initialize MissingLinkedFields with the `field` that lacks one or more target 880s."""
         super().__init__(field)
         self.field = field
 
     def __str__(self):
-        return (
-            self.field.tag
-            + " field includes a subfield 6 but no linked fields could be found."
-        )
-
-
-# This alias for FatalReaderError is here to correct a misspelling that was
-# introduced in v4.0.0. It can be removed in v5.0.0.
-
-FatalReaderEror = FatalReaderError
+        return f"{self.field.tag} field includes a subfield 6 but no linked fields could be found."
```

### Comparing `pymarc-4.2.2/pymarc/field.py` & `pymarc-5.0.0/pymarc/field.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,112 @@
 # This file is part of pymarc. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution and at
 # https://opensource.org/licenses/BSD-2-Clause. pymarc may be copied, modified,
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
 
-"""The pymarc.field file."""
+"""The pymarc field file."""
 
 import logging
 from collections import defaultdict
-from typing import List, Optional, Tuple, DefaultDict
+from typing import List, Optional, DefaultDict, NamedTuple, Iterator, Dict
 
 from pymarc.constants import SUBFIELD_INDICATOR, END_OF_FIELD
 from pymarc.marc8 import marc8_to_unicode
 
+Subfield = NamedTuple("Subfield", [("code", str), ("value", str)])
+
 
 class Field:
     """Field() pass in the field tag, indicators and subfields for the tag.
 
     .. code-block:: python
 
         field = Field(
             tag = '245',
             indicators = ['0','1'],
             subfields = [
-                'a', 'The pragmatic programmer : ',
-                'b', 'from journeyman to master /',
-                'c', 'Andrew Hunt, David Thomas.',
+                Subfield(code='a', value='The pragmatic programmer : '),
+                Subfield(code='b', value='from journeyman to master /'),
+                Subfield(code='c', value='Andrew Hunt, David Thomas.'),
             ])
 
     If you want to create a control field, don't pass in the indicators
     and use a data parameter rather than a subfields parameter:
 
     .. code-block:: python
 
         field = Field(tag='001', data='fol05731351')
     """
 
+    __slots__ = ("tag", "data", "indicators", "subfields", "__pos")
+
     def __init__(
         self,
         tag: str,
         indicators: Optional[List[str]] = None,
-        subfields: Optional[List[str]] = None,
-        data="",
+        subfields: Optional[List[Subfield]] = None,
+        data: str = "",
     ):
         """Initialize a field `tag`."""
         # attempt to normalize integer tags if necessary
         try:
-            self.tag = "%03i" % int(tag)
+            self.tag = f"{int(tag):03}"
         except ValueError:
-            self.tag = "%03s" % tag
+            self.tag = f"{tag}"
 
-        # assume controlfields are numeric only; replicates ruby-marc behavior
+        if subfields and isinstance(subfields[0], str):
+            raise ValueError(
+                """The subfield input no longer accepts strings, and should use Subfield.
+                   Please consult the documentation for details.
+                """
+            )
+
+        # assume control fields are numeric only; replicates ruby-marc behavior
         if self.tag < "010" and self.tag.isdigit():
             self.data = data
         else:
+            self.subfields: List[Subfield] = subfields or []
             self.indicators = [str(x) for x in (indicators or [])]
-            self.subfields = subfields or []
+
+    @classmethod
+    def convert_legacy_subfields(cls, subfields: List[str]) -> List[Subfield]:
+        """
+        Converts older-style subfield lists into Subfield lists.
+
+        Converts the old-style list of strings into a list of Subfields.
+        As a class method this does not actually set any fields; it simply
+        takes a list of strings and returns a list of Subfields.
+
+        .. code-block:: python
+
+            legacy_fields: list[str] = ['a', 'The pragmatic programmer : ',
+                                        'b', 'from journeyman to master /',
+                                        'c', 'Andrew Hunt, David Thomas']
+
+            coded_fields: list[Subfield] = Field.convert_legacy_subfields(legacy_fields)
+
+            myfield = Field(
+                tag="245",
+                indicators = ['0','1'],
+                subfields=coded_fields
+            )
+
+        :param subfields: A list of [code, value, code, value]
+        :return: A list of Subfield named tuples
+        """
+        # Make an iterator out of the incoming subfields.
+        subf_it: Iterator[str] = iter(subfields)
+        # This creates a tuple based on the next value of the iterator. In this case,
+        # the subfield code will be the first element, and then the subfield value
+        # will be the second.
+        subf = zip(subf_it, subf_it)
+        # Create a coded subfield tuple of each (code, value) item in the incoming
+        # subfields.
+        return [Subfield._make(t) for t in subf]
 
     def __iter__(self):
         self.__pos = 0
         return self
 
     def __str__(self) -> str:
         """String representation of the field.
@@ -72,194 +119,225 @@
         newlines to DOS format ('CRLF').
 
         [1] http://www.loc.gov/marc/makrbrkr.html#mechanics
         [2] http://search.cpan.org/~eijabb/MARC-File-MARCMaker/
         [3] http://www.loc.gov/marc/mnemonics.html
         """
         if self.is_control_field():
-            text = "=%s  %s" % (self.tag, self.data.replace(" ", "\\"))
+            _data: str = self.data.replace(" ", "\\")
+            return f"={self.tag}  {_data}"
         else:
-            text = "=%s  " % (self.tag)
+            _ind = []
+            _subf = []
+
             for indicator in self.indicators:
                 if indicator in (" ", "\\"):
-                    text += "\\"
+                    _ind.append("\\")
                 else:
-                    text += "%s" % indicator
-            for subfield in self:
-                text += "$%s%s" % subfield
-        return text
+                    _ind.append(f"{indicator}")
+
+            for subfield in self.subfields:
+                _subf.append(f"${subfield.code}{subfield.value}")
 
-    def __getitem__(self, subfield) -> Optional[str]:
+            return f"={self.tag}  {''.join(_ind)}{''.join(_subf)}"
+
+    def get(self, code: str, default=None):
+        """A dict-like get method with a default value.
+
+        Implements a non-raising getter for a subfield code that will
+        return the value of the first subfield whose code is `key`.
+        """
+        if code not in self:
+            return default
+        return self[code]
+
+    def __getitem__(self, code: str) -> str:
         """Retrieve the first subfield with a given subfield code in a field.
 
+        Raises KeyError if `code` is not in the Field.
+
         .. code-block:: python
 
             field['a']
-
-        Handy for quick lookups.
         """
-        subfields = self.get_subfields(subfield)
-        return subfields[0] if subfields else None
+        if code not in self:
+            raise KeyError
+
+        for subf in self.subfields:
+            if subf.code == code:
+                return subf.value
+        # This should not occur, but just incase we've looped through
+        # and couldn't find the code, default to raising KeyError.
+        raise KeyError
 
-    def __contains__(self, subfield: Optional[str]) -> bool:
+    def __contains__(self, subfield: str) -> bool:
         """Allows a shorthand test of field membership.
 
         .. code-block:: python
 
             'a' in field
 
         """
-        return bool(self.get_subfields(subfield))
+        for s in self.subfields:
+            if s.code == subfield:
+                return True
+        return False
 
     def __setitem__(self, code: str, value: str) -> None:
         """Set the values of the subfield code in a field.
 
         .. code-block:: python
 
             field['a'] = 'value'
 
         Raises KeyError if there is more than one subfield code.
         """
-        subfields = self.get_subfields(code)
-        if len(subfields) > 1:
-            raise KeyError("more than one code '%s'" % code)
-        elif len(subfields) == 0:
-            raise KeyError("no code '%s'" % code)
-        num_code = len(self.subfields) // 2
-        while num_code >= 0:
-            if self.subfields[(num_code * 2) - 2] == code:
-                self.subfields[(num_code * 2) - 1] = value
+        num_subfields: int = [x.code for x in self.subfields].count(code)
+
+        if num_subfields > 1:
+            raise KeyError(f"more than one code '{code}'")
+        elif num_subfields == 0:
+            raise KeyError(f"no code '{code}'")
+
+        for idx, subf in enumerate(self.subfields):
+            if subf.code == code:
+                new_val = Subfield(code=subf.code, value=value)
+                self.subfields[idx] = new_val
                 break
-            num_code -= 1
 
-    def __next__(self) -> Tuple[str, str]:
+    def __next__(self) -> Subfield:
         if not hasattr(self, "subfields"):
             raise StopIteration
-        while self.__pos < len(self.subfields):
-            subfield = (self.subfields[self.__pos], self.subfields[self.__pos + 1])
-            self.__pos += 2
-            return subfield
-        raise StopIteration
+
+        try:
+            subfield = self.subfields[self.__pos]
+            self.__pos += 1
+            return subfield  # type: ignore
+        except IndexError:
+            raise StopIteration
 
     def value(self) -> str:
         """Returns the field as a string w/ tag, indicators, and subfield indicators."""
         if self.is_control_field():
             return self.data
-        return " ".join(subfield[1].strip() for subfield in self)
+        return " ".join(subfield.value.strip() for subfield in self.subfields)
 
     def get_subfields(self, *codes) -> List[str]:
         """Get subfields matching `codes`.
 
         get_subfields() accepts one or more subfield codes and returns
         a list of subfield values.  The order of the subfield values
         in the list will be the order that they appear in the field.
 
         .. code-block:: python
 
             print(field.get_subfields('a'))
             print(field.get_subfields('a', 'b', 'z'))
         """
-        return [subfield[1] for subfield in self if subfield[0] in codes]
+        return [subfield.value for subfield in self.subfields if subfield.code in codes]
 
     def add_subfield(self, code: str, value: str, pos=None) -> None:
         """Adds a subfield code/value to the end of a field or at a position (pos).
 
+        If pos is not supplied or out of range, the subfield will be added at the end.
+
         .. code-block:: python
 
             field.add_subfield('u', 'http://www.loc.gov')
             field.add_subfield('u', 'http://www.loc.gov', 0)
-
-        If pos is not supplied or out of range, the subfield will be added at the end.
         """
-        append = pos is None or (pos + 1) * 2 > len(self.subfields)
+        append: bool = pos is None or pos > len(self.subfields)
+        insertable: Subfield = Subfield(code=code, value=value)
 
         if append:
-            self.subfields.append(code)
-            self.subfields.append(value)
+            self.subfields.append(insertable)
         else:
-            i = pos * 2
-            self.subfields.insert(i, code)
-            self.subfields.insert(i + 1, value)
+            self.subfields.insert(pos, insertable)
 
     def delete_subfield(self, code: str) -> Optional[str]:
         """Deletes the first subfield with the specified 'code' and returns its value.
 
         .. code-block:: python
 
             value = field.delete_subfield('a')
 
         If no subfield is found with the specified code None is returned.
         """
-        try:
-            codes = self.subfields[0::2]
-            index = codes.index(code) * 2
-            value = self.subfields.pop(index + 1)
-            self.subfields.pop(index)
-            return value
-        except ValueError:
+        if code not in self:
             return None
 
-    def subfields_as_dict(self) -> DefaultDict[str, list]:
+        index: int = [s.code for s in self.subfields].index(code)
+        whole_field: Subfield = self.subfields.pop(index)
+
+        return whole_field.value
+
+    def subfields_as_dict(self) -> Dict[str, List]:
         """Returns the subfields as a dictionary.
 
         The dictionary is a mapping of subfield codes and values. Since
         subfield codes can repeat the values are a list.
         """
-        keys = self.subfields[0::2]
-        vals = self.subfields[1::2]
-        subs: DefaultDict[str, list] = defaultdict(list)
-        for k, v in zip(keys, vals):
-            subs[k].append(v)
-        return subs
+        subs: DefaultDict[str, List] = defaultdict(list)
+        for field in self.subfields:
+            subs[field.code].append(field.value)
+        return dict(subs)
 
     def is_control_field(self) -> bool:
         """Returns true or false if the field is considered a control field.
 
         Control fields lack indicators and subfields.
         """
         return self.tag < "010" and self.tag.isdigit()
 
     def linkage_occurrence_num(self) -> Optional[str]:
         """Return the 'occurrence number' part of subfield 6, or None if not present."""
-        ocn = self["6"] or ""
+        ocn = self.get("6", "")
         return ocn.split("-")[1].split("/")[0] if ocn else None
 
     def as_marc(self, encoding: str) -> bytes:
         """Used during conversion of a field to raw marc."""
         if self.is_control_field():
-            return (self.data + END_OF_FIELD).encode(encoding)
-        marc = self.indicator1 + self.indicator2
-        for subfield in self:
-            marc += SUBFIELD_INDICATOR + subfield[0] + subfield[1]
+            return f"{self.data}{END_OF_FIELD}".encode(encoding)
 
-        return (marc + END_OF_FIELD).encode(encoding)
+        _subf = []
+        for subfield in self.subfields:
+            _subf.append(f"{SUBFIELD_INDICATOR}{subfield.code}{subfield.value}")
+
+        return (
+            f"{self.indicator1}{self.indicator2}{''.join(_subf)}{END_OF_FIELD}".encode(
+                encoding
+            )
+        )
 
     # alias for backwards compatibility
     as_marc21 = as_marc
 
     def format_field(self) -> str:
         """Returns the field as a string w/ tag, indicators, and subfield indicators.
 
         Like :func:`Field.value() <pymarc.field.Field.value>`, but prettier
         (adds spaces, formats subject headings).
         """
         if self.is_control_field():
             return self.data
-        fielddata = ""
-        for subfield in self:
-            if subfield[0] == "6":
+
+        field_data: str = ""
+
+        for subfield in self.subfields:
+            if subfield.code == "6":
                 continue
+
             if not self.is_subject_field():
-                fielddata += " %s" % subfield[1]
+                field_data += f" {subfield.value}"
             else:
-                if subfield[0] not in ("v", "x", "y", "z"):
-                    fielddata += " %s" % subfield[1]
+                if subfield.code not in ("v", "x", "y", "z"):
+                    field_data += f" {subfield.value}"
                 else:
-                    fielddata += " -- %s" % subfield[1]
-        return fielddata.strip()
+                    field_data += f" -- {subfield.value}"
+        return field_data.strip()
 
     def is_subject_field(self) -> bool:
         """Returns True or False if the field is considered a subject field.
 
         Used by :func:`format_field() <pymarc.field.Field.format_field>` .
         """
         return self.tag.startswith("6")
@@ -282,35 +360,38 @@
     @indicator2.setter
     def indicator2(self, value: str) -> None:
         """Indicator 2 (setter)."""
         self.indicators[1] = value
 
 
 class RawField(Field):
-    """MARC field that keeps data in raw, undecoded byte strings.
+    """MARC field that keeps data in raw, un-decoded byte strings.
 
     Should only be used when input records are wrongly encoded.
     """
 
     def as_marc(self, encoding: Optional[str] = None):
-        """Used during conversion of a field to raw marc."""
+        """Used during conversion of a field to raw MARC."""
         if encoding is not None:
             logging.warning("Attempt to force a RawField into encoding %s", encoding)
         if self.is_control_field():
-            return self.data + END_OF_FIELD.encode("ascii")
-        marc = self.indicator1.encode("ascii") + self.indicator2.encode("ascii")
-        for subfield in self:
+            return self.data + END_OF_FIELD.encode("ascii")  # type: ignore
+        marc: bytes = self.indicator1.encode("ascii") + self.indicator2.encode("ascii")
+        for subfield in self.subfields:
             marc += (
                 SUBFIELD_INDICATOR.encode("ascii")
-                + subfield[0].encode("ascii")
-                + subfield[1]
+                + subfield.code.encode("ascii")
+                + subfield.value  # type: ignore
             )
         return marc + END_OF_FIELD.encode("ascii")
 
 
 def map_marc8_field(f: Field) -> Field:
     """Map MARC8 field."""
     if f.is_control_field():
         f.data = marc8_to_unicode(f.data)
     else:
-        f.subfields = [marc8_to_unicode(subfield) for subfield in f.subfields]
+        f.subfields = [
+            Subfield(subfield.code, marc8_to_unicode(subfield.value))
+            for subfield in f.subfields
+        ]
     return f
```

### Comparing `pymarc-4.2.2/pymarc/leader.py` & `pymarc-5.0.0/pymarc/leader.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,207 +84,201 @@
 
     def _replace_values(self, position: int, value: str) -> None:
         """Replaces the values in the leader at `position` by `value`."""
         if position < 0:
             raise IndexError("Position must be positive")
         after = position + len(value)
         if after > LEADER_LEN:
-            raise BadLeaderValue(
-                "%s is too long to be inserted at %d" % (value, position)
-            )
+            raise BadLeaderValue(f"{value} is too long to be inserted at {position}")
         self.leader = self.leader[:position] + value + self.leader[after:]
 
     @property
     def record_length(self) -> str:
         """Record length (00-04)."""
         return self.leader[:5]
 
     @record_length.setter
     def record_length(self, value: str) -> None:
         """Record length (00-04)."""
         if len(value) != 5:
-            raise BadLeaderValue("Record length is 4 chars field, got %s" % value)
+            raise BadLeaderValue(f"Record length is 4 chars field, got {value}")
         self._replace_values(position=0, value=value)
 
     @property
     def record_status(self) -> str:
         """Record status (05)."""
         return self.leader[5]
 
     @record_status.setter
     def record_status(self, value: str) -> None:
         """Record status (05)."""
         if len(value) != 1:
-            raise BadLeaderValue("Record status is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Record status is 1 char field, got {value}")
         self._replace_values(position=5, value=value)
 
     @property
     def type_of_record(self) -> str:
         """Type of record (06)."""
         return self.leader[6]
 
     @type_of_record.setter
     def type_of_record(self, value: str) -> None:
         """Type of record (06)."""
         if len(value) != 1:
-            raise BadLeaderValue("Type of record is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Type of record is 1 char field, got {value}")
         self._replace_values(position=6, value=value)
 
     @property
     def bibliographic_level(self) -> str:
         """Bibliographic level (07)."""
         return self.leader[7]
 
     @bibliographic_level.setter
     def bibliographic_level(self, value: str) -> None:
         """Bibliographic level (07)."""
         if len(value) != 1:
-            raise BadLeaderValue("Bibliographic level is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Bibliographic level is 1 char field, got {value}")
         self._replace_values(position=7, value=value)
 
     @property
     def type_of_control(self) -> str:
         """Type of control (08)."""
         return self.leader[8]
 
     @type_of_control.setter
     def type_of_control(self, value: str) -> None:
         """Type of control (08)."""
         if len(value) != 1:
-            raise BadLeaderValue("Type of control is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Type of control is 1 char field, got {value}")
         self._replace_values(position=8, value=value)
 
     @property
     def coding_scheme(self) -> str:
         """Character coding scheme (09)."""
         return self.leader[9]
 
     @coding_scheme.setter
     def coding_scheme(self, value: str) -> None:
         """Character coding scheme (09)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Character coding scheme is 1 char field, got %s" % value
+                f"Character coding scheme is 1 char field, got {value}"
             )
         self._replace_values(position=9, value=value)
 
     @property
     def indicator_count(self) -> str:
         """Indicator count (10)."""
         return self.leader[10]
 
     @indicator_count.setter
     def indicator_count(self, value: str) -> None:
         """Indicator count (10)."""
         if len(value) != 1:
-            raise BadLeaderValue("Indicator count is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Indicator count is 1 char field, got {value}")
         self._replace_values(position=10, value=value)
 
     @property
     def subfield_code_count(self) -> str:
         """Subfield code count (11)."""
         return self.leader[11]
 
     @subfield_code_count.setter
     def subfield_code_count(self, value: str) -> None:
         """Subfield code count (11)."""
         if len(value) != 1:
-            raise BadLeaderValue("Subfield code count is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Subfield code count is 1 char field, got {value}")
         self._replace_values(position=11, value=value)
 
     @property
     def base_address(self) -> str:
         """Base address of data (12-16)."""
         return self.leader[12:17]
 
     @base_address.setter
     def base_address(self, value: str) -> None:
         """Base address of data (12-16)."""
         if len(value) != 5:
-            raise BadLeaderValue(
-                "Base address of data is 4 chars field, got %s" % value
-            )
+            raise BadLeaderValue(f"Base address of data is 4 chars field, got {value}")
         self._replace_values(position=12, value=value)
 
     @property
     def encoding_level(self) -> str:
         """Encoding level (17)."""
         return self.leader[17]
 
     @encoding_level.setter
     def encoding_level(self, value: str) -> None:
         """Encoding level (17)."""
         if len(value) != 1:
-            raise BadLeaderValue("Encoding level is 1 char field, got %s" % value)
+            raise BadLeaderValue(f"Encoding level is 1 char field, got {value}")
         self._replace_values(position=17, value=value)
 
     @property
     def cataloging_form(self) -> str:
         """Descriptive cataloging form (18)."""
         return self.leader[18]
 
     @cataloging_form.setter
     def cataloging_form(self, value: str) -> None:
         """Descriptive cataloging form (18)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Descriptive cataloging form is 1 char field, got %s" % value
+                f"Descriptive cataloging form is 1 char field, got {value}"
             )
         self._replace_values(position=18, value=value)
 
     @property
     def multipart_ressource(self) -> str:
         """Multipart resource record level (19)."""
         return self.leader[19]
 
     @multipart_ressource.setter
     def multipart_ressource(self, value: str) -> None:
         """Multipart resource record level (19)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Multipart resource record level is 1 char field, got %s" % value
+                f"Multipart resource record level is 1 char field, got {value}"
             )
         self._replace_values(position=19, value=value)
 
     @property
     def length_of_field_length(self) -> str:
         """Length of the length-of-field portion (20)."""
         return self.leader[20]
 
     @length_of_field_length.setter
     def length_of_field_length(self, value: str) -> None:
         """Length of the length-of-field portion (20)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Length of the length-of-field portion is 1 char field, got %s" % value
+                f"Length of the length-of-field portion is 1 char field, got {value}"
             )
         self._replace_values(position=20, value=value)
 
     @property
     def starting_character_position_length(self) -> str:
         """Length of the starting-character-position portion (21)."""
         return self.leader[21]
 
     @starting_character_position_length.setter
     def starting_character_position_length(self, value: str) -> None:
         """Length of the starting-character-position portion (21)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Length of the starting-character-position portion is 1 char field, got %s"
-                % value
+                f"Length of the starting-character-position portion is 1 char field, got {value}"
             )
         self._replace_values(position=21, value=value)
 
     @property
     def implementation_defined_length(self) -> str:
         """Length of the implementation-defined portion (22)."""
         return self.leader[22]
 
     @implementation_defined_length.setter
     def implementation_defined_length(self, value: str) -> None:
         """Length of the starting-character-position portion (22)."""
         if len(value) != 1:
             raise BadLeaderValue(
-                "Length of the implementation-defined portion is 1 char field, got %s"
-                % value
+                f"Length of the implementation-defined portion is 1 char field, got {value}"
             )
         self._replace_values(position=22, value=value)
```

### Comparing `pymarc-4.2.2/pymarc/marc8.py` & `pymarc-5.0.0/pymarc/marc8.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,15 @@
                     # we can short circuit because we know these mappings
                     # won't be involved in combinings.  (i hope?)
                     continue
                 except KeyError:
                     pass
                 if not self.quiet:
                     sys.stderr.write(
-                        "Unable to parse character 0x%x in g0=%s g1=%s\n"
-                        % (code_point, self.g0, self.g1)
+                        f"Unable to parse character 0x{code_point:x} in g0={self.g0} g1={self.g1}\n"
                     )
                 uni = ord(" ")
                 cflag = False
 
             if cflag:
                 combinings.append(chr(uni))
             else:
```

### Comparing `pymarc-4.2.2/pymarc/marc8_mapping.py` & `pymarc-5.0.0/pymarc/marc8_mapping.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/pymarc/marcjson.py` & `pymarc-5.0.0/pymarc/marcjson.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # file.
 
 """From JSON to MARC21."""
 
 from pymarc import Field, Record, JSONReader
 
 
-class JsonHandler:
+class JSONHandler:
     """Handle JSON."""
 
     def __init__(self):
         """Init."""
         self.records = []
         self._record = None
         self._field = None
@@ -59,9 +59,9 @@
         """Append `record` to `self.records`."""
         self.records.append(record)
 
 
 def parse_json_to_array(json_file):
     """JSON to elements."""
     json_reader = JSONReader(json_file)
-    handler = JsonHandler()
+    handler = JSONHandler()
     return handler.elements(json_reader.records)
```

### Comparing `pymarc-4.2.2/pymarc/marcxml.py` & `pymarc-5.0.0/pymarc/marcxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,15 @@
             self._field.data = text
             self._record.add_field(self._field)
             self._field = None
         elif element == "datafield":
             self._record.add_field(self._field)
             self._field = None
         elif element == "subfield":
-            self._field.subfields.append(self._subfield_code)
-            self._field.subfields.append(text)
+            self._field.add_subfield(self._subfield_code, text)
             self._subfield_code = None
 
         self._text = []
 
     def characters(self, chars):
         """Append `chars` to `_text`."""
         self._text.append(chars)
@@ -181,11 +180,11 @@
         else:
             data_field = ET.SubElement(root, "datafield")
             data_field.set("ind1", field.indicators[0])
             data_field.set("ind2", field.indicators[1])
             data_field.set("tag", field.tag)
             for subfield in field:
                 data_subfield = ET.SubElement(data_field, "subfield")
-                data_subfield.set("code", subfield[0])
-                data_subfield.text = translate(subfield[1])
+                data_subfield.set("code", subfield.code)
+                data_subfield.text = translate(subfield.value)
 
     return root
```

### Comparing `pymarc-4.2.2/pymarc/reader.py` & `pymarc-5.0.0/pymarc/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import json
 
 from io import IOBase, BytesIO, StringIO
 from typing import Callable, BinaryIO, IO, Iterator, Union
 
 from pymarc.constants import END_OF_RECORD
-from pymarc import Record, Field
+from pymarc import Record, Field, Subfield
 from pymarc import exceptions
 
 
 class Reader:
     """A base class for all iterating readers in the pymarc package."""
 
     def __iter__(self):
@@ -46,16 +46,19 @@
     If you would like to have your Record object contain unicode strings
     use the to_unicode parameter:
 
     .. code-block:: python
 
         reader = MARCReader(open('file.dat', 'rb'), to_unicode=True)
 
-    This will decode from MARC-8 or UTF-8 depending on the value in the
-    MARC leader at position 9.
+    This will decode from MARC-8 or utf-8 depending on the value in the
+    MARC leader at position 9. Upon serialization of the Record object to MARC21,
+    the resulting output will be utf-8 encoded and the value in the MARC leader
+    at position 9 will be set appropriately to indicate the change of
+    character encoding.
 
     If you find yourself in the unfortunate position of having data that
     is utf-8 encoded without the leader set appropriately you can use
     the force_utf8 parameter:
 
     .. code-block:: python
 
@@ -138,45 +141,45 @@
     def close(self) -> None:
         """Close the handle."""
         self.file_handle.close()
 
     def __next__(self):
         """Read and parse the next record."""
         if self._current_exception:
-            if isinstance(self._current_exception, exceptions.FatalReaderEror):
+            if isinstance(self._current_exception, exceptions.FatalReaderError):
                 raise StopIteration
 
         self._current_chunk = None
         self._current_exception = None
 
         self._current_chunk = first5 = self.file_handle.read(5)
         if not first5:
             raise StopIteration
 
         if len(first5) < 5:
             self._current_exception = exceptions.TruncatedRecord()
-            return
+            return None
 
         try:
             length = int(first5)
         except ValueError:
             self._current_exception = exceptions.RecordLengthInvalid()
-            return
+            return None
 
         chunk = self.file_handle.read(length - 5)
         chunk = first5 + chunk
         self._current_chunk = chunk
 
         if len(self._current_chunk) < length:
             self._current_exception = exceptions.TruncatedRecord()
-            return
+            return None
 
         if self._current_chunk[-1] != ord(END_OF_RECORD):
             self._current_exception = exceptions.EndOfRecordNotFound()
-            return
+            return None
 
         try:
             return Record(
                 chunk,
                 to_unicode=self.to_unicode,
                 force_utf8=self.force_utf8,
                 hide_utf8_warnings=self.hide_utf8_warnings,
@@ -246,15 +249,15 @@
         for field in jobj["fields"]:
             k, v = list(field.items())[0]
             if "subfields" in v and hasattr(v, "update"):
                 # flatten m-i-j dict to list in pymarc
                 subfields: list = []
                 for sub in v["subfields"]:
                     for code, value in sub.items():
-                        subfields.extend((code, value))
+                        subfields.append(Subfield(code=code, value=value))
                 fld = Field(
                     tag=k, subfields=subfields, indicators=[v["ind1"], v["ind2"]]
                 )
             else:
                 fld = Field(tag=k, data=v)
             rec.add_field(fld)
         return rec
```

### Comparing `pymarc-4.2.2/pymarc/record.py` & `pymarc-5.0.0/pymarc/record.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is part of pymarc. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution and at
 # https://opensource.org/licenses/BSD-2-Clause. pymarc may be copied, modified,
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
 
 """Pymarc Record."""
-from itertools import zip_longest
 import json
 import logging
 import re
 import unicodedata
 import warnings
 from typing import List, Optional, Dict, Tuple, Any, Pattern
 
@@ -26,20 +25,20 @@
     TruncatedRecord,
 )
 from pymarc.field import (
     END_OF_FIELD,
     SUBFIELD_INDICATOR,
     Field,
     RawField,
+    Subfield,
     map_marc8_field,
 )
 from pymarc.leader import Leader
 from pymarc.marc8 import marc8_to_unicode
 
-
 isbn_regex: Pattern = re.compile(r"([0-9\-xX]+)")
 
 
 class Record:
     """A class for representing a MARC record.
 
     Each Record object is made up of multiple Field objects. You'll probably want to look
@@ -50,17 +49,17 @@
 
     .. code-block:: python
 
         field = Field(
             tag = '245',
             indicators = ['0','1'],
             subfields = [
-                'a', 'The pragmatic programmer : ',
-                'b', 'from journeyman to master /',
-                'c', 'Andrew Hunt, David Thomas.',
+                Subfield(code='a', value='The pragmatic programmer : '),
+                Subfield(code='b', value='from journeyman to master /'),
+                Subfield(code='c', value='Andrew Hunt, David Thomas.'),
             ])
 
         record.add_field(field)
 
     Or creating a record from a chunk of MARC in transmission format:
 
     .. code-block:: python
@@ -73,14 +72,16 @@
 
         raw = record.as_marc()
 
     You'll normally want to use a MARCReader object to iterate through
     MARC records in a file.
     """
 
+    __slots__ = ("leader", "fields", "pos", "force_utf8", "to_unicode", "__pos")
+
     def __init__(
         self,
         data: str = "",
         to_unicode: bool = True,
         force_utf8: bool = False,
         hide_utf8_warnings: bool = False,
         utf8_handling: str = "strict",
@@ -88,14 +89,15 @@
         file_encoding: str = "iso8859-1",
     ) -> None:
         """Initialize a Record."""
         self.leader: Any = Leader(leader[0:10] + "22" + leader[12:20] + "4500")
         self.fields: List = list()
         self.pos: int = 0
         self.force_utf8: bool = force_utf8
+        self.to_unicode: bool = to_unicode
         if len(data) > 0:
             self.decode_marc(
                 data,
                 to_unicode=to_unicode,
                 force_utf8=force_utf8,
                 hide_utf8_warnings=hide_utf8_warnings,
                 utf8_handling=utf8_handling,
@@ -106,40 +108,67 @@
 
     def __str__(self) -> str:
         """Will return a prettified version of the record in MARCMaker format.
 
         See :func:`Field.__str__() <pymarc.record.Field.__str__>` for more information.
         """
         # join is significantly faster than concatenation
-        text_list: List = ["=LDR  %s" % self.leader]
+        text_list: List = [f"=LDR  {self.leader}"]
         text_list.extend([str(field) for field in self.fields])
         text: str = "\n".join(text_list) + "\n"
         return text
 
-    def __getitem__(self, tag: str) -> Optional[Field]:
+    def get(self, tag: str, default: Optional[Field] = None) -> Optional[Field]:
+        """Implements a dict-like get with a default value.
+
+        If `tag` is not found, then the default value will be returned.
+        The default value should be a Field instance.
+
+        .. code-block:: python
+            # returns None if 999 not in record.
+            record.get('999')
+            # returns the default if 999 not in record.
+            record.get('999', Field(tag="999", indicators=[" ", " "]))
+
+
+        """
+        try:
+            return self[tag]
+        except KeyError:
+            return default
+
+    def __getitem__(self, tag: str) -> Field:
         """Allows a shorthand lookup by tag.
 
+        Follows Python behavior and raises KeyError if `tag` is not in the record.
+
         .. code-block:: python
 
             record['245']
         """
-        fields = self.get_fields(tag)
-        if len(fields) > 0:
-            return fields[0]
-        return None
+        if tag not in self:
+            raise KeyError
+
+        fields: List[Field] = self.get_fields(tag)
+        if len(fields) == 0:
+            raise KeyError
+
+        return fields[0]
 
     def __contains__(self, tag: str) -> bool:
         """Allows a shorthand test of tag membership.
 
         .. code-block:: python
 
             '245' in record
         """
-        fields = self.get_fields(tag)
-        return len(fields) > 0
+        for f in self.fields:
+            if f.tag == tag:
+                return True
+        return False
 
     def __iter__(self):
         self.__pos = 0
         return self
 
     def __next__(self) -> Field:
         if self.__pos >= len(self.fields):
@@ -175,15 +204,15 @@
         """
         for f in fields:
             if len(self.fields) == 0 or not f.tag.isdigit():
                 self.fields.append(f)
                 continue
             self._sort_fields(f, "ordered")
 
-    def _sort_fields(self, field: Field, mode: str):
+    def _sort_fields(self, field: Field, mode: str) -> None:
         """Sort fields by `mode`."""
         if mode == "grouped":
             tag = int(field.tag[0])
         else:
             tag = int(field.tag)
 
         i, last_tag = 0, 0
@@ -363,16 +392,18 @@
                     if to_unicode:
                         if self.leader[9] == "a" or force_utf8:
                             data = data.decode("utf-8", utf8_handling)
                         elif encoding == "iso8859-1":
                             data = marc8_to_unicode(data, hide_utf8_warnings)
                         else:
                             data = data.decode(encoding)
-                    subfields.append(code)
-                    subfields.append(data)
+
+                    coded = Subfield(code=code, value=data)
+                    subfields.append(coded)
+
                 if to_unicode:
                     field = Field(
                         tag=entry_tag,
                         indicators=[first_indicator, second_indicator],
                         subfields=subfields,
                     )
                 else:
@@ -389,14 +420,20 @@
 
     def as_marc(self) -> bytes:
         """Returns the record serialized as MARC21."""
         fields = b""
         directory = b""
         offset = 0
 
+        if self.to_unicode:
+            if isinstance(self.leader, Leader):
+                self.leader.coding_scheme = "a"
+            else:
+                self.leader = self.leader[0:9] + "a" + self.leader[10:]
+
         # build the directory
         # each element of the directory includes the tag, the byte length of
         # the field and the offset from the base address where the field data
         # can be found
         if self.leader[9] == "a" or self.force_utf8:
             encoding = "utf-8"
         else:
@@ -426,20 +463,15 @@
         base_address = LEADER_LEN + len(directory)
 
         # figure out the length of the record
         record_length = base_address + len(fields)
 
         # update the leader with the current record length and base address
         # the lengths are fixed width and zero padded
-        strleader = "%05d%s%05d%s" % (
-            record_length,
-            self.leader[5:12],
-            base_address,
-            self.leader[17:],
-        )
+        strleader = f"{record_length:0>5}{self.leader[5:12]}{base_address:0>5}{self.leader[17:]}"
         leader = strleader.encode(encoding)
 
         return leader + directory + fields
 
     # alias for backwards compatibility
     as_marc21 = as_marc
 
@@ -447,180 +479,203 @@
         """Turn a MARC record into a dictionary, which is used for ``as_json``."""
         record: Dict = {"leader": str(self.leader), "fields": []}
 
         for field in self:
             if field.is_control_field():
                 record["fields"].append({field.tag: field.data})
             else:
-                fd: Dict[str, Any] = {}
-                fd["subfields"] = []
-                fd["ind1"] = field.indicator1
-                fd["ind2"] = field.indicator2
-                for tag, value in zip_longest(*[iter(field.subfields)] * 2):
-                    fd["subfields"].append({tag: value})
-                record["fields"].append({field.tag: fd})
+                record["fields"].append(
+                    {
+                        field.tag: {
+                            "ind1": field.indicator1,
+                            "ind2": field.indicator2,
+                            "subfields": [{s.code: s.value} for s in field.subfields],
+                        }
+                    }
+                )
         return record  # as dict
 
     def as_json(self, **kwargs) -> str:
         """Serialize a record as JSON.
 
         See:
-        http://dilettantes.code4lib.org/blog/2010/09/a-proposal-to-serialize-marc-in-json/
+        https://web.archive.org/web/20151112001548/http://dilettantes.code4lib.org/blog/2010/09/a-proposal-to-serialize-marc-in-json
         """
         return json.dumps(self.as_dict(), **kwargs)
 
+    @property
     def title(self) -> Optional[str]:
         """Returns the title of the record (245 $a and $b)."""
-        try:
-            title = self["245"]["a"]  # type: ignore
-        except TypeError:
-            title = None
+        title_field: Optional[Field] = self.get("245")
+        if not title_field:
+            return None
+
+        title: Optional[str] = title_field.get("a")
         if title:
-            try:
-                title += " " + self["245"]["b"]  # type: ignore
-            except TypeError:
-                pass
+            subtitle = title_field.get("b")
+            if subtitle:
+                title += f" {subtitle}"
         return title
 
+    @property
     def issn_title(self) -> Optional[str]:
         """Returns the key title of the record (222 $a and $b)."""
-        try:
-            title = self["222"]["a"]  # type: ignore
-        except TypeError:
-            title = None
+        title_field: Optional[Field] = self.get("222")
+        if not title_field:
+            return None
+
+        title: Optional[str] = title_field.get("a")
         if title:
-            try:
-                title += " " + self["222"]["b"]  # type: ignore
-            except TypeError:
-                pass
+            subtitle = title_field.get("b")
+            if subtitle:
+                title += f" {subtitle}"
         return title
 
+    @property
     def isbn(self) -> Optional[str]:
         """Returns the first ISBN in the record or None if one is not present.
 
         The returned ISBN will be all numeric, except for an
         x/X which may occur in the checksum position.  Dashes and
         extraneous information will be automatically removed. If you need
         this information you'll want to look directly at the 020 field,
-        e.g. record['020']['a']
+        e.g. record['020']['a']. Values that do not match the regex will not
+        be returned.
         """
-        try:
-            isbn_number = self["020"]["a"]  # type: ignore
-            match = isbn_regex.search(isbn_number)  # type: ignore
-            if match:
-                return match.group(1).replace("-", "")
-        except TypeError:
-            # ISBN not set
-            pass
+        isbn_field: Optional[Field] = self.get("020")
+        if not isbn_field:
+            return None
+
+        isbn_number: Optional[str] = isbn_field.get("a")
+        if not isbn_number:
+            return None
+
+        match = isbn_regex.search(isbn_number)  # type: ignore
+        if match:
+            return match.group(1).replace("-", "")
+
         return None
 
+    @property
     def issn(self) -> Optional[str]:
         """Returns the ISSN number [022]['a'] in the record or None."""
-        field = self["022"]
-        return field["a"] if field else None
+        field = self.get("022")
+        return field.get("a") if (field and "a" in field) else None
 
+    @property
     def issnl(self) -> Optional[str]:
         """Returns the ISSN-L number [022]['l'] of the record or None."""
-        field = self["022"]
-        return field["l"] if field else None
+        field = self.get("022")
+        return field["l"] if (field and "l" in field) else None
 
+    @property
     def sudoc(self) -> Optional[str]:
         """Returns a Superintendent of Documents (SuDoc) classification number.
 
         Note: More information can be found at the following URL:
         https://www.fdlp.gov/classification-guidelines/introduction-to-the-classification-guidelines
         """
-        field = self["086"]
+        field = self.get("086")
         return field.format_field() if field else None
 
+    @property
     def author(self) -> Optional[str]:
         """Returns the author from field 100, 110 or 111."""
-        field = self["100"] or self["110"] or self["111"]
+        field = self.get("100") or self.get("110") or self.get("111")
         return field.format_field() if field else None
 
+    @property
     def uniformtitle(self) -> Optional[str]:
         """Returns the uniform title from field 130 or 240."""
-        field = self["130"] or self["240"]
+        field = self.get("130") or self.get("240")
         return field.format_field() if field else None
 
+    @property
     def series(self) -> List[Field]:
         """Returns series fields.
 
         Note: 490 supersedes the 440 series statement which was both
         series statement and added entry. 8XX fields are added entries.
         """
         return self.get_fields("440", "490", "800", "810", "811", "830")
 
+    @property
     def subjects(self) -> List[Field]:
         """Returns subjects fields.
 
         Note: Fields 690-699 are considered "local" added entry fields but
         occur with some frequency in OCLC and RLIN records.
         """
         # fmt: off
         return self.get_fields(
             "600", "610", "611", "630", "648", "650", "651", "653", "654", "655",
             "656", "657", "658", "662", "690", "691", "696", "697", "698", "699",
         )
         # fmt: on
 
+    @property
     def addedentries(self) -> List[Field]:
         """Returns Added entries fields.
 
         Note: Fields 790-799 are considered "local" added entry fields but
         occur with some frequency in OCLC and RLIN records.
         """
         # fmt: off
         return self.get_fields(
             "700", "710", "711", "720", "730", "740", "752", "753", "754", "790",
             "791", "792", "793", "796", "797", "798", "799",
         )
         # fmt: on
 
+    @property
     def location(self) -> List[Field]:
         """Returns location field (852)."""
         return self.get_fields("852")
 
+    @property
     def notes(self) -> List[Field]:
         """Return notes fields (all 5xx fields)."""
         # fmt: off
         return self.get_fields(
             "500", "501", "502", "504", "505", "506", "507", "508", "510", "511",
             "513", "514", "515", "516", "518", "520", "521", "522", "524", "525",
             "526", "530", "533", "534", "535", "536", "538", "540", "541", "544",
             "545", "546", "547", "550", "552", "555", "556", "561", "562", "563",
             "565", "567", "580", "581", "583", "584", "585", "586", "590", "591",
             "592", "593", "594", "595", "596", "597", "598", "599",
         )
         # fmt: on
 
+    @property
     def physicaldescription(self) -> List[Field]:
         """Return physical description fields (300)."""
         return self.get_fields("300")
 
+    @property
     def publisher(self) -> Optional[str]:
         """Return publisher from 260 or 264.
 
         Note: 264 field with second indicator '1' indicates publisher.
         """
         for f in self.get_fields("260", "264"):
-            if self["260"]:
-                return self["260"]["b"]  # type: ignore
-            if self["264"] and f.indicator2 == "1":
-                return self["264"]["b"]  # type: ignore
+            if f.tag == "260":
+                return f.get("b")
+            if f.tag == "264" and f.indicator2 == "1":
+                return f.get("b")
 
         return None
 
+    @property
     def pubyear(self) -> Optional[str]:
         """Returns publication year from 260 or 264."""
         for f in self.get_fields("260", "264"):
-            if self["260"]:
-                return self["260"]["c"]  # type: ignore
-            if self["264"] and f.indicator2 == "1":
-                return self["264"]["c"]  # type: ignore
+            if f.tag == "260":
+                return f.get("c")  # type: ignore
+            if f.tag == "264" and f.indicator2 == "1":
+                return f.get("c")  # type: ignore
         return None
 
 
 def map_marc8_record(record: Record) -> Record:
     """Map MARC-8 record."""
     record.fields = [map_marc8_field(field) for field in record.fields]
     leader: List[str] = list(record.leader)
```

### Comparing `pymarc-4.2.2/pymarc/writer.py` & `pymarc-5.0.0/pymarc/writer.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/pymarc.egg-info/PKG-INFO` & `pymarc-5.0.0/pymarc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pymarc
-Version: 4.2.2
+Version: 5.0.0
 Summary: Read, write and modify MARC bibliographic data
 Home-page: http://gitlab.com/pymarc/pymarc
 Author: Ed Summers
 Author-email: ehs@pobox.com
 License: http://www.opensource.org/licenses/bsd-license.php
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ```
 _|_|_|    _|    _|  _|_|_|  _|_|      _|_|_|  _|  _|_|    _|_|_|
 _|    _|  _|    _|  _|    _|    _|  _|    _|  _|_|      _|
 _|    _|  _|    _|  _|    _|    _|  _|    _|  _|        _|
@@ -73,15 +74,15 @@
 available here in pymarc repository:
 
 ```python
 from pymarc import MARCReader
 with open('test/marc.dat', 'rb') as fh:
     reader = MARCReader(fh)
     for record in reader:
-        print(record.title())
+        print(record.title)
 ```
 ```
 The pragmatic programmer : from journeyman to master /
 Programming Python /
 Learning Python /
 Python cookbook /
 Python programming for the absolute beginner /
@@ -100,22 +101,23 @@
 Programming with Python /
 BSD Sockets programming from a multi-language perspective /
 Design patterns : elements of reusable object-oriented software /
 Introduction to algorithms /
 ANSI Common Lisp /
 ```
 
-A `pymarc.Record` object has a few handy methods like `title` for getting at
+A `pymarc.Record` object has a few handy properties like `title` for getting at
 bits of a bibliographic record, others include: `author`, `isbn`, `subjects`,
 `location`, `notes`, `physicaldescription`, `publisher`, `pubyear`, `issn`,
 `issn_title`. But really, to work with MARC data you need to understand the
 numeric field tags and subfield codes that are used to designate various bits
-of information. There is a lot more hiding in a MARC record than these methods
-provide access to. For example the `title` method extracts the information from
- the `245` field, subfields `a` and `b`. You can access `245a` like so:
+of information. There is a lot more data hidden in a MARC record than these
+helper properties provide access to. For example the `title` property works by
+extracting the information from the `245` field, subfields `a` and `b` behind
+the scenes. You can access `245a` like so:
 
 ```python
 print(record['245']['a'])
 ```
 
 Some fields like subjects can repeat. In cases like that you will want to use
 `get_fields` to get all of them as `pymarc.Field` objects, which you can then
@@ -128,43 +130,68 @@
 
 If you are new to MARC fields [Understanding
 MARC](http://www.loc.gov/marc/umb/) is a pretty good primer, and the [MARC 21
 Formats](http://www.loc.gov/marc/marcdocz.html) page at the Library of Congress is a good reference once you understand the basics.
 
 ### Writing
 
+*Note: As of v5.0.0 `Subfield` is used to create subfields. Prior to v5,
+subfields were constructed and accessed as a list of strings, e.g., `[code,
+value, code, value]`. In v5.0.0 this has been changed to organize the subfields
+into a list of tuples, e.g., `[(code, value), (code, value)]`. The `Subfield`
+is implemented as a `NamedTuple` so that the tuples can be constructed as
+`Subfield(code=code, value=value)`. The old style of creating subfields is no
+longer supported. Attempting to pass a list of strings to the `subfields`
+parameter for the `Field` constructor will raise a `ValueError`. For
+convenience the `Field.convert_legacy_subfields` can be used to convert a
+legacy list of strings into a list of `Subfield`s.*
+
 Here's an example of creating a record and writing it out to a file.
 
 ```python
-from pymarc import Record, Field
+from pymarc import Record, Field, Subfield
+
 record = Record()
 record.add_field(
     Field(
-        tag = '245',
-        indicators = ['0','1'],
-        subfields = [
-            'a', 'The pragmatic programmer : ',
-            'b', 'from journeyman to master /',
-            'c', 'Andrew Hunt, David Thomas.'
+        tag='245',
+        indicators=['0', '1'],
+        subfields=[
+            Subfield(code='a', value='The pragmatic programmer : '),
+            Subfield(code='b', value='from journeyman to master /'),
+            Subfield(code='c', value='Andrew Hunt, David Thomas.')
         ]))
 with open('file.dat', 'wb') as out:
     out.write(record.as_marc())
 ```
 
+To convert from the old string list to a list of `Subfield`s, the `.convert_legacy_subfields` class method
+is provided on the `Field` class.
+
+```python
+from pymarc import Field, Subfield
+
+legacy_fields: list[str] = ['a', 'The pragmatic programmer : ',
+                            'b', 'from journeyman to master /',
+                            'c', 'Andrew Hunt, David Thomas']
+
+coded_fields: list[Subfield] = Field.convert_legacy_subfields(legacy_fields)
+```
+
 ### Updating
 
 Updating works the same way, you read it in, modify it, and then write it out
 again:
 
 ```python
 from pymarc import MARCReader
 with open('test/marc.dat', 'rb') as fh:
     reader = MARCReader(fh)
     record = next(reader)
-    record['245']['a'] = 'The Zombie Programmer'
+    record['245']['a'] = 'The Zombie Programmer : '
 with open('file.dat', 'wb') as out:
     out.write(record.as_marc())
 ```
 
 
 ### JSON and XML
 
@@ -199,14 +226,16 @@
 map_xml(print_title, 'test/batch.xml')
 ```
 
 Also, if you prefer you can pass in a file like object in addition to the path
 to both *map_xml* and *parse_xml_to_array*:
 
 ```python
+from pymarc import parse_xml_to_array
+
 records = parse_xml_to_array(open('test/batch.xml'))
 ```
 
 **JSON**
 
 JSON support is fairly minimal in that you can call a `pymarc.Record`'s
 `as_json()` method to return JSON for a given MARC Record:
@@ -381,9 +410,7 @@
 GitLab to submit feature requests or bug reports. If you've got an itch to
 scratch, please scratch it, and send merge requests on
 [GitLab](http://gitlab.com/pymarc/pymarc).
 
 If you start working with MARC you may feel like you need moral support
 in addition to technical support. The
 [#code4lib](ircs://irc.libera.chat/code4lib) channel on [Libera](https://libera.chat/) is a good place for both.
-
-
```

### Comparing `pymarc-4.2.2/pymarc.egg-info/SOURCES.txt` & `pymarc-5.0.0/pymarc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 README_pt_Br.md
+release.md
 requirements.dev.txt
 setup.cfg
 setup.py
 docs/source/conf.py
 docs/source/index.rst
 pymarc/__init__.py
 pymarc/constants.py
@@ -33,14 +34,15 @@
 test/bad_records.mrc
 test/bad_subfield_code.dat
 test/bad_tag.xml
 test/batch.json
 test/batch.xml
 test/diacritic.dat
 test/marc.dat
+test/marc8-to-unicode.dat
 test/marc8.dat
 test/multi_isbn.dat
 test/one.dat
 test/one.json
 test/regression45.dat
 test/test.dat
 test/test.json
```

### Comparing `pymarc-4.2.2/setup.py` & `pymarc-5.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
 
 """Pymarc setup."""
 
 from setuptools import setup
 
-version = "4.2.2"
+version = "5.0.0"
 
 classifiers = """
 Intended Audience :: Education
 Intended Audience :: Developers
 Intended Audience :: Information Technology
 License :: OSI Approved :: BSD License
 Programming Language :: Python :: 3
-Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
+Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Topic :: Text Processing :: General
 """
 
 
 with open("README.md") as f:
     long_description = f.read()
 
@@ -35,9 +37,9 @@
     license="http://www.opensource.org/licenses/bsd-license.php",
     packages=["pymarc"],
     description="Read, write and modify MARC bibliographic data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=list(filter(None, classifiers.split("\n"))),
     test_suite="test",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

### Comparing `pymarc-4.2.2/test/1251.dat` & `pymarc-5.0.0/test/1251.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/alphatag.dat` & `pymarc-5.0.0/test/alphatag.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 3031 3333 3963 616d 2020 3232 3030 3334  01339cam  220034
+00000000: 3031 3333 3963 616d 2061 3232 3030 3334  01339cam a220034
 00000010: 3920 2020 3435 3030 3030 3130 3031 3030  9   450000100100
 00000020: 3030 3030 3030 3530 3031 3730 3030 3130  0000005001700010
 00000030: 3030 3830 3034 3130 3030 3237 3031 3030  0080041000270100
 00000040: 3032 3130 3030 3638 3032 3030 3030 3930  0210006802000090
 00000050: 3030 3839 3033 3530 3031 3030 3030 3938  0089035001000098
 00000060: 3033 3530 3032 3130 3031 3038 3034 3030  0350021001080400
 00000070: 3031 3330 3031 3239 3034 3930 3031 3530  0130012904900150
```

### Comparing `pymarc-4.2.2/test/bad_eacc_encoding.dat` & `pymarc-5.0.0/test/bad_eacc_encoding.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/bad_indicator.dat` & `pymarc-5.0.0/test/bad_indicator.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/bad_marc8_escape.dat` & `pymarc-5.0.0/test/bad_marc8_escape.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/bad_records.mrc` & `pymarc-5.0.0/test/bad_records.mrc`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/bad_subfield_code.dat` & `pymarc-5.0.0/test/bad_subfield_code.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/bad_tag.xml` & `pymarc-5.0.0/test/bad_tag.xml`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/batch.json` & `pymarc-5.0.0/test/batch.json`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/batch.xml` & `pymarc-5.0.0/test/batch.xml`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/diacritic.dat` & `pymarc-5.0.0/test/diacritic.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/marc.dat` & `pymarc-5.0.0/test/marc.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/marc8.dat` & `pymarc-5.0.0/test/marc8.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/multi_isbn.dat` & `pymarc-5.0.0/test/multi_isbn.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/one.dat` & `pymarc-5.0.0/test/one.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 3030 3735 3563 616d 2020 3232 3030 3234  00755cam  220024
+00000000: 3030 3735 3563 616d 2061 3232 3030 3234  00755cam a220024
 00000010: 3134 6120 3435 3030 3030 3130 3031 3330  14a 450000100130
 00000020: 3030 3030 3030 3330 3030 3630 3030 3133  0000003000600013
 00000030: 3030 3530 3031 3730 3030 3139 3030 3830  0050017000190080
 00000040: 3034 3130 3030 3336 3031 3030 3031 3730  0410003601000170
 00000050: 3030 3737 3032 3030 3034 3330 3030 3934  0077020004300094
 00000060: 3034 3030 3031 3830 3031 3337 3034 3230  0400018001370420
 00000070: 3030 3830 3031 3535 3035 3030 3032 3630  0080015505000260
```

### Comparing `pymarc-4.2.2/test/one.json` & `pymarc-5.0.0/test/one.json`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/regression45.dat` & `pymarc-5.0.0/test/regression45.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test.dat` & `pymarc-5.0.0/test/test.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test.json` & `pymarc-5.0.0/test/test.json`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_encode.py` & `pymarc-5.0.0/test/test_encode.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_json.py` & `pymarc-5.0.0/test/test_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 
 
 class JsonReaderTest(unittest.TestCase):
     def setUp(self):
         with open("test/test.json") as fh:
             self.in_json = json.load(fh, strict=False)
 
-        with open("test/test.json") as fh:
-            self.reader = pymarc.JSONReader(fh)
+        self._js_fh = open("test/test.json")
+        self.reader = pymarc.JSONReader(self._js_fh)
+
+    def tearDown(self) -> None:
+        self._js_fh.close()
 
     def testRoundtrip(self):
         """Test from and to json.
 
         Tests that result of loading records from the test file
         produces objects deeply equal to the result of loading
         marc-in-json files directly
@@ -39,21 +42,30 @@
         data = json.dumps(self.in_json[0])
         reader = pymarc.JSONReader(data)
         self.assertEqual([rec.as_dict() for rec in reader][0], self.in_json[0])
 
 
 class JsonTest(unittest.TestCase):
     def setUp(self):
-        self.reader = pymarc.MARCReader(open("test/test.dat", "rb"))
+        self._test_fh = open("test/test.dat", "rb")
+        self.reader = pymarc.MARCReader(self._test_fh)
         self._record = pymarc.Record()
         field = pymarc.Field(
-            tag="245", indicators=["1", "0"], subfields=["a", "Python", "c", "Guido"]
+            tag="245",
+            indicators=["1", "0"],
+            subfields=[
+                pymarc.Subfield(code="a", value="Python"),
+                pymarc.Subfield(code="c", value="Guido"),
+            ],
         )
         self._record.add_field(field)
 
+    def tearDown(self) -> None:
+        self._test_fh.close()
+
     def test_as_dict_single(self):
         _expected = {
             "fields": [
                 {
                     "245": {
                         "ind1": "1",
                         "ind2": "0",
@@ -99,36 +111,50 @@
     def test_as_json_multiple(self):
         for record in self.reader:
             self.assertEqual(dict, json.loads(record.as_json()).__class__)
 
 
 class JsonParse(unittest.TestCase):
     def setUp(self):
-        self.reader_dat = pymarc.MARCReader(open("test/one.dat", "rb"))
-        self.parse_json = pymarc.parse_json_to_array(open("test/one.json"))
-
-        self.batch_xml = pymarc.parse_xml_to_array(open("test/batch.xml"))
-        self.batch_json = pymarc.parse_json_to_array(open("test/batch.json"))
+        self._one_dat_fh = open("test/one.dat", "rb")
+        self._one_js_fh = open("test/one.json", "r")
+        self._batch_xml_fh = open("test/batch.xml", "r")
+        self._batch_js_fh = open("test/batch.json", "r")
+
+        self.reader_dat = pymarc.MARCReader(self._one_dat_fh)
+        self.parse_json = pymarc.parse_json_to_array(self._one_js_fh)
+        self.batch_xml = pymarc.parse_xml_to_array(self._batch_xml_fh)
+        self.batch_json = pymarc.parse_json_to_array(self._batch_js_fh)
+
+    def tearDown(self) -> None:
+        self._one_dat_fh.close()
+        self._one_js_fh.close()
+        self._batch_js_fh.close()
+        self._batch_xml_fh.close()
 
     def testRoundtrip(self):
         recs = list(self.reader_dat)
         self.assertEqual(
             len(self.parse_json), len(recs), "Incorrect number of records found"
         )
         for from_dat, from_json in zip(recs, self.parse_json):
-            self.assertEqual(from_dat.as_marc(), from_json.as_marc(), "Icorrect Record")
+            self.assertEqual(
+                from_dat.as_marc(), from_json.as_marc(), "Incorrect Record"
+            )
 
     def testParseJsonXml(self):
         self.assertEqual(
             len(self.batch_json),
             len(self.batch_xml),
             "Incorrect number of parse records found",
         )
         for from_dat, from_json in zip(self.batch_json, self.batch_xml):
-            self.assertEqual(from_dat.as_marc(), from_json.as_marc(), "Icorrect Record")
+            self.assertEqual(
+                from_dat.as_marc(), from_json.as_marc(), "Incorrect Record"
+            )
 
 
 def suite():
     test_suite = unittest.makeSuite(JsonTest, "test")
     return test_suite
```

### Comparing `pymarc-4.2.2/test/test_leader.py` & `pymarc-5.0.0/test/test_leader.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_marc8.py` & `pymarc-5.0.0/test/test_marc8.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
 
 import os
 from unittest import TestCase, makeSuite  # type: ignore
 
 
-from pymarc import Field, MARCReader, MARCWriter, RawField, Record, marc8_to_unicode
+from pymarc import (
+    Field,
+    MARCReader,
+    MARCWriter,
+    RawField,
+    Record,
+    marc8_to_unicode,
+    Subfield,
+)
 
 
 class MARC8Test(TestCase):
     def test_marc8_reader(self):
         with open("test/marc8.dat", "rb") as fh:
             reader = MARCReader(fh, to_unicode=False)
             r = next(reader)
@@ -112,15 +120,17 @@
 
         self.assertEqual(count, 1515)
         marc8_file.close()
         utf8_file.close()
 
     def test_writing_unicode(self):
         record = Record()
-        record.add_field(Field(245, ["1", "0"], ["a", chr(0x1234)]))
+        record.add_field(
+            Field("245", ["1", "0"], [Subfield(code="a", value=chr(0x1234))])
+        )
         record.leader = "         a              "
         writer = MARCWriter(open("test/foo", "wb"))
         writer.write(record)
         writer.close()
 
         reader = MARCReader(open("test/foo", "rb"), to_unicode=True)
         record = next(reader)
```

### Comparing `pymarc-4.2.2/test/test_marc8.txt` & `pymarc-5.0.0/test/test_marc8.txt`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_ordered_fields.py` & `pymarc-5.0.0/test/test_ordered_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import unittest
 
 import pymarc
 
 
 class OrderedFieldsTest(unittest.TestCase):
     def test_add_ordered_fields(self):
-
         record = pymarc.Record()
         for tag in ("999", "888", "111", "abc", "666", "988", "998"):
-            field = pymarc.Field(tag, ["0", "0"], ["a", "foo"])
+            field = pymarc.Field(
+                tag, ["0", "0"], [pymarc.Subfield(code="a", value="foo")]
+            )
             record.add_ordered_field(field)
 
         # ensure all numeric fields are in strict order
         ordered = True
         last_tag = 0
         for field in record:
             if not field.tag.isdigit():
@@ -29,15 +30,17 @@
             last_tag = curr_tag
 
         self.assertTrue(ordered, "Fields are not strictly ordered numerically")
 
     def test_add_grouped_fields(self):
         record = pymarc.Record()
         for tag in ("999", "888", "111", "abc", "666", "988", "998"):
-            field = pymarc.Field(tag, ["0", "0"], ["a", "foo"])
+            field = pymarc.Field(
+                tag, ["0", "0"], [pymarc.Subfield(code="a", value="foo")]
+            )
             record.add_grouped_field(field)
 
         # ensure all numeric fields are in grouped order
         grouped = list()
         for field in record:
             if not field.tag.isdigit():
                 continue
```

### Comparing `pymarc-4.2.2/test/test_reader.py` & `pymarc-5.0.0/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_record.py` & `pymarc-5.0.0/test/test_record.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,179 @@
 # This file is part of pymarc. It is subject to the license terms in the
 # LICENSE file found in the top-level directory of this distribution and at
 # https://opensource.org/licenses/BSD-2-Clause. pymarc may be copied, modified,
 # propagated, or distributed according to the terms contained in the LICENSE
 # file.
-
 import unittest
 
 from pymarc.exceptions import (
     BaseAddressInvalid,
     FieldNotFound,
     MissingLinkedFields,
     RecordLeaderInvalid,
 )
-from pymarc.field import Field
+from pymarc.field import Field, Subfield
 from pymarc.reader import MARCReader
 from pymarc.record import Record
 
 
 class RecordTest(unittest.TestCase):
     def test_add_field(self):
         record = Record()
         field = Field(
-            tag="245", indicators=["1", "0"], subfields=["a", "Python", "c", "Guido"]
+            tag="245",
+            indicators=["1", "0"],
+            subfields=[
+                Subfield(code="a", value="Python"),
+                Subfield(code="c", value="Guido"),
+            ],
         )
         record.add_field(field)
         self.assertTrue(field in record.fields, msg="found field")
 
     def test_remove_field(self):
         record = Record()
         field = Field(
-            tag="245", indicators=["1", "0"], subfields=["a", "Python", "c", "Guido"]
+            tag="245",
+            indicators=["1", "0"],
+            subfields=[
+                Subfield(code="a", value="Python"),
+                Subfield(code="c", value="Guido"),
+            ],
         )
         record.add_field(field)
         self.assertEqual(record["245"]["a"], "Python")
 
         # try removing a field that exists
         record.remove_field(field)
-        self.assertEqual(record["245"], None)
+        self.assertEqual(record.get("245"), None)
 
         # try removing a field that doesn't exist
         field = Field("001", data="abcd1234")
         self.assertRaises(FieldNotFound, record.remove_field, field)
 
     def test_quick_access(self):
         record = Record()
         title = Field(
-            tag="245", indicators=["1", "0"], subfields=["a", "Python", "c", "Guido"]
+            tag="245",
+            indicators=["1", "0"],
+            subfields=[
+                Subfield(code="a", value="Python"),
+                Subfield(code="c", value="Guido"),
+            ],
         )
         record.add_field(title)
         self.assertEqual(record["245"], title, "short access")
-        self.assertEqual(record["999"], None, "short access with no field")
+        self.assertEqual(record.get("999"), None, "short access with no field")
 
     def test_membership(self):
         record = Record()
         title = Field(
-            tag="245", indicators=["1", "0"], subfields=["a", "Python", "c", "Guido"]
+            tag="245",
+            indicators=["1", "0"],
+            subfields=[
+                Subfield(code="a", value="Python"),
+                Subfield(code="c", value="Guido"),
+            ],
         )
         record.add_field(title)
         self.assertTrue("245" in record)
         self.assertFalse("999" in record)
 
     def test_field_not_found(self):
         record = Record()
         self.assertEqual(len(record.fields), 0)
 
     def test_find(self):
         record = Record()
         subject1 = Field(
-            tag="650", indicators=["", "0"], subfields=["a", "Programming Language"]
+            tag="650",
+            indicators=["", "0"],
+            subfields=[Subfield(code="a", value="Programming Language")],
         )
         record.add_field(subject1)
         subject2 = Field(
-            tag="650", indicators=["", "0"], subfields=["a", "Object Oriented"]
+            tag="650",
+            indicators=["", "0"],
+            subfields=[Subfield(code="a", value="Object Oriented")],
         )
         record.add_field(subject2)
         found = record.get_fields("650")
         self.assertEqual(found[0], subject1, "get_fields() item 1")
         self.assertEqual(found[0], subject1, "get_fields() item 2")
         found = record.get_fields()
         self.assertEqual(len(found), 2, "get_fields() with no tag")
 
     def test_multi_find(self):
         record = Record()
         subject1 = Field(
-            tag="650", indicators=["", "0"], subfields=["a", "Programming Language"]
+            tag="650",
+            indicators=["", "0"],
+            subfields=[Subfield(code="a", value="Programming Language")],
         )
         record.add_field(subject1)
         subject2 = Field(
-            tag="651", indicators=["", "0"], subfields=["a", "Object Oriented"]
+            tag="651",
+            indicators=["", "0"],
+            subfields=[Subfield(code="a", value="Object Oriented")],
         )
         record.add_field(subject2)
         found = record.get_fields("650", "651")
         self.assertEqual(len(found), 2)
 
     def test_get_linked_fields(self):
         record = Record()
         t1 = Field(
             tag="245",
             indicators=["1", "0"],
-            subfields=["6", "880-01", "a", "Rū Harison no wārudo myūjikku nyūmon"],
+            subfields=[
+                Subfield(code="6", value="880-01"),
+                Subfield(code="a", value="Rū Harison no wārudo myūjikku nyūmon"),
+            ],
         )
         record.add_field(t1)
         t2 = Field(
             tag="880",
             indicators=["1", "0"],
-            subfields=["6", "245-01", "a", "ルー・ハリソンのワールドミュージック入門"],
+            subfields=[
+                Subfield(code="6", value="245-01"),
+                Subfield(code="a", value="ルー・ハリソンのワールドミュージック入門"),
+            ],
         )
         record.add_field(t2)
         pd1 = Field(
-            tag="260", indicators=["0", "2"], subfields=["6", "880-02", "a", "Tōkyō"]
+            tag="260",
+            indicators=["0", "2"],
+            subfields=[
+                Subfield(code="6", value="880-02"),
+                Subfield(code="a", value="Tōkyō"),
+            ],
         )
         record.add_field(pd1)
         pd2 = Field(
-            tag="880", indicators=["0", "2"], subfields=["6", "260-02", "a", "東京"]
+            tag="880",
+            indicators=["0", "2"],
+            subfields=[
+                Subfield(code="6", value="260-02"),
+                Subfield(code="a", value="東京"),
+            ],
         )
         record.add_field(pd2)
         self.assertEqual(record.get_linked_fields(t1), [t2])
         self.assertEqual(record.get_linked_fields(pd1), [pd2])
 
     def test_missing_linked_fields_exception(self):
         record = Record()
         t1 = Field(
             tag="245",
             indicators=["1", "0"],
-            subfields=["6", "880-01", "a", "Rū Harison no wārudo myūjikku nyūmon"],
+            subfields=[
+                Subfield(code="6", value="880-01"),
+                Subfield(code="a", value="Rū Harison no wārudo myūjikku nyūmon"),
+            ],
         )
         record.add_field(t1)
         self.assertRaisesRegex(
             MissingLinkedFields, "^245 field", record.get_linked_fields, t1
         )
 
     def test_bad_leader(self):
@@ -138,348 +184,485 @@
         record = Record()
         self.assertRaises(
             BaseAddressInvalid, record.decode_marc, b"00695cam  2200241Ia 45x00"
         )
 
     def test_title(self):
         record = Record()
-        self.assertEqual(record.title(), None)
-        record.add_field(Field("245", [0, 1], subfields=["a", "Foo :", "b", "bar"]))
-        self.assertEqual(record.title(), "Foo : bar")
+        self.assertEqual(record.title, None)
+        record.add_field(
+            Field(
+                "245",
+                ["0", "1"],
+                subfields=[
+                    Subfield(code="a", value="Foo :"),
+                    Subfield(code="b", value="bar"),
+                ],
+            )
+        )
+        self.assertEqual(record.title, "Foo : bar")
 
         record = Record()
-        record.add_field(Field("245", [0, 1], subfields=["a", "Farghin"]))
-        self.assertEqual(record.title(), "Farghin")
+        record.add_field(
+            Field("245", ["0", "1"], subfields=[Subfield(code="a", value="Farghin")])
+        )
+        self.assertEqual(record.title, "Farghin")
 
     def test_issn_title(self):
         record = Record()
-        self.assertEqual(record.issn_title(), None)
-        record.add_field(Field("222", ["", ""], subfields=["a", "Foo :", "b", "bar"]))
-        self.assertEqual(record.issn_title(), "Foo : bar")
+        self.assertEqual(record.issn_title, None)
+        record.add_field(
+            Field(
+                "222",
+                ["", ""],
+                subfields=[
+                    Subfield(code="a", value="Foo :"),
+                    Subfield(code="b", value="bar"),
+                ],
+            )
+        )
+        self.assertEqual(record.issn_title, "Foo : bar")
 
         record = Record()
-        record.add_field(Field("222", ["", ""], subfields=["a", "Farghin"]))
-        self.assertEqual(record.issn_title(), "Farghin")
+        record.add_field(
+            Field("222", ["", ""], subfields=[Subfield(code="a", value="Farghin")])
+        )
+        self.assertEqual(record.issn_title, "Farghin")
 
         record = Record()
-        record.add_field(Field("222", ["", ""], subfields=["b", "bar"]))
-        self.assertEqual(record.issn_title(), None)
+        record.add_field(
+            Field("222", ["", ""], subfields=[Subfield(code="b", value="bar")])
+        )
+        self.assertEqual(record.issn_title, None)
 
     def test_isbn(self):
         record = Record()
-        self.assertEqual(record.isbn(), None)
-        record.add_field(Field("020", [0, 1], subfields=["a", "9781416566113"]))
-        self.assertEqual(record.isbn(), "9781416566113")
+        self.assertEqual(record.isbn, None)
+        record.add_field(
+            Field(
+                "020",
+                ["0", "1"],
+                subfields=[Subfield(code="a", value="9781416566113")],
+            )
+        )
+        self.assertEqual(record.isbn, "9781416566113")
 
         record = Record()
-        record.add_field(Field("020", [0, 1], subfields=["a", "978-1416566113"]))
-        self.assertEqual(record.isbn(), "9781416566113")
+        record.add_field(
+            Field(
+                "020",
+                ["0", "1"],
+                subfields=[Subfield(code="a", value="978-1416566113")],
+            )
+        )
+        self.assertEqual(record.isbn, "9781416566113")
 
         record = Record()
-        record.add_field(Field("020", [0, 1], subfields=["a", "ISBN-978-1416566113"]))
-        self.assertEqual(record.isbn(), "9781416566113")
+        record.add_field(
+            Field(
+                "020",
+                ["0", "1"],
+                subfields=[Subfield(code="a", value="ISBN-978-1416566113")],
+            )
+        )
+        self.assertEqual(record.isbn, "9781416566113")
 
         record = Record()
         record.add_field(
-            Field("020", [" ", " "], subfields=["a", "0456789012 (reel 1)"])
+            Field(
+                "020",
+                [" ", " "],
+                subfields=[Subfield(code="a", value="0456789012 (reel 1)")],
+            )
         )
-        self.assertEqual(record.isbn(), "0456789012")
+        self.assertEqual(record.isbn, "0456789012")
 
         record = Record()
-        record.add_field(Field("020", [" ", " "], subfields=["a", "006073132X"]))
-        self.assertEqual(record.isbn(), "006073132X")
+        record.add_field(
+            Field(
+                "020",
+                [" ", " "],
+                subfields=[Subfield(code="a", value="006073132X")],
+            )
+        )
+        self.assertEqual(record.isbn, "006073132X")
 
     def test_issn(self):
         record = Record()
-        self.assertEqual(record.issn(), None)
+        self.assertEqual(record.issn, None)
         record.add_field(
-            Field(tag="022", indicators=["0", ""], subfields=["a", "0395-2037"])
+            Field(
+                tag="022",
+                indicators=["0", ""],
+                subfields=[Subfield(code="a", value="0395-2037")],
+            )
         )
-        self.assertEqual(record.issn(), "0395-2037")
+        self.assertEqual(record.issn, "0395-2037")
 
     def test_issnl(self):
         record = Record()
-        self.assertEqual(record.issnl(), None)
+        self.assertEqual(record.issnl, None)
         record.add_field(
-            Field(tag="022", indicators=["0", ""], subfields=["l", "0395-2037"])
+            Field(
+                tag="022",
+                indicators=["0", ""],
+                subfields=[Subfield(code="l", value="0395-2037")],
+            )
         )
-        self.assertEqual(record.issnl(), "0395-2037")
+        self.assertEqual(record.issnl, "0395-2037")
 
     def test_multiple_isbn(self):
         with open("test/multi_isbn.dat", "rb") as fh:
             reader = MARCReader(fh)
             record = next(reader)
-            self.assertEqual(record.isbn(), "0914378287")
+            self.assertEqual(record.isbn, "0914378287")
 
     def test_author(self):
         record = Record()
-        self.assertEqual(record.author(), None)
+        self.assertEqual(record.author, None)
         record.add_field(
-            Field("100", [1, 0], subfields=["a", "Bletch, Foobie,", "d", "1979-1981."])
+            Field(
+                "100",
+                ["1", "0"],
+                subfields=[
+                    Subfield(code="a", value="Bletch, Foobie,"),
+                    Subfield(code="d", value="1979-1981."),
+                ],
+            )
         )
-        self.assertEqual(record.author(), "Bletch, Foobie, 1979-1981.")
+        self.assertEqual(record.author, "Bletch, Foobie, 1979-1981.")
 
         record = Record()
         record.add_field(
-            Field("130", [0, " "], subfields=["a", "Bible.", "l", "Python."])
+            Field(
+                "130",
+                ["0", " "],
+                subfields=[
+                    Subfield(code="a", value="Bible."),
+                    Subfield(code="l", value="Python."),
+                ],
+            )
         )
-        self.assertEqual(record.author(), None)
+        self.assertEqual(record.author, None)
 
     def test_uniformtitle(self):
         record = Record()
-        self.assertEqual(record.uniformtitle(), None)
+        self.assertEqual(record.uniformtitle, None)
         record.add_field(
             Field(
                 "130",
-                [0, " "],
-                subfields=["a", "Tosefta.", "l", "English.", "f", "1977."],
+                ["0", " "],
+                subfields=[
+                    Subfield(code="a", value="Tosefta."),
+                    Subfield(code="l", value="English."),
+                    Subfield(code="f", value="1977."),
+                ],
             )
         )
-        self.assertEqual(record.uniformtitle(), "Tosefta. English. 1977.")
+        self.assertEqual(record.uniformtitle, "Tosefta. English. 1977.")
 
         record = Record()
         record.add_field(
             Field(
-                "240", [1, 4], subfields=["a", "The Pickwick papers.", "l", "French."]
+                "240",
+                ["1", "4"],
+                subfields=[
+                    Subfield(code="a", value="The Pickwick papers."),
+                    Subfield(code="l", value="French."),
+                ],
             )
         )
-        self.assertEqual(record.uniformtitle(), "The Pickwick papers. French.")
+        self.assertEqual(record.uniformtitle, "The Pickwick papers. French.")
 
     def test_subjects(self):
         record = Record()
         subject1 = "=630  0\\$aTosefta.$lEnglish.$f1977."
         subject2 = "=600  10$aLe Peu, Pepe."
         shlist = [subject1, subject2]
-        self.assertEqual(record.subjects(), [])
+        self.assertEqual(record.subjects, [])
         record.add_field(
             Field(
                 "630",
-                [0, " "],
-                subfields=["a", "Tosefta.", "l", "English.", "f", "1977."],
+                ["0", " "],
+                subfields=[
+                    Subfield(code="a", value="Tosefta."),
+                    Subfield(code="l", value="English."),
+                    Subfield(code="f", value="1977."),
+                ],
             )
         )
         record.add_field(
             Field(
                 "730",
-                [0, " "],
-                subfields=["a", "Tosefta.", "l", "English.", "f", "1977."],
+                ["0", " "],
+                subfields=[
+                    Subfield(code="a", value="Tosefta."),
+                    Subfield(code="l", value="English."),
+                    Subfield(code="f", value="1977."),
+                ],
+            )
+        )
+        record.add_field(
+            Field(
+                "600",
+                ["1", "0"],
+                subfields=[Subfield(code="a", value="Le Peu, Pepe.")],
             )
         )
-        record.add_field(Field("600", [1, 0], subfields=["a", "Le Peu, Pepe."]))
-        self.assertEqual(len(record.subjects()), 2)
-        self.assertEqual(record.subjects()[0].__str__(), subject1)
-        self.assertEqual(record.subjects()[1].__str__(), subject2)
-        rshlist = [rsh.__str__() for rsh in record.subjects()]
+        self.assertEqual(len(record.subjects), 2)
+        self.assertEqual(record.subjects[0].__str__(), subject1)
+        self.assertEqual(record.subjects[1].__str__(), subject2)
+        rshlist = [rsh.__str__() for rsh in record.subjects]
         self.assertEqual(shlist, rshlist)
 
     def test_added_entries(self):
         record = Record()
         ae1 = "=730  0\\$aTosefta.$lEnglish.$f1977."
         ae2 = "=700  10$aLe Peu, Pepe."
         aelist = [ae1, ae2]
-        self.assertEqual(record.addedentries(), [])
+        self.assertEqual(record.addedentries, [])
         record.add_field(
             Field(
                 "730",
                 [0, " "],
-                subfields=["a", "Tosefta.", "l", "English.", "f", "1977."],
+                subfields=[
+                    Subfield(code="a", value="Tosefta."),
+                    Subfield(code="l", value="English."),
+                    Subfield(code="f", value="1977."),
+                ],
+            )
+        )
+        record.add_field(
+            Field(
+                "700",
+                ["1", "0"],
+                subfields=[Subfield(code="a", value="Le Peu, Pepe.")],
             )
         )
-        record.add_field(Field("700", [1, 0], subfields=["a", "Le Peu, Pepe."]))
-        record.add_field(Field("245", [0, 0], subfields=["a", "Le Peu's Tosefa."]))
-        self.assertEqual(len(record.addedentries()), 2)
-        self.assertEqual(record.addedentries()[0].__str__(), ae1)
-        self.assertEqual(record.addedentries()[1].__str__(), ae2)
-        raelist = [rae.__str__() for rae in record.addedentries()]
+        record.add_field(
+            Field(
+                "245",
+                ["0", "0"],
+                subfields=[Subfield(code="a", value="Le Peu's Tosefa.")],
+            )
+        )
+        self.assertEqual(len(record.addedentries), 2)
+        self.assertEqual(record.addedentries[0].__str__(), ae1)
+        self.assertEqual(record.addedentries[1].__str__(), ae2)
+        raelist = [rae.__str__() for rae in record.addedentries]
         self.assertEqual(aelist, raelist)
 
     def test_physicaldescription(self):
         record = Record()
         pd1 = "=300  \\$a1 photographic print :$bgelatin silver ;$c10 x 56 in."
         pd2 = "=300  \\$aFOO$bBAR$cBAZ"
         pdlist = [pd1, pd2]
-        self.assertEqual(record.physicaldescription(), [])
+        self.assertEqual(record.physicaldescription, [])
         record.add_field(
             Field(
                 "300",
                 ["\\", ""],
                 subfields=[
-                    "a",
-                    "1 photographic print :",
-                    "b",
-                    "gelatin silver ;",
-                    "c",
-                    "10 x 56 in.",
+                    Subfield(code="a", value="1 photographic print :"),
+                    Subfield(code="b", value="gelatin silver ;"),
+                    Subfield(code="c", value="10 x 56 in."),
                 ],
             )
         )
         record.add_field(
-            Field("300", ["\\", ""], subfields=["a", "FOO", "b", "BAR", "c", "BAZ"])
+            Field(
+                "300",
+                ["\\", ""],
+                subfields=[
+                    Subfield(code="a", value="FOO"),
+                    Subfield(code="b", value="BAR"),
+                    Subfield(code="c", value="BAZ"),
+                ],
+            )
         )
-        self.assertEqual(len(record.physicaldescription()), 2)
-        self.assertEqual(record.physicaldescription()[0].__str__(), pd1)
-        self.assertEqual(record.physicaldescription()[1].__str__(), pd2)
-        rpdlist = [rpd.__str__() for rpd in record.physicaldescription()]
+        self.assertEqual(len(record.physicaldescription), 2)
+        self.assertEqual(record.physicaldescription[0].__str__(), pd1)
+        self.assertEqual(record.physicaldescription[1].__str__(), pd2)
+        rpdlist = [rpd.__str__() for rpd in record.physicaldescription]
         self.assertEqual(pdlist, rpdlist)
 
     def test_location(self):
         record = Record()
         loc1 = "=852  \\\\$aAmerican Institute of Physics.$bNiels Bohr Library and Archives.$eCollege Park, MD"
         loc2 = "=852  01$aCtY$bMain$hLB201$i.M63"
         loclist = [loc1, loc2]
-        self.assertEqual(record.location(), [])
-        record.add_field(Field("040", [" ", " "], subfields=["a", "DLC", "c", "DLC"]))
+        self.assertEqual(record.location, [])
+        record.add_field(
+            Field(
+                "040",
+                [" ", " "],
+                subfields=[
+                    Subfield(code="a", value="DLC"),
+                    Subfield(code="c", value="DLC"),
+                ],
+            )
+        )
         record.add_field(
             Field(
                 "852",
                 [" ", " "],
                 subfields=[
-                    "a",
-                    "American Institute of Physics.",
-                    "b",
-                    "Niels Bohr Library and Archives.",
-                    "e",
-                    "College Park, MD",
+                    Subfield(code="a", value="American Institute of Physics."),
+                    Subfield(code="b", value="Niels Bohr Library and Archives."),
+                    Subfield(code="e", value="College Park, MD"),
                 ],
             )
         )
         record.add_field(
             Field(
                 "852",
-                [0, 1],
-                subfields=["a", "CtY", "b", "Main", "h", "LB201", "i", ".M63"],
+                ["0", "1"],
+                subfields=[
+                    Subfield(code="a", value="CtY"),
+                    Subfield(code="b", value="Main"),
+                    Subfield(code="h", value="LB201"),
+                    Subfield(code="i", value=".M63"),
+                ],
             )
         )
-        self.assertEqual(len(record.location()), 2)
-        self.assertEqual(record.location()[0].__str__(), loc1)
-        self.assertEqual(record.location()[1].__str__(), loc2)
-        rloclist = [rloc.__str__() for rloc in record.location()]
+        self.assertEqual(len(record.location), 2)
+        self.assertEqual(record.location[0].__str__(), loc1)
+        self.assertEqual(record.location[1].__str__(), loc2)
+        rloclist = [rloc.__str__() for rloc in record.location]
         self.assertEqual(loclist, rloclist)
 
     def test_notes(self):
         record = Record()
-        self.assertEqual(record.notes(), [])
+        self.assertEqual(record.notes, [])
         record.add_field(
             Field(
                 "500",
                 [" ", " "],
                 subfields=[
-                    "a",
-                    "Recast in bronze from artist's plaster original of 1903.",
+                    Subfield(
+                        code="a",
+                        value="Recast in bronze from artist's plaster original of 1903.",
+                    ),
                 ],
             )
         )
         self.assertEqual(
-            record.notes()[0].format_field(),
+            record.notes[0].format_field(),
             "Recast in bronze from artist's plaster original of 1903.",
         )
 
     def test_publisher(self):
         record = Record()
-        self.assertEqual(record.publisher(), None)
+        self.assertEqual(record.publisher, None)
         record.add_field(
             Field(
                 "260",
                 [" ", " "],
                 subfields=[
-                    "a",
-                    "Paris :",
-                    "b",
-                    "Gauthier-Villars ;",
-                    "a",
-                    "Chicago :",
-                    "b",
-                    "University of Chicago Press,",
-                    "c",
-                    "1955.",
+                    Subfield(code="a", value="Paris :"),
+                    Subfield(code="b", value="Gauthier-Villars ;"),
+                    Subfield(code="a", value="Chicago :"),
+                    Subfield(code="b", value="University of Chicago Press,"),
+                    Subfield(code="c", value="1955."),
                 ],
             )
         )
-        self.assertEqual(record.publisher(), "Gauthier-Villars ;")
+        self.assertEqual(record.publisher, "Gauthier-Villars ;")
 
         record = Record()
-        self.assertEqual(record.publisher(), None)
+        self.assertEqual(record.publisher, None)
         record.add_field(
             Field(
                 "264",
                 [" ", "1"],
-                subfields=["a", "London :", "b", "Penguin,", "c", "1961."],
+                subfields=[
+                    Subfield(code="a", value="London :"),
+                    Subfield(code="b", value="Penguin,"),
+                    Subfield(code="c", value="1961."),
+                ],
             )
         )
-        self.assertEqual(record.publisher(), "Penguin,")
+        self.assertEqual(record.publisher, "Penguin,")
 
     def test_pubyear(self):
         record = Record()
-        self.assertEqual(record.pubyear(), None)
+        self.assertEqual(record.pubyear, None)
         record.add_field(
             Field(
                 "260",
                 [" ", " "],
                 subfields=[
-                    "a",
-                    "Paris :",
-                    "b",
-                    "Gauthier-Villars ;",
-                    "a",
-                    "Chicago :",
-                    "b",
-                    "University of Chicago Press,",
-                    "c",
-                    "1955.",
+                    Subfield(code="a", value="Paris :"),
+                    Subfield(code="b", value="Gauthier-Villars ;"),
+                    Subfield(code="a", value="Chicago :"),
+                    Subfield(code="b", value="University of Chicago Press,"),
+                    Subfield(code="c", value="1955."),
                 ],
             )
         )
-        self.assertEqual(record.pubyear(), "1955.")
+        self.assertEqual(record.pubyear, "1955.")
 
         record = Record()
-        self.assertEqual(record.pubyear(), None)
+        self.assertEqual(record.pubyear, None)
         record.add_field(
             Field(
                 "264",
                 [" ", "1"],
-                subfields=["a", "London :", "b", "Penguin,", "c", "1961."],
+                subfields=[
+                    Subfield(code="a", value="London :"),
+                    Subfield(code="b", value="Penguin,"),
+                    Subfield(code="c", value="1961."),
+                ],
             )
         )
-        self.assertEqual(record.pubyear(), "1961.")
+        self.assertEqual(record.pubyear, "1961.")
 
     def test_alphatag(self):
         record = Record()
-        record.add_field(Field("CAT", [" ", " "], subfields=["a", "foo"]))
-        record.add_field(Field("CAT", [" ", " "], subfields=["b", "bar"]))
+        record.add_field(
+            Field("CAT", [" ", " "], subfields=[Subfield(code="a", value="foo")])
+        )
+        record.add_field(
+            Field("CAT", [" ", " "], subfields=[Subfield(code="b", value="bar")])
+        )
         fields = record.get_fields("CAT")
         self.assertEqual(len(fields), 2)
         self.assertEqual(fields[0]["a"], "foo")
         self.assertEqual(fields[1]["b"], "bar")
         self.assertEqual(record["CAT"]["a"], "foo")
 
     def test_copy(self):
         from copy import deepcopy
 
         with open("test/one.dat", "rb") as fh:
             r1 = next(MARCReader(fh))
             r2 = deepcopy(r1)
-            r1.add_field(Field("999", [" ", " "], subfields=["a", "foo"]))
-            r2.add_field(Field("999", [" ", " "], subfields=["a", "bar"]))
+            r1.add_field(
+                Field("999", [" ", " "], subfields=[Subfield(code="a", value="foo")])
+            )
+            r2.add_field(
+                Field("999", [" ", " "], subfields=[Subfield(code="a", value="bar")])
+            )
             self.assertEqual(r1["999"]["a"], "foo")
             self.assertEqual(r2["999"]["a"], "bar")
 
     def test_as_marc_with_explicit_leader(self):
         """Test setting an explicit leader.
 
         as_marc() should use the whole leader as set.
         """
         record = Record()
         record.add_field(
             Field(
                 tag="245",
                 indicators=["0", "1"],
-                subfields=["a", "The pragmatic programmer"],
+                subfields=[Subfield(code="a", value="The pragmatic programmer")],
             )
         )
-        record.leader = "00067     2200037   4500"
+        record.leader = "00067    a2200037   4500"
         leader_not_touched = record.leader
         record.as_marc()
         leader_touched = record.leader
         self.assertTrue(leader_not_touched == leader_touched)
 
     def test_remove_fields(self):
         with open("test/testunimarc.dat", "rb") as fh:
@@ -499,60 +682,81 @@
     def test_init_with_no_leader(self):
         """Test creating a Record object with no leader argument."""
         record = Record()
         record.add_field(
             Field(
                 tag="245",
                 indicators=["0", "1"],
-                subfields=["a", "The pragmatic programmer"],
+                subfields=[Subfield(code="a", value="The pragmatic programmer")],
             )
         )
         transmission_format = record.as_marc()
         transmission_format_leader = transmission_format[0:24]
-        self.assertEqual(transmission_format_leader, b"00067     2200037   4500")
+        self.assertEqual(transmission_format_leader, b"00067    a2200037   4500")
 
     def test_init_with_no_leader_but_with_force_utf8(self):
         record = Record(force_utf8=True)
         record.add_field(
             Field(
                 tag="245",
                 indicators=["0", "1"],
-                subfields=["a", "The pragmatic programmer"],
+                subfields=[Subfield(code="a", value="The pragmatic programmer")],
             )
         )
         transmission_format = record.as_marc()
         transmission_format_leader = transmission_format[0:24]
         self.assertEqual(transmission_format_leader, b"00067    a2200037   4500")
 
     def test_init_with_leader(self):
         record = Record(leader="abcdefghijklmnopqrstuvwx")
         record.add_field(
             Field(
                 tag="245",
                 indicators=["0", "1"],
-                subfields=["a", "The pragmatic programmer"],
+                subfields=[Subfield(code="a", value="The pragmatic programmer")],
             )
         )
         transmission_format = record.as_marc()
         transmission_format_leader = transmission_format[0:24]
-        self.assertEqual(transmission_format_leader, b"00067fghij2200037rst4500")
+        self.assertEqual(transmission_format_leader, b"00067fghia2200037rst4500")
 
     def test_init_with_leader_and_force_utf8(self):
         record = Record(leader="abcdefghijklmnopqrstuvwx", force_utf8=True)
         record.add_field(
             Field(
                 tag="245",
                 indicators=["0", "1"],
-                subfields=["a", "The pragmatic programmer"],
+                subfields=[Subfield(code="a", value="The pragmatic programmer")],
             )
         )
         transmission_format = record.as_marc()
         transmission_format_leader = transmission_format[0:24]
         self.assertEqual(transmission_format_leader, b"00067fghia2200037rst4500")
 
+    def test_as_marc_to_unicode_conversion(self):
+        with open("test/marc8-to-unicode.dat", "rb") as fh:
+            modified_record_bytes = fh.read()
+
+        with open("test/marc8.dat", "rb") as fh:
+            original_record_bytes = fh.read()
+            reader = MARCReader(original_record_bytes, to_unicode=True)
+            record = next(reader)
+            record_bytes = record.as_marc()
+            self.assertEqual(record_bytes[9], ord("a"))
+            self.assertEqual(modified_record_bytes, record_bytes)
+
+    def test_map_marc8_record_against_unicode_as_marc(self):
+        from pymarc.record import map_marc8_record
+
+        with open("test/marc8.dat", "rb") as fh:
+            reader = MARCReader(fh, to_unicode=True)
+            record = next(reader)
+            map_marc8_data = map_marc8_record(record)
+            self.assertEqual(map_marc8_data.as_marc(), record.as_marc())
+
 
 def suite():
     test_suite = unittest.makeSuite(RecordTest, "test")
     return test_suite
 
 
 if __name__ == "__main__":
```

### Comparing `pymarc-4.2.2/test/test_utf8.py` & `pymarc-5.0.0/test/test_utf8.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 
         finally:
             # remove it
             os.remove("test/write-utf8-test.dat")
 
     def test_combining_diacritic(self):
         """Issue 74: raises UnicodeEncodeError on Python 2."""
-        reader = pymarc.MARCReader(open("test/diacritic.dat", "rb"))
-        record = next(reader)
-        str(record)
+        with open("test/diacritic.dat", "rb") as fh:
+            reader = pymarc.MARCReader(fh)
+            record = next(reader)
+            str(record)
 
 
 def suite():
     test_suite = unittest.makeSuite(MARCUnicodeTest, "test")
     return test_suite
```

### Comparing `pymarc-4.2.2/test/test_utf8.txt` & `pymarc-5.0.0/test/test_utf8.txt`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/test_writer.py` & `pymarc-5.0.0/test/test_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,17 +105,26 @@
             ]
         """
         )
         file_handle = StringIO()
         try:
             writer = pymarc.JSONWriter(file_handle)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             actual = json.loads(file_handle.getvalue())
             self.assertEqual(actual, expected)
         finally:
             file_handle.close()
@@ -196,28 +205,53 @@
         file_handle = StringIO()
         try:
             writer = pymarc.JSONWriter(file_handle)
             record = pymarc.Record()
             record.add_field(
                 pymarc.Field("008", data="090227s2009    mau                 chi d")
             )
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             actual = json.loads(file_handle.getvalue())
             self.assertEqual(actual, expected)
         finally:
             file_handle.close()
@@ -225,15 +259,17 @@
 
 class MARCWriterTest(unittest.TestCase):
     def test_write(self):
         """Write a record off to a file."""
         file_handle = open("test/writer-test.dat", "wb")
         writer = pymarc.MARCWriter(file_handle)
         record = pymarc.Record()
-        field = pymarc.Field("245", ["0", "0"], ["a", "foo"])
+        field = pymarc.Field(
+            "245", ["0", "0"], [pymarc.Subfield(code="a", value="foo")]
+        )
         record.add_field(field)
         writer.write(record)
         writer.close()
         self.assertTrue(
             file_handle.closed, "The file handle should close when the writer closes"
         )
 
@@ -290,17 +326,26 @@
             =245  00$aFoo /$cby me.
         """
         expected = textwrap.dedent(expected[1:])
         file_handle = StringIO()
         try:
             writer = pymarc.TextWriter(file_handle)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             self.assertEqual(file_handle.getvalue(), expected)
         finally:
             file_handle.close()
 
@@ -322,28 +367,53 @@
         file_handle = StringIO()
         try:
             writer = pymarc.TextWriter(file_handle)
             record = pymarc.Record()
             record.add_field(
                 pymarc.Field("008", data="090227s2009    mau                 chi d")
             )
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             self.assertEqual(file_handle.getvalue(), expected)
         finally:
             file_handle.close()
 
@@ -439,17 +509,26 @@
             </collection>
         """
         expected = textwrap.dedent(expected[1:]).replace("\n", "").encode()
         file_handle = BytesIO()
         try:
             writer = pymarc.XMLWriter(file_handle)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             self.assertEqual(file_handle.getvalue(), expected)
         finally:
             file_handle.close()
 
@@ -491,28 +570,53 @@
         file_handle = BytesIO()
         try:
             writer = pymarc.XMLWriter(file_handle)
             record = pymarc.Record()
             record.add_field(
                 pymarc.Field("008", data="090227s2009    mau                 chi d")
             )
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
-            record.add_field(pymarc.Field("100", ["0", "0"], ["a", "me"]))
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field("100", ["0", "0"], [pymarc.Subfield(code="a", value="me")])
+            )
+            record.add_field(
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             record = pymarc.Record()
             record.add_field(
-                pymarc.Field("245", ["0", "0"], ["a", "Foo /", "c", "by me."])
+                pymarc.Field(
+                    "245",
+                    ["0", "0"],
+                    [
+                        pymarc.Subfield(code="a", value="Foo /"),
+                        pymarc.Subfield(code="c", value="by me."),
+                    ],
+                )
             )
             writer.write(record)
             writer.close(close_fh=False)
             self.assertEqual(file_handle.getvalue(), expected)
         finally:
             file_handle.close()
```

### Comparing `pymarc-4.2.2/test/test_xml.py` & `pymarc-5.0.0/test/test_xml.py`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/testunimarc.dat` & `pymarc-5.0.0/test/testunimarc.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/utf8.xml` & `pymarc-5.0.0/test/utf8.xml`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/utf8_errors.dat` & `pymarc-5.0.0/test/utf8_errors.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/utf8_invalid.mrc` & `pymarc-5.0.0/test/utf8_invalid.mrc`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/utf8_with_leader_flag.dat` & `pymarc-5.0.0/test/utf8_with_leader_flag.dat`

 * *Files identical despite different names*

### Comparing `pymarc-4.2.2/test/utf8_without_leader_flag.dat` & `pymarc-5.0.0/test/utf8_without_leader_flag.dat`

 * *Files identical despite different names*

